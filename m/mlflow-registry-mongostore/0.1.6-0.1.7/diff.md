# Comparing `tmp/mlflow_registry_mongostore-0.1.6-py3-none-any.whl.zip` & `tmp/mlflow_registry_mongostore-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 20557 bytes, number of entries: 10
+Zip file size: 20629 bytes, number of entries: 10
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_registry_mongostore/__init__.py
 -rw-r--r--  2.0 unx    18488 b- defN 23-Jun-29 10:01 mlflow_registry_mongostore/_version.py
--rw-r--r--  2.0 unx     6496 b- defN 23-Jul-12 10:36 mlflow_registry_mongostore/models.py
+-rw-r--r--  2.0 unx     7009 b- defN 23-Aug-02 11:52 mlflow_registry_mongostore/models.py
 -rw-r--r--  2.0 unx    40867 b- defN 23-Jun-30 11:20 mlflow_registry_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-12 10:39 mlflow_registry_mongostore-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1388 b- defN 23-Jul-12 10:39 mlflow_registry_mongostore-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:39 mlflow_registry_mongostore-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      155 b- defN 23-Jul-12 10:39 mlflow_registry_mongostore-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-12 10:39 mlflow_registry_mongostore-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      977 b- defN 23-Jul-12 10:39 mlflow_registry_mongostore-0.1.6.dist-info/RECORD
-10 files, 79847 bytes uncompressed, 18843 bytes compressed:  76.4%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-02 11:58 mlflow_registry_mongostore-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1388 b- defN 23-Aug-02 11:58 mlflow_registry_mongostore-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 11:58 mlflow_registry_mongostore-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      155 b- defN 23-Aug-02 11:58 mlflow_registry_mongostore-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Aug-02 11:58 mlflow_registry_mongostore-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      977 b- defN 23-Aug-02 11:58 mlflow_registry_mongostore-0.1.7.dist-info/RECORD
+10 files, 80360 bytes uncompressed, 18915 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: mlflow_registry_mongostore/models.py
 Comment: 
 
 Filename: mlflow_registry_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.6.dist-info/LICENSE
+Filename: mlflow_registry_mongostore-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.6.dist-info/METADATA
+Filename: mlflow_registry_mongostore-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.6.dist-info/WHEEL
+Filename: mlflow_registry_mongostore-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.6.dist-info/entry_points.txt
+Filename: mlflow_registry_mongostore-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.6.dist-info/top_level.txt
+Filename: mlflow_registry_mongostore-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_registry_mongostore-0.1.6.dist-info/RECORD
+Filename: mlflow_registry_mongostore-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_registry_mongostore/models.py

```diff
@@ -1,8 +1,9 @@
 import numbers
+from datetime import datetime
 from flask import request
 from mlflow.entities.model_registry import (
     RegisteredModel,
     ModelVersion,
     RegisteredModelTag,
     ModelVersionTag,
 )
@@ -17,14 +18,15 @@
     EmbeddedDocumentField,
     IntField,
     LongField,
     ReferenceField,
     CASCADE,
     QuerySet,
     Q,
+    DateTimeField,
 )
 
 
 REGISTERED_MODEL_COLLECTION_NAME = "mlflow_registered_model"
 MODEL_VERSION_COLLECTION_NAME = "mlflow_model_version"
 
 
@@ -113,14 +115,16 @@
     name = StringField(primary_key=True)
     registed_model_id = StringField(max_length=32, db_field="id")
     creation_timestamp = LongField(default=get_current_time_millis)
     last_updated_timestamp = LongField()
     description = StringField(max_length=256)
     tags = ListField(EmbeddedDocumentField(MongoRegisteredModelTag))
     mlflow_workspace_id = StringField(max_length=36)
+    _created_at = DateTimeField(default=datetime.utcnow)
+    _updated_at = DateTimeField(default=datetime.utcnow)
 
     meta = {
         "collection": REGISTERED_MODEL_COLLECTION_NAME,
         "queryset_class": CustomQuerySet,
     }
 
     def to_mlflow_entity(self) -> RegisteredModel:
@@ -132,14 +136,17 @@
             tags=[t.to_mlflow_entity() for t in self.tags],
         )
 
     def get_tags_by_key(self, key):
         return list(filter(lambda param: param.key == key, self.tags))
 
     def save(self, *args, **kwargs):
+        if not self.id:
+            self._created_at = datetime.utcnow()
+        self._updated_at = datetime.utcnow()
         self.mlflow_workspace_id = get_workspace_id()
         self.registed_model_id = self.name
         return super(MongoRegisteredModel, self).save(*args, **kwargs)
 
 
 class MongoModelVersion(Document):
     # name = StringField(primary_key=True)
@@ -158,14 +165,16 @@
     run_id = StringField(max_length=32, db_field="mlflow_run_id")
     run_link = StringField(max_length=500)
     status = StringField(
         max_length=20, default=ModelVersionStatus.to_string(ModelVersionStatus.READY)
     )
     status_message = StringField(max_length=500)
     mlflow_workspace_id = StringField(max_length=36)
+    _created_at = DateTimeField(default=datetime.utcnow)
+    _updated_at = DateTimeField(default=datetime.utcnow)
 
     tags = ListField(EmbeddedDocumentField(MongoModelVersionTag))
 
     meta = {
         "collection": MODEL_VERSION_COLLECTION_NAME,
         "queryset_class": CustomQuerySet,
     }
@@ -193,9 +202,12 @@
     @staticmethod
     def get_attribute_name(mlflow_attribute_name):
         return {"name": "registered_model_id"}.get(
             mlflow_attribute_name, mlflow_attribute_name
         )
 
     def save(self, *args, **kwargs):
+        if not self.id:
+            self._created_at = datetime.utcnow()
+        self._updated_at = datetime.utcnow()
         self.mlflow_workspace_id = get_workspace_id()
         return super(MongoModelVersion, self).save(*args, **kwargs)
```

## Comparing `mlflow_registry_mongostore-0.1.6.dist-info/LICENSE` & `mlflow_registry_mongostore-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_registry_mongostore-0.1.6.dist-info/METADATA` & `mlflow_registry_mongostore-0.1.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-registry-mongostore
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mlflow plugin to use MongoDB as backend for MLflow Model Registry service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
```

## Comparing `mlflow_registry_mongostore-0.1.6.dist-info/RECORD` & `mlflow_registry_mongostore-0.1.7.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mlflow_registry_mongostore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mlflow_registry_mongostore/_version.py,sha256=nTDwWbHLCXMqdi1bkEkchAiz_JAzkXcmH3bKG0jf6fg,18488
-mlflow_registry_mongostore/models.py,sha256=effyacU5A3jByRfExu1FiD1bUI-cWK_RHQ9406g7dUc,6496
+mlflow_registry_mongostore/models.py,sha256=YzaQwr641iR5MTxGJsHHN-IC1YtPfX0FKhKY5Z5s3-M,7009
 mlflow_registry_mongostore/mongo_store.py,sha256=5lxamQ_HlvoRbcZt3wD7NTz3toIk6JfG68bNePWyNzY,40867
-mlflow_registry_mongostore-0.1.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlflow_registry_mongostore-0.1.6.dist-info/METADATA,sha256=e20jvoWkQ90MofvccUDOwEEW_REwbNdmkodBfikO4lU,1388
-mlflow_registry_mongostore-0.1.6.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-mlflow_registry_mongostore-0.1.6.dist-info/entry_points.txt,sha256=tfl_ffj0PkSrXY4rvesmyyvPXDS-j5egPU_XNXoVKm4,155
-mlflow_registry_mongostore-0.1.6.dist-info/top_level.txt,sha256=6DHvL6p3UTy_bC25io6QqOIFVHNwvfFY0Nj_664suUE,27
-mlflow_registry_mongostore-0.1.6.dist-info/RECORD,,
+mlflow_registry_mongostore-0.1.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlflow_registry_mongostore-0.1.7.dist-info/METADATA,sha256=NrJ-qGmMCTpOoIsogrMbcd8SkNCF6BsfthxSfWYom4o,1388
+mlflow_registry_mongostore-0.1.7.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+mlflow_registry_mongostore-0.1.7.dist-info/entry_points.txt,sha256=tfl_ffj0PkSrXY4rvesmyyvPXDS-j5egPU_XNXoVKm4,155
+mlflow_registry_mongostore-0.1.7.dist-info/top_level.txt,sha256=6DHvL6p3UTy_bC25io6QqOIFVHNwvfFY0Nj_664suUE,27
+mlflow_registry_mongostore-0.1.7.dist-info/RECORD,,
```


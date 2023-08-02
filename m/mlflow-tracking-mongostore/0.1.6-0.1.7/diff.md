# Comparing `tmp/mlflow_tracking_mongostore-0.1.6-py3-none-any.whl.zip` & `tmp/mlflow_tracking_mongostore-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 18245 bytes, number of entries: 9
+Zip file size: 18318 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-Jun-29 09:59 mlflow_tracking_mongostore/__init__.py
--rw-r--r--  2.0 unx     9406 b- defN 23-Jul-12 10:35 mlflow_tracking_mongostore/models.py
+-rw-r--r--  2.0 unx    10005 b- defN 23-Aug-02 11:22 mlflow_tracking_mongostore/models.py
 -rw-r--r--  2.0 unx    43818 b- defN 23-Jul-08 17:57 mlflow_tracking_mongostore/mongo_store.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     1389 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      149 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       27 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      881 b- defN 23-Jul-12 10:39 mlflow_tracking_mongostore-0.1.6.dist-info/RECORD
-9 files, 67119 bytes uncompressed, 16683 bytes compressed:  75.1%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-02 11:58 mlflow_tracking_mongostore-0.1.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1389 b- defN 23-Aug-02 11:58 mlflow_tracking_mongostore-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-02 11:58 mlflow_tracking_mongostore-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      149 b- defN 23-Aug-02 11:58 mlflow_tracking_mongostore-0.1.7.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       27 b- defN 23-Aug-02 11:58 mlflow_tracking_mongostore-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      882 b- defN 23-Aug-02 11:58 mlflow_tracking_mongostore-0.1.7.dist-info/RECORD
+9 files, 67719 bytes uncompressed, 16756 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: mlflow_tracking_mongostore/models.py
 Comment: 
 
 Filename: mlflow_tracking_mongostore/mongo_store.py
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE
+Filename: mlflow_tracking_mongostore-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.6.dist-info/METADATA
+Filename: mlflow_tracking_mongostore-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.6.dist-info/WHEEL
+Filename: mlflow_tracking_mongostore-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.6.dist-info/entry_points.txt
+Filename: mlflow_tracking_mongostore-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.6.dist-info/top_level.txt
+Filename: mlflow_tracking_mongostore-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: mlflow_tracking_mongostore-0.1.6.dist-info/RECORD
+Filename: mlflow_tracking_mongostore-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mlflow_tracking_mongostore/models.py

```diff
@@ -1,8 +1,9 @@
 import numbers
+from datetime import datetime
 from flask import request
 from mlflow.entities import (
     Experiment,
     ExperimentTag,
     RunTag,
     RunInfo,
     RunData,
@@ -26,14 +27,15 @@
     BooleanField,
     LongField,
     ReferenceField,
     CASCADE,
     EmbeddedDocumentListField,
     QuerySet,
     Q,
+    DateTimeField,
 )
 
 
 EXPERIMENT_COLLECTION_NAME = "mlflow_experiment"
 RUN_COLLECTION_NAME = "mlflow_run"
 METRIC_COLLECTION_NAME = "mlflow_metric"
 
@@ -132,19 +134,23 @@
 
 
 class MongoExperiment(Document):
     experiment_id = StringField(primary_key=True)
     exp_id = StringField(max_length=32, db_field="id")
     name = StringField(required=True, max_length=200)
     artifact_location = StringField(max_length=256)
-    lifecycle_stage = StringField(max_length=50, default=LifecycleStage.ACTIVE)
+    lifecycle_stage = StringField(
+        max_length=50, default=LifecycleStage.ACTIVE, db_field="_lifecycle_stage"
+    )
     tags = ListField(EmbeddedDocumentField(MongoExperimentTag))
     creation_time = LongField()
     last_update_time = LongField()
     mlflow_workspace_id = StringField(max_length=36)
+    _created_at = DateTimeField(default=datetime.utcnow)
+    _updated_at = DateTimeField(default=datetime.utcnow)
 
     meta = {
         "collection": EXPERIMENT_COLLECTION_NAME,
         "strict": False,
         "queryset_class": CustomQuerySet,
     }
 
@@ -156,14 +162,17 @@
             lifecycle_stage=self.lifecycle_stage,
             tags=[t.to_mlflow_entity() for t in self.tags],
             creation_time=self.creation_time,
             last_update_time=self.last_update_time,
         )
 
     def save(self, *args, **kwargs):
+        if not self.id:
+            self._created_at = datetime.utcnow()
+        self._updated_at = datetime.utcnow()
         self.mlflow_workspace_id = get_workspace_id()
         self.exp_id = self.experiment_id
         return super(MongoExperiment, self).save(*args, **kwargs)
 
 
 class MongoTag(EmbeddedDocument):
     key = StringField(required=True)
@@ -231,21 +240,25 @@
     status = StringField(
         max_length=20, default=RunStatus.to_string(RunStatus.SCHEDULED)
     )
     start_time = LongField(default=get_current_time_millis)
     end_time = LongField()
     deleted_time = LongField()
     source_version = StringField(max_length=50)
-    lifecycle_stage = StringField(max_length=20, default=LifecycleStage.ACTIVE)
+    lifecycle_stage = StringField(
+        max_length=20, default=LifecycleStage.ACTIVE, db_field="_lifecycle_stage"
+    )
     artifact_uri = StringField(max_length=200)
 
     experiment_id = ReferenceField(
         "MongoExperiment", reverse_delete_rule=CASCADE, db_field="mlflow_experiment_id"
     )
     mlflow_workspace_id = StringField(max_length=36)
+    _created_at = DateTimeField(default=datetime.utcnow)
+    _updated_at = DateTimeField(default=datetime.utcnow)
 
     latest_metrics = ListField(EmbeddedDocumentField(MongoLatestMetric))
     params = ListField(EmbeddedDocumentField(MongoParam))
     # tags = ListField(EmbeddedDocumentField(MongoTag))
     tags = EmbeddedDocumentListField(MongoTag)
 
     meta = {"collection": RUN_COLLECTION_NAME, "queryset_class": CustomQuerySet}
@@ -290,10 +303,13 @@
         params = list(filter(lambda param: param.key == key, self.params))
         return params[0] if params else None
 
     def get_tags_by_key(self, key):
         return list(filter(lambda param: param.key == key, self.tags))
 
     def save(self, *args, **kwargs):
+        if not self.id:
+            self._created_at = datetime.utcnow()
+        self._updated_at = datetime.utcnow()
         self.mlflow_workspace_id = get_workspace_id()
         self.run_id = self.run_uuid
         return super(MongoRun, self).save(*args, **kwargs)
```

## Comparing `mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE` & `mlflow_tracking_mongostore-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mlflow_tracking_mongostore-0.1.6.dist-info/METADATA` & `mlflow_tracking_mongostore-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-tracking-mongostore
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mlflow plugin to use MongoDB as backend for MLflow tracking service
 Home-page: UNKNOWN
 Author: Rachid Belmeskine
 Maintainer-email: rachid.belmeskine@gmail.com
 License: UNKNOWN
 Keywords: mlflow
 Platform: UNKNOWN
```

## Comparing `mlflow_tracking_mongostore-0.1.6.dist-info/RECORD` & `mlflow_tracking_mongostore-0.1.7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mlflow_tracking_mongostore/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mlflow_tracking_mongostore/models.py,sha256=PkHb6gWdw4Q9OHpa1YMSD_sdObcaoLVoP9rBv2fU74A,9406
+mlflow_tracking_mongostore/models.py,sha256=WdpK0ilF897Pngyw4AdR8uR6_oRUL_4-Is6eSa7YmmU,10005
 mlflow_tracking_mongostore/mongo_store.py,sha256=PQ58RDY9AtodaKhml7aLQFH-pa7AlkR58QlcdlIh5RE,43818
-mlflow_tracking_mongostore-0.1.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-mlflow_tracking_mongostore-0.1.6.dist-info/METADATA,sha256=5vvSravfOzNy32j_aQX2Z2wWfSpyU2Pnnbxxj-nM-40,1389
-mlflow_tracking_mongostore-0.1.6.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
-mlflow_tracking_mongostore-0.1.6.dist-info/entry_points.txt,sha256=1DhRgG-R9Qmgl1i-WxNc8x5JtKenuAkyVNYfAmZQOBo,149
-mlflow_tracking_mongostore-0.1.6.dist-info/top_level.txt,sha256=OWuYjvOHTC4KzmrdfxF9HUBd_TMuvjKoihXmytBaCKM,27
-mlflow_tracking_mongostore-0.1.6.dist-info/RECORD,,
+mlflow_tracking_mongostore-0.1.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+mlflow_tracking_mongostore-0.1.7.dist-info/METADATA,sha256=Id6rPeSH2tFBBATm7k0Ys_m9_TAUxqGvEwxjf6wQqjw,1389
+mlflow_tracking_mongostore-0.1.7.dist-info/WHEEL,sha256=EVRjI69F5qVjm_YgqcTXPnTAv3BfSUr0WVAHuSP3Xoo,92
+mlflow_tracking_mongostore-0.1.7.dist-info/entry_points.txt,sha256=1DhRgG-R9Qmgl1i-WxNc8x5JtKenuAkyVNYfAmZQOBo,149
+mlflow_tracking_mongostore-0.1.7.dist-info/top_level.txt,sha256=OWuYjvOHTC4KzmrdfxF9HUBd_TMuvjKoihXmytBaCKM,27
+mlflow_tracking_mongostore-0.1.7.dist-info/RECORD,,
```


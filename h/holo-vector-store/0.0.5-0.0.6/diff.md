# Comparing `tmp/holo_vector_store-0.0.5.tar.gz` & `tmp/holo_vector_store-0.0.6.tar.gz`

## Comparing `holo_vector_store-0.0.5.tar` & `holo_vector_store-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/Develop.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/env.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/__about__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/__init__.py
--rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/holo_vector_store.py
--rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/hologres_wrapper.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/tests/test_holo_vector_store.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/README.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/Develop.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/env.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/src/holo_vector_store/__about__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/src/holo_vector_store/__init__.py
+-rw-r--r--   0        0        0     7099 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/src/holo_vector_store/holo_vector_store.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/src/holo_vector_store/hologres_wrapper.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/tests/test_holo_vector_store.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/LICENSE.txt
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/README.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.6/PKG-INFO
```

### Comparing `holo_vector_store-0.0.5/src/holo_vector_store/holo_vector_store.py` & `holo_vector_store-0.0.6/src/holo_vector_store/holo_vector_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
             metadatas: List of metadatas associated with the vectors.
         """
         if ids is None:
             ids = [str(uuid.uuid1()) for _ in vectors]
         if metadatas is None:
             metadatas = [{} for _ in vectors]
         if schema_datas is None:
-            schema_datas = []
+            schema_datas = [{} for _ in vectors]
         try:
             self.storage.batch_upsert(ids, vectors, metadatas, schema_datas)
         except Exception as e:
             self.logger.exception(e)
             self.storage.conn.commit()
             raise e
```

### Comparing `holo_vector_store-0.0.5/src/holo_vector_store/hologres_wrapper.py` & `holo_vector_store-0.0.6/src/holo_vector_store/hologres_wrapper.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.5/tests/test_holo_vector_store.py` & `holo_vector_store-0.0.6/tests/test_holo_vector_store.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.5/LICENSE.txt` & `holo_vector_store-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.5/README.md` & `holo_vector_store-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.5/pyproject.toml` & `holo_vector_store-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.5/PKG-INFO` & `holo_vector_store-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holo-vector-store
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: Documentation, https://github.com/unknown/holo-vector-store#readme
 Project-URL: Issues, https://github.com/unknown/holo-vector-store/issues
 Project-URL: Source, https://github.com/unknown/holo-vector-store
 Author-email: Changgeng Zhao <zhaochanggeng.zcg@alibaba-inc.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/holo_vector_store-0.0.4.tar.gz` & `tmp/holo_vector_store-0.0.5.tar.gz`

## Comparing `holo_vector_store-0.0.4.tar` & `holo_vector_store-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/Develop.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/env.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/__about__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/__init__.py
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/holo_vector_store.py
--rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/hologres_wrapper.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/tests/test_holo_vector_store.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/README.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/Develop.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/env.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/__about__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/__init__.py
+-rw-r--r--   0        0        0     7080 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/holo_vector_store.py
+-rw-r--r--   0        0        0     7684 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/src/holo_vector_store/hologres_wrapper.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/tests/test_holo_vector_store.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/LICENSE.txt
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/README.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.5/PKG-INFO
```

### Comparing `holo_vector_store-0.0.4/src/holo_vector_store/holo_vector_store.py` & `holo_vector_store-0.0.5/src/holo_vector_store/holo_vector_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         vector: list[float],
         k: int = 3,
         select_columns: list[str] | None = None,
         metadata_filters: dict | None = None,
         schema_data_filters: dict | None = None,
     ) -> list[dict[str, Any]]:
         """
-        Return: list[id, metadata::text, distance, select_column_0, ... , select_column_n]
+        Return: list[{id, metadata::text, distance, select_column_0, ... , select_column_n}]
         """
         results: list[tuple] = self.storage.query_nearest_neighbours(
             vector, k, select_columns, metadata_filters, schema_data_filters
         )
         ret = []
         for row in results:
             parsed_row = {
@@ -117,20 +117,37 @@
 
     def query(
         self,
         select_columns: list[str] | None = None,
         metadata_filters: dict | None = None,
         schema_data_filters: dict | None = None,
         limit: int = 100,
-    ):
+    ) -> list[dict[str, Any]]:
         """
         Get data by filter, without using vectors. By default, limit the number of output rows to 100.
-        Return: list[id, vector, metadata::text, distance, select_column_0, ... , select_column_n]
+        Return: list[{id, vector, metadata::text, select_column_0, ... , select_column_n}]
         """
-        return self.storage.query_by_filters(select_columns, metadata_filters, schema_data_filters, limit)
+        results = self.storage.query_by_filters(select_columns, metadata_filters, schema_data_filters, limit)
+        ret = []
+        for row in results:
+            parsed_row = {
+                "id": row[0],
+                "vector": row[1],
+                "metadata": json.loads(row[2]),
+            }
+            if select_columns:
+                i = 3
+                for col_name in select_columns:
+                    parsed_row[col_name] = row[i]
+                    i += 1
+                if i != len(row):
+                    raise AssertionError()
+            ret.append(parsed_row)
+
+        return ret
 
     def delete_vectors(
         self,
         metadata_filters: dict | None = None,
         schema_data_filters: dict | None = None,
     ):
         """Delete by filters."""
```

### Comparing `holo_vector_store-0.0.4/src/holo_vector_store/hologres_wrapper.py` & `holo_vector_store-0.0.5/src/holo_vector_store/hologres_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
         self,
         select_columns: list[str] | None = None,
         metadata_filters: dict[str, str] | None = None,
         schema_data_filters: dict[str, str] | None = None,
         limit: int = 100,
     ) -> list[tuple[Any, ...]]:
         """
-        Return: list[id, vector, metadata::text, distance, select_column_0, ... , select_column_n]
+        Return: list[id, vector, metadata::text, select_column_0, ... , select_column_n]
         """
         filter_clause, params = _get_filter_clause(metadata_filters, schema_data_filters)
 
         col_names = ""
         if select_columns is not None:
             for col_name in select_columns:
                 col_names += f", {col_name}"
```

### Comparing `holo_vector_store-0.0.4/tests/test_holo_vector_store.py` & `holo_vector_store-0.0.5/tests/test_holo_vector_store.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.4/LICENSE.txt` & `holo_vector_store-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.4/README.md` & `holo_vector_store-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.4/pyproject.toml` & `holo_vector_store-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.4/PKG-INFO` & `holo_vector_store-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holo-vector-store
-Version: 0.0.4
+Version: 0.0.5
 Project-URL: Documentation, https://github.com/unknown/holo-vector-store#readme
 Project-URL: Issues, https://github.com/unknown/holo-vector-store/issues
 Project-URL: Source, https://github.com/unknown/holo-vector-store
 Author-email: Changgeng Zhao <zhaochanggeng.zcg@alibaba-inc.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


# Comparing `tmp/holo_vector_store-0.0.3.tar.gz` & `tmp/holo_vector_store-0.0.4.tar.gz`

## Comparing `holo_vector_store-0.0.3.tar` & `holo_vector_store-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/Develop.md
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/env.sh
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/src/holo_vector_store/__about__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/src/holo_vector_store/__init__.py
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/src/holo_vector_store/holo_vector_store.py
--rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/src/holo_vector_store/hologres_wrapper.py
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/tests/test_holo_vector_store.py
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/LICENSE.txt
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/README.md
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/Develop.md
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/env.sh
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/__about__.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/__init__.py
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/holo_vector_store.py
+-rw-r--r--   0        0        0     7694 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/src/holo_vector_store/hologres_wrapper.py
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0     6857 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/tests/test_holo_vector_store.py
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/README.md
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 holo_vector_store-0.0.4/PKG-INFO
```

### Comparing `holo_vector_store-0.0.3/src/holo_vector_store/holo_vector_store.py` & `holo_vector_store-0.0.4/src/holo_vector_store/holo_vector_store.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.3/src/holo_vector_store/hologres_wrapper.py` & `holo_vector_store-0.0.4/src/holo_vector_store/hologres_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         filter_clause, params = _get_filter_clause(metadata_filters, schema_data_filters)
 
         col_names = ""
         if select_columns is not None:
             for col_name in select_columns:
                 col_names += f", {col_name}"
 
-        sql = f"select id, vector, metadata::text, from {self.table_name} {filter_clause} limit %s;"
+        sql = f"select id, vector, metadata::text {col_names} from {self.table_name} {filter_clause} limit %s;"
         self.cursor.execute(sql, (*params, limit))
         self.conn.commit()
         return self.cursor.fetchall()
 
     def delete_by_filters(
         self,
         metadata_filters: dict[str, str] | None = None,
```

### Comparing `holo_vector_store-0.0.3/tests/test_holo_vector_store.py` & `holo_vector_store-0.0.4/tests/test_holo_vector_store.py`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.3/LICENSE.txt` & `holo_vector_store-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.3/README.md` & `holo_vector_store-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.3/pyproject.toml` & `holo_vector_store-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `holo_vector_store-0.0.3/PKG-INFO` & `holo_vector_store-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: holo-vector-store
-Version: 0.0.3
+Version: 0.0.4
 Project-URL: Documentation, https://github.com/unknown/holo-vector-store#readme
 Project-URL: Issues, https://github.com/unknown/holo-vector-store/issues
 Project-URL: Source, https://github.com/unknown/holo-vector-store
 Author-email: Changgeng Zhao <zhaochanggeng.zcg@alibaba-inc.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```


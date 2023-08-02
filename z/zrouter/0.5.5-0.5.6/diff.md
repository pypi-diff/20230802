# Comparing `tmp/zrouter-0.5.5.tar.gz` & `tmp/zrouter-0.5.6.tar.gz`

## Comparing `zrouter-0.5.5.tar` & `zrouter-0.5.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/__init__.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/restful.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/router.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/exceptions/__init__.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.5/src/zrouter/utils/json.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.5/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.5/LICENSE
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.5/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.5/pyproject.toml
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/__init__.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/restful.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/router.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/exceptions/__init__.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 zrouter-0.5.6/src/zrouter/utils/json.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 zrouter-0.5.6/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 zrouter-0.5.6/LICENSE
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 zrouter-0.5.6/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 zrouter-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 zrouter-0.5.6/PKG-INFO
```

### Comparing `zrouter-0.5.5/src/zrouter/restful.py` & `zrouter-0.5.6/src/zrouter/restful.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 def R(mapper_class):
     def get(id: Optional[int] = None, page_num: Optional[int] = None, page_size: Optional[int] = None, **kwargs):
         if id:
             return mapper_class.get_json(id)
         else:
             return mapper_class.get_jsons(page_num=page_num, page_size=page_size)
 
-    def post(data: dict):
-        mapper_class.add(data)
-
-    def put(id: int, data: dict):
-        mapper_class.save(id, data)
+    def post(data: dict, id: Optional[int] = None):
+        if id:
+            mapper_class.save(id, data)
+        else:
+            mapper_class.add(data)
 
     def delete(id: int):
         mapper_class.delete(id=id)
 
     method_dict = {
         'get': get,
         'post': post,
-        'put': put,
         'delete': delete
     }
 
     return type('Resource', (object,), method_dict)
```

### Comparing `zrouter-0.5.5/src/zrouter/router.py` & `zrouter-0.5.6/src/zrouter/router.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.5/src/zrouter/utils/json.py` & `zrouter-0.5.6/src/zrouter/utils/json.py`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.5/LICENSE` & `zrouter-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.5/README.md` & `zrouter-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `zrouter-0.5.5/pyproject.toml` & `zrouter-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "zrouter"
-version = "0.5.5"
+version = "0.5.6"
 authors = [
   { name="inspirare6", email="inspirare6@163.com" },
 ]
 description = "zen router library"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `zrouter-0.5.5/PKG-INFO` & `zrouter-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zrouter
-Version: 0.5.5
+Version: 0.5.6
 Summary: zen router library
 Project-URL: Homepage, https://github.com/inspirare6/zrouter
 Project-URL: Bug Tracker, https://github.com/inspirare6/zrouter/issues
 Author-email: inspirare6 <inspirare6@163.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


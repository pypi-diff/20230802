# Comparing `tmp/pypomes_store-0.1.7.tar.gz` & `tmp/pypomes_store-0.1.8.tar.gz`

## Comparing `pypomes_store-0.1.7.tar` & `pypomes_store-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/src/pypomes_store/__init__.py
--rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/src/pypomes_store/azure_pomes.py
--rw-r--r--   0        0        0    13930 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/src/pypomes_store/minio_pomes.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/README.md
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/src/pypomes_store/__init__.py
+-rw-r--r--   0        0        0     7714 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/src/pypomes_store/azure_pomes.py
+-rw-r--r--   0        0        0    13962 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/src/pypomes_store/minio_pomes.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/README.md
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 pypomes_store-0.1.8/PKG-INFO
```

### Comparing `pypomes_store-0.1.7/src/pypomes_store/__init__.py` & `pypomes_store-0.1.8/src/pypomes_store/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,9 +16,9 @@
     # minio_pomes
     MINIO_BUCKET, MINIO_HOST, MINIO_ACCESS_KEY, MINIO_SECRET_KEY, MINIO_SECURE_ACCESS, MINIO_TEMP_PATH,
     minio_access, minio_file_store, minio_object_store, minio_object_stat,
     minio_object_delete, minio_objects_list, minio_object_retrieve, minio_object_exists,
     minio_object_tags_retrieve, minio_file_retrieve, minio_setup
 ]
 
-__version__ = "0.1.7"
-__version_info__ = (0, 1, 7)
+__version__ = "0.1.8"
+__version_info__ = (0, 1, 8)
```

### Comparing `pypomes_store-0.1.7/src/pypomes_store/azure_pomes.py` & `pypomes_store-0.1.8/src/pypomes_store/azure_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.7/src/pypomes_store/minio_pomes.py` & `pypomes_store-0.1.8/src/pypomes_store/minio_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     except Exception as e:
         errors.append(__minio_except_msg(e))
 
     return result
 
 
 def minio_file_store(errors: list[str], basepath: str,
-                     identifier: str, filepath: str, mimetype: str, tags: dict = None):
+                     identifier: str, filepath: str, mimetype: str, tags: dict = None) -> None:
     """
     Store a file at the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the file at
     :param identifier: the file identifier, tipically a file name
     :param filepath: the path specifying where the file is
@@ -195,15 +195,15 @@
             if not hasattr(e, "code") or e.code != "NoSuchKey":
                 errors.append(__minio_except_msg(e))
 
     return result
 
 
 def minio_object_store(errors: list[str], basepath: str,
-                       identifier: str, obj: any, tags: dict = None):
+                       identifier: str, obj: any, tags: dict = None) -> None:
     """
     Store an object at the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to store the object at
     :param identifier: the object identifier
     :param obj: object to be stored
@@ -247,15 +247,15 @@
         with open(filepath, "rb") as f:
             result = pickle.load(f)
         os.remove(filepath)
 
     return result
 
 
-def minio_object_delete(errors: list[str], basepath: str, identifier: str = None):
+def minio_object_delete(errors: list[str], basepath: str, identifier: str = None) -> None:
     """
     Remove an object from the *MinIO* store.
 
     :param errors: incidental error messages
     :param basepath: the path specifying the location to retrieve the object from
     :param identifier: the object identifier
     """
@@ -338,15 +338,15 @@
                                                recursive=recursive)
         except Exception as e:
             errors.append(__minio_except_msg(e))
 
     return result
 
 
-def __minio_folder_delete(errors: list[str],  minio_client: Minio, basepath: str):
+def __minio_folder_delete(errors: list[str],  minio_client: Minio, basepath: str) -> None:
     """
     Traverse the folders recursively, removing its objects.
 
     :param errors: incidental error messages
     :param minio_client: the MinIO client object
     :param basepath: the path specifying the location to delete the objects at.
     """
```

### Comparing `pypomes_store-0.1.7/LICENSE` & `pypomes_store-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_store-0.1.7/pyproject.toml` & `pypomes_store-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_store"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (object storage modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -21,15 +21,15 @@
 dependencies = [
     "azure-common>=1.1.28",
     "azure-core>=1.28.0",
     "azure-identity>=1.13.0",
     "azure-storage-blob>=12.17.0",
     "minio>=7.1.15",
     "pip>=23.2.1",
-    "pypomes_core>=0.2.1",
+    "pypomes_core>=0.2.2",
     "setuptools>=68.0.0",
     "Unidecode>=1.3.6",
     "wheel>=0.41.0"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/TheWiseCoder/PyPomes-Store"
```

### Comparing `pypomes_store-0.1.7/PKG-INFO` & `pypomes_store-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypomes_store
-Version: 0.1.7
+Version: 0.1.8
 Summary: A collection of Python pomes, pennyeach (object storage modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Store
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Store/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,11 +12,11 @@
 Requires-Python: >=3.10
 Requires-Dist: azure-common>=1.1.28
 Requires-Dist: azure-core>=1.28.0
 Requires-Dist: azure-identity>=1.13.0
 Requires-Dist: azure-storage-blob>=12.17.0
 Requires-Dist: minio>=7.1.15
 Requires-Dist: pip>=23.2.1
-Requires-Dist: pypomes-core>=0.2.1
+Requires-Dist: pypomes-core>=0.2.2
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: unidecode>=1.3.6
 Requires-Dist: wheel>=0.41.0
```


# Comparing `tmp/apify-1.1.2b1.tar.gz` & `tmp/apify-1.1.2b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.1.2b1.tar", last modified: Tue Aug  1 11:36:24 2023, max compression
+gzip compressed data, was "apify-1.1.2b2.tar", last modified: Wed Aug  2 09:12:10 2023, max compression
```

## Comparing `apify-1.1.2b1.tar` & `apify-1.1.2b2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.509369 apify-1.1.2b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-01 11:35:43.000000 apify-1.1.2b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-01 11:36:24.509369 apify-1.1.2b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-01 11:35:43.000000 apify-1.1.2b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-08-01 11:36:20.000000 apify-1.1.2b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 11:36:24.509369 apify-1.1.2b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.501368 apify-1.1.2b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.505369 apify-1.1.2b1/src/apify/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.505369 apify-1.1.2b1/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10160 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.509369 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19703 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19749 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    58948 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.509369 apify-1.1.2b1/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    23436 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-01 11:35:43.000000 apify-1.1.2b1/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 11:36:24.505369 apify-1.1.2b1/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-01 11:36:24.000000 apify-1.1.2b1/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.727965 apify-1.1.2b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-08-02 09:11:22.000000 apify-1.1.2b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-02 09:12:10.727965 apify-1.1.2b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-08-02 09:11:22.000000 apify-1.1.2b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-08-02 09:12:06.000000 apify-1.1.2b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:12:10.727965 apify-1.1.2b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.715965 apify-1.1.2b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.719966 apify-1.1.2b2/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.723966 apify-1.1.2b2/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.723966 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19703 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19725 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12602 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58929 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4026 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15545 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.727965 apify-1.1.2b2/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23436 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10132 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25909 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-08-02 09:11:22.000000 apify-1.1.2b2/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:12:10.719966 apify-1.1.2b2/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-08-02 09:12:10.000000 apify-1.1.2b2/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-08-02 09:12:10.000000 apify-1.1.2b2/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:12:10.000000 apify-1.1.2b2/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-08-02 09:12:10.000000 apify-1.1.2b2/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 09:12:10.000000 apify-1.1.2b2/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.1.2b1/LICENSE` & `apify-1.1.2b2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/PKG-INFO` & `apify-1.1.2b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.2b1
+Version: 1.1.2b2
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.1.2b1/README.md` & `apify-1.1.2b2/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/pyproject.toml` & `apify-1.1.2b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify"
 
-version = "1.1.2b1"
+version = "1.1.2b2"
 description = "Apify SDK for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
@@ -47,17 +47,17 @@
 
 dependencies = [
 
     "aiofiles >= 22.1.0",
 
     "aioshutil >= 1.0",
 
-    "apify-client >= 1.3.1",
+    "apify-client == 1.3.1",
 
-    "apify-shared >= 1.0.0",
+    "apify-shared == 1.0.2",
 
     "colorama >= 0.4.6",
 
     "cryptography >= 39.0.0",
 
     "httpx >= 0.24.1",
 
@@ -103,14 +103,16 @@
 
     "flake8-noqa ~= 1.3.1",
 
     "flake8-pytest-style ~= 1.7.2",
 
     "flake8-quotes ~= 3.3.2",
 
+    "flake8-simplify ~= 0.20.0",
+
     "flake8-unused-arguments ~= 0.0.13",
 
     "isort ~= 5.12.0",
 
     "mypy ~= 1.3.0",
 
     "pep8-naming ~= 0.13.3",
```

### Comparing `apify-1.1.2b1/src/apify/_crypto.py` & `apify-1.1.2b2/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.1.2b2/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.1.2b2/src/apify/_memory_storage/memory_storage_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import contextlib
 import os
 from pathlib import Path
 from typing import List, Optional
 
 import aioshutil
 from aiofiles import ospath
 from aiofiles.os import rename, scandir
@@ -163,19 +164,16 @@
             # Create a temporary folder to save important files in
             Path(temporary_path).mkdir(parents=True, exist_ok=True)
 
             # Go through each file and save the ones that are important
             for entity in possible_input_keys:
                 original_file_path = os.path.join(folder, entity)
                 temp_file_path = os.path.join(temporary_path, entity)
-                try:
+                with contextlib.suppress(Exception):
                     await rename(original_file_path, temp_file_path)
-                except Exception:
-                    # Ignore
-                    pass
 
             # Remove the original folder and all its content
             counter = 0
             temp_path_for_old_folder = os.path.normpath(os.path.join(folder, f'../__OLD_DEFAULT_{counter}__'))
             done = False
             while not done:
                 try:
```

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,32 +89,31 @@
         # First try to find the storage by looking up the directory by name
         if name:
             possible_storage_path = os.path.join(storages_dir, name)
             if os.access(possible_storage_path, os.F_OK):
                 storage_path = possible_storage_path
 
         # If it's not found, try going through the storages dir and finding it by metadata
-        if not storage_path:
-            if os.access(storages_dir, os.F_OK):
-                for entry in os.scandir(storages_dir):
-                    if not entry.is_dir():
-                        continue
-                    metadata_path = os.path.join(entry.path, '__metadata__.json')
-                    if not os.access(metadata_path, os.F_OK):
-                        continue
-                    with open(metadata_path, encoding='utf-8') as metadata_file:
-                        metadata = json.load(metadata_file)
-                    if id and id == metadata.get('id'):
-                        storage_path = entry.path
-                        name = metadata.get(name)
-                        break
-                    if name and name == metadata.get('name'):
-                        storage_path = entry.path
-                        id = metadata.get(id)
-                        break
+        if not storage_path and os.access(storages_dir, os.F_OK):
+            for entry in os.scandir(storages_dir):
+                if not entry.is_dir():
+                    continue
+                metadata_path = os.path.join(entry.path, '__metadata__.json')
+                if not os.access(metadata_path, os.F_OK):
+                    continue
+                with open(metadata_path, encoding='utf-8') as metadata_file:
+                    metadata = json.load(metadata_file)
+                if id and id == metadata.get('id'):
+                    storage_path = entry.path
+                    name = metadata.get(name)
+                    break
+                if name and name == metadata.get('name'):
+                    storage_path = entry.path
+                    id = metadata.get(id)
+                    break
 
         # As a last resort, try to check if the accessed storage is the default one,
         # and the folder has no metadata
         # TODO: make this respect the APIFY_DEFAULT_XXX_ID env var
         if id == 'default':
             possible_storage_path = os.path.join(storages_dir, id)
             if os.access(possible_storage_path, os.F_OK):
```

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

```diff
@@ -309,17 +309,16 @@
                 'contentType': content_type,
             }
 
             old_record = existing_store_by_id._records.get(key)
             existing_store_by_id._records[key] = record
 
             if self._memory_storage_client._persist_storage:
-                if old_record is not None:
-                    if _filename_from_record(old_record) != _filename_from_record(record):
-                        await existing_store_by_id._delete_persisted_record(old_record)
+                if old_record is not None and _filename_from_record(old_record) != _filename_from_record(record):
+                    await existing_store_by_id._delete_persisted_record(old_record)
 
                 await existing_store_by_id._persist_record(record)
 
     async def _persist_record(self, record: KeyValueStoreRecord) -> None:
         store_directory = self._resource_directory
         record_filename = _filename_from_record(record)
         record['filename'] = record_filename
```

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.1.2b2/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/_utils.py` & `apify-1.1.2b2/src/apify/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     DATETIME_ENV_VARS,
     DATETIME_ENV_VARS_TYPE,
     FLOAT_ENV_VARS,
     FLOAT_ENV_VARS_TYPE,
     INTEGER_ENV_VARS,
     INTEGER_ENV_VARS_TYPE,
     STRING_ENV_VARS_TYPE,
+    ActorEnvVars,
     ApifyEnvVars,
 )
 from apify_shared.utils import ignore_docs, is_content_type_json, is_content_type_text, is_content_type_xml, maybe_extract_enum_member_value
 
 from .consts import REQUEST_ID_LENGTH, _StorageTypes
 
 T = TypeVar('T')
@@ -140,15 +141,15 @@
 
 @overload
 def _fetch_and_parse_env_var(env_var: STRING_ENV_VARS_TYPE) -> Optional[str]:
     ...
 
 
 @overload
-def _fetch_and_parse_env_var(env_var: ApifyEnvVars) -> Optional[Any]:
+def _fetch_and_parse_env_var(env_var: Union[ActorEnvVars, ApifyEnvVars]) -> Optional[Any]:
     ...
 
 
 def _fetch_and_parse_env_var(env_var: Any, default: Any = None) -> Any:
     env_var_name = str(maybe_extract_enum_member_value(env_var))
 
     val = os.getenv(env_var_name)
@@ -176,18 +177,16 @@
     return psutil.cpu_percent()
 
 
 def _get_memory_usage_bytes() -> int:
     current_process = psutil.Process(os.getpid())
     mem = int(current_process.memory_info().rss or 0)
     for child in current_process.children(recursive=True):
-        try:
+        with contextlib.suppress(psutil.NoSuchProcess):
             mem += int(child.memory_info().rss or 0)
-        except psutil.NoSuchProcess:
-            pass
     return mem
 
 
 def _maybe_parse_bool(val: Optional[str]) -> bool:
     if val == 'true' or val == 'True' or val == '1':
         return True
     return False
```

### Comparing `apify-1.1.2b1/src/apify/actor.py` & `apify-1.1.2b2/src/apify/actor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
+import contextlib
 import inspect
 import logging
 import os
 import sys
 from datetime import datetime, timezone
 from types import TracebackType
 from typing import Any, Awaitable, Callable, Dict, List, Optional, Type, TypeVar, Union, cast
 
 from apify_client import ApifyClientAsync
-from apify_shared.consts import ActorEventTypes, ActorExitCodes, ApifyEnvVars, WebhookEventType
+from apify_shared.consts import ActorEnvVars, ActorEventTypes, ActorExitCodes, ApifyEnvVars, WebhookEventType
 from apify_shared.utils import ignore_docs, maybe_extract_enum_member_value
 
 from ._crypto import _decrypt_input_secrets, _load_private_key
 from ._memory_storage import MemoryStorageClient
 from ._utils import (
     _fetch_and_parse_env_var,
     _get_cpu_usage_percent,
@@ -267,36 +268,30 @@
 
         return result
 
     async def _respond_to_migrating_event(self, _event_data: Any) -> None:
         # Don't emit any more regular persist state events
         if self._send_persist_state_interval_task and not self._send_persist_state_interval_task.cancelled():
             self._send_persist_state_interval_task.cancel()
-            try:
+            with contextlib.suppress(asyncio.CancelledError):
                 await self._send_persist_state_interval_task
-            except asyncio.CancelledError:
-                pass
 
         self._event_manager.emit(ActorEventTypes.PERSIST_STATE, {'isMigrating': True})
         self._was_final_persist_state_emitted = True
 
     async def _cancel_event_emitting_intervals(self) -> None:
         if self._send_persist_state_interval_task and not self._send_persist_state_interval_task.cancelled():
             self._send_persist_state_interval_task.cancel()
-            try:
+            with contextlib.suppress(asyncio.CancelledError):
                 await self._send_persist_state_interval_task
-            except asyncio.CancelledError:
-                pass
 
         if self._send_system_info_interval_task and not self._send_system_info_interval_task.cancelled():
             self._send_system_info_interval_task.cancel()
-            try:
+            with contextlib.suppress(asyncio.CancelledError):
                 await self._send_system_info_interval_task
-            except asyncio.CancelledError:
-                pass
 
     @classmethod
     async def exit(
         cls,
         *,
         exit_code: int = 0,
         event_listeners_timeout_secs: Optional[float] = EVENT_LISTENERS_TIMEOUT_SECS,
@@ -749,15 +744,15 @@
         """
         return cls._get_default_instance().get_env()
 
     def _get_env_internal(self) -> Dict:
         self._raise_if_not_initialized()
 
         return {
-            env_var.name.lower(): _fetch_and_parse_env_var(env_var) for env_var in ApifyEnvVars
+            env_var.name.lower(): _fetch_and_parse_env_var(env_var) for env_var in [*ActorEnvVars, *ApifyEnvVars]
         }
 
     @classmethod
     async def start(
         cls,
         actor_id: str,
         run_input: Optional[Any] = None,
@@ -1295,16 +1290,16 @@
         proxy_urls: Optional[List[str]] = None,
         new_url_function: Optional[Union[Callable[[Optional[str]], str], Callable[[Optional[str]], Awaitable[str]]]] = None,
     ) -> Optional[ProxyConfiguration]:
         self._raise_if_not_initialized()
 
         if actor_proxy_input is not None:
             if actor_proxy_input.get('useApifyProxy', False):
-                country_code = country_code or actor_proxy_input.get('apifyProxyCountry', None)
-                groups = groups or actor_proxy_input.get('apifyProxyGroups', None)
+                country_code = country_code or actor_proxy_input.get('apifyProxyCountry')
+                groups = groups or actor_proxy_input.get('apifyProxyGroups')
             else:
                 proxy_urls = actor_proxy_input.get('proxyUrls', [])
                 if not proxy_urls:
                     return None
 
         proxy_configuration = ProxyConfiguration(
             password=password,
```

### Comparing `apify-1.1.2b1/src/apify/config.py` & `apify-1.1.2b2/src/apify/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional
 
-from apify_shared.consts import ApifyEnvVars
+from apify_shared.consts import ActorEnvVars, ApifyEnvVars
 
 from ._utils import _fetch_and_parse_env_var
 
 
 class Configuration:
     """A class for specifying the configuration of an actor.
 
@@ -63,49 +63,49 @@
             proxy_port (str, optional): The port of Apify Proxy.
             proxy_status_url (str, optional): The URL on which the Apify Proxy status page is available.
             purge_on_start (str, optional): Whether the actor should purge its default storages on startup, when running locally.
             token (str, optional): The API token for the Apify API this actor should use.
             system_info_interval_millis (str, optional): How often should the actor emit the SYSTEM_INFO event when running locally.
         """
         # TODO: Document all these members
-        self.actor_build_id = _fetch_and_parse_env_var(ApifyEnvVars.ACTOR_BUILD_ID)
-        self.actor_build_number = _fetch_and_parse_env_var(ApifyEnvVars.ACTOR_BUILD_NUMBER)
-        self.actor_events_ws_url = _fetch_and_parse_env_var(ApifyEnvVars.ACTOR_EVENTS_WS_URL)
-        self.actor_id = _fetch_and_parse_env_var(ApifyEnvVars.ACTOR_ID)
-        self.actor_run_id = _fetch_and_parse_env_var(ApifyEnvVars.ACTOR_RUN_ID)
-        self.actor_task_id = _fetch_and_parse_env_var(ApifyEnvVars.ACTOR_TASK_ID)
+        self.actor_build_id = _fetch_and_parse_env_var(ActorEnvVars.BUILD_ID)
+        self.actor_build_number = _fetch_and_parse_env_var(ActorEnvVars.BUILD_NUMBER)
+        self.actor_events_ws_url = _fetch_and_parse_env_var(ActorEnvVars.EVENTS_WEBSOCKET_URL)
+        self.actor_id = _fetch_and_parse_env_var(ActorEnvVars.ID)
+        self.actor_run_id = _fetch_and_parse_env_var(ActorEnvVars.RUN_ID)
+        self.actor_task_id = _fetch_and_parse_env_var(ActorEnvVars.TASK_ID)
         self.api_base_url = api_base_url or _fetch_and_parse_env_var(ApifyEnvVars.API_BASE_URL, 'https://api.apify.com')
         self.api_public_base_url = api_public_base_url or _fetch_and_parse_env_var(ApifyEnvVars.API_PUBLIC_BASE_URL, 'https://api.apify.com')
         self.chrome_executable_path = _fetch_and_parse_env_var(ApifyEnvVars.CHROME_EXECUTABLE_PATH)
-        self.container_port = container_port or _fetch_and_parse_env_var(ApifyEnvVars.CONTAINER_PORT, 4321)
-        self.container_url = container_url or _fetch_and_parse_env_var(ApifyEnvVars.CONTAINER_URL, 'http://localhost:4321')
+        self.container_port = container_port or _fetch_and_parse_env_var(ActorEnvVars.WEB_SERVER_PORT, 4321)
+        self.container_url = container_url or _fetch_and_parse_env_var(ActorEnvVars.WEB_SERVER_URL, 'http://localhost:4321')
         self.dedicated_cpus = _fetch_and_parse_env_var(ApifyEnvVars.DEDICATED_CPUS)
         self.default_browser_path = _fetch_and_parse_env_var(ApifyEnvVars.DEFAULT_BROWSER_PATH)
-        self.default_dataset_id = default_dataset_id or _fetch_and_parse_env_var(ApifyEnvVars.DEFAULT_DATASET_ID, 'default')
-        self.default_key_value_store_id = default_key_value_store_id or _fetch_and_parse_env_var(ApifyEnvVars.DEFAULT_KEY_VALUE_STORE_ID, 'default')
-        self.default_request_queue_id = default_request_queue_id or _fetch_and_parse_env_var(ApifyEnvVars.DEFAULT_REQUEST_QUEUE_ID, 'default')
+        self.default_dataset_id = default_dataset_id or _fetch_and_parse_env_var(ActorEnvVars.DEFAULT_DATASET_ID, 'default')
+        self.default_key_value_store_id = default_key_value_store_id or _fetch_and_parse_env_var(ActorEnvVars.DEFAULT_KEY_VALUE_STORE_ID, 'default')
+        self.default_request_queue_id = default_request_queue_id or _fetch_and_parse_env_var(ActorEnvVars.DEFAULT_REQUEST_QUEUE_ID, 'default')
         self.disable_browser_sandbox = _fetch_and_parse_env_var(ApifyEnvVars.DISABLE_BROWSER_SANDBOX, False)
         self.headless = _fetch_and_parse_env_var(ApifyEnvVars.HEADLESS, True)
-        self.input_key = input_key or _fetch_and_parse_env_var(ApifyEnvVars.INPUT_KEY, 'INPUT')
+        self.input_key = input_key or _fetch_and_parse_env_var(ActorEnvVars.INPUT_KEY, 'INPUT')
         self.input_secrets_private_key_file = _fetch_and_parse_env_var(ApifyEnvVars.INPUT_SECRETS_PRIVATE_KEY_FILE)
         self.input_secrets_private_key_passphrase = _fetch_and_parse_env_var(ApifyEnvVars.INPUT_SECRETS_PRIVATE_KEY_PASSPHRASE)
         self.is_at_home = _fetch_and_parse_env_var(ApifyEnvVars.IS_AT_HOME, False)
         self.max_used_cpu_ratio = max_used_cpu_ratio or _fetch_and_parse_env_var(ApifyEnvVars.MAX_USED_CPU_RATIO, 0.95)
-        self.memory_mbytes = _fetch_and_parse_env_var(ApifyEnvVars.MEMORY_MBYTES)
+        self.memory_mbytes = _fetch_and_parse_env_var(ActorEnvVars.MEMORY_MBYTES)
         self.meta_origin = _fetch_and_parse_env_var(ApifyEnvVars.META_ORIGIN)
         self.metamorph_after_sleep_millis = metamorph_after_sleep_millis or _fetch_and_parse_env_var(ApifyEnvVars.METAMORPH_AFTER_SLEEP_MILLIS, 300000)  # noqa: E501
         self.persist_state_interval_millis = persist_state_interval_millis or _fetch_and_parse_env_var(ApifyEnvVars.PERSIST_STATE_INTERVAL_MILLIS, 60000)  # noqa: E501
         self.persist_storage = persist_storage or _fetch_and_parse_env_var(ApifyEnvVars.PERSIST_STORAGE, True)
         self.proxy_hostname = proxy_hostname or _fetch_and_parse_env_var(ApifyEnvVars.PROXY_HOSTNAME, 'proxy.apify.com')
         self.proxy_password = proxy_password or _fetch_and_parse_env_var(ApifyEnvVars.PROXY_PASSWORD)
         self.proxy_port = proxy_port or _fetch_and_parse_env_var(ApifyEnvVars.PROXY_PORT, 8000)
         self.proxy_status_url = proxy_status_url or _fetch_and_parse_env_var(ApifyEnvVars.PROXY_STATUS_URL, 'http://proxy.apify.com')
         self.purge_on_start = purge_on_start or _fetch_and_parse_env_var(ApifyEnvVars.PURGE_ON_START, False)
-        self.started_at = _fetch_and_parse_env_var(ApifyEnvVars.STARTED_AT)
-        self.timeout_at = _fetch_and_parse_env_var(ApifyEnvVars.TIMEOUT_AT)
+        self.started_at = _fetch_and_parse_env_var(ActorEnvVars.STARTED_AT)
+        self.timeout_at = _fetch_and_parse_env_var(ActorEnvVars.TIMEOUT_AT)
         self.token = token or _fetch_and_parse_env_var(ApifyEnvVars.TOKEN)
         self.user_id = _fetch_and_parse_env_var(ApifyEnvVars.USER_ID)
         self.xvfb = _fetch_and_parse_env_var(ApifyEnvVars.XVFB, False)
         self.system_info_interval_millis = system_info_interval_millis or _fetch_and_parse_env_var(ApifyEnvVars.SYSTEM_INFO_INTERVAL_MILLIS, 60000)
 
     @classmethod
     def _get_default_instance(cls) -> 'Configuration':
```

### Comparing `apify-1.1.2b1/src/apify/consts.py` & `apify-1.1.2b2/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/event_manager.py` & `apify-1.1.2b2/src/apify/event_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import contextlib
 import inspect
 import json
 from collections import defaultdict
 from typing import Any, Callable, Coroutine, Dict, List, Optional, Set, Union
 
 import websockets.client
 from pyee.asyncio import AsyncIOEventEmitter
@@ -196,18 +197,16 @@
 
         if timeout_secs:
             _, pending = await asyncio.wait([asyncio.create_task(_wait_for_listeners())], timeout=timeout_secs)
             if pending:
                 logger.warning('Timed out waiting for event listeners to complete, unfinished event listeners will be canceled')
                 for pending_task in pending:
                     pending_task.cancel()
-                    try:
+                    with contextlib.suppress(asyncio.CancelledError):
                         await pending_task
-                    except asyncio.CancelledError:
-                        pass
         else:
             await _wait_for_listeners()
 
     async def _process_platform_messages(self) -> None:
         # This should be called only on the platform, where we have the ACTOR_EVENTS_WS_URL configured
         assert self._config.actor_events_ws_url is not None
         assert self._connected_to_platform_websocket is not None
```

### Comparing `apify-1.1.2b1/src/apify/log.py` & `apify-1.1.2b2/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/proxy_configuration.py` & `apify-1.1.2b2/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/storages/base_storage.py` & `apify-1.1.2b2/src/apify/storages/base_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,17 +127,16 @@
             cached_storage = cls._cache_by_name.get(name)
 
         if cached_storage is not None:
             # This cast is needed since MyPy doesn't understand very well that Self and Storage are the same
             return cast(Self, cached_storage)
 
         # Purge default storages if configured
-        if used_config.purge_on_start:
-            if isinstance(used_client, MemoryStorageClient):
-                await used_client._purge_on_start()
+        if used_config.purge_on_start and isinstance(used_client, MemoryStorageClient):
+            await used_client._purge_on_start()
 
         assert cls._storage_creating_lock is not None
         async with cls._storage_creating_lock:
             # Create the storage
             if id and not is_default_storage_on_local:
                 single_storage_client = cls._get_single_storage_client(id, used_client)
                 storage_info = await single_storage_client.get()
```

### Comparing `apify-1.1.2b1/src/apify/storages/dataset.py` & `apify-1.1.2b2/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/storages/key_value_store.py` & `apify-1.1.2b2/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/storages/request_queue.py` & `apify-1.1.2b2/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify/storages/storage_client_manager.py` & `apify-1.1.2b2/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify.egg-info/PKG-INFO` & `apify-1.1.2b2/src/apify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.1.2b1
+Version: 1.1.2b2
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.1.2b1/src/apify.egg-info/SOURCES.txt` & `apify-1.1.2b2/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.1.2b1/src/apify.egg-info/requires.txt` & `apify-1.1.2b2/src/apify.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 aiofiles>=22.1.0
 aioshutil>=1.0
-apify-client>=1.3.1
-apify-shared>=1.0.0
+apify-client==1.3.1
+apify-shared==1.0.2
 colorama>=0.4.6
 cryptography>=39.0.0
 httpx>=0.24.1
 psutil>=5.9.5
 pyee>=9.0.0
 sortedcollections>=2.0.1
 typing-extensions>=4.1.0
@@ -22,14 +22,15 @@
 flake8-datetimez~=20.10.0
 flake8-docstrings~=1.7.0
 flake8-encodings~=0.5.0
 flake8-isort~=6.0.0
 flake8-noqa~=1.3.1
 flake8-pytest-style~=1.7.2
 flake8-quotes~=3.3.2
+flake8-simplify~=0.20.0
 flake8-unused-arguments~=0.0.13
 isort~=5.12.0
 mypy~=1.3.0
 pep8-naming~=0.13.3
 pre-commit~=3.3.2
 pytest~=7.3.1
 pytest-asyncio~=0.21.0
```


# Comparing `tmp/DlmEngineUpdater-0.1.0.tar.gz` & `tmp/DlmEngineUpdater-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DlmEngineUpdater-0.1.0.tar", last modified: Wed Aug  2 09:04:35 2023, max compression
+gzip compressed data, was "DlmEngineUpdater-0.1.1.tar", last modified: Wed Aug  2 14:07:33 2023, max compression
```

## Comparing `DlmEngineUpdater-0.1.0.tar` & `DlmEngineUpdater-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/
-drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      750 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/PKG-INFO
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      309 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/SOURCES.txt
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)        1 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/dependency_links.txt
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       23 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/requires.txt
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       19 2023-08-02 09:04:35.000000 DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/top_level.txt
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     1084 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/LICENSE.txt
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       56 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/MANIFEST.in
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      750 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/PKG-INFO
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     4513 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/README.md
-drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/contrib/
--rwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)       98 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.0/contrib/dlm_engine_updater
-drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/dlm_engine_updater/
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)    20373 2023-08-02 09:04:26.000000 DlmEngineUpdater-0.1.0/dlm_engine_updater/__init__.py
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       67 2023-08-02 09:04:35.395892 DlmEngineUpdater-0.1.0/setup.cfg
--rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     1102 2023-08-02 07:17:39.000000 DlmEngineUpdater-0.1.0/setup.py
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 14:07:33.429930 DlmEngineUpdater-0.1.1/
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 14:07:33.428930 DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      750 2023-08-02 14:07:33.000000 DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/PKG-INFO
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      309 2023-08-02 14:07:33.000000 DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/SOURCES.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)        1 2023-08-02 14:07:33.000000 DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/dependency_links.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       23 2023-08-02 14:07:33.000000 DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/requires.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       19 2023-08-02 14:07:33.000000 DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/top_level.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     1084 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.1/LICENSE.txt
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       56 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.1/MANIFEST.in
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)      750 2023-08-02 14:07:33.429930 DlmEngineUpdater-0.1.1/PKG-INFO
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     4513 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.1/README.md
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 14:07:33.428930 DlmEngineUpdater-0.1.1/contrib/
+-rwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)       98 2022-07-27 09:11:12.000000 DlmEngineUpdater-0.1.1/contrib/dlm_engine_updater
+drwxr-xr-x   0 sschultchen (1207048288) domain users (646200513)        0 2023-08-02 14:07:33.429930 DlmEngineUpdater-0.1.1/dlm_engine_updater/
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)    20649 2023-08-02 13:46:47.000000 DlmEngineUpdater-0.1.1/dlm_engine_updater/__init__.py
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)       67 2023-08-02 14:07:33.429930 DlmEngineUpdater-0.1.1/setup.cfg
+-rw-r--r--   0 sschultchen (1207048288) domain users (646200513)     1102 2023-08-02 14:07:19.000000 DlmEngineUpdater-0.1.1/setup.py
```

### Comparing `DlmEngineUpdater-0.1.0/DlmEngineUpdater.egg-info/PKG-INFO` & `DlmEngineUpdater-0.1.1/DlmEngineUpdater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DlmEngineUpdater
-Version: 0.1.0
+Version: 0.1.1
 Summary: DlmEngine, distributed lock implementation on top of MongoDB and Redis
 Home-page: https://github.com/schlitzered/DlmEngineUpdater
 Author: schlitzer
 Author-email: stephan.schultchen@gmail.com
 License: MIT
 Keywords: dlm,distributes lock engine updater
 Platform: posix
```

### Comparing `DlmEngineUpdater-0.1.0/LICENSE.txt` & `DlmEngineUpdater-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `DlmEngineUpdater-0.1.0/PKG-INFO` & `DlmEngineUpdater-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DlmEngineUpdater
-Version: 0.1.0
+Version: 0.1.1
 Summary: DlmEngine, distributed lock implementation on top of MongoDB and Redis
 Home-page: https://github.com/schlitzered/DlmEngineUpdater
 Author: schlitzer
 Author-email: stephan.schultchen@gmail.com
 License: MIT
 Keywords: dlm,distributes lock engine updater
 Platform: posix
```

### Comparing `DlmEngineUpdater-0.1.0/README.md` & `DlmEngineUpdater-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `DlmEngineUpdater-0.1.0/dlm_engine_updater/__init__.py` & `DlmEngineUpdater-0.1.1/dlm_engine_updater/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,18 +213,22 @@
             json=self.payload_acquire,
             timeout=10.0,
             url=self.lock_url,
         )
         if not resp.status_code == 200:
             self.log.info("lock currently not present in the system")
             return
-
-        if not resp.json()['acquired_by'] == socket.getfqdn():
-            self.log.info(f"lock is currently acquired by {resp.json()['acquired_by']}")
-            return
+        if self.api_version == "1":
+            if not resp.json()['data']['acquired_by'] == socket.getfqdn():
+                self.log.info(f"lock is currently acquired by {resp.json()['acquired_by']}")
+                return
+        elif self.api_version == "2":
+            if not resp.json()['acquired_by'] == socket.getfqdn():
+                self.log.info(f"lock is currently acquired by {resp.json()['acquired_by']}")
+                return
 
         self.log.info("lock has been already acquired by this instance")
         return True
 
     def release(self):
         self.log.info(f"trying to release: {self.lock_url}")
         retries = 10
```

### Comparing `DlmEngineUpdater-0.1.0/setup.py` & `DlmEngineUpdater-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='DlmEngineUpdater',
-    version='0.1.0',
+    version='0.1.1',
     description='DlmEngine, distributed lock implementation on top of MongoDB and Redis',
     long_description="""
 DLMEngine implements a restful interface that can be used to implement distributed locks.
 
 The main intention was to orchestrate automated system updates, so only one server at a time will do a update.
 
 Copyright (c) 2023, Stephan Schultchen.
```


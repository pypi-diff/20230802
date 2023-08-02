# Comparing `tmp/integration-wetsuits-0.0.0.tar.gz` & `tmp/integration-wetsuits-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "integration-wetsuits-0.0.0.tar", last modified: Fri Jul 14 09:40:54 2023, max compression
+gzip compressed data, was "integration-wetsuits-0.0.1.tar", last modified: Wed Aug  2 10:04:19 2023, max compression
```

## Comparing `integration-wetsuits-0.0.0.tar` & `integration-wetsuits-0.0.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:40:54.417421 integration-wetsuits-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 09:40:54.417421 integration-wetsuits-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-14 09:40:33.000000 integration-wetsuits-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 09:40:54.417421 integration-wetsuits-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:40:54.417421 integration-wetsuits-0.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:40:33.000000 integration-wetsuits-0.0.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:40:54.417421 integration-wetsuits-0.0.0/src/integration_wetsuits.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-14 09:40:54.000000 integration-wetsuits-0.0.0/src/integration_wetsuits.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-07-14 09:40:54.000000 integration-wetsuits-0.0.0/src/integration_wetsuits.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:40:54.000000 integration-wetsuits-0.0.0/src/integration_wetsuits.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-14 09:40:54.000000 integration-wetsuits-0.0.0/src/integration_wetsuits.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-14 09:40:54.000000 integration-wetsuits-0.0.0/src/integration_wetsuits.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-07-14 09:40:33.000000 integration-wetsuits-0.0.0/src/itsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/src/edi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:04:19.038341 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-02 10:04:19.000000 integration-wetsuits-0.0.1/src/integration_wetsuits.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-08-02 10:03:55.000000 integration-wetsuits-0.0.1/src/itsp.py
```

### Comparing `integration-wetsuits-0.0.0/pyproject.toml` & `integration-wetsuits-0.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "integration-wetsuits"
-version = "0.0.0"
+version = "0.0.1"
 authors= [
     { name="Name", email="info@wetsuits.com" }
 ]
 description = "integration"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `integration-wetsuits-0.0.0/src/itsp.py` & `integration-wetsuits-0.0.1/src/itsp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 import requests
 import clappform
 import clappform.dataclasses as cldc
 import pandas as pd
+import json
 
 class Itsperfect:
     id=None
 
     def __init__(self, url, token, version = "v2"):
         self.url = url
         self.token = token
         self.version = version
 
-    def setFullUrl(self, category):
-        url = f"https://{self.url}/api/{self.version}/{category}/&token={self.token}"
+    def setFullUrl(self, category, id = "", subject = "", filter = ""):
+        if id != "":
+            id = f"/{id}"
+
+        if subject != "":
+            subject = f"/{subject}"
+
+        if filter != "":
+            filter = f"&filter={filter}"
+
+        url = f"https://{self.url}/api/{self.version}/{category}{id}{subject}/&token={self.token}{filter}"
         return url
     
     def getAllPicks(self):
         fullUrl = self.setFullUrl("picks")
         r = requests.get(fullUrl)
         return r.json()
     
@@ -40,30 +50,42 @@
         except clappform.exceptions.HTTPError as exc:
             print(exc.response.text)
 
     def readPicks(self, clp):
         pipeline = {
             "app": "import_database",
             "collection": "picks",
-
-            "pipeline": [{
-                "type": "raw",
-                "stages": [{"$limit": 200}]
-            }, {
-                "type": "fix_sort"
-            }],
+            "pipeline": [],
             "limit": 500
         }
 
         try:
             aggregateResults = pd.DataFrame([])
             for batch in clp.aggregate_dataframe(pipeline):
                 aggregateResults = pd.concat(
                     [aggregateResults, batch], ignore_index=True, sort=False)
         except clappform.exceptions.HTTPError as exc:
             print(exc.response.text)
             print(exc.request.body)
 
         return aggregateResults
+    
+    def getOne(self, keyName, id, subject = "", filter= ""):
+        result = []
+        fullUrl = self.setFullUrl(keyName, id, subject, filter)
+
+        if subject != "":
+            keyName = subject
+
+        response = requests.get(fullUrl)
+        if response.status_code == 200:
+                pageItems = response.json()[keyName]
+                result.extend(pageItems)
+        else:
+            # Handle unsuccessful API response
+            print(f"Failed to fetch data from URL: {fullUrl}")
+        return result
 
-
+    def getAll(self, keyname):
+        return ""
+
```


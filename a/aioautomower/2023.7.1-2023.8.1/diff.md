# Comparing `tmp/aioautomower-2023.7.1.tar.gz` & `tmp/aioautomower-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioautomower-2023.7.1.tar", last modified: Fri Jul 14 17:03:37 2023, max compression
+gzip compressed data, was "aioautomower-2023.8.1.tar", last modified: Wed Aug  2 20:59:23 2023, max compression
```

## Comparing `aioautomower-2023.7.1.tar` & `aioautomower-2023.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/aioautomower/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/aioautomower/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/aioautomower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-14 17:03:37.000000 aioautomower-2023.7.1/aioautomower.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:03:37.734685 aioautomower-2023.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-14 17:03:19.000000 aioautomower-2023.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:59:23.252729 aioautomower-2023.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-08-02 20:59:23.248729 aioautomower-2023.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:59:23.248729 aioautomower-2023.8.1/aioautomower/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/aioautomower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/aioautomower/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/aioautomower/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/aioautomower/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17600 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/aioautomower/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:59:23.248729 aioautomower-2023.8.1/aioautomower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-08-02 20:59:23.000000 aioautomower-2023.8.1/aioautomower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-08-02 20:59:23.000000 aioautomower-2023.8.1/aioautomower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:59:23.000000 aioautomower-2023.8.1/aioautomower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 20:59:23.000000 aioautomower-2023.8.1/aioautomower.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 20:59:23.000000 aioautomower-2023.8.1/aioautomower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 20:59:23.000000 aioautomower-2023.8.1/aioautomower.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:59:23.252729 aioautomower-2023.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-08-02 20:59:10.000000 aioautomower-2023.8.1/setup.py
```

### Comparing `aioautomower-2023.7.1/LICENSE` & `aioautomower-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.1/PKG-INFO` & `aioautomower-2023.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2023.7.1
+Version: 2023.8.1
 Summary: module to communicate to Husqvarna Automower API
 Home-page: https://github.com/Thomas55555/aioautomower
 Author: Thomas Protzner
 Author-email: thomas.protzner@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aioautomower-2023.7.1/README.md` & `aioautomower-2023.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.1/aioautomower/cli.py` & `aioautomower-2023.8.1/aioautomower/cli.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.1/aioautomower/const.py` & `aioautomower-2023.8.1/aioautomower/const.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.1/aioautomower/rest.py` & `aioautomower-2023.8.1/aioautomower/rest.py`

 * *Files identical despite different names*

### Comparing `aioautomower-2023.7.1/aioautomower/session.py` & `aioautomower-2023.8.1/aioautomower/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -238,14 +238,27 @@
 
     def _update_data(self, j):
         if self.data is None:
             _LOGGER.error("Failed to update data with ws response (no data)")
             return
         for datum in self.data["data"]:
             if datum["type"] == "mower" and datum["id"] == j["id"]:
+                if j["type"] == "positions-event":
+                    last_pos_identical = (
+                        datum["attributes"]["positions"][0]
+                        == j["attributes"]["positions"][0]
+                    )
+                    if not last_pos_identical:
+                        j["attributes"]["positions"].extend(
+                            datum["attributes"]["positions"]
+                        )
+                        _LOGGER.debug(
+                            "j['attributes']['positions']: %s",
+                            j["attributes"]["positions"],
+                        )
                 for attrib in j["attributes"]:
                     try:
                         tasks = j["attributes"]["calendar"]["tasks"]
                         if len(tasks) == 0:
                             temp_task = datum["attributes"]["calendar"]["tasks"]
                             datum["attributes"][attrib] = j["attributes"][attrib]
                             datum["attributes"]["calendar"]["tasks"] = temp_task
```

### Comparing `aioautomower-2023.7.1/aioautomower.egg-info/PKG-INFO` & `aioautomower-2023.8.1/aioautomower.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioautomower
-Version: 2023.7.1
+Version: 2023.8.1
 Summary: module to communicate to Husqvarna Automower API
 Home-page: https://github.com/Thomas55555/aioautomower
 Author: Thomas Protzner
 Author-email: thomas.protzner@gmail.com
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aioautomower-2023.7.1/setup.py` & `aioautomower-2023.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,12 +15,12 @@
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     install_requires=list(val.strip() for val in open("requirements.txt")),
-    version="2023.7.1",
+    version="2023.8.1",
     entry_points={
         "console_scripts": ["automower=aioautomower.cli:main"],
     },
 )
```


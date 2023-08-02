# Comparing `tmp/shipper-shippy-2.18.2.tar.gz` & `tmp/shipper-shippy-2.18.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-2.18.2.tar", last modified: Tue Aug  1 23:57:23 2023, max compression
+gzip compressed data, was "shipper-shippy-2.18.3.tar", last modified: Wed Aug  2 00:05:42 2023, max compression
```

## Comparing `shipper-shippy-2.18.2.tar` & `shipper-shippy-2.18.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:23.891934 shipper-shippy-2.18.2/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/shippy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/server_compat_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 00:05:42.000000 shipper-shippy-2.18.3/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:42.807285 shipper-shippy-2.18.3/shippy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 00:05:28.000000 shipper-shippy-2.18.3/shippy/version.py
```

### Comparing `shipper-shippy-2.18.2/PKG-INFO` & `shipper-shippy-2.18.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.18.2
+Version: 2.18.3
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.18.2/README.md` & `shipper-shippy-2.18.3/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.2/setup.py` & `shipper-shippy-2.18.3/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.2/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-2.18.3/shipper_shippy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.18.2
+Version: 2.18.3
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.18.2/shippy/__main__.py` & `shipper-shippy-2.18.3/shippy/__main__.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.2/shippy/client.py` & `shipper-shippy-2.18.3/shippy/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     RATE_LIMIT_MSG,
     UNKNOWN_UPLOAD_ERROR_MSG,
     UNKNOWN_UPLOAD_START_ERROR_MSG,
     WAITING_FINALIZATION_MSG,
     CHUNK_SIZE,
 )
 from .exceptions import LoginException, UploadException
-from .version import server_compat_version, __version__
+from .version import __version__
+from .server_compat_version import server_compat_version
 
 console = Console()
 
 # Set up progress bar
 progress = Progress(
     TextColumn("[progress.description]{task.description}"),
     BarColumn(),
```

### Comparing `shipper-shippy-2.18.2/shippy/config.py` & `shipper-shippy-2.18.3/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.2/shippy/constants.py` & `shipper-shippy-2.18.3/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.2/shippy/helper.py` & `shipper-shippy-2.18.3/shippy/helper.py`

 * *Files identical despite different names*


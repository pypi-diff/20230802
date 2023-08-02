# Comparing `tmp/shipper-shippy-2.18.1.tar.gz` & `tmp/shipper-shippy-2.18.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipper-shippy-2.18.1.tar", last modified: Thu Jul 27 01:36:44 2023, max compression
+gzip compressed data, was "shipper-shippy-2.18.2.tar", last modified: Tue Aug  1 23:57:23 2023, max compression
```

## Comparing `shipper-shippy-2.18.1.tar` & `shipper-shippy-2.18.2.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:36:44.901526 shipper-shippy-2.18.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-27 01:36:44.901526 shipper-shippy-2.18.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 01:36:44.901526 shipper-shippy-2.18.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:36:44.901526 shipper-shippy-2.18.1/shipper_shippy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-27 01:36:44.000000 shipper-shippy-2.18.1/shipper_shippy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-27 01:36:44.000000 shipper-shippy-2.18.1/shipper_shippy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 01:36:44.000000 shipper-shippy-2.18.1/shipper_shippy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-27 01:36:44.000000 shipper-shippy-2.18.1/shipper_shippy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-27 01:36:44.000000 shipper-shippy-2.18.1/shipper_shippy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-27 01:36:44.000000 shipper-shippy-2.18.1/shipper_shippy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 01:36:44.901526 shipper-shippy-2.18.1/shippy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-27 01:36:27.000000 shipper-shippy-2.18.1/shippy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:23.891934 shipper-shippy-2.18.2/shipper_shippy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 23:57:23.000000 shipper-shippy-2.18.2/shipper_shippy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:23.895934 shipper-shippy-2.18.2/shippy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2413 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/server_compat_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-01 23:57:15.000000 shipper-shippy-2.18.2/shippy/version.py
```

### Comparing `shipper-shippy-2.18.1/PKG-INFO` & `shipper-shippy-2.18.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.18.1
+Version: 2.18.2
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.18.1/README.md` & `shipper-shippy-2.18.2/README.md`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.1/setup.py` & `shipper-shippy-2.18.2/setup.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.1/shipper_shippy.egg-info/PKG-INFO` & `shipper-shippy-2.18.2/shipper_shippy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipper-shippy
-Version: 2.18.1
+Version: 2.18.2
 Summary: Client-side tool to interface with shipper
 Home-page: https://github.com/ericswpark/shippy
 Author: Eric Park
 Author-email: me@ericswpark.com
 Project-URL: Bug Tracker, https://github.com/ericswpark/shippy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shipper-shippy-2.18.1/shippy/__main__.py` & `shipper-shippy-2.18.2/shippy/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     FAILED_TO_LOG_IN_ERROR_MSG,
     CANNOT_CONTACT_SERVER_ERROR_MSG,
     PRERELEASE_WARNING_MSG,
     NO_CONFIGURATION_WARNING_MSG,
 )
 from .exceptions import LoginException, UploadException
 from .helper import input_yn, print_error, print_warning, print_success
-from .version import __version__, server_compat_version
+from .version import __version__
+from .server_compat_version import server_compat_version
 
 sentry_sdk.init(
     SENTRY_SDK_URL,
     traces_sample_rate=1.0,
     release=__version__,
     ignore_errors=[ConnectionError],
 )
```

### Comparing `shipper-shippy-2.18.1/shippy/client.py` & `shipper-shippy-2.18.2/shippy/client.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.1/shippy/config.py` & `shipper-shippy-2.18.2/shippy/config.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.1/shippy/constants.py` & `shipper-shippy-2.18.2/shippy/constants.py`

 * *Files identical despite different names*

### Comparing `shipper-shippy-2.18.1/shippy/helper.py` & `shipper-shippy-2.18.2/shippy/helper.py`

 * *Files identical despite different names*


# Comparing `tmp/edx-i18n-tools-1.0.0.tar.gz` & `tmp/edx-i18n-tools-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edx-i18n-tools-1.0.0.tar", last modified: Fri Jul  7 13:15:28 2023, max compression
+gzip compressed data, was "edx-i18n-tools-1.1.0.tar", last modified: Wed Aug  2 18:11:26 2023, max compression
```

## Comparing `edx-i18n-tools-1.0.0.tar` & `edx-i18n-tools-1.1.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5721 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.820283 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      749 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      531 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       46 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-07 13:15:28.000000 edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/i18n/
--rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/branch_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/changed.py
--rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     8965 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/dummy.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/execute.py
--rw-r--r--   0 runner    (1001) docker     (122)    10143 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)     7953 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/generate.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1431 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/main.py
--rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/segment.py
--rw-r--r--   0 runner    (1001) docker     (122)     5532 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/transifex.py
--rw-r--r--   0 runner    (1001) docker     (122)     9864 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/i18n/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      101 2023-07-07 13:15:28.824283 edx-i18n-tools-1.0.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     2199 2023-07-07 13:15:21.000000 edx-i18n-tools-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:11:26.525539 edx-i18n-tools-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-08-02 18:11:26.525539 edx-i18n-tools-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5721 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:11:26.521539 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      749 2023-08-02 18:11:26.000000 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      531 2023-08-02 18:11:26.000000 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-02 18:11:26.000000 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       46 2023-08-02 18:11:26.000000 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-08-02 18:11:26.000000 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-08-02 18:11:26.000000 edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:11:26.525539 edx-i18n-tools-1.1.0/i18n/
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/branch_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1416 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/changed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4031 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8965 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/execute.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10143 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7953 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/generate.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1431 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/main.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5573 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/segment.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5532 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/transifex.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9864 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/i18n/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 18:11:26.525539 edx-i18n-tools-1.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       88 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      101 2023-08-02 18:11:26.529539 edx-i18n-tools-1.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2199 2023-08-02 18:11:21.000000 edx-i18n-tools-1.1.0/setup.py
```

### Comparing `edx-i18n-tools-1.0.0/LICENSE.txt` & `edx-i18n-tools-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/NOTICE.txt` & `edx-i18n-tools-1.1.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/PKG-INFO` & `edx-i18n-tools-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-i18n-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: edX Internationalization Tools
 Home-page: https://github.com/openedx/i18n-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edx-i18n-tools-1.0.0/README.rst` & `edx-i18n-tools-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/PKG-INFO` & `edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edx-i18n-tools
-Version: 1.0.0
+Version: 1.1.0
 Summary: edX Internationalization Tools
 Home-page: https://github.com/openedx/i18n-tools
 Author: edX
 Author-email: oscm@edx.org
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `edx-i18n-tools-1.0.0/edx_i18n_tools.egg-info/SOURCES.txt` & `edx-i18n-tools-1.1.0/edx_i18n_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/__init__.py` & `edx-i18n-tools-1.1.0/i18n/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Tool to be used by other IDAs for internationalization.
 """
 import argparse
 import sys
 
 from . import config
 
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 
 
 class Runner:
     """
     Runner class for internationalization.
     """
     def __init__(self):
```

### Comparing `edx-i18n-tools-1.0.0/i18n/branch_cleanup.py` & `edx-i18n-tools-1.1.0/i18n/branch_cleanup.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/changed.py` & `edx-i18n-tools-1.1.0/i18n/changed.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/config.py` & `edx-i18n-tools-1.1.0/i18n/config.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/converter.py` & `edx-i18n-tools-1.1.0/i18n/converter.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/dummy.py` & `edx-i18n-tools-1.1.0/i18n/dummy.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/execute.py` & `edx-i18n-tools-1.1.0/i18n/execute.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/extract.py` & `edx-i18n-tools-1.1.0/i18n/extract.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/generate.py` & `edx-i18n-tools-1.1.0/i18n/generate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/main.py` & `edx-i18n-tools-1.1.0/i18n/main.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/segment.py` & `edx-i18n-tools-1.1.0/i18n/segment.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/transifex.py` & `edx-i18n-tools-1.1.0/i18n/transifex.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/i18n/validate.py` & `edx-i18n-tools-1.1.0/i18n/validate.py`

 * *Files identical despite different names*

### Comparing `edx-i18n-tools-1.0.0/setup.py` & `edx-i18n-tools-1.1.0/setup.py`

 * *Files identical despite different names*


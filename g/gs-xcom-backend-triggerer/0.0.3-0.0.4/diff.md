# Comparing `tmp/gs_xcom_backend_triggerer-0.0.3.tar.gz` & `tmp/gs_xcom_backend_triggerer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs_xcom_backend_triggerer-0.0.3.tar", last modified: Tue Aug  1 05:33:08 2023, max compression
+gzip compressed data, was "gs_xcom_backend_triggerer-0.0.4.tar", last modified: Wed Aug  2 11:54:55 2023, max compression
```

## Comparing `gs_xcom_backend_triggerer-0.0.3.tar` & `gs_xcom_backend_triggerer-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 05:33:08.130306 gs_xcom_backend_triggerer-0.0.3/
--rw-rw-rw-   0        0        0      536 2023-08-01 05:33:08.129256 gs_xcom_backend_triggerer-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 05:33:08.092982 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/
--rw-rw-rw-   0        0        0        0 2023-08-01 04:44:48.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/__init__.py
--rw-rw-rw-   0        0        0     1289 2023-08-01 05:25:23.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/triggerer.py
-drwxrwxrwx   0        0        0        0 2023-08-01 05:33:08.127228 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/
--rw-rw-rw-   0        0        0      536 2023-08-01 05:33:07.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-08-01 05:33:08.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 05:33:07.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 05:33:07.000000 gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 05:33:08.130306 gs_xcom_backend_triggerer-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      841 2023-08-01 05:33:04.000000 gs_xcom_backend_triggerer-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:54:55.152614 gs_xcom_backend_triggerer-0.0.4/
+-rw-rw-rw-   0        0        0      536 2023-08-02 11:54:55.151614 gs_xcom_backend_triggerer-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 11:54:55.128643 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/
+-rw-rw-rw-   0        0        0        0 2023-08-01 04:44:48.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-08-02 11:49:05.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/deferrer.py
+-rw-rw-rw-   0        0        0     1289 2023-08-01 05:25:23.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/triggerer.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:54:55.149439 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/
+-rw-rw-rw-   0        0        0      536 2023-08-02 11:54:54.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2023-08-02 11:54:55.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:54:54.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 11:54:54.000000 gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 11:54:55.153609 gs_xcom_backend_triggerer-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      841 2023-08-02 11:54:46.000000 gs_xcom_backend_triggerer-0.0.4/setup.py
```

### Comparing `gs_xcom_backend_triggerer-0.0.3/PKG-INFO` & `gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend_triggerer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gs_xcom_backend_triggerer
-Version: 0.0.3
+Name: gs-xcom-backend-triggerer
+Version: 0.0.4
 Summary: triggerer gs_xcom_backend module file
 Author: imvj202
 Author-email: imvj202@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend/triggerer.py` & `gs_xcom_backend_triggerer-0.0.4/gs_xcom_backend/triggerer.py`

 * *Files identical despite different names*

### Comparing `gs_xcom_backend_triggerer-0.0.3/gs_xcom_backend_triggerer.egg-info/PKG-INFO` & `gs_xcom_backend_triggerer-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: gs-xcom-backend-triggerer
-Version: 0.0.3
+Name: gs_xcom_backend_triggerer
+Version: 0.0.4
 Summary: triggerer gs_xcom_backend module file
 Author: imvj202
 Author-email: imvj202@gmail.com
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
```

### Comparing `gs_xcom_backend_triggerer-0.0.3/setup.py` & `gs_xcom_backend_triggerer-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'triggerer gs_xcom_backend module file'
 LONG_DESCRIPTION = 'triggerer gs_xcom_backend module file'
 
 # Setting up
 setup(
     name="gs_xcom_backend_triggerer",
     version=VERSION,
```


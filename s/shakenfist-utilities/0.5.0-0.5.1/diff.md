# Comparing `tmp/shakenfist-utilities-0.5.0.tar.gz` & `tmp/shakenfist-utilities-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shakenfist-utilities-0.5.0.tar", last modified: Wed May 31 09:25:03 2023, max compression
+gzip compressed data, was "shakenfist-utilities-0.5.1.tar", last modified: Wed Aug  2 07:28:53 2023, max compression
```

## Comparing `shakenfist-utilities-0.5.0.tar` & `shakenfist-utilities-0.5.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/AUTHORS
--rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/LICENSE
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      877 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      168 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/README.md
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      866 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/release.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       82 2022-08-07 23:15:20.000000 shakenfist-utilities-0.5.0/requirements.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      652 2023-05-31 09:25:03.754668 shakenfist-utilities-0.5.0/setup.cfg
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      964 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/setup.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/shakenfist_utilities/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/__init__.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     5009 2022-08-08 05:08:58.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/api.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)     6467 2023-05-31 09:24:40.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/logs.py
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      187 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/random.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/shakenfist_utilities/tests/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/shakenfist_utilities/tests/__init__.py
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      877 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      583 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/not-zip-safe
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/pbr.json
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       39 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/requires.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)       21 2023-05-31 09:25:03.000000 shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/top_level.txt
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      138 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/test-requirements.txt
-drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-05-31 09:25:03.750668 shakenfist-utilities-0.5.0/tools/
--rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/tools/flake8wrap.sh
--rw-rw-r--   0 parallels  (1000) parallels  (1000)      624 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.0/tox.ini
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-08-02 07:28:53.024647 shakenfist-utilities-0.5.1/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       34 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/AUTHORS
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)    11357 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/LICENSE
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      827 2023-08-02 07:28:53.024647 shakenfist-utilities-0.5.1/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      168 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/README.md
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      866 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/release.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       82 2022-08-07 23:15:20.000000 shakenfist-utilities-0.5.1/requirements.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      613 2023-08-02 07:28:53.024647 shakenfist-utilities-0.5.1/setup.cfg
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      964 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/setup.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-08-02 07:28:53.020648 shakenfist-utilities-0.5.1/shakenfist_utilities/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/shakenfist_utilities/__init__.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     5009 2022-08-08 05:08:58.000000 shakenfist-utilities-0.5.1/shakenfist_utilities/api.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)     6467 2023-05-31 09:24:40.000000 shakenfist-utilities-0.5.1/shakenfist_utilities/logs.py
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      187 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/shakenfist_utilities/random.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-08-02 07:28:53.024647 shakenfist-utilities-0.5.1/shakenfist_utilities/tests/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        0 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/shakenfist_utilities/tests/__init__.py
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-08-02 07:28:53.024647 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      827 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      583 2023-08-02 07:28:53.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)        1 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/not-zip-safe
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       46 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/pbr.json
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       39 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/requires.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)       21 2023-08-02 07:28:52.000000 shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/top_level.txt
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      138 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/test-requirements.txt
+drwxrwxr-x   0 parallels  (1000) parallels  (1000)        0 2023-08-02 07:28:53.024647 shakenfist-utilities-0.5.1/tools/
+-rwxrwxr-x   0 parallels  (1000) parallels  (1000)      580 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/tools/flake8wrap.sh
+-rw-rw-r--   0 parallels  (1000) parallels  (1000)      624 2022-08-06 06:52:50.000000 shakenfist-utilities-0.5.1/tox.ini
```

### Comparing `shakenfist-utilities-0.5.0/LICENSE` & `shakenfist-utilities-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/PKG-INFO` & `shakenfist-utilities-0.5.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-utilities
-Version: 0.5.0
+Version: 0.5.1
 Summary: Shaken Fist utility libraries
 Home-page: https://github.com/shakenfist/library-utilities
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: # Shaken Fist Utilities
         
@@ -15,9 +15,8 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `shakenfist-utilities-0.5.0/release.sh` & `shakenfist-utilities-0.5.1/release.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/setup.cfg` & `shakenfist-utilities-0.5.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 classifier = 
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
 
 [files]
 packages = 
 	shakenfist_utilities
 
 [pbr]
 skip_changelog = True
```

### Comparing `shakenfist-utilities-0.5.0/setup.py` & `shakenfist-utilities-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/shakenfist_utilities/api.py` & `shakenfist-utilities-0.5.1/shakenfist_utilities/api.py`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/shakenfist_utilities/logs.py` & `shakenfist-utilities-0.5.1/shakenfist_utilities/logs.py`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/PKG-INFO` & `shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shakenfist-utilities
-Version: 0.5.0
+Version: 0.5.1
 Summary: Shaken Fist utility libraries
 Home-page: https://github.com/shakenfist/library-utilities
 Author: Michael Still
 Author-email: mikal@stillhq.com
 License: Apache2
 Description: # Shaken Fist Utilities
         
@@ -15,9 +15,8 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Description-Content-Type: text/markdown
```

### Comparing `shakenfist-utilities-0.5.0/shakenfist_utilities.egg-info/SOURCES.txt` & `shakenfist-utilities-0.5.1/shakenfist_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/tools/flake8wrap.sh` & `shakenfist-utilities-0.5.1/tools/flake8wrap.sh`

 * *Files identical despite different names*

### Comparing `shakenfist-utilities-0.5.0/tox.ini` & `shakenfist-utilities-0.5.1/tox.ini`

 * *Files identical despite different names*


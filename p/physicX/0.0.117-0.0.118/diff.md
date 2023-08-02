# Comparing `tmp/physicX-0.0.117.tar.gz` & `tmp/physicX-0.0.118.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "physicX-0.0.117.tar", last modified: Mon Jul 17 23:18:44 2023, max compression
+gzip compressed data, was "physicX-0.0.118.tar", last modified: Wed Aug  2 03:38:05 2023, max compression
```

## Comparing `physicX-0.0.117.tar` & `physicX-0.0.118.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-07-17 23:18:44.550597 physicX-0.0.117/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      829 2023-07-17 23:18:44.550597 physicX-0.0.117/PKG-INFO
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      263 2023-07-17 23:02:33.000000 physicX-0.0.117/README.md
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      771 2023-07-17 23:18:27.000000 physicX-0.0.117/pyproject.toml
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-07-17 23:02:33.000000 physicX-0.0.117/requirements.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       38 2023-07-17 23:18:44.550597 physicX-0.0.117/setup.cfg
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-07-17 23:18:44.547263 physicX-0.0.117/src/
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-07-17 23:18:44.547263 physicX-0.0.117/src/physicX/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       50 2023-07-17 23:02:33.000000 physicX-0.0.117/src/physicX/__init__.py
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      381 2023-07-17 23:02:33.000000 physicX-0.0.117/src/physicX/constants.py
-drwxr-xr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-07-17 23:18:44.547263 physicX-0.0.117/src/physicX.egg-info/
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      829 2023-07-17 23:18:44.000000 physicX-0.0.117/src/physicX.egg-info/PKG-INFO
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)      264 2023-07-17 23:18:44.000000 physicX-0.0.117/src/physicX.egg-info/SOURCES.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)        1 2023-07-17 23:18:44.000000 physicX-0.0.117/src/physicX.egg-info/dependency_links.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)       31 2023-07-17 23:18:44.000000 physicX-0.0.117/src/physicX.egg-info/requires.txt
--rw-r--r--   0 cunknown  (1000) cunknown  (1000)        8 2023-07-17 23:18:44.000000 physicX-0.0.117/src/physicX.egg-info/top_level.txt
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:38:05.047491 physicX-0.0.118/
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      829 2023-08-02 03:38:05.047491 physicX-0.0.118/PKG-INFO
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      263 2023-08-02 03:10:34.000000 physicX-0.0.118/README.md
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      771 2023-08-02 03:37:33.000000 physicX-0.0.118/pyproject.toml
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       31 2023-08-02 03:10:34.000000 physicX-0.0.118/requirements.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       38 2023-08-02 03:38:05.047491 physicX-0.0.118/setup.cfg
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:38:05.047491 physicX-0.0.118/src/
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:38:05.047491 physicX-0.0.118/src/physicX/
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       76 2023-08-02 03:35:22.000000 physicX-0.0.118/src/physicX/__init__.py
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      880 2023-08-02 03:33:42.000000 physicX-0.0.118/src/physicX/constants.py
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      108 2023-08-02 03:34:53.000000 physicX-0.0.118/src/physicX/law.py
+drwxrwxr-x   0 cunknown  (1000) cunknown  (1000)        0 2023-08-02 03:38:05.047491 physicX-0.0.118/src/physicX.egg-info/
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      829 2023-08-02 03:38:05.000000 physicX-0.0.118/src/physicX.egg-info/PKG-INFO
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)      283 2023-08-02 03:38:05.000000 physicX-0.0.118/src/physicX.egg-info/SOURCES.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)        1 2023-08-02 03:38:05.000000 physicX-0.0.118/src/physicX.egg-info/dependency_links.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)       31 2023-08-02 03:38:05.000000 physicX-0.0.118/src/physicX.egg-info/requires.txt
+-rw-rw-r--   0 cunknown  (1000) cunknown  (1000)        8 2023-08-02 03:38:05.000000 physicX-0.0.118/src/physicX.egg-info/top_level.txt
```

### Comparing `physicX-0.0.117/PKG-INFO` & `physicX-0.0.118/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.117
+Version: 0.0.118
 Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Other OS
```

### Comparing `physicX-0.0.117/pyproject.toml` & `physicX-0.0.118/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy>=1.24.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "physicX"
-version = "0.0.117"
+version = "0.0.118"
 authors = [
   { name="anonymous14725", email="anonymous14725@yahoo.com" },
 ]
 description = "mathematics and physics library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `physicX-0.0.117/src/physicX.egg-info/PKG-INFO` & `physicX-0.0.118/src/physicX.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: physicX
-Version: 0.0.117
+Version: 0.0.118
 Summary: mathematics and physics library
 Author-email: anonymous14725 <anonymous14725@yahoo.com>
 Project-URL: Homepage, https://github.com/anonymous14725/physicX
 Project-URL: Bug Tracker, https://github.com/anonymous14725/physicX/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: Other OS
```


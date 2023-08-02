# Comparing `tmp/setuptools_ocrd-0.0.7.tar.gz` & `tmp/setuptools_ocrd-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools_ocrd-0.0.7.tar", last modified: Tue Aug  1 18:10:54 2023, max compression
+gzip compressed data, was "setuptools_ocrd-0.0.8.tar", last modified: Tue Aug  1 18:23:17 2023, max compression
```

## Comparing `setuptools_ocrd-0.0.7.tar` & `setuptools_ocrd-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:10:54.223512 setuptools_ocrd-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 18:10:54.223512 setuptools_ocrd-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:10:54.223512 setuptools_ocrd-0.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:10:54.223512 setuptools_ocrd-0.0.7/setuptools_ocrd/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/setuptools_ocrd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/setuptools_ocrd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/setuptools_ocrd/_get_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:10:54.223512 setuptools_ocrd-0.0.7/setuptools_ocrd/_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/setuptools_ocrd/_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 18:10:43.000000 setuptools_ocrd-0.0.7/setuptools_ocrd/_integration/setuptools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:10:54.223512 setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 18:10:54.000000 setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 18:10:54.000000 setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:10:54.000000 setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 18:10:54.000000 setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 18:10:54.000000 setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:23:17.654104 setuptools_ocrd-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 18:23:17.650104 setuptools_ocrd-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 18:23:17.654104 setuptools_ocrd-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:23:17.650104 setuptools_ocrd-0.0.8/setuptools_ocrd/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/setuptools_ocrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/setuptools_ocrd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/setuptools_ocrd/_get_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:23:17.650104 setuptools_ocrd-0.0.8/setuptools_ocrd/_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/setuptools_ocrd/_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-08-01 18:23:05.000000 setuptools_ocrd-0.0.8/setuptools_ocrd/_integration/setuptools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:23:17.650104 setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-08-01 18:23:17.000000 setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-01 18:23:17.000000 setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:23:17.000000 setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-01 18:23:17.000000 setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-01 18:23:17.000000 setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/top_level.txt
```

### Comparing `setuptools_ocrd-0.0.7/LICENSE` & `setuptools_ocrd-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools_ocrd-0.0.7/PKG-INFO` & `setuptools_ocrd-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools_ocrd
-Version: 0.0.7
+Version: 0.0.8
 Summary: Manage your package version through ocrd-tool.json
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>
 Keywords: ocr-d,setuptools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `setuptools_ocrd-0.0.7/pyproject.toml` & `setuptools_ocrd-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "setuptools_ocrd"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
     {name = "Mike Gerber", email = "mike.gerber@sbb.spk-berlin.de"},
 ]
 description = "Manage your package version through ocrd-tool.json"
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["ocr-d", "setuptools"]
```

### Comparing `setuptools_ocrd-0.0.7/setuptools_ocrd/_integration/setuptools.py` & `setuptools_ocrd-0.0.8/setuptools_ocrd/_integration/setuptools.py`

 * *Files identical despite different names*

### Comparing `setuptools_ocrd-0.0.7/setuptools_ocrd.egg-info/PKG-INFO` & `setuptools_ocrd-0.0.8/setuptools_ocrd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setuptools-ocrd
-Version: 0.0.7
+Version: 0.0.8
 Summary: Manage your package version through ocrd-tool.json
 Author-email: Mike Gerber <mike.gerber@sbb.spk-berlin.de>
 Keywords: ocr-d,setuptools
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


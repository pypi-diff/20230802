# Comparing `tmp/bioio-base-0.2.0.tar.gz` & `tmp/bioio-base-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioio-base-0.2.0.tar", last modified: Tue Aug  1 14:45:07 2023, max compression
+gzip compressed data, was "bioio-base-0.3.0.tar", last modified: Wed Aug  2 17:53:36 2023, max compression
```

## Comparing `bioio-base-0.2.0.tar` & `bioio-base-0.3.0.tar`

### file list

```diff
@@ -1,50 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.369191 bioio-base-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.cookiecutter.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.361191 bioio-base-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.361191 bioio-base-0.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.365191 bioio-base-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-01 14:44:51.000000 bioio-base-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-01 14:44:51.000000 bioio-base-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-01 14:44:51.000000 bioio-base-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-01 14:44:51.000000 bioio-base-0.2.0/Justfile
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-01 14:44:51.000000 bioio-base-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 14:45:07.369191 bioio-base-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-01 14:44:51.000000 bioio-base-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.365191 bioio-base-0.2.0/bioio_base/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/dimensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/image_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/io.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29812 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/reader_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    11438 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.369191 bioio-base-0.2.0/bioio_base/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/tests/test_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)    14493 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-01 14:44:51.000000 bioio-base-0.2.0/bioio_base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.365191 bioio-base-0.2.0/bioio_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-01 14:45:07.000000 bioio-base-0.2.0/bioio_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:45:07.369191 bioio-base-0.2.0/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5377 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-01 14:44:51.000000 bioio-base-0.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-01 14:44:51.000000 bioio-base-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:45:07.369191 bioio-base-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.806386 bioio-base-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.794386 bioio-base-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.798385 bioio-base-0.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.798385 bioio-base-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-02 17:53:19.000000 bioio-base-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-08-02 17:53:19.000000 bioio-base-0.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-08-02 17:53:19.000000 bioio-base-0.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-08-02 17:53:19.000000 bioio-base-0.3.0/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-02 17:53:19.000000 bioio-base-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-02 17:53:36.802385 bioio-base-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-08-02 17:53:19.000000 bioio-base-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.802385 bioio-base-0.3.0/bioio_base/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/image_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/noop_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31072 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/reader_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11012 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.802385 bioio-base-0.3.0/bioio_base/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/tests/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15154 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14907 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-08-02 17:53:19.000000 bioio-base-0.3.0/bioio_base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.802385 bioio-base-0.3.0/bioio_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-08-02 17:53:36.000000 bioio-base-0.3.0/bioio_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-02 17:53:36.000000 bioio-base-0.3.0/bioio_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:53:36.000000 bioio-base-0.3.0/bioio_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:53:36.000000 bioio-base-0.3.0/bioio_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-08-02 17:53:36.000000 bioio-base-0.3.0/bioio_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 17:53:36.000000 bioio-base-0.3.0/bioio_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:53:36.802385 bioio-base-0.3.0/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5377 2023-08-02 17:53:19.000000 bioio-base-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 17:53:19.000000 bioio-base-0.3.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-08-02 17:53:19.000000 bioio-base-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-02 17:53:19.000000 bioio-base-0.3.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-08-02 17:53:19.000000 bioio-base-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:53:36.806386 bioio-base-0.3.0/setup.cfg
```

### Comparing `bioio-base-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `bioio-base-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `bioio-base-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `bioio-base-0.3.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/.github/workflows/ci.yml` & `bioio-base-0.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/.github/workflows/docs.yml` & `bioio-base-0.3.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/.gitignore` & `bioio-base-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/.pre-commit-config.yaml` & `bioio-base-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/CODE_OF_CONDUCT.md` & `bioio-base-0.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/CONTRIBUTING.md` & `bioio-base-0.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/Justfile` & `bioio-base-0.3.0/Justfile`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 	rm -fr htmlcov
 	rm -fr .pytest_cache
 	rm -fr .mypy_cache
 
 # install with all deps
 install:
 	pip install -e .[lint,test,docs,dev]
+	pre-commit install
 
 # lint, format, and check all files
 lint:
 	pre-commit run --all-files
 
 # run tests
 test:
```

### Comparing `bioio-base-0.2.0/LICENSE` & `bioio-base-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/PKG-INFO` & `bioio-base-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioio-base
-Version: 0.2.0
+Version: 0.3.0
 Summary: Typing, base classes, and more for BioIO projects.
 Author-email: Eva Maxfield Brown <evamaxfieldbrown@gmail.com>, Dan Toloudis <danielt@alleninstitute.org>
 License: BSD License
 Project-URL: Homepage, https://github.com/bioio-devs/bioio-base
 Project-URL: Bug Tracker, https://github.com/bioio-devs/bioio-base/issues
 Project-URL: Documentation, https://bioio-devs.github.io/bioio-base
 Project-URL: User Support, https://github.com/bioio-devs/bioio-base/issues
```

### Comparing `bioio-base-0.2.0/README.md` & `bioio-base-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/bioio_base/dimensions.py` & `bioio-base-0.3.0/bioio_base/dimensions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from collections.abc import Sequence as seq
-from typing import ItemsView, Iterable, Sequence, Tuple, Union
+from typing import Collection, ItemsView, Sequence, Tuple, Union
 
 ###############################################################################
 
 
 class DimensionNames:
     Time = "T"
     Channel = "C"
@@ -60,33 +60,47 @@
     DimensionNames.Samples,
 ]
 
 ###############################################################################
 
 
 class Dimensions:
-    def __init__(self, dims: Union[str, Iterable], shape: Tuple[int, ...]):
+    def __init__(self, dims: Collection[str], shape: Tuple[int, ...]):
         """
         A general object for managing the pairing of dimension name and dimension size.
 
         Parameters
         ----------
-        dims: Union[str, Iterable]
-            An ordered string or iterable of the dimensions to pair with their sizes.
+        dims: Collection[str]
+            An ordered string or collection of the dimensions to pair with their sizes.
         shape: Tuple[int, ...]
             An ordered tuple of the dimensions sizes to pair with their names.
 
         Examples
         --------
         >>> dims = Dimensions("TCZYX", (1, 4, 75, 624, 924))
         ... dims.X
         ... dims['T', 'X']
         """
+        # zip(strict=True) only in Python 3.10
+        # Check equal length dims and shape
+        if len(dims) != len(shape):
+            raise ValueError(
+                f"Number of dimensions provided ({len(dims)} -- '{dims}') "
+                f"does not match shape size provided ({len(shape)} -- '{shape}')."
+            )
+
         # Make dims a string
         if not isinstance(dims, str):
+            if any([len(c) != 1 for c in dims]):
+                raise ValueError(
+                    f"When providing a list of dimension strings, "
+                    f"each dimension may only be a single character long "
+                    f"(received: '{dims}')."
+                )
             dims = "".join(dims)
 
         # Store order and shape
         self._order = dims
         self._shape = shape
 
         # Create attributes
@@ -138,7 +152,14 @@
                 return tuple(self._dims_shape[k] for k in key)
             else:
                 raise IndexError(f"{', '.join(invalid_dims)} not in {self._order}")
         else:
             raise TypeError(
                 f"Key must be a string or list of strings but got type {type(key)}"
             )
+
+    def __setattr__(self, __name: str, __value: int) -> None:
+        super().__setattr__(__name, __value)
+
+    def __getattr__(self, __name: str) -> int:
+        # TODO: Py310 __match_args__ for better typing
+        return super().__getattribute__(__name)
```

### Comparing `bioio-base-0.2.0/bioio_base/exceptions.py` & `bioio-base-0.3.0/bioio_base/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from typing import Optional
 
-###############################################################################
-
 
 class ConflictingArgumentsError(Exception):
     """
-    This exception is returned when two or more arguments to the
-    same function are in conflict.
+    This exception is returned when 2 arguments to the same function are in conflict.
     """
 
 
 class InvalidDimensionOrderingError(Exception):
     """
     A general exception that can be thrown when handling dimension ordering or
     validation. Should be provided with a message for the user to be given more context.
```

### Comparing `bioio-base-0.2.0/bioio_base/image_container.py` & `bioio-base-0.3.0/bioio_base/image_container.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, Union
+from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
-if TYPE_CHECKING:
-    import dask.array as da
-    import numpy as np
-    import xarray as xr
+import dask.array as da
+import numpy as np
+import xarray as xr
 
 from .dimensions import Dimensions
 from .types import ImageLike, PhysicalPixelSizes
 
 ###############################################################################
 
 
@@ -43,35 +42,35 @@
 
     @abstractmethod
     def set_scene(self, scene_id: Union[str, int]) -> None:
         pass
 
     @property
     @abstractmethod
-    def xarray_dask_data(self) -> "xr.DataArray":
+    def xarray_dask_data(self) -> xr.DataArray:
         pass
 
     @property
     @abstractmethod
-    def xarray_data(self) -> "xr.DataArray":
+    def xarray_data(self) -> xr.DataArray:
         pass
 
     @property
     @abstractmethod
-    def dask_data(self) -> "da.Array":
+    def dask_data(self) -> da.Array:
         pass
 
     @property
     @abstractmethod
-    def data(self) -> "np.ndarray":
+    def data(self) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
-    def dtype(self) -> "np.dtype":
+    def dtype(self) -> np.dtype:
         pass
 
     @property
     @abstractmethod
     def shape(self) -> Tuple[int, ...]:
         pass
 
@@ -79,21 +78,21 @@
     @abstractmethod
     def dims(self) -> Dimensions:
         pass
 
     @abstractmethod
     def get_image_dask_data(
         self, dimension_order_out: Optional[str] = None, **kwargs: Any
-    ) -> "da.Array":
+    ) -> da.Array:
         pass
 
     @abstractmethod
     def get_image_data(
         self, dimension_order_out: Optional[str] = None, **kwargs: Any
-    ) -> "np.ndarray":
+    ) -> np.ndarray:
         pass
 
     @property
     @abstractmethod
     def metadata(self) -> Any:
         pass
```

### Comparing `bioio-base-0.2.0/bioio_base/io.py` & `bioio-base-0.3.0/bioio_base/io.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/bioio_base/reader.py` & `bioio-base-0.3.0/bioio_base/reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Dict, List, Optional, Tuple, Union
 
-if TYPE_CHECKING:
-    import dask.array as da
-    import numpy as np
-    import xarray as xr
-    from fsspec.spec import AbstractFileSystem
-    from ome_types import OME
+import dask.array as da
+import numpy as np
+import xarray as xr
+from fsspec.spec import AbstractFileSystem
+from ome_types import OME
 
-from . import constants, exceptions, io, transforms, types
+from . import constants, exceptions, transforms, types
 from .dimensions import DEFAULT_DIMENSION_ORDER, DimensionNames, Dimensions
 from .image_container import ImageContainer
+from .io import pathlike_to_fs
 from .types import PhysicalPixelSizes
 
 ###############################################################################
 
 
 class Reader(ImageContainer, ABC):
     """
@@ -35,30 +35,30 @@
 
     Notes
     -----
     It is up to the implementer of the Reader to decide which types they would like to
     accept (certain readers may not support buffers for example).
     """
 
-    _xarray_dask_data: Optional["xr.DataArray"] = None
-    _xarray_data: Optional["xr.DataArray"] = None
-    _mosaic_xarray_dask_data: Optional["xr.DataArray"] = None
-    _mosaic_xarray_data: Optional["xr.DataArray"] = None
+    _xarray_dask_data: Optional[xr.DataArray] = None
+    _xarray_data: Optional[xr.DataArray] = None
+    _mosaic_xarray_dask_data: Optional[xr.DataArray] = None
+    _mosaic_xarray_data: Optional[xr.DataArray] = None
     _dims: Optional[Dimensions] = None
     _metadata: Optional[Any] = None
     _scenes: Optional[Tuple[str, ...]] = None
     _current_scene_index: int = 0
     # Do not default because they aren't used by all readers
-    _fs: "AbstractFileSystem"
+    _fs: AbstractFileSystem
     _path: str
 
     @staticmethod
     @abstractmethod
     def _is_supported_image(
-        fs: "AbstractFileSystem",
+        fs: AbstractFileSystem,
         path: str,
         **kwargs: Any,
     ) -> bool:
         """
         The per-Reader implementation used to validate that an image is supported or not
         by the Reader itself.
 
@@ -108,15 +108,15 @@
         ------
         TypeError
             Invalid type provided to image parameter.
         """
         # Check path
         if isinstance(image, (str, Path)):
             # Expand details of provided image
-            fs, path = io.pathlike_to_fs(
+            fs, path = pathlike_to_fs(
                 image,
                 enforce_exists=True,
                 fs_kwargs=fs_kwargs,
             )
 
             return cls._is_supported_image(fs, path, **kwargs)
 
@@ -241,16 +241,16 @@
         elif isinstance(scene_id, int):
             # Only need to run when scene index is different from current scene
             if scene_id != self.current_scene_index:
                 # Validate scene index
                 if scene_id >= len(self.scenes):
                     raise IndexError(
                         f"Scene index: {scene_id} "
-                        f"is greater than the number of available scenes "
-                        f"present in the file."
+                        f"is greater than the maximum available scene index "
+                        f"({len(self.scenes) - 1}) present in the file."
                     )
 
                 # Update current scene
                 self._current_scene_index = scene_id
 
                 # Reset set for future read
                 self._reset_self()
@@ -258,15 +258,15 @@
         else:
             raise TypeError(
                 f"Must provide either a string (for scene id) "
                 f"or integer (for scene index). Provided: {scene_id} ({type(scene_id)}."
             )
 
     @abstractmethod
-    def _read_delayed(self) -> "xr.DataArray":
+    def _read_delayed(self) -> xr.DataArray:
         """
         The delayed data array constructor for the image.
 
         Returns
         -------
         data: xr.DataArray
             The fully constructed delayed DataArray.
@@ -279,15 +279,15 @@
         Requirements for the returned xr.DataArray:
         * Must have the `dims` populated.
         * If a channel dimension is present, please populate the channel dimensions
         coordinate array the respective channel coordinate values.
         """
 
     @abstractmethod
-    def _read_immediate(self) -> "xr.DataArray":
+    def _read_immediate(self) -> xr.DataArray:
         """
         The immediate data array constructor for the image.
 
         Returns
         -------
         data: xr.DataArray
             The fully read data array.
@@ -296,15 +296,15 @@
         -----
         Requirements for the returned xr.DataArray:
         * Must have the `dims` populated.
         * If a channel dimension is present, please populate the channel dimensions
         coordinate array the respective channel coordinate values.
         """
 
-    def _get_stitched_dask_mosaic(self) -> "xr.DataArray":
+    def _get_stitched_dask_mosaic(self) -> xr.DataArray:
         """
         Stitch all mosaic tiles back together and return as a single xr.DataArray with
         a delayed dask array for backing data.
 
         Returns
         -------
         mosaic: xr.DataArray
@@ -321,15 +321,15 @@
         Implementers can determine how to chunk the array.
         Most common is to chunk by tile.
         """
         raise NotImplementedError(
             "This reader does not support reconstructing mosaic images."
         )
 
-    def _get_stitched_mosaic(self) -> "xr.DataArray":
+    def _get_stitched_mosaic(self) -> xr.DataArray:
         """
         Stitch all mosaic tiles back together and return as a single xr.DataArray with
         an in-memory numpy array for backing data.
 
         Returns
         -------
         mosaic: np.ndarray
@@ -342,28 +342,28 @@
             Reader or format doesn't support reconstructing mosaic tiles.
         """
         raise NotImplementedError(
             "This reader does not support reconstructing mosaic images."
         )
 
     @property
-    def xarray_dask_data(self) -> "xr.DataArray":
+    def xarray_dask_data(self) -> xr.DataArray:
         """
         Returns
         -------
         xarray_dask_data: xr.DataArray
             The delayed image and metadata as an annotated data array.
         """
         if self._xarray_dask_data is None:
             self._xarray_dask_data = self._read_delayed()
 
         return self._xarray_dask_data
 
     @property
-    def xarray_data(self) -> "xr.DataArray":
+    def xarray_data(self) -> xr.DataArray:
         """
         Returns
         -------
         xarray_data: xr.DataArray
             The fully read image and metadata as an annotated data array.
         """
         if self._xarray_data is None:
@@ -377,35 +377,35 @@
                 coords=self._xarray_data.coords,
                 attrs=self._xarray_data.attrs,
             )
 
         return self._xarray_data
 
     @property
-    def dask_data(self) -> "da.Array":
+    def dask_data(self) -> da.Array:
         """
         Returns
         -------
         dask_data: da.Array
             The image as a dask array with the native dimension ordering.
         """
         return self.xarray_dask_data.data
 
     @property
-    def data(self) -> "np.ndarray":
+    def data(self) -> np.ndarray:
         """
         Returns
         -------
         data: np.ndarray
             The image as a numpy array with native dimension ordering.
         """
         return self.xarray_data.data
 
     @property
-    def mosaic_xarray_dask_data(self) -> "xr.DataArray":
+    def mosaic_xarray_dask_data(self) -> xr.DataArray:
         """
         Returns
         -------
         xarray_dask_data: xr.DataArray
             The delayed mosaic image and metadata as an annotated data array.
 
         Raises
@@ -427,15 +427,15 @@
         # Stitch, store, and return
         if self._mosaic_xarray_dask_data is None:
             self._mosaic_xarray_dask_data = self._get_stitched_dask_mosaic()
 
         return self._mosaic_xarray_dask_data
 
     @property
-    def mosaic_xarray_data(self) -> "xr.DataArray":
+    def mosaic_xarray_data(self) -> xr.DataArray:
         """
         Returns
         -------
         xarray_dask_data: xr.DataArray
             The in-memory mosaic image and metadata as an annotated data array.
 
         Raises
@@ -456,15 +456,15 @@
         # Stitch, store, and return
         if self._mosaic_xarray_data is None:
             self._mosaic_xarray_data = self._get_stitched_mosaic()
 
         return self._mosaic_xarray_data
 
     @property
-    def mosaic_dask_data(self) -> "da.Array":
+    def mosaic_dask_data(self) -> da.Array:
         """
         Returns
         -------
         dask_data: da.Array
             The stitched together mosaic image as a dask array.
 
         Raises
@@ -476,15 +476,15 @@
         -----
         Each reader can implement mosaic tile stitching differently but it is common
         that each tile is a dask array chunk.
         """
         return self.mosaic_xarray_dask_data.data
 
     @property
-    def mosaic_data(self) -> "np.ndarray":
+    def mosaic_data(self) -> np.ndarray:
         """
         Returns
         -------
         data: np.ndarray
             The stitched together mosaic image as a numpy array.
 
         Raises
@@ -495,15 +495,15 @@
         Notes
         -----
         Very large images should use `mosaic_dask_data` to avoid seg-faults.
         """
         return self.mosaic_xarray_data.data
 
     @property
-    def dtype(self) -> "np.dtype":
+    def dtype(self) -> np.dtype:
         """
         Returns
         -------
         dtype: np.dtype
             Data-type of the image array's elements.
         """
         return self.xarray_dask_data.dtype
@@ -529,15 +529,15 @@
         if self._dims is None:
             self._dims = Dimensions(dims=self.xarray_dask_data.dims, shape=self.shape)
 
         return self._dims
 
     def get_image_dask_data(
         self, dimension_order_out: Optional[str] = None, **kwargs: Any
-    ) -> "da.Array":
+    ) -> da.Array:
         """
         Get specific dimension image data out of an image as a dask array.
 
         Parameters
         ----------
         dimension_order_out: Optional[str]
             A string containing the dimension ordering desired for the returned ndarray.
@@ -606,15 +606,15 @@
             given_dims=self.dims.order,
             return_dims=dimension_order_out,
             **kwargs,
         )
 
     def get_image_data(
         self, dimension_order_out: Optional[str] = None, **kwargs: Any
-    ) -> "np.ndarray":
+    ) -> np.ndarray:
         """
         Read the image as a numpy array then return specific dimension image data.
 
         Parameters
         ----------
         dimension_order_out: Optional[str]
             A string containing the dimension ordering desired for the returned ndarray.
@@ -710,15 +710,15 @@
                 self._metadata = self.xarray_dask_data.attrs[
                     constants.METADATA_UNPROCESSED
                 ]
 
         return self._metadata
 
     @property
-    def ome_metadata(self) -> "OME":
+    def ome_metadata(self) -> OME:
         """
         Returns
         -------
         metadata: OME
             The original metadata transformed into the OME specfication.
             This likely isn't a complete transformation but is guarenteed to
             be a valid transformation.
@@ -743,15 +743,15 @@
             return list(self.xarray_dask_data[DimensionNames.Channel].values)
 
         return None
 
     @staticmethod
     def _generate_coord_array(
         start: Union[int, float], stop: Union[int, float], step_size: Union[int, float]
-    ) -> "np.ndarray":
+    ) -> np.ndarray:
         """
         Generate an np.ndarray for coordinate values.
 
         Parameters
         ----------
         start: Union[int, float]
             The start value.
@@ -788,24 +788,30 @@
         -----
         We currently do not handle unit attachment to these values. Please see the file
         metadata for unit information.
         """
         return PhysicalPixelSizes(None, None, None)
 
     def get_mosaic_tile_position(
-        self, mosaic_tile_index: int
-    ) -> Optional[Tuple[int, int]]:
+        self, mosaic_tile_index: int, **kwargs: int
+    ) -> Tuple[int, int]:
         """
         Get the absolute position of the top left point for a single mosaic tile.
-        Returns None if the image is not a mosaic.
 
         Parameters
         ----------
         mosaic_tile_index: int
             The index for the mosaic tile to retrieve position information for.
+        kwargs: int
+            The keywords below allow you to specify the dimensions that you wish
+            to match. If you under-specify the constraints you can easily
+            end up with a massive image stack.
+                       Z = 1   # The Z-dimension.
+                       C = 2   # The C-dimension ("channel").
+                       T = 3   # The T-dimension ("time").
 
         Returns
         -------
         top: int
             The Y coordinate for the tile position.
         left: int
             The X coordinate for the tile position.
@@ -815,29 +821,56 @@
         UnexpectedShapeError
             The image has no mosaic dimension available.
         IndexError
             No matching mosaic tile index found.
         """
         raise NotImplementedError()
 
+    def get_mosaic_tile_positions(self, **kwargs: int) -> List[Tuple[int, int]]:
+        """
+        Get the absolute positions of the top left points for each mosaic tile
+        matching the specified dimensions and current scene.
+
+        Parameters
+        ----------
+        kwargs: int
+            The keywords below allow you to specify the dimensions that you wish
+            to match. If you under-specify the constraints you can easily
+            end up with a massive image stack.
+                       Z = 1   # The Z-dimension.
+                       C = 2   # The C-dimension ("channel").
+                       T = 3   # The T-dimension ("time").
+
+        Returns
+        -------
+        mosaic_tile_positions: List[Tuple[int, int]]
+            List of the Y and X coordinate for the tile positions.
+
+        Raises
+        ------
+        UnexpectedShapeError
+            The image has no mosaic dimension available.
+        """
+        raise NotImplementedError()
+
     @property
     def mosaic_tile_dims(self) -> Optional[Dimensions]:
         """
         Returns
         -------
         tile_dims: Optional[Dimensions]
             The dimensions for each tile in the mosaic image.
             If the image is not a mosaic image, returns None.
         """
         if DimensionNames.MosaicTile in self.dims.order:
-            return Dimensions("YX", (self.dims.Y, self.dims.X))  # type: ignore
+            return Dimensions("YX", (self.dims.Y, self.dims.X))
 
         return None
 
-    def get_stack(self, **kwargs: Any) -> "np.ndarray":
+    def get_stack(self, **kwargs: Any) -> np.ndarray:
         """
         Get all scenes stacked in to a single array.
 
         Returns
         -------
         stack: np.ndarray
             The fully stacked array. This can be 6+ dimensions with Scene being
@@ -849,15 +882,15 @@
         See Also
         --------
         aicsimageio.transforms.generate_stack:
             Underlying function for generating various scene stacks.
         """
         return transforms.generate_stack(self, mode="data", **kwargs)
 
-    def get_dask_stack(self, **kwargs: Any) -> "da.Array":
+    def get_dask_stack(self, **kwargs: Any) -> da.Array:
         """
         Get all scenes stacked in to a single array.
 
         Returns
         -------
         stack: da.Array
             The fully stacked array. This can be 6+ dimensions with Scene being
@@ -869,15 +902,15 @@
         See Also
         --------
         aicsimageio.transforms.generate_stack:
             Underlying function for generating various scene stacks.
         """
         return transforms.generate_stack(self, mode="dask_data", **kwargs)
 
-    def get_xarray_stack(self, **kwargs: Any) -> "xr.DataArray":
+    def get_xarray_stack(self, **kwargs: Any) -> xr.DataArray:
         """
         Get all scenes stacked in to a single array.
 
 
         Returns
         -------
         stack: xr.DataArray
@@ -895,15 +928,15 @@
         Notes
         -----
         When requesting an xarray stack, the first scene's coordinate planes
         are used for the returned xarray DataArray object coordinate planes.
         """
         return transforms.generate_stack(self, mode="xarray_data", **kwargs)
 
-    def get_xarray_dask_stack(self, **kwargs: Any) -> "xr.DataArray":
+    def get_xarray_dask_stack(self, **kwargs: Any) -> xr.DataArray:
         """
         Get all scenes stacked in to a single array.
 
         Returns
         -------
         stack: xr.DataArray
             The fully stacked array. This can be 6+ dimensions with Scene being
```

### Comparing `bioio-base-0.2.0/bioio_base/test_utilities.py` & `bioio-base-0.3.0/bioio_base/test_utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,14 @@
     assert image_container.physical_pixel_sizes == expected_physical_pixel_sizes
     assert isinstance(image_container.metadata, expected_metadata_type)
 
     # Read different chunks
     zyx_chunk_from_delayed = image_container.get_image_dask_data("ZYX").compute()
     cyx_chunk_from_delayed = image_container.get_image_dask_data("CYX").compute()
 
-    # Check image still not fully in memory
-    assert image_container.xarray_data is None
-
     # Read in mem then pull chunks
     zyx_chunk_from_mem = image_container.get_image_data("ZYX")
     cyz_chunk_from_mem = image_container.get_image_data("CYX")
 
     # Compare chunk reads
     np.testing.assert_array_equal(
         zyx_chunk_from_delayed,
@@ -226,19 +223,14 @@
 
     check_local_file_not_open(image_container)
     check_can_serialize_image_container(image_container)
 
     # Change scene
     image_container.set_scene(second_scene_id)
 
-    # Check data was reset
-    assert image_container.xarray_dask_data is None
-    assert image_container.xarray_data is None
-    assert image_container.dims is None
-
     # Check basics
     if isinstance(second_scene_id, str):
         assert image_container.current_scene == second_scene_id
     else:
         assert image_container.current_scene_index == second_scene_id
     assert image_container.shape == second_scene_shape
     assert image_container.dtype == second_scene_dtype
@@ -302,19 +294,14 @@
     check_can_serialize_image_container(image_container)
 
     # Change scene
     image_container.set_scene(1)
 
     assert image_container.current_scene_index == 1
 
-    # Check data was reset
-    assert image_container.xarray_dask_data is None
-    assert image_container.xarray_data is None
-    assert image_container.dims is None
-
     # Check basics
     if isinstance(second_scene_id, str):
         assert image_container.current_scene == second_scene_id
     else:
         assert image_container.current_scene_index == second_scene_id
     assert image_container.dtype == second_scene_dtype
```

### Comparing `bioio-base-0.2.0/bioio_base/transforms.py` & `bioio-base-0.3.0/bioio_base/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,41 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import annotations
 
 from collections import Counter
-from typing import Any, Literal, Optional, Union
+from typing import Any, List, Literal, Optional, Tuple, Union
 
 import dask.array as da
 import numpy as np
 import xarray as xr
 
 from . import types
 from .exceptions import ConflictingArgumentsError, UnexpectedShapeError
 from .image_container import ImageContainer
 
 ###############################################################################
 
 
+def reduce_to_slice(L: Union[List, Tuple]) -> Union[int, List, slice, Tuple]:
+    # if the list only has one element, then just use it
+    if len(L) == 1:
+        return slice(L[0], L[0] + 1)
+    # if the list has at least 2 elements we can check for sliceable
+    # it is convertable to a slice if the step size between each
+    # consecutive pair of elements is equal and positive
+    # 1. get all the deltas in a list:
+    steps = [(L[i + 1] - L[i]) for i in range(len(L) - 1)]
+    # 2. check if all the deltas are equal and positive
+    if steps[0] > 0 and steps.count(steps[0]) == len(steps):
+        return slice(min(L), max(L) + 1, steps[0])
+    # if we can't convert to a slice, then just return the list unmodified
+    return L
+
+
 def transpose_to_dims(
     data: types.ArrayLike,
     given_dims: str,
     return_dims: str,
 ) -> types.ArrayLike:
     """
     This shuffles the data dimensions from given_dims to return_dims. Each dimension
@@ -152,25 +168,14 @@
     Selections, empty dimension expansions, and dimension order shuffle
 
     >>> data = np.random.rand((10, 100, 100))
     ... example = reshape_data(data, "CYX", "BSTCZYX", C=slice(0, -1, 3))
     """
     # Check for parameter conflicts
     for dim in given_dims:
-        # return_dims='TCZYX' and fixed dimensions 'C=1'
-        # Dimension is in kwargs
-        # Dimension is an integer
-        # Dimension is in return dimensions
-        if isinstance(kwargs.get(dim), int) and dim in return_dims:
-            raise ConflictingArgumentsError(
-                f"When selecting a single dimension index, the specified dimension can "
-                f"not be provided in return_dims. "
-                f"return_dims={return_dims}, dimension {dim} = {kwargs.get(dim)}"
-            )
-
         # return_dims='CZYX' and iterable dimensions 'T=range(10)'
         # Dimension is in kwargs
         # Dimension is an iterable
         # Dimension is not in return dimensions
         if (
             isinstance(kwargs.get(dim), (list, tuple, range, slice))
             and dim not in return_dims
@@ -184,47 +189,52 @@
     # Process each dimension available
     new_dims = given_dims
     dim_specs = []
     for dim in given_dims:
         # Store index of the dim as it is in given data
         dim_index = given_dims.index(dim)
 
-        # Handle dim in return dims which means that it is
+        # Handle dim in return_dims which means that it is
         # an iterable or None selection
         if dim in return_dims:
             # Specific iterable requested
             if dim in kwargs:
                 # Actual dim specification
                 # The specification provided for this dimension in the kwargs
                 dim_spec = kwargs.get(dim)
                 display_dim_spec = dim_spec
 
+                if isinstance(dim_spec, int):
+                    dim_spec = slice(dim_spec, dim_spec + 1)
+
                 # Convert operator to standard list or slice
                 # dask.Array and numpy.ndarray both natively support
                 # List[int] and slices being passed to getitem so no need to cast them
                 # to anything different
                 if isinstance(dim_spec, (tuple, range)):
                     dim_spec = list(dim_spec)
 
                 # Get the largest absolute value index in the list using min and max
                 if isinstance(dim_spec, list):
                     check_selection_max = max([abs(min(dim_spec)), max(dim_spec)])
+                    # try to convert to slice if possible
+                    dim_spec = reduce_to_slice(dim_spec)
 
                 # Get the largest absolute value index from start and stop of slice
                 if isinstance(dim_spec, slice):
                     check_selection_max = max([abs(dim_spec.stop), abs(dim_spec.start)])
             else:
                 # Nothing was requested from this dimension
                 dim_spec = slice(None, None, None)
                 display_dim_spec = dim_spec
 
                 # No op means that it doesn't matter how much data is in this dimension
                 check_selection_max = 0
 
-        # Not in given dims means that it is a fixed integer selection
+        # Not in return_dims means that it is a fixed integer selection
         else:
             if dim in kwargs:
                 # Integer requested
                 dim_spec = kwargs.get(dim)
                 display_dim_spec = dim_spec
 
                 # Check that integer
@@ -268,15 +278,15 @@
     image_container: ImageContainer,
     mode: Literal["data", "dask_data", "xarray_data", "xarray_dask_data"],
     drop_non_matching_scenes: bool = False,
     select_scenes: Optional[
         Union[list[Union[str, int]], tuple[Union[str, int], ...]]
     ] = None,
     scene_character: str = "I",
-    scene_coord_values: Literal["index", "names"] = "index",
+    scene_coord_values: str = "index",
 ) -> types.MetaArrayLike:
     """
     Stack each scene contained in the reader into a
     single array. This method handles the logic of determining which
     stack function to use (dask or numpy) and whether or not to return a
     labelled array (xr.DataArray). Users should prefer
     to use one of get_stack, get_dask_stack, get_xarray_stack, or
@@ -297,15 +307,15 @@
         as a list or tuple of scene indices or names. It is recommended to
         use the scene integer index instead of the scene name to avoid
         duplicate scene name lookup issues.
         Default: None (stack all scenes)
     scene_character: str
         Character to use as the name of the scene dimension on the output
         array. Default "I"
-    scene_coord_values: Literal["index", "names"]
+    scene_coord_values : str
         How to assign coordinates to the scene dimension of the final
         array. If scene_coord_values="names" use the scene name from
         the reader object. If scene_coord_values="index" don't attach any
         coordinates and fall back to integer values.
         Default: "index"
 
     Returns
```

### Comparing `bioio-base-0.2.0/bioio_base/types.py` & `bioio-base-0.3.0/bioio_base/types.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/bioio_base.egg-info/PKG-INFO` & `bioio-base-0.3.0/bioio_base.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioio-base
-Version: 0.2.0
+Version: 0.3.0
 Summary: Typing, base classes, and more for BioIO projects.
 Author-email: Eva Maxfield Brown <evamaxfieldbrown@gmail.com>, Dan Toloudis <danielt@alleninstitute.org>
 License: BSD License
 Project-URL: Homepage, https://github.com/bioio-devs/bioio-base
 Project-URL: Bug Tracker, https://github.com/bioio-devs/bioio-base/issues
 Project-URL: Documentation, https://bioio-devs.github.io/bioio-base
 Project-URL: User Support, https://github.com/bioio-devs/bioio-base/issues
```

### Comparing `bioio-base-0.2.0/docs/conf.py` & `bioio-base-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/docs/installation.rst` & `bioio-base-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `bioio-base-0.2.0/pyproject.toml` & `bioio-base-0.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Natural Language :: English",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 dynamic = ["version"]
 dependencies = [
-  "dask>=2021.4.1,!=2022.5.1",
+  "dask[array,distributed]>=2021.4.1,!=2022.5.1",
   "fsspec>=2021.4.0,!=2022.7.0",
   "numpy~=1.16",
   "ome-types>=0.2",
   "xarray>=2022.6.0",
 ]
 
 [project.urls]
```


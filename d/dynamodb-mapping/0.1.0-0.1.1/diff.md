# Comparing `tmp/dynamodb_mapping-0.1.0.tar.gz` & `tmp/dynamodb_mapping-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynamodb_mapping-0.1.0.tar", last modified: Tue Aug  1 15:09:52 2023, max compression
+gzip compressed data, was "dynamodb_mapping-0.1.1.tar", last modified: Wed Aug  2 07:41:48 2023, max compression
```

## Comparing `dynamodb_mapping-0.1.0.tar` & `dynamodb_mapping-0.1.1.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.304660 dynamodb_mapping-0.1.0/
--rw-r--r--   0 janos      (502) staff       (20)      164 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/AUTHORS.rst
--rw-r--r--   0 janos      (502) staff       (20)     3604 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 janos      (502) staff       (20)       89 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/HISTORY.rst
--rw-r--r--   0 janos      (502) staff       (20)     1073 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/LICENSE
--rw-r--r--   0 janos      (502) staff       (20)      262 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/MANIFEST.in
--rw-r--r--   0 janos      (502) staff       (20)     6352 2023-08-01 15:09:52.304745 dynamodb_mapping-0.1.0/PKG-INFO
--rw-r--r--   0 janos      (502) staff       (20)     5511 2023-07-28 16:58:21.000000 dynamodb_mapping-0.1.0/README.rst
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.302989 dynamodb_mapping-0.1.0/docs/
--rw-r--r--   0 janos      (502) staff       (20)      614 2023-07-28 15:11:12.000000 dynamodb_mapping-0.1.0/docs/Makefile
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.300537 dynamodb_mapping-0.1.0/docs/_build/
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.300585 dynamodb_mapping-0.1.0/docs/_build/html/
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.303316 dynamodb_mapping-0.1.0/docs/_build/html/_static/
--rw-r--r--   0 janos      (502) staff       (20)      286 2023-07-28 15:16:48.000000 dynamodb_mapping-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0 janos      (502) staff       (20)       90 2023-07-28 15:16:48.000000 dynamodb_mapping-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 janos      (502) staff       (20)       90 2023-07-28 15:16:48.000000 dynamodb_mapping-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 janos      (502) staff       (20)       28 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/docs/authors.rst
--rwxr-xr-x   0 janos      (502) staff       (20)     5574 2023-07-31 15:23:54.000000 dynamodb_mapping-0.1.0/docs/conf.py
--rw-r--r--   0 janos      (502) staff       (20)       33 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/docs/contributing.rst
--rw-r--r--   0 janos      (502) staff       (20)       28 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/docs/history.rst
--rw-r--r--   0 janos      (502) staff       (20)      294 2023-07-31 12:37:55.000000 dynamodb_mapping-0.1.0/docs/index.rst
--rw-r--r--   0 janos      (502) staff       (20)      814 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/docs/make.bat
--rw-r--r--   0 janos      (502) staff       (20)      124 2023-07-31 15:55:30.000000 dynamodb_mapping-0.1.0/docs/modules.rst
--rw-r--r--   0 janos      (502) staff       (20)       27 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/docs/readme.rst
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.303547 dynamodb_mapping-0.1.0/dynamodb_mapping/
--rw-r--r--   0 janos      (502) staff       (20)      341 2023-08-01 14:30:48.000000 dynamodb_mapping-0.1.0/dynamodb_mapping/__init__.py
--rw-r--r--   0 janos      (502) staff       (20)    23733 2023-08-01 14:30:48.000000 dynamodb_mapping-0.1.0/dynamodb_mapping/dynamodb_mapping.py
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.304312 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/
--rw-r--r--   0 janos      (502) staff       (20)     6352 2023-08-01 15:09:52.000000 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/PKG-INFO
--rw-r--r--   0 janos      (502) staff       (20)      691 2023-08-01 15:09:52.000000 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/SOURCES.txt
--rw-r--r--   0 janos      (502) staff       (20)        1 2023-08-01 15:09:52.000000 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/dependency_links.txt
--rw-r--r--   0 janos      (502) staff       (20)        1 2023-08-01 15:09:52.000000 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/not-zip-safe
--rw-r--r--   0 janos      (502) staff       (20)        6 2023-08-01 15:09:52.000000 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/requires.txt
--rw-r--r--   0 janos      (502) staff       (20)       17 2023-08-01 15:09:52.000000 dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/top_level.txt
--rw-r--r--   0 janos      (502) staff       (20)      453 2023-08-01 15:09:52.305580 dynamodb_mapping-0.1.0/setup.cfg
--rw-r--r--   0 janos      (502) staff       (20)     1365 2023-08-01 14:55:55.000000 dynamodb_mapping-0.1.0/setup.py
-drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-01 15:09:52.304561 dynamodb_mapping-0.1.0/tests/
--rw-r--r--   0 janos      (502) staff       (20)       46 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.0/tests/__init__.py
--rw-r--r--   0 janos      (502) staff       (20)     5902 2023-08-01 14:32:42.000000 dynamodb_mapping-0.1.0/tests/test_dynamodb_mapping.py
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.856819 dynamodb_mapping-0.1.1/
+-rw-r--r--   0 janos      (502) staff       (20)      164 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/AUTHORS.rst
+-rw-r--r--   0 janos      (502) staff       (20)     3604 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 janos      (502) staff       (20)       89 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/HISTORY.rst
+-rw-r--r--   0 janos      (502) staff       (20)     1073 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/LICENSE
+-rw-r--r--   0 janos      (502) staff       (20)      262 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/MANIFEST.in
+-rw-r--r--   0 janos      (502) staff       (20)     6225 2023-08-02 07:41:48.856909 dynamodb_mapping-0.1.1/PKG-INFO
+-rw-r--r--   0 janos      (502) staff       (20)     5384 2023-08-01 15:43:33.000000 dynamodb_mapping-0.1.1/README.rst
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.852935 dynamodb_mapping-0.1.1/docs/
+-rw-r--r--   0 janos      (502) staff       (20)      614 2023-07-28 15:11:12.000000 dynamodb_mapping-0.1.1/docs/Makefile
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.847756 dynamodb_mapping-0.1.1/docs/_build/
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.847862 dynamodb_mapping-0.1.1/docs/_build/html/
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.853870 dynamodb_mapping-0.1.1/docs/_build/html/_static/
+-rw-r--r--   0 janos      (502) staff       (20)      286 2023-07-28 15:16:48.000000 dynamodb_mapping-0.1.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 janos      (502) staff       (20)       90 2023-07-28 15:16:48.000000 dynamodb_mapping-0.1.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 janos      (502) staff       (20)       90 2023-07-28 15:16:48.000000 dynamodb_mapping-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 janos      (502) staff       (20)       28 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 janos      (502) staff       (20)     5574 2023-07-31 15:23:54.000000 dynamodb_mapping-0.1.1/docs/conf.py
+-rw-r--r--   0 janos      (502) staff       (20)       33 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/docs/contributing.rst
+-rw-r--r--   0 janos      (502) staff       (20)       28 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/docs/history.rst
+-rw-r--r--   0 janos      (502) staff       (20)      294 2023-07-31 12:37:55.000000 dynamodb_mapping-0.1.1/docs/index.rst
+-rw-r--r--   0 janos      (502) staff       (20)      814 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/docs/make.bat
+-rw-r--r--   0 janos      (502) staff       (20)      124 2023-07-31 15:55:30.000000 dynamodb_mapping-0.1.1/docs/modules.rst
+-rw-r--r--   0 janos      (502) staff       (20)       27 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/docs/readme.rst
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.855285 dynamodb_mapping-0.1.1/dynamodb_mapping/
+-rw-r--r--   0 janos      (502) staff       (20)      341 2023-08-02 07:35:14.000000 dynamodb_mapping-0.1.1/dynamodb_mapping/__init__.py
+-rw-r--r--   0 janos      (502) staff       (20)    23733 2023-08-01 14:30:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping/dynamodb_mapping.py
+-rw-r--r--   0 janos      (502) staff       (20)        0 2023-08-02 07:32:56.000000 dynamodb_mapping-0.1.1/dynamodb_mapping/py.typed
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.856106 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/
+-rw-r--r--   0 janos      (502) staff       (20)     6225 2023-08-02 07:41:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/PKG-INFO
+-rw-r--r--   0 janos      (502) staff       (20)      717 2023-08-02 07:41:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/SOURCES.txt
+-rw-r--r--   0 janos      (502) staff       (20)        1 2023-08-02 07:41:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/dependency_links.txt
+-rw-r--r--   0 janos      (502) staff       (20)        1 2023-08-02 07:41:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/not-zip-safe
+-rw-r--r--   0 janos      (502) staff       (20)        6 2023-08-02 07:41:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/requires.txt
+-rw-r--r--   0 janos      (502) staff       (20)       17 2023-08-02 07:41:48.000000 dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/top_level.txt
+-rw-r--r--   0 janos      (502) staff       (20)      453 2023-08-02 07:41:48.857910 dynamodb_mapping-0.1.1/setup.cfg
+-rw-r--r--   0 janos      (502) staff       (20)     1418 2023-08-02 07:35:14.000000 dynamodb_mapping-0.1.1/setup.py
+drwxr-xr-x   0 janos      (502) staff       (20)        0 2023-08-02 07:41:48.856530 dynamodb_mapping-0.1.1/tests/
+-rw-r--r--   0 janos      (502) staff       (20)       46 2023-07-28 14:22:05.000000 dynamodb_mapping-0.1.1/tests/__init__.py
+-rw-r--r--   0 janos      (502) staff       (20)     5902 2023-08-01 14:32:42.000000 dynamodb_mapping-0.1.1/tests/test_dynamodb_mapping.py
```

### Comparing `dynamodb_mapping-0.1.0/CONTRIBUTING.rst` & `dynamodb_mapping-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dynamodb_mapping-0.1.0/LICENSE` & `dynamodb_mapping-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamodb_mapping-0.1.0/PKG-INFO` & `dynamodb_mapping-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamodb_mapping
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python dictionary-like interface for an Amazon DynamoDB table.
 Home-page: https://github.com/mrtj/dynamodb_mapping
 Author: Janos Tolgyesi
 Author-email: janos.tolgyesi@gmail.com
 License: MIT license
 Keywords: dynamodb_mapping
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,27 +23,22 @@
 DynamoDB Mapping
 ================
 
 
 .. image:: https://img.shields.io/pypi/v/dynamodb_mapping.svg
         :target: https://pypi.python.org/pypi/dynamodb_mapping
 
-.. image:: https://img.shields.io/travis/mrtj/dynamodb_mapping.svg
-        :target: https://travis-ci.com/mrtj/dynamodb_mapping
+.. image:: https://codecov.io/gh/mrtj/dynamodb-mapping/branch/main/graph/badge.svg?token=Y44R08UKEG
+        :target: https://codecov.io/gh/mrtj/dynamodb-mapping
 
 .. image:: https://readthedocs.org/projects/dynamodb-mapping/badge/?version=latest
         :target: https://dynamodb-mapping.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
-.. image:: https://pyup.io/repos/github/mrtj/dynamodb_mapping/shield.svg
-     :target: https://pyup.io/repos/github/mrtj/dynamodb_mapping/
-     :alt: Updates
-
-
 
 A Python dictionary-like interface for an Amazon DynamoDB table.
 
 DynamoDBMapping is an alternative API for `Amazon DynamoDB`_ that implements the Python
 ``collections.abc.MutableMapping`` abstract base class, effectively allowing you to use a DynamoDB
 table as if it were a Python dictionary.
```

### Comparing `dynamodb_mapping-0.1.0/README.rst` & `dynamodb_mapping-0.1.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,22 @@
 DynamoDB Mapping
 ================
 
 
 .. image:: https://img.shields.io/pypi/v/dynamodb_mapping.svg
         :target: https://pypi.python.org/pypi/dynamodb_mapping
 
-.. image:: https://img.shields.io/travis/mrtj/dynamodb_mapping.svg
-        :target: https://travis-ci.com/mrtj/dynamodb_mapping
+.. image:: https://codecov.io/gh/mrtj/dynamodb-mapping/branch/main/graph/badge.svg?token=Y44R08UKEG
+        :target: https://codecov.io/gh/mrtj/dynamodb-mapping
 
 .. image:: https://readthedocs.org/projects/dynamodb-mapping/badge/?version=latest
         :target: https://dynamodb-mapping.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
-.. image:: https://pyup.io/repos/github/mrtj/dynamodb_mapping/shield.svg
-     :target: https://pyup.io/repos/github/mrtj/dynamodb_mapping/
-     :alt: Updates
-
-
 
 A Python dictionary-like interface for an Amazon DynamoDB table.
 
 DynamoDBMapping is an alternative API for `Amazon DynamoDB`_ that implements the Python
 ``collections.abc.MutableMapping`` abstract base class, effectively allowing you to use a DynamoDB
 table as if it were a Python dictionary.
```

### Comparing `dynamodb_mapping-0.1.0/docs/Makefile` & `dynamodb_mapping-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dynamodb_mapping-0.1.0/docs/conf.py` & `dynamodb_mapping-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dynamodb_mapping-0.1.0/docs/make.bat` & `dynamodb_mapping-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dynamodb_mapping-0.1.0/dynamodb_mapping/dynamodb_mapping.py` & `dynamodb_mapping-0.1.1/dynamodb_mapping/dynamodb_mapping.py`

 * *Files identical despite different names*

### Comparing `dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/PKG-INFO` & `dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynamodb-mapping
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python dictionary-like interface for an Amazon DynamoDB table.
 Home-page: https://github.com/mrtj/dynamodb_mapping
 Author: Janos Tolgyesi
 Author-email: janos.tolgyesi@gmail.com
 License: MIT license
 Keywords: dynamodb_mapping
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -23,27 +23,22 @@
 DynamoDB Mapping
 ================
 
 
 .. image:: https://img.shields.io/pypi/v/dynamodb_mapping.svg
         :target: https://pypi.python.org/pypi/dynamodb_mapping
 
-.. image:: https://img.shields.io/travis/mrtj/dynamodb_mapping.svg
-        :target: https://travis-ci.com/mrtj/dynamodb_mapping
+.. image:: https://codecov.io/gh/mrtj/dynamodb-mapping/branch/main/graph/badge.svg?token=Y44R08UKEG
+        :target: https://codecov.io/gh/mrtj/dynamodb-mapping
 
 .. image:: https://readthedocs.org/projects/dynamodb-mapping/badge/?version=latest
         :target: https://dynamodb-mapping.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
-.. image:: https://pyup.io/repos/github/mrtj/dynamodb_mapping/shield.svg
-     :target: https://pyup.io/repos/github/mrtj/dynamodb_mapping/
-     :alt: Updates
-
-
 
 A Python dictionary-like interface for an Amazon DynamoDB table.
 
 DynamoDBMapping is an alternative API for `Amazon DynamoDB`_ that implements the Python
 ``collections.abc.MutableMapping`` abstract base class, effectively allowing you to use a DynamoDB
 table as if it were a Python dictionary.
```

### Comparing `dynamodb_mapping-0.1.0/dynamodb_mapping.egg-info/SOURCES.txt` & `dynamodb_mapping-0.1.1/dynamodb_mapping.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/modules.rst
 docs/readme.rst
 docs/_build/html/_static/file.png
 docs/_build/html/_static/minus.png
 docs/_build/html/_static/plus.png
 dynamodb_mapping/__init__.py
 dynamodb_mapping/dynamodb_mapping.py
+dynamodb_mapping/py.typed
 dynamodb_mapping.egg-info/PKG-INFO
 dynamodb_mapping.egg-info/SOURCES.txt
 dynamodb_mapping.egg-info/dependency_links.txt
 dynamodb_mapping.egg-info/not-zip-safe
 dynamodb_mapping.egg-info/requires.txt
 dynamodb_mapping.egg-info/top_level.txt
 tests/__init__.py
```

### Comparing `dynamodb_mapping-0.1.0/setup.py` & `dynamodb_mapping-0.1.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,13 +35,14 @@
     install_requires=requirements,
     license="MIT license",
     long_description=readme + "\n\n" + history,
     include_package_data=True,
     keywords="dynamodb_mapping",
     name="dynamodb_mapping",
     packages=find_packages(include=["dynamodb_mapping", "dynamodb_mapping.*"]),
+    package_data={"dynamodb_mapping": ["py.typed"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/mrtj/dynamodb_mapping",
-    version="0.1.0",
+    version="0.1.1",
     zip_safe=False,
 )
```

### Comparing `dynamodb_mapping-0.1.0/tests/test_dynamodb_mapping.py` & `dynamodb_mapping-0.1.1/tests/test_dynamodb_mapping.py`

 * *Files identical despite different names*


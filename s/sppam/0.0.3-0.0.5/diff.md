# Comparing `tmp/sppam-0.0.3.tar.gz` & `tmp/sppam-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sppam-0.0.3.tar", last modified: Tue Aug  1 22:53:39 2023, max compression
+gzip compressed data, was "sppam-0.0.5.tar", last modified: Tue Aug  1 23:47:30 2023, max compression
```

## Comparing `sppam-0.0.3.tar` & `sppam-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 22:53:39.859274 sppam-0.0.3/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.3/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.3/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3084 2023-08-01 22:53:39.859274 sppam-0.0.3/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2073 2023-08-01 21:29:25.000000 sppam-0.0.3/README.rst
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.3/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-01 22:53:39.859274 sppam-0.0.3/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2824 2023-08-01 21:35:31.000000 sppam-0.0.3/setup.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 22:53:39.859274 sppam-0.0.3/sppam/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.3/sppam/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-01 22:51:11.000000 sppam-0.0.3/sppam/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8168 2023-08-01 22:50:18.000000 sppam-0.0.3/sppam/sppam.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 22:53:39.859274 sppam-0.0.3/sppam/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.3/sppam/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.3/sppam/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.3/sppam/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 22:53:39.859274 sppam-0.0.3/sppam.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3084 2023-08-01 22:53:39.000000 sppam-0.0.3/sppam.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-01 22:53:39.000000 sppam-0.0.3/sppam.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.3/sppam.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.3/sppam.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-01 22:53:39.000000 sppam-0.0.3/sppam.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-01 22:53:39.000000 sppam-0.0.3/sppam.egg-info/top_level.txt
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.335206 sppam-0.0.5/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.5/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.5/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3250 2023-08-01 23:47:30.335206 sppam-0.0.5/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2239 2023-08-01 23:37:38.000000 sppam-0.0.5/README.rst
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.5/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-01 23:47:30.335206 sppam-0.0.5/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2824 2023-08-01 21:35:31.000000 sppam-0.0.5/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.331206 sppam-0.0.5/sppam/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.5/sppam/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-01 23:37:59.000000 sppam-0.0.5/sppam/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8168 2023-08-01 22:50:18.000000 sppam-0.0.5/sppam/sppam.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.335206 sppam-0.0.5/sppam/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.5/sppam/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.5/sppam/tests/test_common.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.5/sppam/tests/test_template.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.331206 sppam-0.0.5/sppam.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     3250 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.5/sppam.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/top_level.txt
```

### Comparing `sppam-0.0.3/LICENSE` & `sppam-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sppam-0.0.3/PKG-INFO` & `sppam-0.0.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.3
+Version: 0.0.5
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -23,17 +23,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|Travis|_ |ReadTheDocs|_
 
-.. |ReadTheDocs| image:: https://readthedocs.org/projects/scorelp/badge/?version=latest
+.. |Travis| image:: https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master
+.. _Travis: https://app.travis-ci.com/github/hrolfrc/sppam
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
 SPPAM - Saddle point problem for AUC maximization
 ============================================================
 
 An AUC optimizing binomial classifier.
```

### Comparing `sppam-0.0.3/README.rst` & `sppam-0.0.5/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|Travis|_ |ReadTheDocs|_
 
-.. |ReadTheDocs| image:: https://readthedocs.org/projects/scorelp/badge/?version=latest
+.. |Travis| image:: https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master
+.. _Travis: https://app.travis-ci.com/github/hrolfrc/sppam
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
 SPPAM - Saddle point problem for AUC maximization
 ============================================================
 
 An AUC optimizing binomial classifier.
```

### Comparing `sppam-0.0.3/setup.py` & `sppam-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `sppam-0.0.3/sppam/sppam.py` & `sppam-0.0.5/sppam/sppam.py`

 * *Files identical despite different names*

### Comparing `sppam-0.0.3/sppam.egg-info/PKG-INFO` & `sppam-0.0.5/sppam.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.3
+Version: 0.0.5
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
@@ -23,17 +23,20 @@
 Classifier: Programming Language :: Python :: 3.7
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|ReadTheDocs|_
+|Travis|_ |ReadTheDocs|_
 
-.. |ReadTheDocs| image:: https://readthedocs.org/projects/scorelp/badge/?version=latest
+.. |Travis| image:: https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master
+.. _Travis: https://app.travis-ci.com/github/hrolfrc/sppam
+
+.. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
 SPPAM - Saddle point problem for AUC maximization
 ============================================================
 
 An AUC optimizing binomial classifier.
```


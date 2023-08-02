# Comparing `tmp/sppam-0.0.5.tar.gz` & `tmp/sppam-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sppam-0.0.5.tar", last modified: Tue Aug  1 23:47:30 2023, max compression
+gzip compressed data, was "sppam-0.0.7.tar", last modified: Wed Aug  2 00:00:19 2023, max compression
```

## Comparing `sppam-0.0.5.tar` & `sppam-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.335206 sppam-0.0.5/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.5/LICENSE
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.5/MANIFEST.in
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3250 2023-08-01 23:47:30.335206 sppam-0.0.5/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2239 2023-08-01 23:37:38.000000 sppam-0.0.5/README.rst
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.5/requirements.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-01 23:47:30.335206 sppam-0.0.5/setup.cfg
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     2824 2023-08-01 21:35:31.000000 sppam-0.0.5/setup.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.331206 sppam-0.0.5/sppam/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.5/sppam/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-01 23:37:59.000000 sppam-0.0.5/sppam/_version.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     8168 2023-08-01 22:50:18.000000 sppam-0.0.5/sppam/sppam.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.335206 sppam-0.0.5/sppam/tests/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.5/sppam/tests/__init__.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.5/sppam/tests/test_common.py
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.5/sppam/tests/test_template.py
-drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-01 23:47:30.331206 sppam-0.0.5/sppam.egg-info/
--rw-rw-r--   0 rolf      (1000) rolf      (1000)     3250 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/PKG-INFO
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/SOURCES.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/dependency_links.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.5/sppam.egg-info/not-zip-safe
--rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/requires.txt
--rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-01 23:47:30.000000 sppam-0.0.5/sppam.egg-info/top_level.txt
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 00:00:19.856121 sppam-0.0.7/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     1529 2023-07-30 01:58:42.000000 sppam-0.0.7/LICENSE
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       25 2023-07-30 01:58:42.000000 sppam-0.0.7/MANIFEST.in
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 00:00:19.856121 sppam-0.0.7/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2071 2023-08-01 23:51:40.000000 sppam-0.0.7/README.rst
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      142 2023-08-01 20:18:30.000000 sppam-0.0.7/requirements.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      148 2023-08-02 00:00:19.856121 sppam-0.0.7/setup.cfg
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2617 2023-08-01 23:57:37.000000 sppam-0.0.7/setup.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 00:00:19.852121 sppam-0.0.7/sppam/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      145 2023-08-01 18:31:29.000000 sppam-0.0.7/sppam/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)       22 2023-08-01 23:58:36.000000 sppam-0.0.7/sppam/_version.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     8168 2023-08-01 22:50:18.000000 sppam-0.0.7/sppam/sppam.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 00:00:19.856121 sppam-0.0.7/sppam/tests/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        0 2023-07-30 01:58:42.000000 sppam-0.0.7/sppam/tests/__init__.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      239 2023-08-01 18:32:49.000000 sppam-0.0.7/sppam/tests/test_common.py
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      389 2023-08-01 20:08:16.000000 sppam-0.0.7/sppam/tests/test_template.py
+drwxrwxr-x   0 rolf      (1000) rolf      (1000)        0 2023-08-02 00:00:19.852121 sppam-0.0.7/sppam.egg-info/
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)     2904 2023-08-02 00:00:19.000000 sppam-0.0.7/sppam.egg-info/PKG-INFO
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      369 2023-08-02 00:00:19.000000 sppam-0.0.7/sppam.egg-info/SOURCES.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-02 00:00:19.000000 sppam-0.0.7/sppam.egg-info/dependency_links.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        1 2023-08-01 22:53:39.000000 sppam-0.0.7/sppam.egg-info/not-zip-safe
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)      119 2023-08-02 00:00:19.000000 sppam-0.0.7/sppam.egg-info/requires.txt
+-rw-rw-r--   0 rolf      (1000) rolf      (1000)        6 2023-08-02 00:00:19.000000 sppam-0.0.7/sppam.egg-info/top_level.txt
```

### Comparing `sppam-0.0.5/LICENSE` & `sppam-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `sppam-0.0.5/PKG-INFO` & `sppam-0.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.5
+Version: 0.0.7
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|Travis|_ |ReadTheDocs|_
-
-.. |Travis| image:: https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master
-.. _Travis: https://app.travis-ci.com/github/hrolfrc/sppam
+|ReadTheDocs|_
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
 SPPAM - Saddle point problem for AUC maximization
 ============================================================
```

### Comparing `sppam-0.0.5/README.rst` & `sppam-0.0.7/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 .. -*- mode: rst -*-
 
-|Travis|_ |ReadTheDocs|_
-
-.. |Travis| image:: https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master
-.. _Travis: https://app.travis-ci.com/github/hrolfrc/sppam
+|ReadTheDocs|_
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
 SPPAM - Saddle point problem for AUC maximization
 ============================================================
```

### Comparing `sppam-0.0.5/setup.py` & `sppam-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -45,26 +45,22 @@
 URL = 'https://github.com/hrolfrc/sppam'
 LICENSE = 'new BSD'
 DOWNLOAD_URL = 'https://github.com/hrolfrc/sppam'
 VERSION = _version.__version__
 INSTALL_REQUIRES = ['numpy', 'scipy', 'scikit-learn']
 CLASSIFIERS = ['Intended Audience :: Science/Research',
                'Intended Audience :: Developers',
+               'Topic :: Scientific/Engineering :: Artificial Intelligence',
+               'Topic :: Scientific/Engineering :: Mathematics',
+               'Development Status :: 2 - Pre-Alpha',
                'License :: OSI Approved',
-               'Programming Language :: Python',
-               'Topic :: Software Development',
                'Topic :: Scientific/Engineering',
-               'Operating System :: Microsoft :: Windows',
-               'Operating System :: POSIX',
-               'Operating System :: Unix',
-               'Operating System :: MacOS',
-               'Programming Language :: Python :: 2.7',
-               'Programming Language :: Python :: 3.5',
-               'Programming Language :: Python :: 3.6',
-               'Programming Language :: Python :: 3.7']
+               'Operating System :: OS Independent',
+               'Programming Language :: Python :: 3']
+
 EXTRAS_REQUIRE = {
     'tests': [
         'pytest',
         'pytest-cov'],
     'docs': [
         'sphinx',
         'sphinx-gallery',
```

### Comparing `sppam-0.0.5/sppam/sppam.py` & `sppam-0.0.7/sppam/sppam.py`

 * *Files identical despite different names*

### Comparing `sppam-0.0.5/sppam.egg-info/PKG-INFO` & `sppam-0.0.7/sppam.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 Metadata-Version: 2.1
 Name: sppam
-Version: 0.0.5
+Version: 0.0.7
 Summary: A classifier that endeavors to solve the saddle point problem for AUC maximization.
 Home-page: https://github.com/hrolfrc/sppam
 Download-URL: https://github.com/hrolfrc/sppam
 Maintainer: Carlson Research, LLC
 Maintainer-email: hrolfrc@gmail.com
 License: new BSD
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 .. -*- mode: rst -*-
 
-|Travis|_ |ReadTheDocs|_
-
-.. |Travis| image:: https://travis-ci.org/scikit-learn-contrib/project-template.svg?branch=master
-.. _Travis: https://app.travis-ci.com/github/hrolfrc/sppam
+|ReadTheDocs|_
 
 .. |ReadTheDocs| image:: https://readthedocs.org/projects/sppam/badge/?version=latest
 .. _ReadTheDocs: https://sppam.readthedocs.io/en/latest/?badge=latest
 
 SPPAM - Saddle point problem for AUC maximization
 ============================================================
```


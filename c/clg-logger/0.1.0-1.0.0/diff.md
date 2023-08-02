# Comparing `tmp/clg-logger-0.1.0.tar.gz` & `tmp/clg-logger-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clg-logger-0.1.0.tar", last modified: Wed Aug  2 09:30:11 2023, max compression
+gzip compressed data, was "clg-logger-1.0.0.tar", last modified: Wed Aug  2 09:33:44 2023, max compression
```

## Comparing `clg-logger-0.1.0.tar` & `clg-logger-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-08-02 09:30:11.898662 clg-logger-0.1.0/
--rw-r--r--   0 francois  (1000) francois  (1000)     1063 2023-08-02 09:26:03.000000 clg-logger-0.1.0/LICENSE
--rw-r--r--   0 francois  (1000) francois  (1000)       35 2023-08-02 09:26:03.000000 clg-logger-0.1.0/MANIFEST.in
--rw-r--r--   0 francois  (1000) francois  (1000)      876 2023-08-02 09:30:11.898662 clg-logger-0.1.0/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)       43 2023-08-02 09:29:18.000000 clg-logger-0.1.0/README.rst
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-08-02 09:30:11.895329 clg-logger-0.1.0/clg/
--rw-r--r--   0 francois  (1000) francois  (1000)     5018 2023-08-02 09:29:38.000000 clg-logger-0.1.0/clg/logger.py
-drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-08-02 09:30:11.898662 clg-logger-0.1.0/clg_logger.egg-info/
--rw-r--r--   0 francois  (1000) francois  (1000)      876 2023-08-02 09:30:11.000000 clg-logger-0.1.0/clg_logger.egg-info/PKG-INFO
--rw-r--r--   0 francois  (1000) francois  (1000)      222 2023-08-02 09:30:11.000000 clg-logger-0.1.0/clg_logger.egg-info/SOURCES.txt
--rw-r--r--   0 francois  (1000) francois  (1000)        1 2023-08-02 09:30:11.000000 clg-logger-0.1.0/clg_logger.egg-info/dependency_links.txt
--rw-r--r--   0 francois  (1000) francois  (1000)        4 2023-08-02 09:30:11.000000 clg-logger-0.1.0/clg_logger.egg-info/requires.txt
--rw-r--r--   0 francois  (1000) francois  (1000)       11 2023-08-02 09:30:11.000000 clg-logger-0.1.0/clg_logger.egg-info/top_level.txt
--rw-r--r--   0 francois  (1000) francois  (1000)       38 2023-08-02 09:30:11.898662 clg-logger-0.1.0/setup.cfg
--rw-r--r--   0 francois  (1000) francois  (1000)     1043 2023-08-02 09:28:35.000000 clg-logger-0.1.0/setup.py
+drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-08-02 09:33:44.200893 clg-logger-1.0.0/
+-rw-r--r--   0 francois  (1000) francois  (1000)     1063 2023-08-02 09:26:03.000000 clg-logger-1.0.0/LICENSE
+-rw-r--r--   0 francois  (1000) francois  (1000)       35 2023-08-02 09:26:03.000000 clg-logger-1.0.0/MANIFEST.in
+-rw-r--r--   0 francois  (1000) francois  (1000)      881 2023-08-02 09:33:44.200893 clg-logger-1.0.0/PKG-INFO
+-rw-r--r--   0 francois  (1000) francois  (1000)       43 2023-08-02 09:29:18.000000 clg-logger-1.0.0/README.rst
+drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-08-02 09:33:44.197560 clg-logger-1.0.0/clg/
+-rw-r--r--   0 francois  (1000) francois  (1000)     7430 2023-08-02 09:31:58.000000 clg-logger-1.0.0/clg/logger.py
+drwxr-xr-x   0 francois  (1000) francois  (1000)        0 2023-08-02 09:33:44.197560 clg-logger-1.0.0/clg_logger.egg-info/
+-rw-r--r--   0 francois  (1000) francois  (1000)      881 2023-08-02 09:33:44.000000 clg-logger-1.0.0/clg_logger.egg-info/PKG-INFO
+-rw-r--r--   0 francois  (1000) francois  (1000)      222 2023-08-02 09:33:44.000000 clg-logger-1.0.0/clg_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)        1 2023-08-02 09:33:44.000000 clg-logger-1.0.0/clg_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)        4 2023-08-02 09:33:44.000000 clg-logger-1.0.0/clg_logger.egg-info/requires.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)       11 2023-08-02 09:33:44.000000 clg-logger-1.0.0/clg_logger.egg-info/top_level.txt
+-rw-r--r--   0 francois  (1000) francois  (1000)       38 2023-08-02 09:33:44.200893 clg-logger-1.0.0/setup.cfg
+-rw-r--r--   0 francois  (1000) francois  (1000)     1048 2023-08-02 09:32:59.000000 clg-logger-1.0.0/setup.py
```

### Comparing `clg-logger-0.1.0/LICENSE` & `clg-logger-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clg-logger-0.1.0/PKG-INFO` & `clg-logger-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: clg-logger
-Version: 0.1.0
+Version: 1.0.0
 Summary: Manage logging based on command-line options.
-Home-page: https://clg.readthedocs.org/en/latest/
+Home-page: http://github.com/fmenabe/python-clg-logger
 Download-URL: http://github.com/fmenabe/python-clg-logger
 Author: François Ménabé
 Author-email: francois.menabe@gmail.com
 License: MIT License
 Keywords: command-line,argparse,wrapper,clg,logging
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `clg-logger-0.1.0/clg_logger.egg-info/PKG-INFO` & `clg-logger-1.0.0/clg_logger.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: clg-logger
-Version: 0.1.0
+Version: 1.0.0
 Summary: Manage logging based on command-line options.
-Home-page: https://clg.readthedocs.org/en/latest/
+Home-page: http://github.com/fmenabe/python-clg-logger
 Download-URL: http://github.com/fmenabe/python-clg-logger
 Author: François Ménabé
 Author-email: francois.menabe@gmail.com
 License: MIT License
 Keywords: command-line,argparse,wrapper,clg,logging
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `clg-logger-0.1.0/setup.py` & `clg-logger-1.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # -*- coding: utf-8 -*-
 
 from setuptools import setup
 
 setup(
     name='clg-logger',
-    version='0.1.0',
+    version='1.0.0',
     author='François Ménabé',
     author_email='francois.menabe@gmail.com',
-    url = 'https://clg.readthedocs.org/en/latest/',
+    url = 'http://github.com/fmenabe/python-clg-logger',
     download_url = 'http://github.com/fmenabe/python-clg-logger',
     license='MIT License',
     description='Manage logging based on command-line options.',
     long_description=open('README.rst').read(),
     keywords=['command-line', 'argparse', 'wrapper', 'clg', 'logging'],
     classifiers=[
         'Development Status :: 3 - Alpha',
```


# Comparing `tmp/fwdviewpy-0.1.9.tar.gz` & `tmp/fwdviewpy-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fwdviewpy-0.1.9.tar", last modified: Thu Apr 27 15:00:28 2023, max compression
+gzip compressed data, was "fwdviewpy-0.2.1.tar", last modified: Wed Aug  2 13:48:00 2023, max compression
```

## Comparing `fwdviewpy-0.1.9.tar` & `fwdviewpy-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 15:00:28.185900 fwdviewpy-0.1.9/
--rw-rw-rw-   0        0        0      620 2023-04-27 15:00:28.166819 fwdviewpy-0.1.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-27 15:00:28.102046 fwdviewpy-0.1.9/fwdviewpy/
--rw-rw-rw-   0        0        0      101 2023-04-18 10:09:30.000000 fwdviewpy-0.1.9/fwdviewpy/__init__.py
--rw-rw-rw-   0        0        0    13308 2023-04-27 14:57:11.000000 fwdviewpy-0.1.9/fwdviewpy/main.py
-drwxrwxrwx   0        0        0        0 2023-04-27 15:00:28.163016 fwdviewpy-0.1.9/fwdviewpy.egg-info/
--rw-rw-rw-   0        0        0      620 2023-04-27 15:00:27.000000 fwdviewpy-0.1.9/fwdviewpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-04-27 15:00:27.000000 fwdviewpy-0.1.9/fwdviewpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 15:00:27.000000 fwdviewpy-0.1.9/fwdviewpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-04-27 15:00:27.000000 fwdviewpy-0.1.9/fwdviewpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-27 15:00:27.000000 fwdviewpy-0.1.9/fwdviewpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 15:00:28.187898 fwdviewpy-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-04-27 15:00:21.000000 fwdviewpy-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:48:00.003085 fwdviewpy-0.2.1/
+-rw-rw-rw-   0        0        0      620 2023-08-02 13:48:00.000941 fwdviewpy-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 13:47:59.974148 fwdviewpy-0.2.1/fwdviewpy/
+-rw-rw-rw-   0        0        0      135 2023-07-05 15:13:34.000000 fwdviewpy-0.2.1/fwdviewpy/__init__.py
+-rw-rw-rw-   0        0        0    34128 2023-08-02 13:35:18.000000 fwdviewpy-0.2.1/fwdviewpy/main.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:47:59.987619 fwdviewpy-0.2.1/fwdviewpy.egg-info/
+-rw-rw-rw-   0        0        0      620 2023-08-02 13:47:59.000000 fwdviewpy-0.2.1/fwdviewpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-08-02 13:47:59.000000 fwdviewpy-0.2.1/fwdviewpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:47:59.000000 fwdviewpy-0.2.1/fwdviewpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 13:47:59.000000 fwdviewpy-0.2.1/fwdviewpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 13:47:59.000000 fwdviewpy-0.2.1/fwdviewpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:48:00.003584 fwdviewpy-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      818 2023-08-02 13:43:49.000000 fwdviewpy-0.2.1/setup.py
```

### Comparing `fwdviewpy-0.1.9/PKG-INFO` & `fwdviewpy-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.9
+Version: 0.2.1
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.1.9/fwdviewpy.egg-info/PKG-INFO` & `fwdviewpy-0.2.1/fwdviewpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fwdviewpy
-Version: 0.1.9
+Version: 0.2.1
 Summary: Python package developed by FWD View - The Data Transformation Specialists.
 Author: Cameron Bose & Ryan Springett
 Author-email: cameron.bose@fwdview.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Mathematics
```

### Comparing `fwdviewpy-0.1.9/setup.py` & `fwdviewpy-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fwdviewpy',
-    version='0.1.9',
+    version='0.2.01',
     description='Python package developed by FWD View - The Data Transformation Specialists.',
     long_description='Python package developed by FWD View to automate actions on both the Delphix Virtualization engine and Delphix Continuous Compliance engine.',
     packages=find_packages(),
     author='Cameron Bose & Ryan Springett',
     author_email="cameron.bose@fwdview.com",
 
     install_requires=[
@@ -16,12 +16,7 @@
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Mathematics',
         'License :: OSI Approved :: MIT License',
     ]
 )
-
-
-
-
-
```


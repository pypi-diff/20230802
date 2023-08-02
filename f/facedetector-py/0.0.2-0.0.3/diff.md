# Comparing `tmp/facedetector-py-0.0.2.tar.gz` & `tmp/facedetector-py-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facedetector-py-0.0.2.tar", last modified: Wed Aug  2 02:42:30 2023, max compression
+gzip compressed data, was "facedetector-py-0.0.3.tar", last modified: Wed Aug  2 03:00:23 2023, max compression
```

## Comparing `facedetector-py-0.0.2.tar` & `facedetector-py-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.161993 facedetector-py-0.0.2/
--rw-r--r--   0 Arhey      (501) staff       (20)     1061 2023-08-01 01:15:52.000000 facedetector-py-0.0.2/LICENSE
--rw-r--r--   0 Arhey      (501) staff       (20)     1286 2023-08-02 02:42:30.161526 facedetector-py-0.0.2/PKG-INFO
--rw-r--r--   0 Arhey      (501) staff       (20)      983 2023-08-02 02:42:07.000000 facedetector-py-0.0.2/README.md
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.158381 facedetector-py-0.0.2/facedetector_py.egg-info/
--rw-r--r--   0 Arhey      (501) staff       (20)     1286 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/PKG-INFO
--rw-r--r--   0 Arhey      (501) staff       (20)      314 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/SOURCES.txt
--rw-r--r--   0 Arhey      (501) staff       (20)        1 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/dependency_links.txt
--rw-r--r--   0 Arhey      (501) staff       (20)       66 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/requires.txt
--rw-r--r--   0 Arhey      (501) staff       (20)       10 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/top_level.txt
--rw-r--r--   0 Arhey      (501) staff       (20)       38 2023-08-02 02:42:30.162115 facedetector-py-0.0.2/setup.cfg
--rw-r--r--   0 Arhey      (501) staff       (20)      582 2023-08-02 02:18:01.000000 facedetector-py-0.0.2/setup.py
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.159977 facedetector-py-0.0.2/src/
--rw-r--r--   0 Arhey      (501) staff       (20)     1746 2023-08-02 02:37:30.000000 facedetector-py-0.0.2/src/FaceDetector.py
--rw-r--r--   0 Arhey      (501) staff       (20)        0 2022-08-06 20:13:11.000000 facedetector-py-0.0.2/src/__init__.py
--rw-r--r--   0 Arhey      (501) staff       (20)     3734 2023-08-02 02:36:05.000000 facedetector-py-0.0.2/src/utils.py
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.161048 facedetector-py-0.0.2/tests/
--rw-r--r--   0 Arhey      (501) staff       (20)      447 2023-08-02 02:41:45.000000 facedetector-py-0.0.2/tests/FaceDetector_test.py
--rw-r--r--   0 Arhey      (501) staff       (20)        0 2023-08-01 01:43:23.000000 facedetector-py-0.0.2/tests/__init__.py
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 03:00:23.667646 facedetector-py-0.0.3/
+-rw-r--r--   0 Arhey      (501) staff       (20)     1061 2023-08-01 01:15:52.000000 facedetector-py-0.0.3/LICENSE
+-rw-r--r--   0 Arhey      (501) staff       (20)     1286 2023-08-02 03:00:23.667027 facedetector-py-0.0.3/PKG-INFO
+-rw-r--r--   0 Arhey      (501) staff       (20)      983 2023-08-02 02:42:07.000000 facedetector-py-0.0.3/README.md
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 03:00:23.663435 facedetector-py-0.0.3/facedetector/
+-rw-r--r--   0 Arhey      (501) staff       (20)     1746 2023-08-02 02:37:30.000000 facedetector-py-0.0.3/facedetector/FaceDetector.py
+-rw-r--r--   0 Arhey      (501) staff       (20)        0 2022-08-06 20:13:11.000000 facedetector-py-0.0.3/facedetector/__init__.py
+-rw-r--r--   0 Arhey      (501) staff       (20)     3734 2023-08-02 02:36:05.000000 facedetector-py-0.0.3/facedetector/utils.py
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 03:00:23.665666 facedetector-py-0.0.3/facedetector_py.egg-info/
+-rw-r--r--   0 Arhey      (501) staff       (20)     1286 2023-08-02 03:00:23.000000 facedetector-py-0.0.3/facedetector_py.egg-info/PKG-INFO
+-rw-r--r--   0 Arhey      (501) staff       (20)      341 2023-08-02 03:00:23.000000 facedetector-py-0.0.3/facedetector_py.egg-info/SOURCES.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)        1 2023-08-02 03:00:23.000000 facedetector-py-0.0.3/facedetector_py.egg-info/dependency_links.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)       66 2023-08-02 03:00:23.000000 facedetector-py-0.0.3/facedetector_py.egg-info/requires.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)       19 2023-08-02 03:00:23.000000 facedetector-py-0.0.3/facedetector_py.egg-info/top_level.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)       38 2023-08-02 03:00:23.667814 facedetector-py-0.0.3/setup.cfg
+-rw-r--r--   0 Arhey      (501) staff       (20)      582 2023-08-02 02:58:40.000000 facedetector-py-0.0.3/setup.py
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 03:00:23.666608 facedetector-py-0.0.3/tests/
+-rw-r--r--   0 Arhey      (501) staff       (20)      456 2023-08-02 02:58:57.000000 facedetector-py-0.0.3/tests/FaceDetector_test.py
+-rw-r--r--   0 Arhey      (501) staff       (20)        0 2023-08-01 01:43:23.000000 facedetector-py-0.0.3/tests/__init__.py
```

### Comparing `facedetector-py-0.0.2/LICENSE` & `facedetector-py-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `facedetector-py-0.0.2/PKG-INFO` & `facedetector-py-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facedetector-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python script for detecting faces in an image
 Home-page: https://github.com/freearhey/facedetector
 Author: Arhey
 License: MIT
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `facedetector-py-0.0.2/README.md` & `facedetector-py-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `facedetector-py-0.0.2/facedetector_py.egg-info/PKG-INFO` & `facedetector-py-0.0.3/facedetector_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facedetector-py
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python script for detecting faces in an image
 Home-page: https://github.com/freearhey/facedetector
 Author: Arhey
 License: MIT
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `facedetector-py-0.0.2/setup.py` & `facedetector-py-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 setup(
   name="facedetector-py",
-  version="0.0.2",
+  version="0.0.3",
   description='Python script for detecting faces in an image',
   long_description=long_description,
   long_description_content_type='text/markdown',
   packages=find_packages(),
   url='https://github.com/freearhey/facedetector',
   author='Arhey',
   license='MIT',
```

### Comparing `facedetector-py-0.0.2/src/FaceDetector.py` & `facedetector-py-0.0.3/facedetector/FaceDetector.py`

 * *Files identical despite different names*

### Comparing `facedetector-py-0.0.2/src/utils.py` & `facedetector-py-0.0.3/facedetector/utils.py`

 * *Files identical despite different names*


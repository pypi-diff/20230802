# Comparing `tmp/facedetector-py-0.0.1.tar.gz` & `tmp/facedetector-py-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "facedetector-py-0.0.1.tar", last modified: Tue Aug  1 20:39:22 2023, max compression
+gzip compressed data, was "facedetector-py-0.0.2.tar", last modified: Wed Aug  2 02:42:30 2023, max compression
```

## Comparing `facedetector-py-0.0.1.tar` & `facedetector-py-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,19 @@
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-01 20:39:22.399492 facedetector-py-0.0.1/
--rw-r--r--   0 Arhey      (501) staff       (20)     1061 2023-08-01 01:15:52.000000 facedetector-py-0.0.1/LICENSE
--rw-r--r--   0 Arhey      (501) staff       (20)     1156 2023-08-01 20:39:22.399069 facedetector-py-0.0.1/PKG-INFO
--rw-r--r--   0 Arhey      (501) staff       (20)      853 2023-08-01 20:32:22.000000 facedetector-py-0.0.1/README.md
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-01 20:39:22.393935 facedetector-py-0.0.1/facedetector_py.egg-info/
--rw-r--r--   0 Arhey      (501) staff       (20)     1156 2023-08-01 20:39:22.000000 facedetector-py-0.0.1/facedetector_py.egg-info/PKG-INFO
--rw-r--r--   0 Arhey      (501) staff       (20)      382 2023-08-01 20:39:22.000000 facedetector-py-0.0.1/facedetector_py.egg-info/SOURCES.txt
--rw-r--r--   0 Arhey      (501) staff       (20)        1 2023-08-01 20:39:22.000000 facedetector-py-0.0.1/facedetector_py.egg-info/dependency_links.txt
--rw-r--r--   0 Arhey      (501) staff       (20)       66 2023-08-01 20:39:22.000000 facedetector-py-0.0.1/facedetector_py.egg-info/requires.txt
--rw-r--r--   0 Arhey      (501) staff       (20)       10 2023-08-01 20:39:22.000000 facedetector-py-0.0.1/facedetector_py.egg-info/top_level.txt
--rw-r--r--   0 Arhey      (501) staff       (20)       38 2023-08-01 20:39:22.399604 facedetector-py-0.0.1/setup.cfg
--rw-r--r--   0 Arhey      (501) staff       (20)      582 2023-08-01 20:34:05.000000 facedetector-py-0.0.1/setup.py
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-01 20:39:22.395132 facedetector-py-0.0.1/src/
--rw-r--r--   0 Arhey      (501) staff       (20)     1176 2023-08-01 19:56:28.000000 facedetector-py-0.0.1/src/FaceDetector.py
--rw-r--r--   0 Arhey      (501) staff       (20)        0 2022-08-06 20:13:11.000000 facedetector-py-0.0.1/src/__init__.py
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-01 20:39:22.397329 facedetector-py-0.0.1/src/util/
--rw-r--r--   0 Arhey      (501) staff       (20)        0 2022-08-01 16:34:51.000000 facedetector-py-0.0.1/src/util/__init__.py
--rw-r--r--   0 Arhey      (501) staff       (20)     1960 2022-07-31 23:45:58.000000 facedetector-py-0.0.1/src/util/align.py
--rw-r--r--   0 Arhey      (501) staff       (20)     1386 2023-08-01 19:56:20.000000 facedetector-py-0.0.1/src/util/detector.py
--rw-r--r--   0 Arhey      (501) staff       (20)      646 2022-07-31 23:45:58.000000 facedetector-py-0.0.1/src/util/geometry.py
-drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-01 20:39:22.398696 facedetector-py-0.0.1/tests/
--rw-r--r--   0 Arhey      (501) staff       (20)      447 2023-08-01 19:37:43.000000 facedetector-py-0.0.1/tests/FaceDetector_test.py
--rw-r--r--   0 Arhey      (501) staff       (20)        0 2023-08-01 01:43:23.000000 facedetector-py-0.0.1/tests/__init__.py
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.161993 facedetector-py-0.0.2/
+-rw-r--r--   0 Arhey      (501) staff       (20)     1061 2023-08-01 01:15:52.000000 facedetector-py-0.0.2/LICENSE
+-rw-r--r--   0 Arhey      (501) staff       (20)     1286 2023-08-02 02:42:30.161526 facedetector-py-0.0.2/PKG-INFO
+-rw-r--r--   0 Arhey      (501) staff       (20)      983 2023-08-02 02:42:07.000000 facedetector-py-0.0.2/README.md
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.158381 facedetector-py-0.0.2/facedetector_py.egg-info/
+-rw-r--r--   0 Arhey      (501) staff       (20)     1286 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/PKG-INFO
+-rw-r--r--   0 Arhey      (501) staff       (20)      314 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/SOURCES.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)        1 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/dependency_links.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)       66 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/requires.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)       10 2023-08-02 02:42:30.000000 facedetector-py-0.0.2/facedetector_py.egg-info/top_level.txt
+-rw-r--r--   0 Arhey      (501) staff       (20)       38 2023-08-02 02:42:30.162115 facedetector-py-0.0.2/setup.cfg
+-rw-r--r--   0 Arhey      (501) staff       (20)      582 2023-08-02 02:18:01.000000 facedetector-py-0.0.2/setup.py
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.159977 facedetector-py-0.0.2/src/
+-rw-r--r--   0 Arhey      (501) staff       (20)     1746 2023-08-02 02:37:30.000000 facedetector-py-0.0.2/src/FaceDetector.py
+-rw-r--r--   0 Arhey      (501) staff       (20)        0 2022-08-06 20:13:11.000000 facedetector-py-0.0.2/src/__init__.py
+-rw-r--r--   0 Arhey      (501) staff       (20)     3734 2023-08-02 02:36:05.000000 facedetector-py-0.0.2/src/utils.py
+drwxr-xr-x   0 Arhey      (501) staff       (20)        0 2023-08-02 02:42:30.161048 facedetector-py-0.0.2/tests/
+-rw-r--r--   0 Arhey      (501) staff       (20)      447 2023-08-02 02:41:45.000000 facedetector-py-0.0.2/tests/FaceDetector_test.py
+-rw-r--r--   0 Arhey      (501) staff       (20)        0 2023-08-01 01:43:23.000000 facedetector-py-0.0.2/tests/__init__.py
```

### Comparing `facedetector-py-0.0.1/LICENSE` & `facedetector-py-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `facedetector-py-0.0.1/PKG-INFO` & `facedetector-py-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facedetector-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python script for detecting faces in an image
 Home-page: https://github.com/freearhey/facedetector
 Author: Arhey
 License: MIT
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -31,32 +31,37 @@
 print(faces)
 ```
 
 Output:
 
 ```py
 [
-	{
-		'score': 0.9990496039390564,
-		'angle': -5.194428907734846,
-		'size': 73, 
-		'pivot': (1960, 819),
-		'bounding_box': [(1920, 782), (1993, 775), (1999, 848), (1927, 855)],
-		'landmarks': {
-			'right_eye': (1949.1595, 809.30695), 
-			'left_eye': (1970.3654, 808.0268), 
-			'nose': (1963.1459, 819.6671), 
-			'mouth_right': (1953.5267, 830.48206), 
-			'mouth_left': (1968.4865, 829.6616), 
-			'eyes_center': (1959, 808), 
-			'mouth_center': (1961, 830),
-			'face_center': (1960, 819)
-		}
-	},
-	...
+  {
+    'score': 0.9990496039390564, 
+    'angle': -5.194428907734846, 
+    'pivot': (1960, 819), 
+    'coordinates': [(1920, 782), (1993, 775), (1999, 848), (1927, 855)],
+    'bounding_box': {
+      'x': 1920, 
+      'y': 775, 
+      'width': 79, 
+      'height': 80
+    }, 
+    'landmarks': {
+      'right_eye': (1949.1595, 809.30695), 
+      'left_eye': (1970.3654, 808.0268), 
+      'nose': (1963.1459, 819.6671), 
+      'mouth_right': (1953.5267, 830.48206), 
+      'mouth_left': (1968.4865, 829.6616), 
+      'eyes_center': (1959, 808), 
+      'mouth_center': (1961, 830),
+      'face_center': (1960, 819)
+    }
+  },
+  ...
 ]
 ```
 
 ## Test
 
 ```sh
 pytest tests/
```

### Comparing `facedetector-py-0.0.1/facedetector_py.egg-info/PKG-INFO` & `facedetector-py-0.0.2/facedetector_py.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: facedetector-py
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python script for detecting faces in an image
 Home-page: https://github.com/freearhey/facedetector
 Author: Arhey
 License: MIT
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 Provides-Extra: dev
@@ -31,32 +31,37 @@
 print(faces)
 ```
 
 Output:
 
 ```py
 [
-	{
-		'score': 0.9990496039390564,
-		'angle': -5.194428907734846,
-		'size': 73, 
-		'pivot': (1960, 819),
-		'bounding_box': [(1920, 782), (1993, 775), (1999, 848), (1927, 855)],
-		'landmarks': {
-			'right_eye': (1949.1595, 809.30695), 
-			'left_eye': (1970.3654, 808.0268), 
-			'nose': (1963.1459, 819.6671), 
-			'mouth_right': (1953.5267, 830.48206), 
-			'mouth_left': (1968.4865, 829.6616), 
-			'eyes_center': (1959, 808), 
-			'mouth_center': (1961, 830),
-			'face_center': (1960, 819)
-		}
-	},
-	...
+  {
+    'score': 0.9990496039390564, 
+    'angle': -5.194428907734846, 
+    'pivot': (1960, 819), 
+    'coordinates': [(1920, 782), (1993, 775), (1999, 848), (1927, 855)],
+    'bounding_box': {
+      'x': 1920, 
+      'y': 775, 
+      'width': 79, 
+      'height': 80
+    }, 
+    'landmarks': {
+      'right_eye': (1949.1595, 809.30695), 
+      'left_eye': (1970.3654, 808.0268), 
+      'nose': (1963.1459, 819.6671), 
+      'mouth_right': (1953.5267, 830.48206), 
+      'mouth_left': (1968.4865, 829.6616), 
+      'eyes_center': (1959, 808), 
+      'mouth_center': (1961, 830),
+      'face_center': (1960, 819)
+    }
+  },
+  ...
 ]
 ```
 
 ## Test
 
 ```sh
 pytest tests/
```

### Comparing `facedetector-py-0.0.1/setup.py` & `facedetector-py-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
   long_description = f.read()
 
 setup(
   name="facedetector-py",
-  version="0.0.1",
+  version="0.0.2",
   description='Python script for detecting faces in an image',
   long_description=long_description,
   long_description_content_type='text/markdown',
   packages=find_packages(),
   url='https://github.com/freearhey/facedetector',
   author='Arhey',
   license='MIT',
```


# Comparing `tmp/large-image-source-multi-1.23.3.dev59.tar.gz` & `tmp/large-image-source-multi-1.23.3.dev60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.23.3.dev59.tar", last modified: Wed Aug  2 19:37:29 2023, max compression
+gzip compressed data, was "large-image-source-multi-1.23.3.dev60.tar", last modified: Wed Aug  2 19:37:39 2023, max compression
```

## Comparing `large-image-source-multi-1.23.3.dev59.tar` & `large-image-source-multi-1.23.3.dev60.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:29.247295 large-image-source-multi-1.23.3.dev59/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 19:37:28.000000 large-image-source-multi-1.23.3.dev59/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 19:37:29.247295 large-image-source-multi-1.23.3.dev59/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 19:37:28.000000 large-image-source-multi-1.23.3.dev59/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:29.243295 large-image-source-multi-1.23.3.dev59/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-08-02 19:36:19.000000 large-image-source-multi-1.23.3.dev59/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:29.243295 large-image-source-multi-1.23.3.dev59/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45193 2023-08-02 19:36:19.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-08-02 19:36:19.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:29.247295 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 19:37:29.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-08-02 19:37:29.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 19:37:29.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-08-02 19:37:29.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-08-02 19:37:29.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-02 19:37:29.000000 large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 19:37:29.247295 large-image-source-multi-1.23.3.dev59/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-02 19:36:19.000000 large-image-source-multi-1.23.3.dev59/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:39.254973 large-image-source-multi-1.23.3.dev60/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 19:37:38.000000 large-image-source-multi-1.23.3.dev60/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 19:37:39.254973 large-image-source-multi-1.23.3.dev60/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 19:37:38.000000 large-image-source-multi-1.23.3.dev60/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:39.254973 large-image-source-multi-1.23.3.dev60/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-08-02 19:36:33.000000 large-image-source-multi-1.23.3.dev60/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:39.254973 large-image-source-multi-1.23.3.dev60/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45193 2023-08-02 19:36:33.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-08-02 19:36:33.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:39.254973 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 19:37:39.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-08-02 19:37:39.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 19:37:39.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-08-02 19:37:39.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-08-02 19:37:39.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-02 19:37:39.000000 large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 19:37:39.254973 large-image-source-multi-1.23.3.dev60/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-02 19:36:33.000000 large-image-source-multi-1.23.3.dev60/setup.py
```

### Comparing `large-image-source-multi-1.23.3.dev59/LICENSE` & `large-image-source-multi-1.23.3.dev60/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev59/PKG-INFO` & `large-image-source-multi-1.23.3.dev60/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.23.3.dev59
+Version: 1.23.3.dev60
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.23.3.dev59/README.rst` & `large-image-source-multi-1.23.3.dev60/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev59/docs/specification.rst` & `large-image-source-multi-1.23.3.dev60/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev59/large_image_source_multi/__init__.py` & `large-image-source-multi-1.23.3.dev60/large_image_source_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev59/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.23.3.dev60/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev59/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.23.3.dev60/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.23.3.dev59
+Version: 1.23.3.dev60
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.23.3.dev59/setup.py` & `large-image-source-multi-1.23.3.dev60/setup.py`

 * *Files identical despite different names*


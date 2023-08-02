# Comparing `tmp/large-image-source-multi-1.23.3.dev30.tar.gz` & `tmp/large-image-source-multi-1.23.3.dev31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-multi-1.23.3.dev30.tar", last modified: Wed Aug  2 12:53:00 2023, max compression
+gzip compressed data, was "large-image-source-multi-1.23.3.dev31.tar", last modified: Wed Aug  2 12:55:21 2023, max compression
```

## Comparing `large-image-source-multi-1.23.3.dev30.tar` & `large-image-source-multi-1.23.3.dev31.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:00.966297 large-image-source-multi-1.23.3.dev30/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 12:53:00.966297 large-image-source-multi-1.23.3.dev30/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:00.966297 large-image-source-multi-1.23.3.dev30/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-08-02 12:51:59.000000 large-image-source-multi-1.23.3.dev30/docs/specification.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:00.966297 large-image-source-multi-1.23.3.dev30/large_image_source_multi/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45193 2023-08-02 12:51:59.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-08-02 12:51:59.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:00.966297 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-02 12:53:00.000000 large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 12:53:00.966297 large-image-source-multi-1.23.3.dev30/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-02 12:51:59.000000 large-image-source-multi-1.23.3.dev30/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:21.669386 large-image-source-multi-1.23.3.dev31/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 12:55:21.669386 large-image-source-multi-1.23.3.dev31/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:21.669386 large-image-source-multi-1.23.3.dev31/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3381 2023-08-02 12:54:22.000000 large-image-source-multi-1.23.3.dev31/docs/specification.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:21.669386 large-image-source-multi-1.23.3.dev31/large_image_source_multi/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45193 2023-08-02 12:54:22.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1356 2023-08-02 12:54:22.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:21.669386 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      967 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      141 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-02 12:55:21.000000 large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 12:55:21.669386 large-image-source-multi-1.23.3.dev31/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2637 2023-08-02 12:54:22.000000 large-image-source-multi-1.23.3.dev31/setup.py
```

### Comparing `large-image-source-multi-1.23.3.dev30/LICENSE` & `large-image-source-multi-1.23.3.dev31/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev30/PKG-INFO` & `large-image-source-multi-1.23.3.dev31/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.23.3.dev30
+Version: 1.23.3.dev31
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.23.3.dev30/README.rst` & `large-image-source-multi-1.23.3.dev31/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev30/docs/specification.rst` & `large-image-source-multi-1.23.3.dev31/docs/specification.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev30/large_image_source_multi/__init__.py` & `large-image-source-multi-1.23.3.dev31/large_image_source_multi/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev30/large_image_source_multi/girder_source.py` & `large-image-source-multi-1.23.3.dev31/large_image_source_multi/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-multi-1.23.3.dev30/large_image_source_multi.egg-info/PKG-INFO` & `large-image-source-multi-1.23.3.dev31/large_image_source_multi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-multi
-Version: 1.23.3.dev30
+Version: 1.23.3.dev31
 Summary: A tilesource for large_image to composite other tile sources
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-multi-1.23.3.dev30/setup.py` & `large-image-source-multi-1.23.3.dev31/setup.py`

 * *Files identical despite different names*


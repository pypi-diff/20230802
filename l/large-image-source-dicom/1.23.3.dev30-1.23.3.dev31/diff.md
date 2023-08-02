# Comparing `tmp/large-image-source-dicom-1.23.3.dev30.tar.gz` & `tmp/large-image-source-dicom-1.23.3.dev31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.23.3.dev30.tar", last modified: Wed Aug  2 12:52:43 2023, max compression
+gzip compressed data, was "large-image-source-dicom-1.23.3.dev31.tar", last modified: Wed Aug  2 12:55:05 2023, max compression
```

## Comparing `large-image-source-dicom-1.23.3.dev30.tar` & `large-image-source-dicom-1.23.3.dev31.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:52:43.982156 large-image-source-dicom-1.23.3.dev30/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-08-02 12:52:43.982156 large-image-source-dicom-1.23.3.dev30/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:52:43.978156 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10178 2023-08-02 12:51:59.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-08-02 12:51:59.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:52:43.982156 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-02 12:52:43.000000 large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 12:52:43.982156 large-image-source-dicom-1.23.3.dev30/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-08-02 12:51:59.000000 large-image-source-dicom-1.23.3.dev30/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:05.005301 large-image-source-dicom-1.23.3.dev31/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-08-02 12:55:05.001301 large-image-source-dicom-1.23.3.dev31/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:05.001301 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10178 2023-08-02 12:54:22.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-08-02 12:54:22.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:55:05.001301 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      817 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       85 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-08-02 12:55:04.000000 large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 12:55:05.005301 large-image-source-dicom-1.23.3.dev31/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-08-02 12:54:22.000000 large-image-source-dicom-1.23.3.dev31/setup.py
```

### Comparing `large-image-source-dicom-1.23.3.dev30/LICENSE` & `large-image-source-dicom-1.23.3.dev31/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.3.dev30/PKG-INFO` & `large-image-source-dicom-1.23.3.dev31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.23.3.dev30
+Version: 1.23.3.dev31
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.23.3.dev30/README.rst` & `large-image-source-dicom-1.23.3.dev31/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.3.dev30/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.23.3.dev31/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.3.dev30/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.23.3.dev31/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.23.3.dev30/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.23.3.dev31/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.23.3.dev30
+Version: 1.23.3.dev31
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.23.3.dev30/setup.py` & `large-image-source-dicom-1.23.3.dev31/setup.py`

 * *Files identical despite different names*


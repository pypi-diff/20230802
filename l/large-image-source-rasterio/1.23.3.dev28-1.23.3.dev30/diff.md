# Comparing `tmp/large-image-source-rasterio-1.23.3.dev28.tar.gz` & `tmp/large-image-source-rasterio-1.23.3.dev30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-rasterio-1.23.3.dev28.tar", last modified: Tue Aug  1 17:18:29 2023, max compression
+gzip compressed data, was "large-image-source-rasterio-1.23.3.dev30.tar", last modified: Wed Aug  2 12:53:27 2023, max compression
```

## Comparing `large-image-source-rasterio-1.23.3.dev28.tar` & `large-image-source-rasterio-1.23.3.dev30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 17:18:29.957374 large-image-source-rasterio-1.23.3.dev28/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-08-01 17:18:29.957374 large-image-source-rasterio-1.23.3.dev28/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 17:18:29.957374 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43030 2023-08-01 17:17:02.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-08-01 17:17:02.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-01 17:18:29.957374 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-08-01 17:18:29.000000 large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-01 17:18:29.957374 large-image-source-rasterio-1.23.3.dev28/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-08-01 17:17:02.000000 large-image-source-rasterio-1.23.3.dev28/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:27.270491 large-image-source-rasterio-1.23.3.dev30/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-08-02 12:53:27.270491 large-image-source-rasterio-1.23.3.dev30/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:27.270491 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43030 2023-08-02 12:51:59.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1444 2023-08-02 12:51:59.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 12:53:27.270491 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      846 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      420 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       28 2023-08-02 12:53:27.000000 large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 12:53:27.270491 large-image-source-rasterio-1.23.3.dev30/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2615 2023-08-02 12:51:59.000000 large-image-source-rasterio-1.23.3.dev30/setup.py
```

### Comparing `large-image-source-rasterio-1.23.3.dev28/LICENSE` & `large-image-source-rasterio-1.23.3.dev30/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev28/PKG-INFO` & `large-image-source-rasterio-1.23.3.dev30/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.3.dev28
+Version: 1.23.3.dev30
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.3.dev28/README.rst` & `large-image-source-rasterio-1.23.3.dev30/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio/__init__.py` & `large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio/girder_source.py` & `large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-rasterio-1.23.3.dev28/large_image_source_rasterio.egg-info/PKG-INFO` & `large-image-source-rasterio-1.23.3.dev30/large_image_source_rasterio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-rasterio
-Version: 1.23.3.dev28
+Version: 1.23.3.dev30
 Summary: A rasterio tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-rasterio-1.23.3.dev28/setup.py` & `large-image-source-rasterio-1.23.3.dev30/setup.py`

 * *Files identical despite different names*


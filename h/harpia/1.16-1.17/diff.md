# Comparing `tmp/harpia-1.16.tar.gz` & `tmp/harpia-1.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.16.tar", last modified: Wed Aug  2 02:19:26 2023, max compression
+gzip compressed data, was "harpia-1.17.tar", last modified: Wed Aug  2 02:49:42 2023, max compression
```

## Comparing `harpia-1.16.tar` & `harpia-1.17.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.353310 harpia-1.16/
--rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.16/LICENSE
--rw-rw-rw-   0        0        0      554 2023-08-02 02:19:26.353310 harpia-1.16/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.16/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.222972 harpia-1.16/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.16/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.238589 harpia-1.16/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.16/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.257151 harpia-1.16/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1216 2023-08-01 06:57:57.000000 harpia-1.16/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.16/harpia/tropomi/no2/converter.py
--rw-rw-rw-   0        0        0     3191 2023-08-02 02:17:50.000000 harpia-1.16/harpia/tropomi/no2/cp_completion.py
--rw-rw-rw-   0        0        0     3155 2023-08-01 05:23:46.000000 harpia-1.16/harpia/tropomi/no2/kriging.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.206458 harpia-1.16/harpia/tropomi/no2/lib/
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.257151 harpia-1.16/harpia/tropomi/no2/lib/random_missing_indices/
--rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.16/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.350731 harpia-1.16/harpia/tropomi/no2/lib/raster_templates/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
--rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.16/harpia/tropomi/no2/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:19:26.237082 harpia-1.16/harpia.egg-info/
--rw-rw-rw-   0        0        0      554 2023-08-02 02:19:26.000000 harpia-1.16/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-08-02 02:19:26.000000 harpia-1.16/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 02:19:26.000000 harpia-1.16/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-02 02:19:26.000000 harpia-1.16/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 02:19:26.000000 harpia-1.16/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 02:19:26.353310 harpia-1.16/setup.cfg
--rw-rw-rw-   0        0        0     2226 2023-08-02 02:18:50.000000 harpia-1.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.691641 harpia-1.17/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.17/LICENSE
+-rw-rw-rw-   0        0        0      554 2023-08-02 02:49:42.691641 harpia-1.17/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.17/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.631337 harpia-1.17/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.17/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.642916 harpia-1.17/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.17/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.642916 harpia-1.17/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1216 2023-08-01 06:57:57.000000 harpia-1.17/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.17/harpia/tropomi/no2/converter.py
+-rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.17/harpia/tropomi/no2/cp_completion.py
+-rw-rw-rw-   0        0        0     3155 2023-08-01 05:23:46.000000 harpia-1.17/harpia/tropomi/no2/kriging.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.631337 harpia-1.17/harpia/tropomi/no2/lib/
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.642916 harpia-1.17/harpia/tropomi/no2/lib/random_missing_indices/
+-rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.17/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.691641 harpia-1.17/harpia/tropomi/no2/lib/raster_templates/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
+-rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.17/harpia/tropomi/no2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:49:42.642916 harpia-1.17/harpia.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-08-02 02:49:42.000000 harpia-1.17/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      863 2023-08-02 02:49:42.000000 harpia-1.17/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:49:42.000000 harpia-1.17/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-02 02:49:42.000000 harpia-1.17/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 02:49:42.000000 harpia-1.17/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:49:42.691641 harpia-1.17/setup.cfg
+-rw-rw-rw-   0        0        0     2226 2023-08-02 02:49:14.000000 harpia-1.17/setup.py
```

### Comparing `harpia-1.16/LICENSE` & `harpia-1.17/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.16/PKG-INFO` & `harpia-1.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.16
+Version: 1.17
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.16/harpia/__init__.py` & `harpia-1.17/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/__init__.py` & `harpia-1.17/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/__init__.py` & `harpia-1.17/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/converter.py` & `harpia-1.17/harpia/tropomi/no2/converter.py`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/cp_completion.py` & `harpia-1.17/harpia/tropomi/no2/cp_completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
 Created on Sun Dec  4 14:03:42 2022
 
 @author: Ryan Solgi
 """
-
 import numpy as np
 from tensorlearn.decomposition import candecomp_parafac as cp
 from tensorlearn.operations import tensor_operations as top
 from tensorlearn.operations import matrix_operations as mop
 
 from harpia.tropomi.no2 import cp_completion
 
@@ -83,14 +82,14 @@
         if verbose:
             print('Error', error_ratio)
             
                
     
     return weights, factors, log
 
-def run_cp_completion(data,mask,rank,iteration, verbose=True):
+def run_cp_completion(data,mask,rank,iteration):
     data_array=data.copy()
     data_array[np.where(np.isnan(data_array))]=0
-    weights, factors, error_log=cp_completion.cp_completion_als(data_array, mask, rank, iteration, verbose)
-    reterived_array=top.cp_to_tensor(weights, factors)
+    weights, factors, error_log=cp_completion.cp_completion_als(data_array, mask, rank, iteration)
+    reterived_array=top.cp_to_tensor(weights.copy(), factors.copy())
     return reterived_array, error_log
```

### Comparing `harpia-1.16/harpia/tropomi/no2/kriging.py` & `harpia-1.17/harpia/tropomi/no2/kriging.py`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy` & `harpia-1.17/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif` & `harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif` & `harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif` & `harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif` & `harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif` & `harpia-1.17/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia/tropomi/no2/utils.py` & `harpia-1.17/harpia/tropomi/no2/utils.py`

 * *Files identical despite different names*

### Comparing `harpia-1.16/harpia.egg-info/PKG-INFO` & `harpia-1.17/harpia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.16
+Version: 1.17
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.16/harpia.egg-info/SOURCES.txt` & `harpia-1.17/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.16/setup.py` & `harpia-1.17/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.16",
+    version="1.17",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```


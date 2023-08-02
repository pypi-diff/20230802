# Comparing `tmp/harpia-1.21.tar.gz` & `tmp/harpia-1.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.21.tar", last modified: Wed Aug  2 17:36:27 2023, max compression
+gzip compressed data, was "harpia-1.22.tar", last modified: Wed Aug  2 17:39:52 2023, max compression
```

## Comparing `harpia-1.21.tar` & `harpia-1.22.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.214262 harpia-1.21/
--rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.21/LICENSE
--rw-rw-rw-   0        0        0      554 2023-08-02 17:36:27.214262 harpia-1.21/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.21/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.073346 harpia-1.21/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.21/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.093556 harpia-1.21/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.21/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.103699 harpia-1.21/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1216 2023-08-01 06:57:57.000000 harpia-1.21/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.21/harpia/tropomi/no2/converter.py
--rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.21/harpia/tropomi/no2/cp_completion.py
--rw-rw-rw-   0        0        0     4473 2023-08-02 05:41:14.000000 harpia-1.21/harpia/tropomi/no2/imputation.py
--rw-rw-rw-   0        0        0     3448 2023-08-02 05:26:18.000000 harpia-1.21/harpia/tropomi/no2/kriging.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.059724 harpia-1.21/harpia/tropomi/no2/lib/
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.165534 harpia-1.21/harpia/tropomi/no2/lib/random_missing_indices/
--rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.21/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
--rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.21/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.214262 harpia-1.21/harpia/tropomi/no2/lib/raster_templates/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
--rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.21/harpia/tropomi/no2/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:36:27.085999 harpia-1.21/harpia.egg-info/
--rw-rw-rw-   0        0        0      554 2023-08-02 17:36:27.000000 harpia-1.21/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-08-02 17:36:27.000000 harpia-1.21/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 17:36:27.000000 harpia-1.21/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-02 17:36:27.000000 harpia-1.21/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 17:36:27.000000 harpia-1.21/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 17:36:27.214262 harpia-1.21/setup.cfg
--rw-rw-rw-   0        0        0     2226 2023-08-02 17:35:54.000000 harpia-1.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:52.030976 harpia-1.22/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.22/LICENSE
+-rw-rw-rw-   0        0        0      554 2023-08-02 17:39:52.030976 harpia-1.22/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.22/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:51.944902 harpia-1.22/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.22/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:51.961631 harpia-1.22/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.22/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:51.976195 harpia-1.22/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1242 2023-08-02 17:39:12.000000 harpia-1.22/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.22/harpia/tropomi/no2/converter.py
+-rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.22/harpia/tropomi/no2/cp_completion.py
+-rw-rw-rw-   0        0        0     4473 2023-08-02 05:41:14.000000 harpia-1.22/harpia/tropomi/no2/imputation.py
+-rw-rw-rw-   0        0        0     3448 2023-08-02 05:26:18.000000 harpia-1.22/harpia/tropomi/no2/kriging.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:51.944902 harpia-1.22/harpia/tropomi/no2/lib/
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:52.010916 harpia-1.22/harpia/tropomi/no2/lib/random_missing_indices/
+-rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.22/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
+-rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.22/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:52.030976 harpia-1.22/harpia/tropomi/no2/lib/raster_templates/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
+-rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.22/harpia/tropomi/no2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:39:51.961631 harpia-1.22/harpia.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-08-02 17:39:51.000000 harpia-1.22/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-08-02 17:39:51.000000 harpia-1.22/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 17:39:51.000000 harpia-1.22/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-02 17:39:51.000000 harpia-1.22/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 17:39:51.000000 harpia-1.22/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 17:39:52.030976 harpia-1.22/setup.cfg
+-rw-rw-rw-   0        0        0     2226 2023-08-02 17:39:28.000000 harpia-1.22/setup.py
```

### Comparing `harpia-1.21/LICENSE` & `harpia-1.22/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.21/PKG-INFO` & `harpia-1.22/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.21
+Version: 1.22
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.21/harpia/__init__.py` & `harpia-1.22/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/__init__.py` & `harpia-1.22/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/__init__.py` & `harpia-1.22/harpia/tropomi/no2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 SOFTWARE.
 '''
 
 from . import converter
 from . import utils
 from . import cp_completion
 from . import kriging
+from . import imputation
```

### Comparing `harpia-1.21/harpia/tropomi/no2/converter.py` & `harpia-1.22/harpia/tropomi/no2/converter.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/cp_completion.py` & `harpia-1.22/harpia/tropomi/no2/cp_completion.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/imputation.py` & `harpia-1.22/harpia/tropomi/no2/imputation.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/kriging.py` & `harpia-1.22/harpia/tropomi/no2/kriging.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy` & `harpia-1.22/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy` & `harpia-1.22/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif` & `harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif` & `harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif` & `harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif` & `harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif` & `harpia-1.22/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia/tropomi/no2/utils.py` & `harpia-1.22/harpia/tropomi/no2/utils.py`

 * *Files identical despite different names*

### Comparing `harpia-1.21/harpia.egg-info/PKG-INFO` & `harpia-1.22/harpia.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.21
+Version: 1.22
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.21/harpia.egg-info/SOURCES.txt` & `harpia-1.22/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.21/setup.py` & `harpia-1.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.21",
+    version="1.22",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```


# Comparing `tmp/harpia-1.18.tar.gz` & `tmp/harpia-1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.18.tar", last modified: Wed Aug  2 04:07:06 2023, max compression
+gzip compressed data, was "harpia-1.19.tar", last modified: Wed Aug  2 04:24:28 2023, max compression
```

## Comparing `harpia-1.18.tar` & `harpia-1.19.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.372968 harpia-1.18/
--rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.18/LICENSE
--rw-rw-rw-   0        0        0      554 2023-08-02 04:07:06.372968 harpia-1.18/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.18/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.300955 harpia-1.18/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.18/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.314669 harpia-1.18/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.18/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.314669 harpia-1.18/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1216 2023-08-01 06:57:57.000000 harpia-1.18/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.18/harpia/tropomi/no2/converter.py
--rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.18/harpia/tropomi/no2/cp_completion.py
--rw-rw-rw-   0        0        0     3155 2023-08-01 05:23:46.000000 harpia-1.18/harpia/tropomi/no2/kriging.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.300955 harpia-1.18/harpia/tropomi/no2/lib/
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.351807 harpia-1.18/harpia/tropomi/no2/lib/random_missing_indices/
--rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.18/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
--rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.18/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.372968 harpia-1.18/harpia/tropomi/no2/lib/raster_templates/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
--rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.18/harpia/tropomi/no2/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 04:07:06.314669 harpia-1.18/harpia.egg-info/
--rw-rw-rw-   0        0        0      554 2023-08-02 04:07:06.000000 harpia-1.18/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      958 2023-08-02 04:07:06.000000 harpia-1.18/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:07:06.000000 harpia-1.18/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-02 04:07:06.000000 harpia-1.18/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 04:07:06.000000 harpia-1.18/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 04:07:06.372968 harpia-1.18/setup.cfg
--rw-rw-rw-   0        0        0     2226 2023-08-02 04:06:41.000000 harpia-1.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:28.069674 harpia-1.19/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.19/LICENSE
+-rw-rw-rw-   0        0        0      554 2023-08-02 04:24:28.066050 harpia-1.19/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.19/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:27.988312 harpia-1.19/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.19/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:28.002796 harpia-1.19/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.19/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:28.008827 harpia-1.19/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1216 2023-08-01 06:57:57.000000 harpia-1.19/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.19/harpia/tropomi/no2/converter.py
+-rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.19/harpia/tropomi/no2/cp_completion.py
+-rw-rw-rw-   0        0        0     3157 2023-08-02 04:20:48.000000 harpia-1.19/harpia/tropomi/no2/kriging.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:27.988312 harpia-1.19/harpia/tropomi/no2/lib/
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:28.039260 harpia-1.19/harpia/tropomi/no2/lib/random_missing_indices/
+-rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.19/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
+-rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.19/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:28.066050 harpia-1.19/harpia/tropomi/no2/lib/raster_templates/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
+-rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.19/harpia/tropomi/no2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:28.002796 harpia-1.19/harpia.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-08-02 04:24:27.000000 harpia-1.19/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      958 2023-08-02 04:24:27.000000 harpia-1.19/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:24:27.000000 harpia-1.19/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-02 04:24:27.000000 harpia-1.19/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 04:24:27.000000 harpia-1.19/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:24:28.069674 harpia-1.19/setup.cfg
+-rw-rw-rw-   0        0        0     2226 2023-08-02 04:23:56.000000 harpia-1.19/setup.py
```

### Comparing `harpia-1.18/LICENSE` & `harpia-1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.18/PKG-INFO` & `harpia-1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.18
+Version: 1.19
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.18/harpia/__init__.py` & `harpia-1.19/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/__init__.py` & `harpia-1.19/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/__init__.py` & `harpia-1.19/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/converter.py` & `harpia-1.19/harpia/tropomi/no2/converter.py`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/cp_completion.py` & `harpia-1.19/harpia/tropomi/no2/cp_completion.py`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/kriging.py` & `harpia-1.19/harpia/tropomi/no2/kriging.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             k_data[:,(row_size*i):(row_size*(i+1)),(column_size*j):(column_size*(j+1))]=data_array
         #print(i)
     return k_data   
     
 def run_ordinary_kriging(data,random_mask,resolution, partitioning=False):
     if resolution=='050':
         k_data=kriging.run_ordinary_krigin_helper(data,random_mask,1,1,70,140)
-    if resolution=='025':
+    elif resolution=='025':
         if partitioning:
             k_data=kriging.run_ordinary_krigin_helper(data,random_mask,3,1,47,281)
         else:
             k_data=kriging.run_ordinary_krigin_helper(data,random_mask,1,1,141,281)
     else:
         raise "resolution is not recognized"
     return k_data
```

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy` & `harpia-1.19/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy` & `harpia-1.19/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif` & `harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif` & `harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif` & `harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif` & `harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif` & `harpia-1.19/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia/tropomi/no2/utils.py` & `harpia-1.19/harpia/tropomi/no2/utils.py`

 * *Files identical despite different names*

### Comparing `harpia-1.18/harpia.egg-info/PKG-INFO` & `harpia-1.19/harpia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.18
+Version: 1.19
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.18/harpia.egg-info/SOURCES.txt` & `harpia-1.19/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.18/setup.py` & `harpia-1.19/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.18",
+    version="1.19",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```


# Comparing `tmp/harpia-1.23.tar.gz` & `tmp/harpia-1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harpia-1.23.tar", last modified: Wed Aug  2 17:51:33 2023, max compression
+gzip compressed data, was "harpia-1.24.tar", last modified: Wed Aug  2 18:20:04 2023, max compression
```

## Comparing `harpia-1.23.tar` & `harpia-1.24.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.218104 harpia-1.23/
--rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.23/LICENSE
--rw-rw-rw-   0        0        0      554 2023-08-02 17:51:33.208102 harpia-1.23/PKG-INFO
--rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.23/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.132220 harpia-1.23/harpia/
--rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.23/harpia/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.143796 harpia-1.23/harpia/tropomi/
--rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.23/harpia/tropomi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.152300 harpia-1.23/harpia/tropomi/no2/
--rw-rw-rw-   0        0        0     1242 2023-08-02 17:39:12.000000 harpia-1.23/harpia/tropomi/no2/__init__.py
--rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.23/harpia/tropomi/no2/converter.py
--rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.23/harpia/tropomi/no2/cp_completion.py
--rw-rw-rw-   0        0        0     4515 2023-08-02 17:50:42.000000 harpia-1.23/harpia/tropomi/no2/imputation.py
--rw-rw-rw-   0        0        0     3448 2023-08-02 05:26:18.000000 harpia-1.23/harpia/tropomi/no2/kriging.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.132220 harpia-1.23/harpia/tropomi/no2/lib/
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.192516 harpia-1.23/harpia/tropomi/no2/lib/random_missing_indices/
--rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.23/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
--rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.23/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.208102 harpia-1.23/harpia/tropomi/no2/lib/raster_templates/
--rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
--rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
--rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
--rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
--rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
--rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.23/harpia/tropomi/no2/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-02 17:51:33.143796 harpia-1.23/harpia.egg-info/
--rw-rw-rw-   0        0        0      554 2023-08-02 17:51:33.000000 harpia-1.23/harpia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      991 2023-08-02 17:51:33.000000 harpia-1.23/harpia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 17:51:33.000000 harpia-1.23/harpia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-02 17:51:33.000000 harpia-1.23/harpia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 17:51:33.000000 harpia-1.23/harpia.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 17:51:33.218104 harpia-1.23/setup.cfg
--rw-rw-rw-   0        0        0     2226 2023-08-02 17:50:58.000000 harpia-1.23/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.924419 harpia-1.24/
+-rw-rw-rw-   0        0        0     1080 2023-07-31 03:26:07.000000 harpia-1.24/LICENSE
+-rw-rw-rw-   0        0        0      554 2023-08-02 18:20:04.924419 harpia-1.24/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-07-31 03:26:07.000000 harpia-1.24/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.834922 harpia-1.24/harpia/
+-rw-rw-rw-   0        0        0     1141 2023-07-31 03:26:07.000000 harpia-1.24/harpia/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.844932 harpia-1.24/harpia/tropomi/
+-rw-rw-rw-   0        0        0     1137 2023-07-31 03:26:07.000000 harpia-1.24/harpia/tropomi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.860597 harpia-1.24/harpia/tropomi/no2/
+-rw-rw-rw-   0        0        0     1242 2023-08-02 17:39:12.000000 harpia-1.24/harpia/tropomi/no2/__init__.py
+-rw-rw-rw-   0        0        0     6734 2023-07-31 04:10:19.000000 harpia-1.24/harpia/tropomi/no2/converter.py
+-rw-rw-rw-   0        0        0     3181 2023-08-02 02:48:42.000000 harpia-1.24/harpia/tropomi/no2/cp_completion.py
+-rw-rw-rw-   0        0        0     4549 2023-08-02 18:18:53.000000 harpia-1.24/harpia/tropomi/no2/imputation.py
+-rw-rw-rw-   0        0        0     3448 2023-08-02 05:26:18.000000 harpia-1.24/harpia/tropomi/no2/kriging.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.834922 harpia-1.24/harpia/tropomi/no2/lib/
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.900793 harpia-1.24/harpia/tropomi/no2/lib/random_missing_indices/
+-rw-rw-rw-   0        0        0 33554168 2023-07-29 01:01:49.000000 harpia-1.24/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy
+-rw-rw-rw-   0        0        0  8366192 2023-07-29 17:57:48.000000 harpia-1.24/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.924419 harpia-1.24/harpia/tropomi/no2/lib/raster_templates/
+-rw-rw-rw-   0        0        0  7844566 2023-07-31 03:26:07.000000 harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif
+-rw-rw-rw-   0        0        0  1970880 2023-07-31 03:26:07.000000 harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif
+-rw-rw-rw-   0        0        0   317616 2023-07-31 03:26:07.000000 harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif
+-rw-rw-rw-   0        0        0    78826 2023-07-31 03:26:07.000000 harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif
+-rw-rw-rw-   0        0        0    19984 2023-07-31 03:26:07.000000 harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif
+-rw-rw-rw-   0        0        0     5883 2023-08-01 05:28:02.000000 harpia-1.24/harpia/tropomi/no2/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-02 18:20:04.844932 harpia-1.24/harpia.egg-info/
+-rw-rw-rw-   0        0        0      554 2023-08-02 18:20:04.000000 harpia-1.24/harpia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      991 2023-08-02 18:20:04.000000 harpia-1.24/harpia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 18:20:04.000000 harpia-1.24/harpia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-02 18:20:04.000000 harpia-1.24/harpia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 18:20:04.000000 harpia-1.24/harpia.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 18:20:04.924419 harpia-1.24/setup.cfg
+-rw-rw-rw-   0        0        0     2226 2023-08-02 18:19:30.000000 harpia-1.24/setup.py
```

### Comparing `harpia-1.23/LICENSE` & `harpia-1.24/LICENSE`

 * *Files identical despite different names*

### Comparing `harpia-1.23/PKG-INFO` & `harpia-1.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.23
+Version: 1.24
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.23/harpia/__init__.py` & `harpia-1.24/harpia/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/__init__.py` & `harpia-1.24/harpia/tropomi/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/__init__.py` & `harpia-1.24/harpia/tropomi/no2/__init__.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/converter.py` & `harpia-1.24/harpia/tropomi/no2/converter.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/cp_completion.py` & `harpia-1.24/harpia/tropomi/no2/cp_completion.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/imputation.py` & `harpia-1.24/harpia/tropomi/no2/imputation.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         file_name="TC_results_"+start_date+'_'+end_date+'_'+resolution+'_'+qa_value+'_'+added_missing_ratio+'_'+str(rank)+'.pickle'
         writing_file=os.path.join(writing_directory, file_name)
         with open(writing_file, 'wb') as file:
             pickle.dump(results_dict,file)
         
     return results_dict
 
-def kriging(kriging_type,prediction_interval,raster_directory,start_date,end_date,resolution,qa_value,added_missing_ratio, writing_directory=None):
+def kriging(kriging_type,prediction_interval,raster_directory,start_date,end_date,resolution,qa_value,added_missing_ratio, writing_directory=None, partitioning=False):
     
     random_indices_name="random_indices_"+start_date+'_'+end_date+'_'+resolution+'_'+qa_value+'_'+added_missing_ratio+'.npy'
     data, existed_dates, missed_dates=hp.utils.raster_to_array(raster_directory,start_date,end_date,resolution,qa_value)
     data=hp.utils.add_nans(data) #### nan values must be added before any change in the data values 
     data=hp.utils.molec_per_cm2(data)
     #mask=hp.utils.make_mask(data)  IT MUST NOT USE BECAUSE IT INCLUDE NAN VALUES TOO. 
     mask=np.ones(data.shape)
@@ -66,15 +66,15 @@
     
     raw_observations=cut_data[cut_random_indices]
     data_array=(data-np.nanmin(data))/(np.nanmax(data)-np.nanmin(data))
     cut_data_array=data_array[prediction_interval[0]:prediction_interval[1],:,:]
     normalized_observations=cut_data_array[cut_random_indices]
     start=time.time()
     
-    reterived_array=hp.kriging.run_kriging(cut_data_array,cut_mask,resolution, kriging_type)
+    reterived_array=hp.kriging.run_kriging(cut_data_array,cut_mask,resolution, kriging_type, partitioning)
     
     end=time.time()
     
     normalized_predictions=reterived_array[cut_random_indices]
     raw_reterived_array=reterived_array*(np.nanmax(data)-np.nanmin(data))+np.nanmin(data)
     raw_predictions=raw_reterived_array[cut_random_indices]
```

### Comparing `harpia-1.23/harpia/tropomi/no2/kriging.py` & `harpia-1.24/harpia/tropomi/no2/kriging.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy` & `harpia-1.24/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_025_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy` & `harpia-1.24/harpia/tropomi/no2/lib/random_missing_indices/random_indices_20190101_20200101_050_0.5_0.1.npy`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif` & `harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_005.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif` & `harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_010.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif` & `harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_025.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif` & `harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_050.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif` & `harpia-1.24/harpia/tropomi/no2/lib/raster_templates/raster_template_130w60w20n55n_100.tif`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia/tropomi/no2/utils.py` & `harpia-1.24/harpia/tropomi/no2/utils.py`

 * *Files identical despite different names*

### Comparing `harpia-1.23/harpia.egg-info/PKG-INFO` & `harpia-1.24/harpia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harpia
-Version: 1.23
+Version: 1.24
 Summary: A Python Package for Development
 Home-page: https://github.com/rmsolgi/harpia.git
 Author: Ryan Solgi
 Author-email: ryan.solgi@gmail.com
 Maintainer: Ryan Solgi
 Keywords: harpia
 Classifier: Programming Language :: Python :: 3
```

### Comparing `harpia-1.23/harpia.egg-info/SOURCES.txt` & `harpia-1.24/harpia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harpia-1.23/setup.py` & `harpia-1.24/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="harpia",
-    version="1.23",
+    version="1.24",
     author="Ryan Solgi",
     author_email="ryan.solgi@gmail.com",
     maintainer='Ryan Solgi',
     description="A Python Package for Development",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rmsolgi/harpia.git",
```


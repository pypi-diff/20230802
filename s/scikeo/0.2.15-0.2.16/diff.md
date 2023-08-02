# Comparing `tmp/scikeo-0.2.15.tar.gz` & `tmp/scikeo-0.2.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikeo-0.2.15.tar", last modified: Thu Jul 27 16:36:32 2023, max compression
+gzip compressed data, was "scikeo-0.2.16.tar", last modified: Wed Aug  2 17:04:00 2023, max compression
```

## Comparing `scikeo-0.2.15.tar` & `scikeo-0.2.16.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 16:36:32.025515 scikeo-0.2.15/
--rw-rw-rw-   0        0        0      613 2023-06-26 18:09:00.000000 scikeo-0.2.15/LICENSE
--rw-rw-rw-   0        0        0      130 2023-06-26 18:09:00.000000 scikeo-0.2.15/MANIFEST.in
--rw-rw-rw-   0        0        0     8738 2023-07-27 16:36:32.025515 scikeo-0.2.15/PKG-INFO
--rw-rw-rw-   0        0        0     7984 2023-07-27 16:35:12.000000 scikeo-0.2.15/README.md
--rw-rw-rw-   0        0        0       62 2023-06-26 18:09:00.000000 scikeo-0.2.15/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-27 16:36:31.999416 scikeo-0.2.15/scikeo/
--rw-rw-rw-   0        0        0      143 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/__init__.py
--rw-rw-rw-   0        0        0    10900 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/atmosCorr.py
--rw-rw-rw-   0        0        0     5794 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/calkmeans.py
--rw-rw-rw-   0        0        0    19966 2023-07-27 16:35:12.000000 scikeo-0.2.15/scikeo/calmla.py
--rw-rw-rw-   0        0        0     9989 2023-07-27 16:35:12.000000 scikeo-0.2.15/scikeo/deeplearning.py
--rw-rw-rw-   0        0        0     6113 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/fusionrs.py
--rw-rw-rw-   0        0        0     6668 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/linearTrend.py
--rw-rw-rw-   0        0        0    26407 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/mla.py
--rw-rw-rw-   0        0        0     5043 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/pca.py
--rw-rw-rw-   0        0        0     5789 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/plot.py
--rw-rw-rw-   0        0        0    12253 2023-07-27 16:35:12.000000 scikeo-0.2.15/scikeo/process.py
--rw-rw-rw-   0        0        0     1871 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/rkmeans.py
--rw-rw-rw-   0        0        0     3819 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/sma.py
--rw-rw-rw-   0        0        0     5235 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/tassCap.py
--rw-rw-rw-   0        0        0     2068 2023-06-26 18:09:00.000000 scikeo-0.2.15/scikeo/writeRaster.py
-drwxrwxrwx   0        0        0        0 2023-07-27 16:36:32.025004 scikeo-0.2.15/scikeo.egg-info/
--rw-rw-rw-   0        0        0     8738 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      516 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       56 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 18:09:08.000000 scikeo-0.2.15/scikeo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       55 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-07-27 16:36:31.000000 scikeo-0.2.15/scikeo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      414 2023-07-27 16:36:32.027517 scikeo-0.2.15/setup.cfg
--rw-rw-rw-   0        0        0     1813 2023-07-27 16:35:12.000000 scikeo-0.2.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:00.568056 scikeo-0.2.16/
+-rw-rw-rw-   0        0        0      613 2023-08-02 17:03:55.000000 scikeo-0.2.16/LICENSE
+-rw-rw-rw-   0        0        0      130 2023-08-02 17:03:55.000000 scikeo-0.2.16/MANIFEST.in
+-rw-rw-rw-   0        0        0     8829 2023-08-02 17:04:00.568056 scikeo-0.2.16/PKG-INFO
+-rw-rw-rw-   0        0        0     8075 2023-08-02 17:03:55.000000 scikeo-0.2.16/README.md
+-rw-rw-rw-   0        0        0       62 2023-08-02 17:03:55.000000 scikeo-0.2.16/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:00.520924 scikeo-0.2.16/scikeo/
+-rw-rw-rw-   0        0        0      143 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/__init__.py
+-rw-rw-rw-   0        0        0    10960 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/atmosCorr.py
+-rw-rw-rw-   0        0        0     5749 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/calkmeans.py
+-rw-rw-rw-   0        0        0    20683 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/calmla.py
+-rw-rw-rw-   0        0        0     9989 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/deeplearning.py
+-rw-rw-rw-   0        0        0     6139 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/fusionrs.py
+-rw-rw-rw-   0        0        0     6325 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/linearTrend.py
+-rw-rw-rw-   0        0        0    26407 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/mla.py
+-rw-rw-rw-   0        0        0     5043 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/pca.py
+-rw-rw-rw-   0        0        0     5660 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/plot.py
+-rw-rw-rw-   0        0        0    12255 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/process.py
+-rw-rw-rw-   0        0        0     1863 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/rkmeans.py
+-rw-rw-rw-   0        0        0     3854 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/sma.py
+-rw-rw-rw-   0        0        0     5247 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/tassCap.py
+-rw-rw-rw-   0        0        0     2068 2023-08-02 17:03:55.000000 scikeo-0.2.16/scikeo/writeRaster.py
+drwxrwxrwx   0        0        0        0 2023-08-02 17:04:00.561546 scikeo-0.2.16/scikeo.egg-info/
+-rw-rw-rw-   0        0        0     8829 2023-08-02 17:04:00.000000 scikeo-0.2.16/scikeo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      516 2023-08-02 17:04:00.000000 scikeo-0.2.16/scikeo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       56 2023-08-02 17:04:00.000000 scikeo-0.2.16/scikeo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 17:04:00.000000 scikeo-0.2.16/scikeo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       55 2023-08-02 17:04:00.000000 scikeo-0.2.16/scikeo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 17:04:00.000000 scikeo-0.2.16/scikeo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      414 2023-08-02 17:04:00.568056 scikeo-0.2.16/setup.cfg
+-rw-rw-rw-   0        0        0     1813 2023-08-02 17:03:55.000000 scikeo-0.2.16/setup.py
```

### Comparing `scikeo-0.2.15/LICENSE` & `scikeo-0.2.16/LICENSE`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.15/PKG-INFO` & `scikeo-0.2.16/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikeo
-Version: 0.2.15
+Version: 0.2.16
 Summary: Remote Sensing Tools
 Home-page: https://github.com/ytarazona/scikit-eo
 Author: Yonatan Tarazona Coronel
 Author-email: geoyons@gmail.com
 License: Apache Software License 2.0
 Keywords: scikeo
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
 [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
 [![tests](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml/badge.svg)](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml)
 
 
-
+<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 <!-- #region -->
 # Introduction
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
 
 Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
@@ -202,22 +202,21 @@
 ```
 
 <p align="left">
   <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
 </a>
 </p>
 
-<!-- #region -->
+
 -   Free software: Apache Software License 2.0
 -   Documentation: 
 
 ## Acknowledgment
 
 Special thanks to:
 - [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
 
 - [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
-<!-- #endregion -->
```

### Comparing `scikeo-0.2.15/README.md` & `scikeo-0.2.16/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
 [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
 [![tests](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml/badge.svg)](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml)
 
 
-
+<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 <!-- #region -->
 # Introduction
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
 
 Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
@@ -181,22 +181,21 @@
 ```
 
 <p align="left">
   <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
 </a>
 </p>
 
-<!-- #region -->
+
 -   Free software: Apache Software License 2.0
 -   Documentation: 
 
 ## Acknowledgment
 
 Special thanks to:
 - [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
 
 - [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
-<!-- #endregion -->
```

### Comparing `scikeo-0.2.15/scikeo/atmosCorr.py` & `scikeo-0.2.16/scikeo/atmosCorr.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class atmosCorr(object):
     
     '''Atmospheric Correction in Optical domain'''
     
     def __init__(self, path, nodata = -99999):
         
         '''
+        
         Parameter:
         
             path: String. The folder in which the satellite bands are located. This images could be Landsat
                   Collection 2 Level-1. For example: path = r'/folder/image/raster'.
             
             nodata: The NoData value to replace with -99999.
         '''
@@ -58,15 +59,16 @@
         ML = Band-specific multiplicative rescaling factor from the metadata (RADIANCE_MULT_BAND_x, where x is the band number)
         AL = Band-specific additive rescaling factor from the metadata (RADIANCE_ADD_BAND_x, where x is the band number)
         Qcal =  Quantized and calibrated standard product pixel values (DN) 
 
         Parameters:
             sat: Type of Satellite. It could be Landsat-5 TM, Landsat-8 OLI or Landsat-9 OLI-2.
         
-        Return: An array with radiance values with 3d, i.e. (rows, cols, bands).
+        Return: 
+            An array with radiance values with 3d, i.e. (rows, cols, bands).
         '''
         
         if sat == 'LC09':
             # Landsat-9 bands -> blue, green, red, nir, swir1 and swir2
             bands_lc09 = ['B2.','B3.','B4.','B5.','B6.','B7.']
             output_names = [name for name in self.names_bands if (name[41:44] in bands_lc09)]
         
@@ -132,15 +134,16 @@
         ρλ′ = Mρ*DN + Aρ
         
         ρλ = ρλ′/sin(theta)
         
         Parameters:
             sat: Type of Satellite. It could be Landsat-5 TM, Landsat-8 OLI or Landsat-9 OLI-2.
         
-        Return: An array with TOA values with 3d, i.e. (rows, cols, bands).
+        Return: 
+            An array with TOA values with 3d, i.e. (rows, cols, bands).
         '''
         
         if sat == 'LC09':
             # Landsat-9 bands -> blue, green, red, nir, swir1 and swir2
             bands_lc09 = ['B2.','B3.','B4.','B5.','B6.','B7.']
             output_names = [name for name in self.names_bands if (name[41:44] in bands_lc09)]
         
@@ -208,18 +211,20 @@
         
         Parameters:
         
             sat: Type of Satellite. It could be Landsat-5 TM, Landsat-8 OLI or Landsat-9 OLI-2.
             
             mindn: Min of digital number for each band in a list.
             
-        Return: An array with Surface Reflectance values with 3d, i.e. (rows, cols, bands).
+        Return: 
+            An array with Surface Reflectance values with 3d, i.e. (rows, cols, bands).
         
         References:
-            - Chavez, P.S. (1988). An Improved Dark-Object Subtraction Technique for Atmospheric 
+        
+            Chavez, P.S. (1988). An Improved Dark-Object Subtraction Technique for Atmospheric 
             Scattering Correction of Multispectral Data. Remote Sensing of Envrironment, 24(3), 459-479.
         '''
         
         if sat == 'LC09':
             bands_lc09 = ['B2.','B3.','B4.','B5.','B6.','B7.']
             output_names = [name for name in self.names_bands if (name[41:44] in bands_lc09)]
             # ESUN for Landsat-9 bands -> blue, green, red, nir, swir1 and swir2
```

### Comparing `scikeo-0.2.15/scikeo/calkmeans.py` & `scikeo-0.2.16/scikeo/calkmeans.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,43 +8,40 @@
     
     '''
     Calibrating kmeans
     
     This function allows to calibrate the kmeans algorithm. It is possible to obtain
     the best 'k' value and the best embedded algorithm in KMmeans.
         
-        Parameters:
+    Parameters:
+        image: Optical images. It must be rasterio.io.DatasetReader with 3d.
             
-            image: Optical images. It must be rasterio.io.DatasetReader with 3d.
-            
-            k: k This argument is None when the objective is to obtain the best 'k' value. 
-            If the objective is to select the best algorithm embedded in kmeans, please specify a 'k' value.
+        k: k This argument is None when the objective is to obtain the best 'k' value. 
+           f the objective is to select the best algorithm embedded in kmeans, please specify a 'k' value.
     
-            max_iter: The maximum number of iterations allowed. Strictly related to KMeans. Please see
-            https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
+        max_iter: The maximum number of iterations allowed. Strictly related to KMeans. Please see
+                  https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html
             
-            algo: It can be "auto" and 'elkan'. "auto" and "full" are deprecated and they will be 
-            removed in Scikit-Learn 1.3. They are both aliases for "lloyd".
+        algo: It can be "auto" and 'elkan'. "auto" and "full" are deprecated and they will be 
+              removed in Scikit-Learn 1.3. They are both aliases for "lloyd".
             
-            Changed in version 1.1: Renamed “full” to “lloyd”, and deprecated “auto” and “full”. 
-            Changed “auto” to use “lloyd” instead of “elkan”.
+        Changed in version 1.1: Renamed “full” to “lloyd”, and deprecated “auto” and “full”. 
+                               Changed “auto” to use “lloyd” instead of “elkan”.
             
-            n_iter: Iterations number to obtain the best 'k' value. 'n_iter' must be greater than the 
-            number of classes expected to be obtained in the classification. Default is 10.
+        n_iter: Iterations number to obtain the best 'k' value. 'n_iter' must be greater than the 
+                number of classes expected to be obtained in the classification. Default is 10.
             
-            nodata: The NoData value to replace with -99999. 
+        nodata: The NoData value to replace with -99999. 
                      
-            **kwargs: These will be passed to scikit-learn KMeans, please see full lists at:
+        **kwargs: These will be passed to scikit-learn KMeans, please see full lists at:
                   https://scikit-learn.org/stable/modules/generated/sklearn.cluster.KMeans.html.
     
         Return:
-        
             Labels of classification as numpy object with 2d.
             
-            
         Note:
         If the idea is to find the optimal value of 'k' (clusters or classes), k = None as an 
         argument of the function must be put, because the function find 'k' for which the intra-class 
         inertia is stabilized. If the 'k' value is known and the idea is to find the best algorithm 
         embedded in kmeans (that maximizes inter-class distances), k = n, which 'n' is a specific 
         class number, must be put. It can be greater than or equal to 0.
```

### Comparing `scikeo-0.2.15/scikeo/calmla.py` & `scikeo-0.2.16/scikeo/calmla.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,31 @@
     Leave-One-Out Cross-Validation (LOOCV), Cross-Validation (k-fold) and 
     Monte Carlo Cross-Validation (MCCV)'''
     
     def __init__(self, endmembers):
         
         '''
         Parameter:
-            
+        
             endmembers: Endmembers must be a matrix (numpy.ndarray) and with more than one endmember. 
-                    Rows represent the endmembers and columns represent the spectral bands.
-                    The number of bands must be equal to the number of endmembers.
-                    E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
-                    is rows with the number of endmembers and 6 is the number of bands 
-                    (should be equal).
-                    In addition, Endmembers must have a field (type int or float) with the names 
-                    of classes to be predicted.
-                    
+                        Rows represent the endmembers and columns represent the spectral bands.
+                        The number of bands must be equal to the number of endmembers.
+                        E.g. an image with 6 bands, endmembers dimension should be $n*6$, where $n$ 
+                        is rows with the number of endmembers and 6 is the number of bands 
+                        (should be equal).
+                        In addition, Endmembers must have a field (type int or float) with the names 
+                        of classes to be predicted.
+        
+        References:
+        
+            Tarazona, Y., Zabala, A., Pons, X., Broquetas, A., Nowosad, J., and Zurqani, H.A. 
+            Fusing Landsat and SAR data for mapping tropical deforestation through machine learning 
+            classification and the PVts-β non-seasonal detection approach, Canadian Journal of Remote 
+            Sensing., vol. 47, no. 5, pp. 677–696, Sep. 2021.
+      
         '''
         
         self.endm = endmembers
         
         # if it is read by pandas.read_csv()
         if isinstance(self.endm, (pd.core.frame.DataFrame)):
             
@@ -108,14 +115,15 @@
             
             n_iter: Number of iterations, i.e number of times the analysis is executed.
             
             **kwargs: These will be passed to SVM, DT, RF, NB and NN, please see full lists at:
                   https://scikit-learn.org/stable/supervised_learning.html#supervised-learning
             
         Return:  
+            A graphic with errors for each machine learning algorithms.
         '''
         svm_error_sa = []
         dt_error_sa = []
         rf_error_sa = []
         nb_error_sa = []
         nn_error_sa = []
         
@@ -230,15 +238,16 @@
             for testing data. Following Leave One Out Cross-Validation.
             
             n_iter: Number of iterations, i.e number of times the analysis is executed.
             
             **kwargs: These will be passed to SVM, DT, RF, NB and NN, please see full lists at:
                   https://scikit-learn.org/stable/supervised_learning.html#supervised-learning
             
-        Return: 
+        Return:  
+            A graphic with errors for each machine learning algorithms. 
         '''
         svm_error_loocv = []
         dt_error_loocv = []
         rf_error_loocv = []
         nb_error_loocv = []
         nn_error_loocv = []
         
@@ -327,15 +336,16 @@
             for testing data. Following Leave One Out Cross-Validation.
             
             n_iter: Number of iterations, i.e number of times the analysis is executed.
             
             **kwargs: These will be passed to SVM, DT, RF, NB and NN, please see full lists at:
                   https://scikit-learn.org/stable/supervised_learning.html#supervised-learning
             
-        Return:
+        Return:  
+            A graphic with errors for each machine learning algorithms.
         '''
         
         svm_error_cv = []
         dt_error_cv = []
         rf_error_cv = []
         nb_error_cv = []
         nn_error_cv = []
@@ -427,15 +437,16 @@
             for testing data. Following Leave One Out Cross-Validation.
             
             n_iter: Number of iterations, i.e number of times the analysis is executed.
             
             **kwargs: These will be passed to SVM, DT, RF, NB and NN, please see full lists at:
                   https://scikit-learn.org/stable/supervised_learning.html#supervised-learning
             
-        Return: 
+        Return:  
+            A graphic with errors for each machine learning algorithms. 
         '''
         
         svm_error_mccv = []
         dt_error_mccv = []
         rf_error_mccv = []
         nb_error_mccv = []
         nn_error_mccv = []
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scikeo-0.2.15/scikeo/deeplearning.py` & `scikeo-0.2.16/scikeo/deeplearning.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.15/scikeo/fusionrs.py` & `scikeo-0.2.16/scikeo/fusionrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,33 +30,35 @@
         **kwargs: These will be passed to scikit-learn PCA, please see full lists at:
                   https://scikit-learn.org/stable/modules/generated/sklearn.decomposition.PCA.html
     
     Return:
     
         A dictionary.
     
+    References:
+    
+        Tarazona, Y., Zabala, A., Pons, X., Broquetas, A., Nowosad, J., and Zurqani, H.A. 
+        Fusing Landsat and SAR data for mapping tropical deforestation through machine learning 
+        classification and the PVts-β non-seasonal detection approach, Canadian Journal of Remote 
+        Sensing., vol. 47, no. 5, pp. 677–696, Sep. 2021.
+      
     Note:
     Before executing the function, it is recommended that images coming from different sensors 
     or from the same sensor have a co-registration.
     
     The contributions of variables in accounting for the variability in a given principal component 
     are expressed in percentage. Variables that are correlated with PC1 (i.e., Dim.1) and PC2 
     (i.e., Dim.2) are the most important in explaining the variability in the data set. Variables 
     that do not correlated with any PC or correlated with the last dimensions are variables with 
     low contribution and might be removed to simplify the overall analysis.
     The contribution is a scaled version of the squared correlation between variables and component 
     axes (or the cosine, from a geometrical point of view) --- this is used to assess the quality of 
     the representation of the variables of the principal component, and it is computed as 
     (cos(variable,axis)^2/total cos2 of the component)×100.
-
-    References:
-    - Tarazona, Y., Zabala, A., Pons, X., Broquetas, A., Nowosad, J., and Zurqani, H.A. 
-      Fusing Landsat and SAR data for mapping tropical deforestation through machine learning 
-      classification and the PVts-β non-seasonal detection approach, Canadian Journal of Remote 
-      Sensing., vol. 47, no. 5, pp. 677–696, Sep. 2021.
+    
     '''
     
     for args in [optical, radar]:
         if not isinstance(args, (rasterio.io.DatasetReader)): 
             raise TypeError('The arguments A and B must be rasterio.io.DatasetReader.')
     
     if not optical.width != radar.width and optical.height != radar.height:
```

### Comparing `scikeo-0.2.15/scikeo/linearTrend.py` & `scikeo-0.2.16/scikeo/linearTrend.py`

 * *Files 5% similar despite different names*

```diff
@@ -34,36 +34,32 @@
         
             **kwargs: These will be passed to LN, please see full lists at:
                   https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.linregress.html
                   
         Return:
             a dictionary with slope, intercept and p-value obtained. All of them in numpy.ndarray 
             with 2d.
-            
-        Note:
-        Linear regression is widely used to analyze forest degradation or land degradation.
-        Specifically, the slope and its reliability are used as main parameters and they
-        can be obtained with this function. On the other hand, logistic regression allows
-        obtaining a degradation risk map, in other words, it is a probability map.
         
         References:
-        - Tarazona, Y., Maria, Miyasiro-Lopez. (2020). Monitoring tropical forest degradation using
-          remote sensing. Challenges and opportunities in the Madre de Dios region, Peru. Remote
-          Sensing Applications: Society and Environment, 19, 100337.
         
-        - Wilkinson, G.N., Rogers, C.E., 1973. Symbolic descriptions of factorial models for
-          analysis of variance. Appl. Stat. 22, 392-399.
+            Tarazona, Y., Maria, Miyasiro-Lopez. (2020). Monitoring tropical forest degradation using
+            remote sensing. Challenges and opportunities in the Madre de Dios region, Peru. Remote
+            Sensing Applications: Society and Environment, 19, 100337.
+        
+            Wilkinson, G.N., Rogers, C.E., 1973. Symbolic descriptions of factorial models for
+            analysis of variance. Appl. Stat. 22, 392-399.
+        
+            Chambers, J.M., 1992. Statistical Models in S. CRS Press.
         
-        - Chambers, J.M., 1992. Statistical Models in S. CRS Press.
-    
         Note:
         Linear regression is widely used to analyze forest degradation or land degradation.
         Specifically, the slope and its reliability are used as main parameters and they
         can be obtained with this function. On the other hand, logistic regression allows
         obtaining a degradation risk map, in other words, it is a probability map.
+        
         '''
         
         if not isinstance(self.image, (rasterio.io.DatasetReader)):
             raise TypeError(f'"image" must be raster read by rasterio.open(). {type(self.image)}')
         
         if not self.image.count >= 2:
             raise ValueError(f'The number of bands must be greater than 2. shape = {self.image.count}')
@@ -116,24 +112,24 @@
         
             **kwargs: These will be passed to MLN, please see full lists at:
                   https://www.statsmodels.org/dev/generated/statsmodels.discrete.discrete_model.Logit.html
                   
         Return:
             a dictionary with the summary of logistic regression and an array of probability with 2d.
             
+        References:
+            Tarazona, Y., Maria, Miyasiro-Lopez. (2020). Monitoring tropical forest degradation using
+            remote sensing. Challenges and opportunities in the Madre de Dios region, Peru. Remote
+            Sensing Applications: Society and Environment, 19, 100337.
+        
+            Chambers, J.M., 1992. Statistical Models in S. CRS Press.
+        
         Note:
         Logistic regression allows obtaining a degradation risk map (for instance), in other words, 
         it is a probability map.
-        
-        References:
-        - Tarazona, Y., Maria, Miyasiro-Lopez. (2020). Monitoring tropical forest degradation using
-          remote sensing. Challenges and opportunities in the Madre de Dios region, Peru. Remote
-          Sensing Applications: Society and Environment, 19, 100337.
-        
-        - Chambers, J.M., 1992. Statistical Models in S. CRS Press.
         '''
         
         if not isinstance(self.image, (rasterio.io.DatasetReader)):
             raise TypeError(f'"image" must be raster read by rasterio.open(). {type(self.image)}')
         
         if not self.image.count >= 2:
             raise ValueError(f'The number of bands must be greater than 2. shape = {self.image.count}')
```

### Comparing `scikeo-0.2.15/scikeo/mla.py` & `scikeo-0.2.16/scikeo/mla.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.15/scikeo/pca.py` & `scikeo-0.2.16/scikeo/pca.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.15/scikeo/plot.py` & `scikeo-0.2.16/scikeo/plot.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,41 +6,39 @@
 
 def plotHist(image, bands = 1, bins = 128, alpha = 0.8, title = None, xlabel = None, ylabel = None,
              label = None, ax = None, density = True, **kwargs):
     
     '''
     This function allows to plot satellite images histogram.
     
-        Parameters:
+    Parameters:
+        image: Optical images. It must be rasterio.io.DatasetReader with 3d or 2d.
             
-            image: Optical images. It must be rasterio.io.DatasetReader with 3d or 2d.
+        bands: Must be specified as a number of a list.
             
-            bands: Must be specified as a number of a list.
+        bins: By default is 128. 
             
-            bins: By default is 128. 
+        alpha: Percentage (%) of transparency between 0 and 1. 0 indicates 0% and 1 indicates
+               100%. By default is 80%.
             
-            alpha: Percentage (%) of transparency between 0 and 1. 0 indicates 0% and 1 indicates
-            100%. By default is 80%.
-            
-            title: Assigned title.
+        title: Assigned title.
         
-            xlabel: X axis title.
+        xlabel: X axis title.
         
-            ylabel: Y axis title.
+        ylabel: Y axis title.
             
-            label: Labeling the histogram.
+        label: Labeling the histogram.
         
-            ax: current axes
+        ax: current axes
         
-            **kwargs: These will be passed to the matplotlib imshow(), please see full lists at:
+        **kwargs: These will be passed to the matplotlib imshow(), please see full lists at:
                 https://matplotlib.org/stable/api/_as_gen/matplotlib.axes.Axes.hist.html
     
-        Return:
-        
-            ax : A histogram of an image.
+    Return:
+        ax: A histogram of an image.
         
     '''
     
     if not isinstance(image, (rasterio.io.DatasetReader)):
         raise TypeError('"image" must be raster read by rasterio.open().')
     
     st = image.read()
@@ -93,41 +91,40 @@
             ax = None, **kwargs):
     
     '''
     Plotting an image in RGB.
     
     This function allows to plot an satellite image in RGB channels.
         
-        Parameters:
+    Parameters:
             
-            image: Optical images. It must be rasterio.io.DatasetReader with 3d.
+        image: Optical images. It must be rasterio.io.DatasetReader with 3d.
             
-            bands: A list contain the order of bands to be used in order to plot in RGB. For example,
+        bands: A list contain the order of bands to be used in order to plot in RGB. For example,
                    for six bands (blue, green, red, nir, swir1 and swir2), number four (4) indicates 
                    the swir1 band, number three (3) indicates the nir band and the number two (2) indicates
                    the red band.
                    
-            stretch: Contrast enhancement using the histogram. There are two options here: i) using
+        stretch: Contrast enhancement using the histogram. There are two options here: i) using
                      standard deviation ('std') and ii) using percentiles ('per'). For default is 'std', which means
                      standard deviation.
             
-            title: Assigned title.
+        title: Assigned title.
         
-            xlabel: X axis title.
+        xlabel: X axis title.
         
-            ylabel: Y axis title.
+        ylabel: Y axis title.
         
-            ax: current axes
+        ax: current axes
         
-            **kwargs: These will be passed to the matplotlib imshow(), please see full lists at:
+        **kwargs: These will be passed to the matplotlib imshow(), please see full lists at:
                 https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.imshow.html
     
-        Return:
-        
-            ax : Graphic of an image in RGB.
+    Return:
+        ax: Graphic of an image in RGB.
         
     '''
     
     if not isinstance(image, (rasterio.io.DatasetReader)):
         raise TypeError('"image" must be raster read by rasterio.open().')
         
     st = image.read()
```

### Comparing `scikeo-0.2.15/scikeo/process.py` & `scikeo-0.2.16/scikeo/process.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,23 +178,23 @@
             
         conf: Confidence interval. By default is 95%.
     
     Return:
         
         Information of confusion matrix by proportions of area, overall accuracy, user's accuracy with confidence interval 
         and estimated area with confidence interval as well.
-        
-    Note:
-        Columns and rows in a confusion matrix indicate reference and prediction respectively. 
-        
+         
     Reference:
-    - Olofsson, P., Foody, G.M., Herold, M., Stehman, S.V., Woodcock, C.E., and Wulder, M.A. 2014. “Good practices 
-      for estimating area and assessing accuracy of land change.” Remote Sensing of Environment, Vol. 148: 42–57. 
-      doi:https://doi.org/10.1016/j.rse.2014.02.015.
     
+        Olofsson, P., Foody, G.M., Herold, M., Stehman, S.V., Woodcock, C.E., and Wulder, M.A. 2014. “Good practices 
+        for estimating area and assessing accuracy of land change.” Remote Sensing of Environment, Vol. 148: 42–57. 
+        doi:https://doi.org/10.1016/j.rse.2014.02.015.
+    
+    Note:
+        Columns and rows in a confusion matrix indicate reference and prediction respectively.
     '''
     
     if not isinstance(matrix, (np.ndarray)):
         raise TypeError('"matrix" must be numpy.ndarray with rows and cols.')
         
     if isinstance(image_pred, (np.ndarray)):
```

### Comparing `scikeo-0.2.15/scikeo/rkmeans.py` & `scikeo-0.2.16/scikeo/rkmeans.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     This function allows to classify satellite images using k-means
     
     In principle, this function allows to classify satellite images specifying
     a ```k``` value (clusters), however it is recommended to find the optimal value of ```k``` using
     the ```calkmeans``` function embedded in this package.
         
     Parameters:
-            
+    
         image: Optical images. It must be rasterio.io.DatasetReader with 3d.
         
         k: The number of clusters to be detected.
     
         nodata: The NoData value to replace with -99999.
                      
         **kwargs: These will be passed to scikit-learn KMeans, please see full lists at:
```

### Comparing `scikeo-0.2.15/scikeo/sma.py` & `scikeo-0.2.16/scikeo/sma.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,23 +26,24 @@
                     
         nodata: The NoData value to replace with -99999.
     
     Return:
     
         numpy.ndarray with 2d.
         
-    References
-    Adams, J. B., Smith, M. O., & Gillespie, A. R. (1993). Imaging spectroscopy:
-    Interpretation based on spectral mixture analysis. In C. M. Pieters & P.
-    Englert (Eds.), Remote geochemical analysis: Elements and mineralogical
-    composition. NY: Cambridge Univ. Press 145-166 pp.
+    References:
     
-    Shimabukuro, Y.E. and Smith, J., (1991). The least squares mixing models to
-    generate fraction images derived from remote sensing multispectral data.
-    IEEE Transactions on Geoscience and Remote Sensing, 29, pp. 16-21.
+        Adams, J. B., Smith, M. O., & Gillespie, A. R. (1993). Imaging spectroscopy:
+        Interpretation based on spectral mixture analysis. In C. M. Pieters & P.
+        Englert (Eds.), Remote geochemical analysis: Elements and mineralogical
+        composition. NY: Cambridge Univ. Press 145-166 pp.
+    
+        Shimabukuro, Y.E. and Smith, J., (1991). The least squares mixing models to
+        generate fraction images derived from remote sensing multispectral data.
+        IEEE Transactions on Geoscience and Remote Sensing, 29, pp. 16-21.
     
     Note:
     A regression analysis is used to obtain the fractions. In least squares
     inversion algorithms, the common objective is to estimate abundances that
     minimize the squared error between the actual spectrum and the estimated spectrum.
     The values of the fractions will be between 0 and 1.
     '''
```

### Comparing `scikeo-0.2.15/scikeo/tassCap.py` & `scikeo-0.2.16/scikeo/tassCap.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,24 +21,24 @@
         scale: Conversion of coefficients values
     
     Return:
         numpy.ndarray with 3d containing brightness, greenness and wetness indices.
     
     References:
     
-    - Crist, E.P., R. Laurin, and R.C. Cicone. 1986. Vegetation and soils information 
-      contained in transformed Thematic Mapper data. Pages 1465-1470 Ref. ESA SP-254. 
-      European Space Agency, Paris, France. http://www.ciesin.org/docs/005-419/005-419.html.
-    
-    - Baig, M.H.A., Shuai, T., Tong, Q., 2014. Derivation of a tasseled cap transformation 
-      based on Landsat 8 at-satellite reflectance. Remote Sensing Letters, 5(5), 423-431. 
-    
-    - Li, B., Ti, C., Zhao, Y., Yan, X., 2016. Estimating Soil Moisture with Landsat Data 
-      and Its Application in Extracting the Spatial Distribution of Winter Flooded Paddies. 
-      Remote Sensing, 8(1), 38.
+        Crist, E.P., R. Laurin, and R.C. Cicone. 1986. Vegetation and soils information 
+        contained in transformed Thematic Mapper data. Pages 1465-1470 Ref. ESA SP-254. 
+        European Space Agency, Paris, France. http://www.ciesin.org/docs/005-419/005-419.html.
+
+        Baig, M.H.A., Shuai, T., Tong, Q., 2014. Derivation of a tasseled cap transformation 
+        based on Landsat 8 at-satellite reflectance. Remote Sensing Letters, 5(5), 423-431. 
+    
+        Li, B., Ti, C., Zhao, Y., Yan, X., 2016. Estimating Soil Moisture with Landsat Data 
+        and Its Application in Extracting the Spatial Distribution of Winter Flooded Paddies. 
+        Remote Sensing, 8(1), 38.
     
     Note:
     Currently implemented for satellites such as Landsat-4 TM, Landsat-5 TM, Landsat-7 ETM+, 
     Landsat-8 OLI and Sentinel2. The input data must be in top of atmosphere reflectance (toa). 
     Bands required as input must be ordered as:
     
     Consider using the following satellite bands:
```

### Comparing `scikeo-0.2.15/scikeo/writeRaster.py` & `scikeo-0.2.16/scikeo/writeRaster.py`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.15/scikeo.egg-info/PKG-INFO` & `scikeo-0.2.16/scikeo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikeo
-Version: 0.2.15
+Version: 0.2.16
 Summary: Remote Sensing Tools
 Home-page: https://github.com/ytarazona/scikit-eo
 Author: Yonatan Tarazona Coronel
 Author-email: geoyons@gmail.com
 License: Apache Software License 2.0
 Keywords: scikeo
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 [![PyPI version](https://badge.fury.io/py/scikeo.svg)](https://badge.fury.io/py/scikeo)
 [![Youtube](https://img.shields.io/badge/YouTube-Channel-red)]()
 [![Downloads](https://pepy.tech/badge/scikeo)](https://pepy.tech/project/scikeo)
 [![Downloads](https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/docs-passing-brightgreen.svg)]()
 [![tests](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml/badge.svg)](https://github.com/ytarazona/scikit-eo/actions/workflows/tests.yml)
 
 
-
+<img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/scikit-eo_logo.jpg" align="right" width="220"/>
 
 <!-- #region -->
 # Introduction
 
 Nowadays, remotely sensed data has increased dramatically. Microwaves and optical images with different spatial and temporal resolutions are available and are used to monitor a variety of environmental issues such as deforestation, land degradation, land use and land cover change, among others. Although there are efforts (i.e., Python packages, forums, communities, etc.) to make available line-of-code tools for pre-processing, processing and analysis of satellite imagery, there is still a gap that needs to be filled. In other words, too much time is still spent by many users developing Python lines of code. Algorithms for mapping land degradation through a linear trend of vegetation indices, fusion optical and radar images to classify vegetation cover, and calibration of machine learning algorithms, among others, are not available yet.
 
 Therefore, **scikit-eo** is a Python package that provides tools for remote sensing. This package was developed to fill the gaps in remotely sensed data processing tools. Most of the tools are based on scientific publications, and others are useful algorithms that will allow processing to be done in a few lines of code. With these tools, the user will be able to invest time in analyzing the results of their data and not spend time on elaborating lines of code, which can sometimes be stressful.
@@ -202,22 +202,21 @@
 ```
 
 <p align="left">
   <a href="https://github.com/ytarazona/scikit-eo"><img src="https://raw.githubusercontent.com/ytarazona/scikit-eo/main/docs/images/classification.png" alt ="header" width = "750">
 </a>
 </p>
 
-<!-- #region -->
+
 -   Free software: Apache Software License 2.0
 -   Documentation: 
 
 ## Acknowledgment
 
 Special thanks to:
 - [David Montero Loaiza](https://github.com/davemlz) for the idea of the package name **scikit-eo**.
 
 - [Qiusheng Wu](https://github.com/giswqs) for the suggestions that helped to improve the package.
 
 ## Credits
 
 This package was created with [Cookiecutter](https://github.com/cookiecutter/cookiecutter)
-<!-- #endregion -->
```

### Comparing `scikeo-0.2.15/scikeo.egg-info/SOURCES.txt` & `scikeo-0.2.16/scikeo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scikeo-0.2.15/setup.py` & `scikeo-0.2.16/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,10 +48,10 @@
     keywords='scikeo',
     name='scikeo',
     packages=find_packages(include=['scikeo', 'scikeo.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ytarazona/scikit-eo',
-    version='0.2.15',
+    version='0.2.16',
     zip_safe=False,
 )
```


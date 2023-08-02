# Comparing `tmp/glm-met-0.0.1.tar.gz` & `tmp/glm-met-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glm-met-0.0.1.tar", last modified: Mon Jul 31 03:43:35 2023, max compression
+gzip compressed data, was "glm-met-0.0.2.tar", last modified: Wed Aug  2 07:19:56 2023, max compression
```

## Comparing `glm-met-0.0.1.tar` & `glm-met-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:43:35.403095 glm-met-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-24 05:41:35.000000 glm-met-0.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4505 2023-07-31 03:43:35.397704 glm-met-0.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4038 2023-07-28 09:25:04.000000 glm-met-0.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:43:35.281479 glm-met-0.0.1/glm_met/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 07:19:03.000000 glm-met-0.0.1/glm_met/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1254 2023-07-20 07:22:59.000000 glm-met-0.0.1/glm_met/glm_met.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:43:35.367775 glm-met-0.0.1/glm_met/openmeteo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 09:35:04.000000 glm-met-0.0.1/glm_met/openmeteo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8506 2023-07-28 11:00:29.000000 glm-met-0.0.1/glm_met/openmeteo/climate_change.py
--rw-r--r--   0 root         (0) root         (0)    10463 2023-07-28 11:01:37.000000 glm-met-0.0.1/glm_met/openmeteo/historical.py
--rw-r--r--   0 root         (0) root         (0)      808 2023-07-28 11:00:29.000000 glm-met-0.0.1/glm_met/openmeteo/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:43:35.328946 glm-met-0.0.1/glm_met.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4505 2023-07-31 03:43:35.000000 glm-met-0.0.1/glm_met.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      420 2023-07-31 03:43:35.000000 glm-met-0.0.1/glm_met.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-31 03:43:35.000000 glm-met-0.0.1/glm_met.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-31 03:43:35.000000 glm-met-0.0.1/glm_met.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-07-31 03:43:35.000000 glm-met-0.0.1/glm_met.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-31 03:41:23.000000 glm-met-0.0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-31 03:43:35.403850 glm-met-0.0.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-31 03:43:35.390851 glm-met-0.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)     7481 2023-07-28 06:47:29.000000 glm-met-0.0.1/tests/test_openmeteo_climate.py
--rw-r--r--   0 root         (0) root         (0)     8534 2023-07-27 06:29:29.000000 glm-met-0.0.1/tests/test_openmeteo_historical.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:19:56.375923 glm-met-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-07-24 05:41:35.000000 glm-met-0.0.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-08-02 07:19:56.369445 glm-met-0.0.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4039 2023-08-02 06:46:53.000000 glm-met-0.0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:19:56.165551 glm-met-0.0.2/glm_met/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 07:19:03.000000 glm-met-0.0.2/glm_met/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1254 2023-07-20 07:22:59.000000 glm-met-0.0.2/glm_met/glm_met.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:19:56.342482 glm-met-0.0.2/glm_met/openmeteo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-19 09:35:04.000000 glm-met-0.0.2/glm_met/openmeteo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-08-02 07:18:43.000000 glm-met-0.0.2/glm_met/openmeteo/climate_change.py
+-rw-r--r--   0 root         (0) root         (0)    10616 2023-08-02 07:18:43.000000 glm-met-0.0.2/glm_met/openmeteo/historical.py
+-rw-r--r--   0 root         (0) root         (0)      808 2023-07-28 11:00:29.000000 glm-met-0.0.2/glm_met/openmeteo/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:19:56.288175 glm-met-0.0.2/glm_met.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-08-02 07:19:56.000000 glm-met-0.0.2/glm_met.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      420 2023-08-02 07:19:56.000000 glm-met-0.0.2/glm_met.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:19:56.000000 glm-met-0.0.2/glm_met.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-08-02 07:19:56.000000 glm-met-0.0.2/glm_met.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-02 07:19:56.000000 glm-met-0.0.2/glm_met.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      695 2023-08-02 07:18:27.000000 glm-met-0.0.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:19:56.377916 glm-met-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:19:56.363655 glm-met-0.0.2/tests/
+-rw-r--r--   0 root         (0) root         (0)     7481 2023-07-28 06:47:29.000000 glm-met-0.0.2/tests/test_openmeteo_climate.py
+-rw-r--r--   0 root         (0) root         (0)     8534 2023-07-27 06:29:29.000000 glm-met-0.0.2/tests/test_openmeteo_historical.py
```

### Comparing `glm-met-0.0.1/LICENSE` & `glm-met-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glm-met-0.0.1/PKG-INFO` & `glm-met-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glm-met
-Version: 0.0.1
+Version: 0.0.2
 Summary: Download meteorological data for the General Lake Model
 Author: John Duncan
 Project-URL: Homepage, https://wet-tool.github.io/glm-met/
 Keywords: GLM,meterological,weather,climate
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 
 <a href="https://colab.research.google.com/github/WET-tool/glm-met/blob/main/example-use.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ```
 import os
-import glm_met.openmeteo.hisorical as historical
+import glm_met.openmeteo.historical as historical
 
 # initialise a Historical object
 # the object attributes are set to:
 # - query the open-meteo Historical API 
 # - query for hourly met data from 1970 to 2022
 # - query a location in Western Australia
 hist = historical.Historical(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glm-met Version: 0.0.1 Summary: Download
+Metadata-Version: 2.1 Name: glm-met Version: 0.0.2 Summary: Download
 meteorological data for the General Lake Model Author: John Duncan Project-URL:
 Homepage, https://wet-tool.github.io/glm-met/ Keywords:
 GLM,meterological,weather,climate Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # GLM-met A Python package for downloading
 meteorological data and processing it to formats required for running the GLM
@@ -17,15 +17,15 @@
 available as an executable for Linux (Ubuntu), MacOS, and Windows. It is
 actively developed by the Aquatic EcoDynamics research group at The University
 of Western Australia. ## Install ``` pip install glm-met ``` ## Use Import the
 glm-met package into a Python program and use to download meteorological data
 from a supported data provider. The following Jupyter notebook can be opened on
 Google Colab to demonstrate how glm-met can be used to download meteorological
 data from open-meteo's Historical API: [Open_In_Colab] ``` import os import
-glm_met.openmeteo.hisorical as historical # initialise a Historical object #
+glm_met.openmeteo.historical as historical # initialise a Historical object #
 the object attributes are set to: # - query the open-meteo Historical API # -
 query for hourly met data from 1970 to 2022 # - query a location in Western
 Australia hist = historical.Historical( location=(116.691155, -34.225812),
 date_range=("1970-01-01", "2022-12-31"), variables=["temperature_2m",
 "relativehumidity_2m"], met_data=None, glm_met_data=None ) # make a call to the
 open-meteo Historical API # download requested data and store as DataFrame # in
 the `hist.met_data.data` attribute hist.get_variables() # convert downloaded
```

### Comparing `glm-met-0.0.1/README.md` & `glm-met-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 <a href="https://colab.research.google.com/github/WET-tool/glm-met/blob/main/example-use.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ```
 import os
-import glm_met.openmeteo.hisorical as historical
+import glm_met.openmeteo.historical as historical
 
 # initialise a Historical object
 # the object attributes are set to:
 # - query the open-meteo Historical API 
 # - query for hourly met data from 1970 to 2022
 # - query a location in Western Australia
 hist = historical.Historical(
```

#### html2text {}

```diff
@@ -11,15 +11,15 @@
 MacOS, and Windows. It is actively developed by the Aquatic EcoDynamics
 research group at The University of Western Australia. ## Install ``` pip
 install glm-met ``` ## Use Import the glm-met package into a Python program and
 use to download meteorological data from a supported data provider. The
 following Jupyter notebook can be opened on Google Colab to demonstrate how
 glm-met can be used to download meteorological data from open-meteo's
 Historical API: [Open_In_Colab] ``` import os import
-glm_met.openmeteo.hisorical as historical # initialise a Historical object #
+glm_met.openmeteo.historical as historical # initialise a Historical object #
 the object attributes are set to: # - query the open-meteo Historical API # -
 query for hourly met data from 1970 to 2022 # - query a location in Western
 Australia hist = historical.Historical( location=(116.691155, -34.225812),
 date_range=("1970-01-01", "2022-12-31"), variables=["temperature_2m",
 "relativehumidity_2m"], met_data=None, glm_met_data=None ) # make a call to the
 open-meteo Historical API # download requested data and store as DataFrame # in
 the `hist.met_data.data` attribute hist.get_variables() # convert downloaded
```

### Comparing `glm-met-0.0.1/glm_met/glm_met.py` & `glm-met-0.0.2/glm_met/glm_met.py`

 * *Files identical despite different names*

### Comparing `glm-met-0.0.1/glm_met/openmeteo/climate_change.py` & `glm-met-0.0.2/glm_met/openmeteo/climate_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,17 @@
         Parameters
         ----------
         path : str
             Path to the directory where the zip file should be saved.
         """
 
         with tempfile.TemporaryDirectory() as tmpdir:
-            self.met_data.data.to_csv(os.path.join(tmpdir, "met_raw.csv"))
+            self.met_data.data.to_csv(
+                os.path.join(tmpdir, "met_raw.csv"), index=False
+            )
 
             with open(
                 os.path.join(tmpdir, "met_raw_metadata.json"), "w"
             ) as dst:
                 json.dump(self.met_data.metadata, dst)
 
             data_fpath = os.path.join(tmpdir, "met_raw.csv")
@@ -223,15 +225,17 @@
             Path to the directory where the zip file should be saved.
         """
 
         files = []
         with tempfile.TemporaryDirectory() as tmpdir:
             for m in self.models:
                 tmp_df = self.glm_met_data[m]
-                tmp_df.to_csv(os.path.join(tmpdir, f"met_{m}.csv"))
+                tmp_df.to_csv(
+                    os.path.join(tmpdir, f"met_{m}.csv"), index=False
+                )
                 files.append(os.path.join(tmpdir, f"met_{m}.csv"))
 
             with zipfile.ZipFile(
                 os.path.join(path, "met_glm.zip"), mode="w"
             ) as z_dst:
                 for file in files:
                     z_dst.write(file, arcname=file.split("/")[-1])
```

### Comparing `glm-met-0.0.1/glm_met/openmeteo/historical.py` & `glm-met-0.0.2/glm_met/openmeteo/historical.py`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,17 @@
         Parameters
         ----------
         path : str
             Path to the directory where the zip file should be saved.
         """
 
         with tempfile.TemporaryDirectory() as tmpdir:
-            self.met_data.data.to_csv(os.path.join(tmpdir, "met_raw.csv"))
+            self.met_data.data.to_csv(
+                os.path.join(tmpdir, "met_raw.csv"), index=False
+            )
 
             with open(
                 os.path.join(tmpdir, "met_raw_metadata.json"), "w"
             ) as dst:
                 json.dump(self.met_data.metadata, dst)
 
             data_fpath = os.path.join(tmpdir, "met_raw.csv")
@@ -261,15 +263,17 @@
         """
 
         if self.hourly:
             glm_metadata = self.met_data.metadata.pop("hourly_units")
 
             if zip_f:
                 with tempfile.TemporaryDirectory() as tmpdir:
-                    self.glm_met_data.to_csv(os.path.join(tmpdir, "met.csv"))
+                    self.glm_met_data.to_csv(
+                        os.path.join(tmpdir, "met.csv"), index=False
+                    )
 
                     with open(
                         os.path.join(tmpdir, "met_glm_metadata.json"), "w"
                     ) as dst:
                         json.dump(glm_metadata, dst)
 
                     data_fpath = os.path.join(tmpdir, "met.csv")
@@ -281,8 +285,10 @@
 
                     with zipfile.ZipFile(
                         os.path.join(path, "met_glm.zip"), mode="w"
                     ) as z_dst:
                         for file in files:
                             z_dst.write(file, arcname=file.split("/")[-1])
             else:
-                self.glm_met_data.to_csv(os.path.join(path, fname))
+                self.glm_met_data.to_csv(
+                    os.path.join(path, fname), index=False
+                )
```

### Comparing `glm-met-0.0.1/glm_met/openmeteo/settings.py` & `glm-met-0.0.2/glm_met/openmeteo/settings.py`

 * *Files identical despite different names*

### Comparing `glm-met-0.0.1/glm_met.egg-info/PKG-INFO` & `glm-met-0.0.2/glm_met.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glm-met
-Version: 0.0.1
+Version: 0.0.2
 Summary: Download meteorological data for the General Lake Model
 Author: John Duncan
 Project-URL: Homepage, https://wet-tool.github.io/glm-met/
 Keywords: GLM,meterological,weather,climate
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 
 <a href="https://colab.research.google.com/github/WET-tool/glm-met/blob/main/example-use.ipynb" target="_blank">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 
 ```
 import os
-import glm_met.openmeteo.hisorical as historical
+import glm_met.openmeteo.historical as historical
 
 # initialise a Historical object
 # the object attributes are set to:
 # - query the open-meteo Historical API 
 # - query for hourly met data from 1970 to 2022
 # - query a location in Western Australia
 hist = historical.Historical(
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glm-met Version: 0.0.1 Summary: Download
+Metadata-Version: 2.1 Name: glm-met Version: 0.0.2 Summary: Download
 meteorological data for the General Lake Model Author: John Duncan Project-URL:
 Homepage, https://wet-tool.github.io/glm-met/ Keywords:
 GLM,meterological,weather,climate Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Requires-Python: >=3.9 Description-Content-Type: text/
 markdown License-File: LICENSE # GLM-met A Python package for downloading
 meteorological data and processing it to formats required for running the GLM
@@ -17,15 +17,15 @@
 available as an executable for Linux (Ubuntu), MacOS, and Windows. It is
 actively developed by the Aquatic EcoDynamics research group at The University
 of Western Australia. ## Install ``` pip install glm-met ``` ## Use Import the
 glm-met package into a Python program and use to download meteorological data
 from a supported data provider. The following Jupyter notebook can be opened on
 Google Colab to demonstrate how glm-met can be used to download meteorological
 data from open-meteo's Historical API: [Open_In_Colab] ``` import os import
-glm_met.openmeteo.hisorical as historical # initialise a Historical object #
+glm_met.openmeteo.historical as historical # initialise a Historical object #
 the object attributes are set to: # - query the open-meteo Historical API # -
 query for hourly met data from 1970 to 2022 # - query a location in Western
 Australia hist = historical.Historical( location=(116.691155, -34.225812),
 date_range=("1970-01-01", "2022-12-31"), variables=["temperature_2m",
 "relativehumidity_2m"], met_data=None, glm_met_data=None ) # make a call to the
 open-meteo Historical API # download requested data and store as DataFrame # in
 the `hist.met_data.data` attribute hist.get_variables() # convert downloaded
```

### Comparing `glm-met-0.0.1/pyproject.toml` & `glm-met-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "glm-met"
-version = "0.0.1"
+version = "0.0.2"
 description = "Download meteorological data for the General Lake Model"
 readme = "README.md"
 authors = [{name = "John Duncan"}]
 license = { file = "LICESNE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `glm-met-0.0.1/tests/test_openmeteo_climate.py` & `glm-met-0.0.2/tests/test_openmeteo_climate.py`

 * *Files identical despite different names*

### Comparing `glm-met-0.0.1/tests/test_openmeteo_historical.py` & `glm-met-0.0.2/tests/test_openmeteo_historical.py`

 * *Files identical despite different names*


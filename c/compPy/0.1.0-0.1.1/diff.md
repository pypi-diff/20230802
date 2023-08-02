# Comparing `tmp/compPy-0.1.0.tar.gz` & `tmp/compPy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "compPy-0.1.0.tar", last modified: Wed Aug  2 08:49:37 2023, max compression
+gzip compressed data, was "compPy-0.1.1.tar", last modified: Wed Aug  2 09:07:07 2023, max compression
```

## Comparing `compPy-0.1.0.tar` & `compPy-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.633652 compPy-0.1.0/
--rw-r--r--   0 richardmorton   (502) staff       (20)     1305 2023-08-01 19:36:20.000000 compPy-0.1.0/LICENSE
--rw-r--r--   0 richardmorton   (502) staff       (20)      693 2023-08-02 08:49:37.633262 compPy-0.1.0/PKG-INFO
--rw-r--r--   0 richardmorton   (502) staff       (20)       10 2023-08-01 14:52:20.000000 compPy-0.1.0/README.md
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.615962 compPy-0.1.0/compPy/
--rw-r--r--   0 richardmorton   (502) staff       (20)      242 2023-08-01 19:56:57.000000 compPy-0.1.0/compPy/__init__.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     7561 2023-07-10 14:19:22.000000 compPy-0.1.0/compPy/align.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    14153 2023-07-12 09:30:44.000000 compPy-0.1.0/compPy/compute_speed.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    16011 2023-08-01 20:21:01.000000 compPy-0.1.0/compPy/compute_waveang.py
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.619084 compPy-0.1.0/compPy/density/
--rw-r--r--   0 richardmorton   (502) staff       (20)        0 2023-08-02 07:46:37.000000 compPy-0.1.0/compPy/density/__init__.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     6199 2022-07-04 10:43:10.000000 compPy-0.1.0/compPy/density/density.py
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.621985 compPy-0.1.0/compPy/developments/
--rw-r--r--   0 richardmorton   (502) staff       (20)    17752 2021-05-25 15:32:02.000000 compPy-0.1.0/compPy/developments/compute_speed_old.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    15365 2022-01-24 13:03:29.000000 compPy-0.1.0/compPy/developments/compute_waveang_dev_v2.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     9371 2022-01-24 13:03:29.000000 compPy-0.1.0/compPy/developments/compute_waveang_old.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    18096 2021-05-24 07:54:26.000000 compPy-0.1.0/compPy/developments/velocity_calc.py
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.623992 compPy-0.1.0/compPy/io/
--rw-r--r--   0 richardmorton   (502) staff       (20)        0 2023-08-01 19:46:50.000000 compPy-0.1.0/compPy/io/__init__.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    17967 2022-07-04 10:38:30.000000 compPy-0.1.0/compPy/io/in_out.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    14074 2022-06-22 13:19:11.000000 compPy-0.1.0/compPy/io/save_load.py
--rw-r--r--   0 richardmorton   (502) staff       (20)      613 2021-07-28 08:40:17.000000 compPy-0.1.0/compPy/load_defaults.py
--rw-r--r--   0 richardmorton   (502) staff       (20)    17121 2023-08-02 07:46:03.000000 compPy-0.1.0/compPy/space_time_run.py
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.625877 compPy-0.1.0/compPy/tests/
--rw-r--r--   0 richardmorton   (502) staff       (20)     2895 2021-05-24 07:54:48.000000 compPy-0.1.0/compPy/tests/test_io.py
--rw-r--r--   0 richardmorton   (502) staff       (20)      269 2021-05-24 07:54:54.000000 compPy-0.1.0/compPy/tests/test_load_defaults.py
--rw-r--r--   0 richardmorton   (502) staff       (20)      365 2021-05-24 07:54:59.000000 compPy-0.1.0/compPy/tests/test_util.py
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.632495 compPy-0.1.0/compPy/util/
--rw-r--r--   0 richardmorton   (502) staff       (20)       30 2023-08-01 20:05:34.000000 compPy-0.1.0/compPy/util/__init__.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     2411 2023-08-01 10:51:41.000000 compPy-0.1.0/compPy/util/config.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     1703 2022-01-24 13:03:29.000000 compPy-0.1.0/compPy/util/do_apod.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     1818 2022-03-25 16:26:53.000000 compPy-0.1.0/compPy/util/filter_funcs.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     4092 2021-08-04 12:57:25.000000 compPy-0.1.0/compPy/util/intensity_filler.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     4111 2021-05-27 10:00:09.000000 compPy-0.1.0/compPy/util/map_tools.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     5083 2022-01-24 13:03:29.000000 compPy-0.1.0/compPy/util/spectraldensity.py
--rw-r--r--   0 richardmorton   (502) staff       (20)     3496 2023-08-01 20:02:11.000000 compPy-0.1.0/compPy/util/util.py
-drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 08:49:37.618426 compPy-0.1.0/compPy.egg-info/
--rw-r--r--   0 richardmorton   (502) staff       (20)      693 2023-08-02 08:49:37.000000 compPy-0.1.0/compPy.egg-info/PKG-INFO
--rw-r--r--   0 richardmorton   (502) staff       (20)      890 2023-08-02 08:49:37.000000 compPy-0.1.0/compPy.egg-info/SOURCES.txt
--rw-r--r--   0 richardmorton   (502) staff       (20)        1 2023-08-02 08:49:37.000000 compPy-0.1.0/compPy.egg-info/dependency_links.txt
--rw-r--r--   0 richardmorton   (502) staff       (20)      125 2023-08-02 08:49:37.000000 compPy-0.1.0/compPy.egg-info/requires.txt
--rw-r--r--   0 richardmorton   (502) staff       (20)        7 2023-08-02 08:49:37.000000 compPy-0.1.0/compPy.egg-info/top_level.txt
--rw-r--r--   0 richardmorton   (502) staff       (20)      921 2023-08-02 08:49:25.000000 compPy-0.1.0/pyproject.toml
--rw-r--r--   0 richardmorton   (502) staff       (20)       38 2023-08-02 08:49:37.633742 compPy-0.1.0/setup.cfg
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.950000 compPy-0.1.1/
+-rw-r--r--   0 richardmorton   (502) staff       (20)     1305 2023-08-01 19:36:20.000000 compPy-0.1.1/LICENSE
+-rw-r--r--   0 richardmorton   (502) staff       (20)      693 2023-08-02 09:07:07.949758 compPy-0.1.1/PKG-INFO
+-rw-r--r--   0 richardmorton   (502) staff       (20)       10 2023-08-01 14:52:20.000000 compPy-0.1.1/README.md
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.936560 compPy-0.1.1/compPy/
+-rw-r--r--   0 richardmorton   (502) staff       (20)      242 2023-08-01 19:56:57.000000 compPy-0.1.1/compPy/__init__.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     7561 2023-07-10 14:19:22.000000 compPy-0.1.1/compPy/align.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    14153 2023-07-12 09:30:44.000000 compPy-0.1.1/compPy/compute_speed.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    16011 2023-08-01 20:21:01.000000 compPy-0.1.1/compPy/compute_waveang.py
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.938791 compPy-0.1.1/compPy/density/
+-rw-r--r--   0 richardmorton   (502) staff       (20)        0 2023-08-02 07:46:37.000000 compPy-0.1.1/compPy/density/__init__.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     6199 2022-07-04 10:43:10.000000 compPy-0.1.1/compPy/density/density.py
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.941412 compPy-0.1.1/compPy/developments/
+-rw-r--r--   0 richardmorton   (502) staff       (20)    17752 2021-05-25 15:32:02.000000 compPy-0.1.1/compPy/developments/compute_speed_old.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    15365 2022-01-24 13:03:29.000000 compPy-0.1.1/compPy/developments/compute_waveang_dev_v2.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     9371 2022-01-24 13:03:29.000000 compPy-0.1.1/compPy/developments/compute_waveang_old.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    18096 2021-05-24 07:54:26.000000 compPy-0.1.1/compPy/developments/velocity_calc.py
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.943549 compPy-0.1.1/compPy/io/
+-rw-r--r--   0 richardmorton   (502) staff       (20)        0 2023-08-01 19:46:50.000000 compPy-0.1.1/compPy/io/__init__.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    17967 2022-07-04 10:38:30.000000 compPy-0.1.1/compPy/io/in_out.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    14074 2022-06-22 13:19:11.000000 compPy-0.1.1/compPy/io/save_load.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)      613 2021-07-28 08:40:17.000000 compPy-0.1.1/compPy/load_defaults.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)    17121 2023-08-02 07:46:03.000000 compPy-0.1.1/compPy/space_time_run.py
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.945252 compPy-0.1.1/compPy/tests/
+-rw-r--r--   0 richardmorton   (502) staff       (20)     2895 2021-05-24 07:54:48.000000 compPy-0.1.1/compPy/tests/test_io.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)      269 2021-05-24 07:54:54.000000 compPy-0.1.1/compPy/tests/test_load_defaults.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)      365 2021-05-24 07:54:59.000000 compPy-0.1.1/compPy/tests/test_util.py
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.949188 compPy-0.1.1/compPy/util/
+-rw-r--r--   0 richardmorton   (502) staff       (20)       30 2023-08-01 20:05:34.000000 compPy-0.1.1/compPy/util/__init__.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     2411 2023-08-01 10:51:41.000000 compPy-0.1.1/compPy/util/config.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     1703 2022-01-24 13:03:29.000000 compPy-0.1.1/compPy/util/do_apod.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     1818 2022-03-25 16:26:53.000000 compPy-0.1.1/compPy/util/filter_funcs.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     4092 2021-08-04 12:57:25.000000 compPy-0.1.1/compPy/util/intensity_filler.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     4111 2021-05-27 10:00:09.000000 compPy-0.1.1/compPy/util/map_tools.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     5083 2022-01-24 13:03:29.000000 compPy-0.1.1/compPy/util/spectraldensity.py
+-rw-r--r--   0 richardmorton   (502) staff       (20)     3496 2023-08-01 20:02:11.000000 compPy-0.1.1/compPy/util/util.py
+drwxr-xr-x   0 richardmorton   (502) staff       (20)        0 2023-08-02 09:07:07.938328 compPy-0.1.1/compPy.egg-info/
+-rw-r--r--   0 richardmorton   (502) staff       (20)      693 2023-08-02 09:07:07.000000 compPy-0.1.1/compPy.egg-info/PKG-INFO
+-rw-r--r--   0 richardmorton   (502) staff       (20)      890 2023-08-02 09:07:07.000000 compPy-0.1.1/compPy.egg-info/SOURCES.txt
+-rw-r--r--   0 richardmorton   (502) staff       (20)        1 2023-08-02 09:07:07.000000 compPy-0.1.1/compPy.egg-info/dependency_links.txt
+-rw-r--r--   0 richardmorton   (502) staff       (20)      126 2023-08-02 09:07:07.000000 compPy-0.1.1/compPy.egg-info/requires.txt
+-rw-r--r--   0 richardmorton   (502) staff       (20)        7 2023-08-02 09:07:07.000000 compPy-0.1.1/compPy.egg-info/top_level.txt
+-rw-r--r--   0 richardmorton   (502) staff       (20)      922 2023-08-02 09:06:53.000000 compPy-0.1.1/pyproject.toml
+-rw-r--r--   0 richardmorton   (502) staff       (20)       38 2023-08-02 09:07:07.950068 compPy-0.1.1/setup.cfg
```

### Comparing `compPy-0.1.0/LICENSE` & `compPy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/PKG-INFO` & `compPy-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for working with (u)CoMP data.
 Author-email: Richard Morton <richard.morton@northumbria.ac.uk>
 Project-URL: Homepage, https://github.com/Richardjmorton/compPy
 Project-URL: Bug Tracker, https://github.com/Richardjmorton/compPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `compPy-0.1.0/compPy/align.py` & `compPy-0.1.1/compPy/align.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/compute_speed.py` & `compPy-0.1.1/compPy/compute_speed.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/compute_waveang.py` & `compPy-0.1.1/compPy/compute_waveang.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/density/density.py` & `compPy-0.1.1/compPy/density/density.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/developments/compute_speed_old.py` & `compPy-0.1.1/compPy/developments/compute_speed_old.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/developments/compute_waveang_dev_v2.py` & `compPy-0.1.1/compPy/developments/compute_waveang_dev_v2.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/developments/compute_waveang_old.py` & `compPy-0.1.1/compPy/developments/compute_waveang_old.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/developments/velocity_calc.py` & `compPy-0.1.1/compPy/developments/velocity_calc.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/io/in_out.py` & `compPy-0.1.1/compPy/io/in_out.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/io/save_load.py` & `compPy-0.1.1/compPy/io/save_load.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/load_defaults.py` & `compPy-0.1.1/compPy/load_defaults.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/space_time_run.py` & `compPy-0.1.1/compPy/space_time_run.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/tests/test_io.py` & `compPy-0.1.1/compPy/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/config.py` & `compPy-0.1.1/compPy/util/config.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/do_apod.py` & `compPy-0.1.1/compPy/util/do_apod.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/filter_funcs.py` & `compPy-0.1.1/compPy/util/filter_funcs.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/intensity_filler.py` & `compPy-0.1.1/compPy/util/intensity_filler.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/map_tools.py` & `compPy-0.1.1/compPy/util/map_tools.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/spectraldensity.py` & `compPy-0.1.1/compPy/util/spectraldensity.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy/util/util.py` & `compPy-0.1.1/compPy/util/util.py`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/compPy.egg-info/PKG-INFO` & `compPy-0.1.1/compPy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compPy
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for working with (u)CoMP data.
 Author-email: Richard Morton <richard.morton@northumbria.ac.uk>
 Project-URL: Homepage, https://github.com/Richardjmorton/compPy
 Project-URL: Bug Tracker, https://github.com/Richardjmorton/compPy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `compPy-0.1.0/compPy.egg-info/SOURCES.txt` & `compPy-0.1.1/compPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compPy-0.1.0/pyproject.toml` & `compPy-0.1.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "compPy"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Richard Morton", email="richard.morton@northumbria.ac.uk" },
 ]
 description = "A package for working with (u)CoMP data."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -17,15 +17,15 @@
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 dependencies = [
-  "sunpy>5.0.0",
+  "sunpy>=5.0.0",
   "numpy>=1.21.0",
   "scipy>=1.7.0,!=1.10.0",
   "matplotlib>=3.5.0",
   "astropy>=5.0.1",
   "more-itertools>=10.0.0",
   "scikit-image>=0.18.0"
 ]
```


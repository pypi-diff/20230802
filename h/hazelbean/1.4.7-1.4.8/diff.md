# Comparing `tmp/hazelbean-1.4.7.tar.gz` & `tmp/hazelbean-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazelbean-1.4.7.tar", last modified: Mon Jun 19 18:10:00 2023, max compression
+gzip compressed data, was "hazelbean-1.4.8.tar", last modified: Wed Aug  2 16:24:25 2023, max compression
```

## Comparing `hazelbean-1.4.7.tar` & `hazelbean-1.4.8.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 18:10:00.900000 hazelbean-1.4.7/
--rw-rw-rw-   0        0        0    14763 2023-06-19 18:09:54.000000 hazelbean-1.4.7/LICENSE
--rw-rw-rw-   0        0        0      145 2023-06-19 18:09:54.000000 hazelbean-1.4.7/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-06-19 18:10:00.868000 hazelbean-1.4.7/PKG-INFO
--rw-rw-rw-   0        0        0     4863 2023-06-19 18:09:54.000000 hazelbean-1.4.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 18:09:59.303000 hazelbean-1.4.7/hazelbean/
--rw-rw-rw-   0        0        0     8196 2022-09-28 15:14:40.000000 hazelbean-1.4.7/hazelbean/__init__.py
--rw-rw-rw-   0        0        0    15645 2022-09-28 14:32:01.000000 hazelbean-1.4.7/hazelbean/arrayframe.py
--rw-rw-rw-   0        0        0     6865 2022-05-09 18:31:33.000000 hazelbean-1.4.7/hazelbean/arrayframe_functions.py
--rw-rw-rw-   0        0        0     5787 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/arrayframe_numpy_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-19 18:10:00.258000 hazelbean-1.4.7/hazelbean/calculation_core/
--rw-rw-rw-   0        0        0     2523 2022-09-27 18:48:13.000000 hazelbean-1.4.7/hazelbean/calculation_core/__init__.py
--rw-rw-rw-   0        0        0   364367 2023-01-30 15:25:17.000000 hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.c
--rw-rw-rw-   0        0        0    59392 2023-01-30 15:25:21.000000 hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0   370413 2023-06-06 15:16:35.000000 hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.cpp
--rw-rw-rw-   0        0        0     5843 2023-01-30 15:25:06.000000 hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.pyx
--rw-rw-rw-   0        0        0      746 2023-06-01 20:11:21.000000 hazelbean-1.4.7/hazelbean/calculation_core/compile_cython_functions.py
--rw-rw-rw-   0        0        0  3445406 2023-06-01 20:11:20.000000 hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.c
--rw-rw-rw-   0        0        0   567808 2023-06-02 01:58:12.000000 hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  3452047 2023-06-06 15:16:35.000000 hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.cpp
--rw-rw-rw-   0        0        0   150011 2023-06-01 20:11:20.000000 hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.pyx
--rw-rw-rw-   0        0        0     4830 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/cat_ears.py
--rw-rw-rw-   0        0        0     7588 2023-06-12 16:50:12.000000 hazelbean-1.4.7/hazelbean/cloud_utils.py
--rw-rw-rw-   0        0        0    19206 2022-09-23 17:47:57.000000 hazelbean-1.4.7/hazelbean/config.py
--rw-rw-rw-   0        0        0     3471 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/conventions.py
--rw-rw-rw-   0        0        0     8594 2023-06-05 19:37:33.000000 hazelbean-1.4.7/hazelbean/core.py
--rw-rw-rw-   0        0        0    21132 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/data_structures.py
--rw-rw-rw-   0        0        0    30780 2023-02-16 18:33:50.000000 hazelbean-1.4.7/hazelbean/file_io.py
--rw-rw-rw-   0        0        0   115964 2022-09-23 21:13:00.000000 hazelbean-1.4.7/hazelbean/geoprocessing.py
--rw-rw-rw-   0        0        0    74113 2023-03-08 17:18:14.000000 hazelbean-1.4.7/hazelbean/geoprocessing_extension.py
--rw-rw-rw-   0        0        0    44554 2022-09-22 15:56:20.000000 hazelbean-1.4.7/hazelbean/globals.py
--rw-rw-rw-   0        0        0    43887 2023-06-01 20:11:20.000000 hazelbean-1.4.7/hazelbean/netcdf.py
--rw-rw-rw-   0        0        0    75326 2023-06-01 20:11:20.000000 hazelbean-1.4.7/hazelbean/os_utils.py
--rw-rw-rw-   0        0        0    20647 2023-01-28 21:04:04.000000 hazelbean-1.4.7/hazelbean/parallel.py
--rw-rw-rw-   0        0        0    52148 2023-05-08 17:19:48.000000 hazelbean-1.4.7/hazelbean/project_flow.py
--rw-rw-rw-   0        0        0   100770 2023-05-09 13:27:50.000000 hazelbean-1.4.7/hazelbean/pyramids.py
--rw-rw-rw-   0        0        0    52342 2022-06-15 17:44:31.000000 hazelbean-1.4.7/hazelbean/raster_vector_interface.py
--rw-rw-rw-   0        0        0      290 2022-09-22 18:26:12.000000 hazelbean-1.4.7/hazelbean/slow_config.py
--rw-rw-rw-   0        0        0    38359 2022-09-28 14:32:01.000000 hazelbean-1.4.7/hazelbean/spatial_projection.py
--rw-rw-rw-   0        0        0   237426 2023-06-01 20:11:20.000000 hazelbean-1.4.7/hazelbean/spatial_utils.py
--rw-rw-rw-   0        0        0    90574 2023-01-12 21:05:30.000000 hazelbean-1.4.7/hazelbean/stats.py
-drwxrwxrwx   0        0        0        0 2023-06-19 18:10:00.850000 hazelbean-1.4.7/hazelbean/ui/
--rw-rw-rw-   0        0        0        0 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/__init__.py
--rw-rw-rw-   0        0        0     5376 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/auto_ui.py
--rw-rw-rw-   0        0        0     6353 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/auto_ui_tg.py
--rw-rw-rw-   0        0        0    23376 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/cli.py
--rw-rw-rw-   0        0        0    24868 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/datastack.py
--rw-rw-rw-   0        0        0     2621 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/execution.py
--rw-rw-rw-   0        0        0   102272 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/inputs.py
--rw-rw-rw-   0        0        0     2565 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/launcher.py
--rw-rw-rw-   0        0        0   112823 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/model.py
--rw-rw-rw-   0        0        0    10862 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/usage.py
--rw-rw-rw-   0        0        0     3750 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/usage_logger.py
--rw-rw-rw-   0        0        0    18766 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/utils.py
--rw-rw-rw-   0        0        0     5941 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/ui/validation.py
--rw-rw-rw-   0        0        0    32538 2023-06-19 17:00:23.000000 hazelbean-1.4.7/hazelbean/utils.py
--rw-rw-rw-   0        0        0    82552 2023-03-03 14:42:11.000000 hazelbean-1.4.7/hazelbean/visualization.py
--rw-rw-rw-   0        0        0     8838 2022-03-21 14:48:42.000000 hazelbean-1.4.7/hazelbean/watershed_processing.py
-drwxrwxrwx   0        0        0        0 2023-06-19 18:09:59.450000 hazelbean-1.4.7/hazelbean.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-19 18:09:57.000000 hazelbean-1.4.7/hazelbean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1857 2023-06-19 18:09:57.000000 hazelbean-1.4.7/hazelbean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 18:09:57.000000 hazelbean-1.4.7/hazelbean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-19 18:09:57.000000 hazelbean-1.4.7/hazelbean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-19 18:10:00.897000 hazelbean-1.4.7/setup.cfg
--rw-rw-rw-   0        0        0     1708 2023-06-19 18:09:54.000000 hazelbean-1.4.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:24:25.310000 hazelbean-1.4.8/
+-rw-rw-rw-   0        0        0    14763 2023-08-02 16:24:11.000000 hazelbean-1.4.8/LICENSE
+-rw-rw-rw-   0        0        0      145 2023-08-02 16:24:11.000000 hazelbean-1.4.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-08-02 16:24:25.271000 hazelbean-1.4.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4863 2023-08-02 16:24:11.000000 hazelbean-1.4.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:24:22.085000 hazelbean-1.4.8/hazelbean/
+-rw-rw-rw-   0        0        0     8196 2022-09-28 15:14:40.000000 hazelbean-1.4.8/hazelbean/__init__.py
+-rw-rw-rw-   0        0        0    15645 2022-09-28 14:32:01.000000 hazelbean-1.4.8/hazelbean/arrayframe.py
+-rw-rw-rw-   0        0        0     6865 2022-05-09 18:31:33.000000 hazelbean-1.4.8/hazelbean/arrayframe_functions.py
+-rw-rw-rw-   0        0        0     5787 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/arrayframe_numpy_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:24:23.910000 hazelbean-1.4.8/hazelbean/calculation_core/
+-rw-rw-rw-   0        0        0     2523 2022-09-27 18:48:13.000000 hazelbean-1.4.8/hazelbean/calculation_core/__init__.py
+-rw-rw-rw-   0        0        0   387786 2023-07-18 16:00:58.000000 hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.c
+-rw-rw-rw-   0        0        0    67584 2023-07-18 16:01:02.000000 hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   394185 2023-08-02 16:24:14.000000 hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.cpp
+-rw-rw-rw-   0        0        0     7088 2023-07-18 16:00:20.000000 hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.pyx
+-rw-rw-rw-   0        0        0      746 2023-06-01 20:11:21.000000 hazelbean-1.4.8/hazelbean/calculation_core/compile_cython_functions.py
+-rw-rw-rw-   0        0        0  3445406 2023-06-01 20:11:20.000000 hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.c
+-rw-rw-rw-   0        0        0   567808 2023-06-02 01:58:12.000000 hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  3452047 2023-06-06 15:16:35.000000 hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.cpp
+-rw-rw-rw-   0        0        0   150011 2023-06-01 20:11:20.000000 hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.pyx
+-rw-rw-rw-   0        0        0     4830 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/cat_ears.py
+-rw-rw-rw-   0        0        0     7588 2023-06-12 16:50:12.000000 hazelbean-1.4.8/hazelbean/cloud_utils.py
+-rw-rw-rw-   0        0        0    19206 2022-09-23 17:47:57.000000 hazelbean-1.4.8/hazelbean/config.py
+-rw-rw-rw-   0        0        0     3471 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/conventions.py
+-rw-rw-rw-   0        0        0     8594 2023-06-05 19:37:33.000000 hazelbean-1.4.8/hazelbean/core.py
+-rw-rw-rw-   0        0        0    21132 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/data_structures.py
+-rw-rw-rw-   0        0        0    30780 2023-02-16 18:33:50.000000 hazelbean-1.4.8/hazelbean/file_io.py
+-rw-rw-rw-   0        0        0   115964 2022-09-23 21:13:00.000000 hazelbean-1.4.8/hazelbean/geoprocessing.py
+-rw-rw-rw-   0        0        0    74113 2023-03-08 17:18:14.000000 hazelbean-1.4.8/hazelbean/geoprocessing_extension.py
+-rw-rw-rw-   0        0        0    44554 2022-09-22 15:56:20.000000 hazelbean-1.4.8/hazelbean/globals.py
+-rw-rw-rw-   0        0        0    43887 2023-06-01 20:11:20.000000 hazelbean-1.4.8/hazelbean/netcdf.py
+-rw-rw-rw-   0        0        0    75326 2023-06-01 20:11:20.000000 hazelbean-1.4.8/hazelbean/os_utils.py
+-rw-rw-rw-   0        0        0    20647 2023-01-28 21:04:04.000000 hazelbean-1.4.8/hazelbean/parallel.py
+-rw-rw-rw-   0        0        0    52149 2023-07-06 17:44:52.000000 hazelbean-1.4.8/hazelbean/project_flow.py
+-rw-rw-rw-   0        0        0   100770 2023-05-09 13:27:50.000000 hazelbean-1.4.8/hazelbean/pyramids.py
+-rw-rw-rw-   0        0        0    52342 2022-06-15 17:44:31.000000 hazelbean-1.4.8/hazelbean/raster_vector_interface.py
+-rw-rw-rw-   0        0        0      290 2022-09-22 18:26:12.000000 hazelbean-1.4.8/hazelbean/slow_config.py
+-rw-rw-rw-   0        0        0    38359 2022-09-28 14:32:01.000000 hazelbean-1.4.8/hazelbean/spatial_projection.py
+-rw-rw-rw-   0        0        0   237426 2023-06-01 20:11:20.000000 hazelbean-1.4.8/hazelbean/spatial_utils.py
+-rw-rw-rw-   0        0        0    90574 2023-01-12 21:05:30.000000 hazelbean-1.4.8/hazelbean/stats.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:24:25.252000 hazelbean-1.4.8/hazelbean/ui/
+-rw-rw-rw-   0        0        0        0 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/__init__.py
+-rw-rw-rw-   0        0        0     5376 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/auto_ui.py
+-rw-rw-rw-   0        0        0     6353 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/auto_ui_tg.py
+-rw-rw-rw-   0        0        0    23376 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/cli.py
+-rw-rw-rw-   0        0        0    24868 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/datastack.py
+-rw-rw-rw-   0        0        0     2621 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/execution.py
+-rw-rw-rw-   0        0        0   102272 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/inputs.py
+-rw-rw-rw-   0        0        0     2565 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/launcher.py
+-rw-rw-rw-   0        0        0   112823 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/model.py
+-rw-rw-rw-   0        0        0    10862 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/usage.py
+-rw-rw-rw-   0        0        0     3750 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/usage_logger.py
+-rw-rw-rw-   0        0        0    18766 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/utils.py
+-rw-rw-rw-   0        0        0     5941 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/ui/validation.py
+-rw-rw-rw-   0        0        0    32538 2023-06-19 17:00:23.000000 hazelbean-1.4.8/hazelbean/utils.py
+-rw-rw-rw-   0        0        0    82552 2023-07-12 15:18:53.000000 hazelbean-1.4.8/hazelbean/visualization.py
+-rw-rw-rw-   0        0        0     8838 2022-03-21 14:48:42.000000 hazelbean-1.4.8/hazelbean/watershed_processing.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:24:22.383000 hazelbean-1.4.8/hazelbean.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-08-02 16:24:15.000000 hazelbean-1.4.8/hazelbean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1857 2023-08-02 16:24:16.000000 hazelbean-1.4.8/hazelbean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:24:15.000000 hazelbean-1.4.8/hazelbean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 16:24:15.000000 hazelbean-1.4.8/hazelbean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 16:24:25.306000 hazelbean-1.4.8/setup.cfg
+-rw-rw-rw-   0        0        0     1708 2023-08-02 16:24:11.000000 hazelbean-1.4.8/setup.py
```

### Comparing `hazelbean-1.4.7/LICENSE` & `hazelbean-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/README.md` & `hazelbean-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/__init__.py` & `hazelbean-1.4.8/hazelbean/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/arrayframe.py` & `hazelbean-1.4.8/hazelbean/arrayframe.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/arrayframe_functions.py` & `hazelbean-1.4.8/hazelbean/arrayframe_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/arrayframe_numpy_functions.py` & `hazelbean-1.4.8/hazelbean/arrayframe_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/__init__.py` & `hazelbean-1.4.8/hazelbean/calculation_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.c` & `hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.33 */
+/* Generated by Cython 0.29.34 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_33"
-#define CYTHON_HEX_VERSION 0x001D21F0
+#define CYTHON_ABI "0_29_34"
+#define CYTHON_HEX_VERSION 0x001D22F0
 #define CYTHON_FUTURE_DIVISION 0
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -199,15 +199,15 @@
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
   #if PY_VERSION_HEX < 0x02070000
     #undef CYTHON_USE_PYLONG_INTERNALS
     #define CYTHON_USE_PYLONG_INTERNALS 0
   #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
-    #define CYTHON_USE_PYLONG_INTERNALS 1
+    #define CYTHON_USE_PYLONG_INTERNALS (PY_VERSION_HEX < 0x030C00A5)
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
@@ -238,15 +238,15 @@
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+    #define CYTHON_USE_DICT_VERSIONS ((PY_VERSION_HEX >= 0x030600B1) && (PY_VERSION_HEX < 0x030C00A5))
   #endif
   #if PY_VERSION_HEX >= 0x030B00A4
     #undef CYTHON_USE_EXC_INFO_STACK
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
@@ -1020,195 +1020,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":689
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":690
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":691
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":692
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":696
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":697
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":698
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":699
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":703
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":704
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":713
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":714
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":715
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":715
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":717
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":718
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":719
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":719
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":721
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":722
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":724
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":725
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":726
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1271,42 +1271,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":728
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":729
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":730
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":732
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -1633,20 +1633,28 @@
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
 /* TypeImport.proto */
 #ifndef __PYX_HAVE_RT_ImportType_proto
 #define __PYX_HAVE_RT_ImportType_proto
+#if __STDC_VERSION__ >= 201112L
+#include <stdalign.h>
+#endif
+#if __STDC_VERSION__ >= 201112L || __cplusplus >= 201103L
+#define __PYX_GET_STRUCT_ALIGNMENT(s) alignof(s)
+#else
+#define __PYX_GET_STRUCT_ALIGNMENT(s) sizeof(void*)
+#endif
 enum __Pyx_ImportType_CheckSize {
    __Pyx_ImportType_CheckSize_Error = 0,
    __Pyx_ImportType_CheckSize_Warn = 1,
    __Pyx_ImportType_CheckSize_Ignore = 2
 };
-static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, enum __Pyx_ImportType_CheckSize check_size);
+static PyTypeObject *__Pyx_ImportType(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size);
 #endif
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
@@ -1899,14 +1907,15 @@
 static const char __pyx_k_fc[] = "fc";
 static const char __pyx_k_fr[] = "fr";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_byte[] = "byte";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_math[] = "math";
+static const char __pyx_k_mean[] = "mean";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_int64[] = "int64";
@@ -1936,14 +1945,15 @@
 static const char __pyx_k_naive_downscale[] = "naive_downscale";
 static const char __pyx_k_num_coarse_cols[] = "num_coarse_cols";
 static const char __pyx_k_num_coarse_rows[] = "num_coarse_rows";
 static const char __pyx_k_coarse_res_array[] = "coarse_res_array";
 static const char __pyx_k_downscale_factor[] = "downscale_factor";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_current_proportion[] = "current_proportion";
+static const char __pyx_k_upscale_using_mean[] = "upscale_using_mean";
 static const char __pyx_k_naive_downscale_byte[] = "naive_downscale_byte";
 static const char __pyx_k_upscale_retaining_sum[] = "upscale_retaining_sum";
 static const char __pyx_k_aspect_ratio_array_functions[] = "aspect_ratio_array_functions";
 static const char __pyx_k_coarse_res_proporition_array[] = "coarse_res_proporition_array";
 static const char __pyx_k_fine_res_cells_per_coarse_cell[] = "fine_res_cells_per_coarse_cell";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_aspect_ratio_array_functions_pyx[] = "aspect_ratio_array_functions.pyx";
@@ -1982,14 +1992,15 @@
 static PyObject *__pyx_n_s_fr_start;
 static PyObject *__pyx_n_s_high_res_array;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_s_int64;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_math;
+static PyObject *__pyx_n_s_mean;
 static PyObject *__pyx_n_s_naive_downscale;
 static PyObject *__pyx_n_s_naive_downscale_byte;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_num_coarse_cols;
 static PyObject *__pyx_n_s_num_coarse_rows;
 static PyObject *__pyx_n_s_num_fine_cols;
@@ -2000,28 +2011,32 @@
 static PyObject *__pyx_n_s_output_array;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_sum;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_upscale_factor;
 static PyObject *__pyx_n_s_upscale_retaining_sum;
+static PyObject *__pyx_n_s_upscale_using_mean;
 static PyObject *__pyx_pf_28aspect_ratio_array_functions_cython_calc_proportion_of_coarse_res_with_valid_fine_res(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_coarse_res_array, PyArrayObject *__pyx_v_fine_res_array); /* proto */
 static PyObject *__pyx_pf_28aspect_ratio_array_functions_2naive_downscale(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_coarse_res_array, PY_LONG_LONG __pyx_v_downscale_factor); /* proto */
 static PyObject *__pyx_pf_28aspect_ratio_array_functions_4naive_downscale_byte(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_coarse_res_array, PY_LONG_LONG __pyx_v_downscale_factor); /* proto */
 static PyObject *__pyx_pf_28aspect_ratio_array_functions_6upscale_retaining_sum(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_high_res_array, PY_LONG_LONG __pyx_v_upscale_factor); /* proto */
+static PyObject *__pyx_pf_28aspect_ratio_array_functions_8upscale_using_mean(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_high_res_array, PY_LONG_LONG __pyx_v_upscale_factor); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
 /* Late includes */
 
 /* "aspect_ratio_array_functions.pyx":45
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def cython_calc_proportion_of_coarse_res_with_valid_fine_res(np.ndarray[np.float64_t, ndim=2] coarse_res_array,             # <<<<<<<<<<<<<<
  *                                                       np.ndarray[np.int64_t, ndim=2] fine_res_array,
@@ -3130,21 +3145,21 @@
   return __pyx_r;
 }
 
 /* "aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_28aspect_ratio_array_functions_7upscale_retaining_sum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_28aspect_ratio_array_functions_6upscale_retaining_sum[] = "upscale_retaining_sum(ndarray high_res_array, long long upscale_factor)\nReturn an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res.";
+static char __pyx_doc_28aspect_ratio_array_functions_6upscale_retaining_sum[] = "upscale_retaining_sum(ndarray high_res_array, long long upscale_factor)\nReturn an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res.";
 static PyMethodDef __pyx_mdef_28aspect_ratio_array_functions_7upscale_retaining_sum = {"upscale_retaining_sum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_28aspect_ratio_array_functions_7upscale_retaining_sum, METH_VARARGS|METH_KEYWORDS, __pyx_doc_28aspect_ratio_array_functions_6upscale_retaining_sum};
 static PyObject *__pyx_pw_28aspect_ratio_array_functions_7upscale_retaining_sum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_high_res_array = 0;
   PY_LONG_LONG __pyx_v_upscale_factor;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3259,15 +3274,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_high_res_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 111, __pyx_L1_error)
   }
   __pyx_pybuffernd_high_res_array.diminfo[0].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_high_res_array.diminfo[0].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_high_res_array.diminfo[1].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_high_res_array.diminfo[1].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[1];
 
   /* "aspect_ratio_array_functions.pyx":114
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  *     cdef long long num_fine_rows = high_res_array.shape[0]             # <<<<<<<<<<<<<<
  *     cdef long long num_fine_cols = high_res_array.shape[1]
  * 
  */
   __pyx_v_num_fine_rows = (__pyx_v_high_res_array->dimensions[0]);
 
@@ -3501,15 +3516,15 @@
   __pyx_r = ((PyObject *)__pyx_v_output_array);
   goto __pyx_L0;
 
   /* "aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -3533,15 +3548,422 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_output_array);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":734
+/* "aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_28aspect_ratio_array_functions_9upscale_using_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_28aspect_ratio_array_functions_8upscale_using_mean[] = "upscale_using_mean(ndarray high_res_array, long long upscale_factor)\nReturn an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res.";
+static PyMethodDef __pyx_mdef_28aspect_ratio_array_functions_9upscale_using_mean = {"upscale_using_mean", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_28aspect_ratio_array_functions_9upscale_using_mean, METH_VARARGS|METH_KEYWORDS, __pyx_doc_28aspect_ratio_array_functions_8upscale_using_mean};
+static PyObject *__pyx_pw_28aspect_ratio_array_functions_9upscale_using_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyArrayObject *__pyx_v_high_res_array = 0;
+  PY_LONG_LONG __pyx_v_upscale_factor;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("upscale_using_mean (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_high_res_array,&__pyx_n_s_upscale_factor,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_high_res_array)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upscale_factor)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("upscale_using_mean", 1, 2, 2, 1); __PYX_ERR(0, 142, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "upscale_using_mean") < 0)) __PYX_ERR(0, 142, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_high_res_array = ((PyArrayObject *)values[0]);
+    __pyx_v_upscale_factor = __Pyx_PyInt_As_PY_LONG_LONG(values[1]); if (unlikely((__pyx_v_upscale_factor == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("upscale_using_mean", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 142, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("aspect_ratio_array_functions.upscale_using_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_high_res_array), __pyx_ptype_5numpy_ndarray, 1, "high_res_array", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_r = __pyx_pf_28aspect_ratio_array_functions_8upscale_using_mean(__pyx_self, __pyx_v_high_res_array, __pyx_v_upscale_factor);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_28aspect_ratio_array_functions_8upscale_using_mean(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_high_res_array, PY_LONG_LONG __pyx_v_upscale_factor) {
+  CYTHON_UNUSED PY_LONG_LONG __pyx_v_num_fine_rows;
+  CYTHON_UNUSED PY_LONG_LONG __pyx_v_num_fine_cols;
+  PY_LONG_LONG __pyx_v_num_coarse_rows;
+  PY_LONG_LONG __pyx_v_num_coarse_cols;
+  PY_LONG_LONG __pyx_v_cr;
+  PY_LONG_LONG __pyx_v_cc;
+  PY_LONG_LONG __pyx_v_fr_start;
+  PY_LONG_LONG __pyx_v_fr_end;
+  PY_LONG_LONG __pyx_v_fc_start;
+  PY_LONG_LONG __pyx_v_fc_end;
+  PyArrayObject *__pyx_v_output_array = 0;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_high_res_array;
+  __Pyx_Buffer __pyx_pybuffer_high_res_array;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_output_array;
+  __Pyx_Buffer __pyx_pybuffer_output_array;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyArrayObject *__pyx_t_6 = NULL;
+  PY_LONG_LONG __pyx_t_7;
+  PY_LONG_LONG __pyx_t_8;
+  PY_LONG_LONG __pyx_t_9;
+  PY_LONG_LONG __pyx_t_10;
+  PY_LONG_LONG __pyx_t_11;
+  PY_LONG_LONG __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
+  __pyx_t_5numpy_float64_t __pyx_t_14;
+  PY_LONG_LONG __pyx_t_15;
+  PY_LONG_LONG __pyx_t_16;
+  int __pyx_t_17;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("upscale_using_mean", 0);
+  __pyx_pybuffer_output_array.pybuffer.buf = NULL;
+  __pyx_pybuffer_output_array.refcount = 0;
+  __pyx_pybuffernd_output_array.data = NULL;
+  __pyx_pybuffernd_output_array.rcbuffer = &__pyx_pybuffer_output_array;
+  __pyx_pybuffer_high_res_array.pybuffer.buf = NULL;
+  __pyx_pybuffer_high_res_array.refcount = 0;
+  __pyx_pybuffernd_high_res_array.data = NULL;
+  __pyx_pybuffernd_high_res_array.rcbuffer = &__pyx_pybuffer_high_res_array;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_high_res_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_high_res_array.diminfo[0].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_high_res_array.diminfo[0].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_high_res_array.diminfo[1].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_high_res_array.diminfo[1].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[1];
+
+  /* "aspect_ratio_array_functions.pyx":145
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ *     cdef long long num_fine_rows = high_res_array.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef long long num_fine_cols = high_res_array.shape[1]
+ * 
+ */
+  __pyx_v_num_fine_rows = (__pyx_v_high_res_array->dimensions[0]);
+
+  /* "aspect_ratio_array_functions.pyx":146
+ * 
+ *     cdef long long num_fine_rows = high_res_array.shape[0]
+ *     cdef long long num_fine_cols = high_res_array.shape[1]             # <<<<<<<<<<<<<<
+ * 
+ *     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)
+ */
+  __pyx_v_num_fine_cols = (__pyx_v_high_res_array->dimensions[1]);
+
+  /* "aspect_ratio_array_functions.pyx":148
+ *     cdef long long num_fine_cols = high_res_array.shape[1]
+ * 
+ *     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)             # <<<<<<<<<<<<<<
+ *     cdef long long num_coarse_cols = <long long>(high_res_array.shape[1] / upscale_factor)
+ * 
+ */
+  __pyx_v_num_coarse_rows = ((PY_LONG_LONG)((__pyx_v_high_res_array->dimensions[0]) / __pyx_v_upscale_factor));
+
+  /* "aspect_ratio_array_functions.pyx":149
+ * 
+ *     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)
+ *     cdef long long num_coarse_cols = <long long>(high_res_array.shape[1] / upscale_factor)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_v_num_coarse_cols = ((PY_LONG_LONG)((__pyx_v_high_res_array->dimensions[1]) / __pyx_v_upscale_factor));
+
+  /* "aspect_ratio_array_functions.pyx":154
+ *     cdef long long cr, cc, fr_start, fr_end, fc_start, fc_end
+ * 
+ *     cdef np.ndarray[np.float64_t, ndim=2] output_array = np.empty([num_coarse_rows, num_coarse_cols], dtype=np.float64)             # <<<<<<<<<<<<<<
+ * 
+ *     for cr in range(num_coarse_rows):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_num_coarse_rows); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_num_coarse_cols); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
+  __pyx_t_1 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
+      __pyx_v_output_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_output_array.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 154, __pyx_L1_error)
+    } else {__pyx_pybuffernd_output_array.diminfo[0].strides = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output_array.diminfo[0].shape = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_output_array.diminfo[1].strides = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_output_array.diminfo[1].shape = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.shape[1];
+    }
+  }
+  __pyx_t_6 = 0;
+  __pyx_v_output_array = ((PyArrayObject *)__pyx_t_5);
+  __pyx_t_5 = 0;
+
+  /* "aspect_ratio_array_functions.pyx":156
+ *     cdef np.ndarray[np.float64_t, ndim=2] output_array = np.empty([num_coarse_rows, num_coarse_cols], dtype=np.float64)
+ * 
+ *     for cr in range(num_coarse_rows):             # <<<<<<<<<<<<<<
+ *         fr_start = cr * upscale_factor
+ *         fr_end = (cr + 1) * upscale_factor
+ */
+  __pyx_t_7 = __pyx_v_num_coarse_rows;
+  __pyx_t_8 = __pyx_t_7;
+  for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
+    __pyx_v_cr = __pyx_t_9;
+
+    /* "aspect_ratio_array_functions.pyx":157
+ * 
+ *     for cr in range(num_coarse_rows):
+ *         fr_start = cr * upscale_factor             # <<<<<<<<<<<<<<
+ *         fr_end = (cr + 1) * upscale_factor
+ *         for cc in range(num_coarse_cols):
+ */
+    __pyx_v_fr_start = (__pyx_v_cr * __pyx_v_upscale_factor);
+
+    /* "aspect_ratio_array_functions.pyx":158
+ *     for cr in range(num_coarse_rows):
+ *         fr_start = cr * upscale_factor
+ *         fr_end = (cr + 1) * upscale_factor             # <<<<<<<<<<<<<<
+ *         for cc in range(num_coarse_cols):
+ * 
+ */
+    __pyx_v_fr_end = ((__pyx_v_cr + 1) * __pyx_v_upscale_factor);
+
+    /* "aspect_ratio_array_functions.pyx":159
+ *         fr_start = cr * upscale_factor
+ *         fr_end = (cr + 1) * upscale_factor
+ *         for cc in range(num_coarse_cols):             # <<<<<<<<<<<<<<
+ * 
+ *             fc_start = cc * upscale_factor
+ */
+    __pyx_t_10 = __pyx_v_num_coarse_cols;
+    __pyx_t_11 = __pyx_t_10;
+    for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+      __pyx_v_cc = __pyx_t_12;
+
+      /* "aspect_ratio_array_functions.pyx":161
+ *         for cc in range(num_coarse_cols):
+ * 
+ *             fc_start = cc * upscale_factor             # <<<<<<<<<<<<<<
+ *             fc_end = (cc + 1) * upscale_factor
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+ */
+      __pyx_v_fc_start = (__pyx_v_cc * __pyx_v_upscale_factor);
+
+      /* "aspect_ratio_array_functions.pyx":162
+ * 
+ *             fc_start = cc * upscale_factor
+ *             fc_end = (cc + 1) * upscale_factor             # <<<<<<<<<<<<<<
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+ * 
+ */
+      __pyx_v_fc_end = ((__pyx_v_cc + 1) * __pyx_v_upscale_factor);
+
+      /* "aspect_ratio_array_functions.pyx":163
+ *             fc_start = cc * upscale_factor
+ *             fc_end = (cc + 1) * upscale_factor
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])             # <<<<<<<<<<<<<<
+ * 
+ *     return output_array
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fr_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fr_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = PySlice_New(__pyx_t_4, __pyx_t_2, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fc_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fc_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = PySlice_New(__pyx_t_2, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_GIVEREF(__pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+      __Pyx_GIVEREF(__pyx_t_13);
+      PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_13);
+      __pyx_t_1 = 0;
+      __pyx_t_13 = 0;
+      __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_high_res_array), __pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_4);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_13);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_14 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_15 = __pyx_v_cr;
+      __pyx_t_16 = __pyx_v_cc;
+      __pyx_t_17 = -1;
+      if (__pyx_t_15 < 0) {
+        __pyx_t_17 = 0;
+      } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_output_array.diminfo[0].shape)) __pyx_t_17 = 0;
+      if (__pyx_t_16 < 0) {
+        __pyx_t_17 = 1;
+      } else if (unlikely(__pyx_t_16 >= __pyx_pybuffernd_output_array.diminfo[1].shape)) __pyx_t_17 = 1;
+      if (unlikely(__pyx_t_17 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_17);
+        __PYX_ERR(0, 163, __pyx_L1_error)
+      }
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output_array.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_output_array.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_output_array.diminfo[1].strides) = __pyx_t_14;
+    }
+  }
+
+  /* "aspect_ratio_array_functions.pyx":165
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+ * 
+ *     return output_array             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_output_array));
+  __pyx_r = ((PyObject *)__pyx_v_output_array);
+  goto __pyx_L0;
+
+  /* "aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_13);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output_array.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("aspect_ratio_array_functions.upscale_using_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output_array.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_output_array);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3550,29 +3972,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":735
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":734
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3583,15 +4005,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":737
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3600,29 +4022,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":738
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":737
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3633,15 +4055,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":740
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3650,29 +4072,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":741
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":740
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3683,15 +4105,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":743
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3700,29 +4122,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":744
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":743
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3733,15 +4155,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":746
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3750,29 +4172,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":747
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":746
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3783,212 +4205,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":749
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":750
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":751
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":750
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":753
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":749
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":928
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":929
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":930
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":928
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":932
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":933
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":934
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":935
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":934
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":936
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":932
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":940
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4004,15 +4426,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":941
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4020,53 +4442,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":942
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":941
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":943
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":944
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
@@ -4074,30 +4496,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":941
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":940
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4112,15 +4534,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":946
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4136,15 +4558,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":947
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4152,53 +4574,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":948
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":947
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":949
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":950
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
@@ -4206,30 +4628,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":947
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":946
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4244,15 +4666,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":952
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4268,15 +4690,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":953
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4284,53 +4706,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":954
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":953
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":955
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":956
+      /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
@@ -4338,30 +4760,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":953
+    /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":952
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4376,176 +4798,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":966
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":978
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":966
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":981
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":993
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":981
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":996
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1003
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":996
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1006
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1010
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1006
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1013
+/* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1017
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1013
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4633,14 +5055,15 @@
   {&__pyx_n_s_fr_start, __pyx_k_fr_start, sizeof(__pyx_k_fr_start), 0, 0, 1, 1},
   {&__pyx_n_s_high_res_array, __pyx_k_high_res_array, sizeof(__pyx_k_high_res_array), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_math, __pyx_k_math, sizeof(__pyx_k_math), 0, 0, 1, 1},
+  {&__pyx_n_s_mean, __pyx_k_mean, sizeof(__pyx_k_mean), 0, 0, 1, 1},
   {&__pyx_n_s_naive_downscale, __pyx_k_naive_downscale, sizeof(__pyx_k_naive_downscale), 0, 0, 1, 1},
   {&__pyx_n_s_naive_downscale_byte, __pyx_k_naive_downscale_byte, sizeof(__pyx_k_naive_downscale_byte), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_num_coarse_cols, __pyx_k_num_coarse_cols, sizeof(__pyx_k_num_coarse_cols), 0, 0, 1, 1},
   {&__pyx_n_s_num_coarse_rows, __pyx_k_num_coarse_rows, sizeof(__pyx_k_num_coarse_rows), 0, 0, 1, 1},
   {&__pyx_n_s_num_fine_cols, __pyx_k_num_fine_cols, sizeof(__pyx_k_num_fine_cols), 0, 0, 1, 1},
@@ -4651,40 +5074,41 @@
   {&__pyx_n_s_output_array, __pyx_k_output_array, sizeof(__pyx_k_output_array), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_upscale_factor, __pyx_k_upscale_factor, sizeof(__pyx_k_upscale_factor), 0, 0, 1, 1},
   {&__pyx_n_s_upscale_retaining_sum, __pyx_k_upscale_retaining_sum, sizeof(__pyx_k_upscale_retaining_sum), 0, 0, 1, 1},
+  {&__pyx_n_s_upscale_using_mean, __pyx_k_upscale_using_mean, sizeof(__pyx_k_upscale_using_mean), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":944
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_s_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":950
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_s_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
@@ -4727,21 +5151,33 @@
   __Pyx_GIVEREF(__pyx_tuple__7);
   __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aspect_ratio_array_functions_pyx, __pyx_n_s_naive_downscale_byte, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 91, __pyx_L1_error)
 
   /* "aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
   __pyx_tuple__9 = PyTuple_Pack(13, __pyx_n_s_high_res_array, __pyx_n_s_upscale_factor, __pyx_n_s_num_fine_rows, __pyx_n_s_num_fine_cols, __pyx_n_s_num_coarse_rows, __pyx_n_s_num_coarse_cols, __pyx_n_s_cr, __pyx_n_s_cc, __pyx_n_s_fr_start, __pyx_n_s_fr_end, __pyx_n_s_fc_start, __pyx_n_s_fc_end, __pyx_n_s_output_array); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aspect_ratio_array_functions_pyx, __pyx_n_s_upscale_retaining_sum, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 111, __pyx_L1_error)
+
+  /* "aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+  __pyx_tuple__11 = PyTuple_Pack(13, __pyx_n_s_high_res_array, __pyx_n_s_upscale_factor, __pyx_n_s_num_fine_rows, __pyx_n_s_num_fine_cols, __pyx_n_s_num_coarse_rows, __pyx_n_s_num_coarse_cols, __pyx_n_s_cr, __pyx_n_s_cc, __pyx_n_s_fr_start, __pyx_n_s_fr_end, __pyx_n_s_fc_start, __pyx_n_s_fc_end, __pyx_n_s_output_array); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_aspect_ratio_array_functions_pyx, __pyx_n_s_upscale_using_mean, 142, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4807,52 +5243,67 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_4type_type = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT(PyHeapTypeObject),
   #endif
   __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(2, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT(PyArray_Descr),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayMultiIterObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT(PyArrayObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_number = __Pyx_ImportType(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __Pyx_ImportType_CheckSize_Warn);
+  __pyx_ptype_5numpy_character = __Pyx_ImportType(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT(PyObject),
+  __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __Pyx_ImportType_CheckSize_Ignore);
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT(PyUFuncObject),
+  __Pyx_ImportType_CheckSize_Ignore);
    if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
@@ -5233,33 +5684,45 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_naive_downscale_byte, __pyx_t_2) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_28aspect_ratio_array_functions_7upscale_retaining_sum, NULL, __pyx_n_s_aspect_ratio_array_functions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_upscale_retaining_sum, __pyx_t_2) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
+  /* "aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_28aspect_ratio_array_functions_9upscale_using_mean, NULL, __pyx_n_s_aspect_ratio_array_functions); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_upscale_using_mean, __pyx_t_2) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "aspect_ratio_array_functions.pyx":1
  * # cython: cdivision=True             # <<<<<<<<<<<<<<
  * # define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
  * #cython: boundscheck=False, wraparound=False
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "C:/Users/jajohns/AppData/Local/mambaforge/envs/allenv/lib/site-packages/numpy/__init__.pxd":1013
+  /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -6816,70 +7279,88 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
-#else
+#if CYTHON_FAST_THREAD_STATE
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
+#else
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* TypeImport */
   #ifndef __PYX_HAVE_RT_ImportType
 #define __PYX_HAVE_RT_ImportType
 static PyTypeObject *__Pyx_ImportType(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, enum __Pyx_ImportType_CheckSize check_size)
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
+    Py_ssize_t itemsize;
 #ifdef Py_LIMITED_API
     PyObject *py_basicsize;
+    PyObject *py_itemsize;
 #endif
     result = PyObject_GetAttrString(module, class_name);
     if (!result)
         goto bad;
     if (!PyType_Check(result)) {
         PyErr_Format(PyExc_TypeError,
             "%.200s.%.200s is not a type object",
             module_name, class_name);
         goto bad;
     }
 #ifndef Py_LIMITED_API
     basicsize = ((PyTypeObject *)result)->tp_basicsize;
+    itemsize = ((PyTypeObject *)result)->tp_itemsize;
 #else
     py_basicsize = PyObject_GetAttrString(result, "__basicsize__");
     if (!py_basicsize)
         goto bad;
     basicsize = PyLong_AsSsize_t(py_basicsize);
     Py_DECREF(py_basicsize);
     py_basicsize = 0;
     if (basicsize == (Py_ssize_t)-1 && PyErr_Occurred())
         goto bad;
+    py_itemsize = PyObject_GetAttrString(result, "__itemsize__");
+    if (!py_itemsize)
+        goto bad;
+    itemsize = PyLong_AsSsize_t(py_itemsize);
+    Py_DECREF(py_itemsize);
+    py_itemsize = 0;
+    if (itemsize == (Py_ssize_t)-1 && PyErr_Occurred())
+        goto bad;
 #endif
-    if ((size_t)basicsize < size) {
+    if (itemsize) {
+        if (size % alignment) {
+            alignment = size % alignment;
+        }
+        if (itemsize < (Py_ssize_t)alignment)
+            itemsize = (Py_ssize_t)alignment;
+    }
+    if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         goto bad;
     }
     if (check_size == __Pyx_ImportType_CheckSize_Error && (size_t)basicsize != size) {
```

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.cpp` & `hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1944,14 +1944,15 @@
 static const char __pyx_k_fc[] = "fc";
 static const char __pyx_k_fr[] = "fr";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_sum[] = "sum";
 static const char __pyx_k_byte[] = "byte";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_math[] = "math";
+static const char __pyx_k_mean[] = "mean";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_time[] = "time";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_empty[] = "empty";
 static const char __pyx_k_int32[] = "int32";
 static const char __pyx_k_int64[] = "int64";
@@ -1981,14 +1982,15 @@
 static const char __pyx_k_naive_downscale[] = "naive_downscale";
 static const char __pyx_k_num_coarse_cols[] = "num_coarse_cols";
 static const char __pyx_k_num_coarse_rows[] = "num_coarse_rows";
 static const char __pyx_k_coarse_res_array[] = "coarse_res_array";
 static const char __pyx_k_downscale_factor[] = "downscale_factor";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_current_proportion[] = "current_proportion";
+static const char __pyx_k_upscale_using_mean[] = "upscale_using_mean";
 static const char __pyx_k_naive_downscale_byte[] = "naive_downscale_byte";
 static const char __pyx_k_upscale_retaining_sum[] = "upscale_retaining_sum";
 static const char __pyx_k_coarse_res_proporition_array[] = "coarse_res_proporition_array";
 static const char __pyx_k_fine_res_cells_per_coarse_cell[] = "fine_res_cells_per_coarse_cell";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_cython_calc_proportion_of_coarse[] = "cython_calc_proportion_of_coarse_res_with_valid_fine_res";
 static const char __pyx_k_hazelbean_calculation_core_aspec[] = "hazelbean\\calculation_core\\aspect_ratio_array_functions.pyx";
@@ -2027,14 +2029,15 @@
 static PyObject *__pyx_n_s_hazelbean_calculation_core_aspec_2;
 static PyObject *__pyx_n_s_high_res_array;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_int32;
 static PyObject *__pyx_n_s_int64;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_math;
+static PyObject *__pyx_n_s_mean;
 static PyObject *__pyx_n_s_naive_downscale;
 static PyObject *__pyx_n_s_naive_downscale_byte;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_num_coarse_cols;
 static PyObject *__pyx_n_s_num_coarse_rows;
 static PyObject *__pyx_n_s_num_fine_cols;
@@ -2045,28 +2048,32 @@
 static PyObject *__pyx_n_s_output_array;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_sum;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_n_s_time;
 static PyObject *__pyx_n_s_upscale_factor;
 static PyObject *__pyx_n_s_upscale_retaining_sum;
+static PyObject *__pyx_n_s_upscale_using_mean;
 static PyObject *__pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_cython_calc_proportion_of_coarse_res_with_valid_fine_res(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_coarse_res_array, PyArrayObject *__pyx_v_fine_res_array); /* proto */
 static PyObject *__pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_2naive_downscale(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_coarse_res_array, PY_LONG_LONG __pyx_v_downscale_factor); /* proto */
 static PyObject *__pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_4naive_downscale_byte(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_coarse_res_array, PY_LONG_LONG __pyx_v_downscale_factor); /* proto */
 static PyObject *__pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_6upscale_retaining_sum(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_high_res_array, PY_LONG_LONG __pyx_v_upscale_factor); /* proto */
+static PyObject *__pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_8upscale_using_mean(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_high_res_array, PY_LONG_LONG __pyx_v_upscale_factor); /* proto */
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__6;
 static PyObject *__pyx_codeobj__8;
 static PyObject *__pyx_codeobj__10;
+static PyObject *__pyx_codeobj__12;
 /* Late includes */
 
 /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":45
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def cython_calc_proportion_of_coarse_res_with_valid_fine_res(np.ndarray[np.float64_t, ndim=2] coarse_res_array,             # <<<<<<<<<<<<<<
  *                                                       np.ndarray[np.int64_t, ndim=2] fine_res_array,
@@ -3175,21 +3182,21 @@
   return __pyx_r;
 }
 
 /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_9hazelbean_16calculation_core_28aspect_ratio_array_functions_7upscale_retaining_sum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static char __pyx_doc_9hazelbean_16calculation_core_28aspect_ratio_array_functions_6upscale_retaining_sum[] = "upscale_retaining_sum(ndarray high_res_array, long long upscale_factor)\nReturn an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res.";
+static char __pyx_doc_9hazelbean_16calculation_core_28aspect_ratio_array_functions_6upscale_retaining_sum[] = "upscale_retaining_sum(ndarray high_res_array, long long upscale_factor)\nReturn an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res.";
 static PyMethodDef __pyx_mdef_9hazelbean_16calculation_core_28aspect_ratio_array_functions_7upscale_retaining_sum = {"upscale_retaining_sum", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9hazelbean_16calculation_core_28aspect_ratio_array_functions_7upscale_retaining_sum, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9hazelbean_16calculation_core_28aspect_ratio_array_functions_6upscale_retaining_sum};
 static PyObject *__pyx_pw_9hazelbean_16calculation_core_28aspect_ratio_array_functions_7upscale_retaining_sum(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyArrayObject *__pyx_v_high_res_array = 0;
   PY_LONG_LONG __pyx_v_upscale_factor;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
@@ -3304,15 +3311,15 @@
   {
     __Pyx_BufFmt_StackElem __pyx_stack[1];
     if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_high_res_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 111, __pyx_L1_error)
   }
   __pyx_pybuffernd_high_res_array.diminfo[0].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_high_res_array.diminfo[0].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_high_res_array.diminfo[1].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_high_res_array.diminfo[1].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[1];
 
   /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":114
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  *     cdef long long num_fine_rows = high_res_array.shape[0]             # <<<<<<<<<<<<<<
  *     cdef long long num_fine_cols = high_res_array.shape[1]
  * 
  */
   __pyx_v_num_fine_rows = (__pyx_v_high_res_array->dimensions[0]);
 
@@ -3546,15 +3553,15 @@
   __pyx_r = ((PyObject *)__pyx_v_output_array);
   goto __pyx_L0;
 
   /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
@@ -3578,14 +3585,421 @@
   __pyx_L2:;
   __Pyx_XDECREF((PyObject *)__pyx_v_output_array);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
+/* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_9hazelbean_16calculation_core_28aspect_ratio_array_functions_9upscale_using_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_9hazelbean_16calculation_core_28aspect_ratio_array_functions_8upscale_using_mean[] = "upscale_using_mean(ndarray high_res_array, long long upscale_factor)\nReturn an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res.";
+static PyMethodDef __pyx_mdef_9hazelbean_16calculation_core_28aspect_ratio_array_functions_9upscale_using_mean = {"upscale_using_mean", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_9hazelbean_16calculation_core_28aspect_ratio_array_functions_9upscale_using_mean, METH_VARARGS|METH_KEYWORDS, __pyx_doc_9hazelbean_16calculation_core_28aspect_ratio_array_functions_8upscale_using_mean};
+static PyObject *__pyx_pw_9hazelbean_16calculation_core_28aspect_ratio_array_functions_9upscale_using_mean(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyArrayObject *__pyx_v_high_res_array = 0;
+  PY_LONG_LONG __pyx_v_upscale_factor;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("upscale_using_mean (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_high_res_array,&__pyx_n_s_upscale_factor,0};
+    PyObject* values[2] = {0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_high_res_array)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_upscale_factor)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("upscale_using_mean", 1, 2, 2, 1); __PYX_ERR(0, 142, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "upscale_using_mean") < 0)) __PYX_ERR(0, 142, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 2) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+    }
+    __pyx_v_high_res_array = ((PyArrayObject *)values[0]);
+    __pyx_v_upscale_factor = __Pyx_PyInt_As_PY_LONG_LONG(values[1]); if (unlikely((__pyx_v_upscale_factor == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 142, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("upscale_using_mean", 1, 2, 2, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 142, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("hazelbean.calculation_core.aspect_ratio_array_functions.upscale_using_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_high_res_array), __pyx_ptype_5numpy_ndarray, 1, "high_res_array", 0))) __PYX_ERR(0, 142, __pyx_L1_error)
+  __pyx_r = __pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_8upscale_using_mean(__pyx_self, __pyx_v_high_res_array, __pyx_v_upscale_factor);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_9hazelbean_16calculation_core_28aspect_ratio_array_functions_8upscale_using_mean(CYTHON_UNUSED PyObject *__pyx_self, PyArrayObject *__pyx_v_high_res_array, PY_LONG_LONG __pyx_v_upscale_factor) {
+  CYTHON_UNUSED PY_LONG_LONG __pyx_v_num_fine_rows;
+  CYTHON_UNUSED PY_LONG_LONG __pyx_v_num_fine_cols;
+  PY_LONG_LONG __pyx_v_num_coarse_rows;
+  PY_LONG_LONG __pyx_v_num_coarse_cols;
+  PY_LONG_LONG __pyx_v_cr;
+  PY_LONG_LONG __pyx_v_cc;
+  PY_LONG_LONG __pyx_v_fr_start;
+  PY_LONG_LONG __pyx_v_fr_end;
+  PY_LONG_LONG __pyx_v_fc_start;
+  PY_LONG_LONG __pyx_v_fc_end;
+  PyArrayObject *__pyx_v_output_array = 0;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_high_res_array;
+  __Pyx_Buffer __pyx_pybuffer_high_res_array;
+  __Pyx_LocalBuf_ND __pyx_pybuffernd_output_array;
+  __Pyx_Buffer __pyx_pybuffer_output_array;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  PyObject *__pyx_t_5 = NULL;
+  PyArrayObject *__pyx_t_6 = NULL;
+  PY_LONG_LONG __pyx_t_7;
+  PY_LONG_LONG __pyx_t_8;
+  PY_LONG_LONG __pyx_t_9;
+  PY_LONG_LONG __pyx_t_10;
+  PY_LONG_LONG __pyx_t_11;
+  PY_LONG_LONG __pyx_t_12;
+  PyObject *__pyx_t_13 = NULL;
+  __pyx_t_5numpy_float64_t __pyx_t_14;
+  PY_LONG_LONG __pyx_t_15;
+  PY_LONG_LONG __pyx_t_16;
+  int __pyx_t_17;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("upscale_using_mean", 0);
+  __pyx_pybuffer_output_array.pybuffer.buf = NULL;
+  __pyx_pybuffer_output_array.refcount = 0;
+  __pyx_pybuffernd_output_array.data = NULL;
+  __pyx_pybuffernd_output_array.rcbuffer = &__pyx_pybuffer_output_array;
+  __pyx_pybuffer_high_res_array.pybuffer.buf = NULL;
+  __pyx_pybuffer_high_res_array.refcount = 0;
+  __pyx_pybuffernd_high_res_array.data = NULL;
+  __pyx_pybuffernd_high_res_array.rcbuffer = &__pyx_pybuffer_high_res_array;
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer, (PyObject*)__pyx_v_high_res_array, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES, 2, 0, __pyx_stack) == -1)) __PYX_ERR(0, 142, __pyx_L1_error)
+  }
+  __pyx_pybuffernd_high_res_array.diminfo[0].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_high_res_array.diminfo[0].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_high_res_array.diminfo[1].strides = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_high_res_array.diminfo[1].shape = __pyx_pybuffernd_high_res_array.rcbuffer->pybuffer.shape[1];
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":145
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ *     cdef long long num_fine_rows = high_res_array.shape[0]             # <<<<<<<<<<<<<<
+ *     cdef long long num_fine_cols = high_res_array.shape[1]
+ * 
+ */
+  __pyx_v_num_fine_rows = (__pyx_v_high_res_array->dimensions[0]);
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":146
+ * 
+ *     cdef long long num_fine_rows = high_res_array.shape[0]
+ *     cdef long long num_fine_cols = high_res_array.shape[1]             # <<<<<<<<<<<<<<
+ * 
+ *     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)
+ */
+  __pyx_v_num_fine_cols = (__pyx_v_high_res_array->dimensions[1]);
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":148
+ *     cdef long long num_fine_cols = high_res_array.shape[1]
+ * 
+ *     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)             # <<<<<<<<<<<<<<
+ *     cdef long long num_coarse_cols = <long long>(high_res_array.shape[1] / upscale_factor)
+ * 
+ */
+  __pyx_v_num_coarse_rows = ((PY_LONG_LONG)((__pyx_v_high_res_array->dimensions[0]) / __pyx_v_upscale_factor));
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":149
+ * 
+ *     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)
+ *     cdef long long num_coarse_cols = <long long>(high_res_array.shape[1] / upscale_factor)             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_v_num_coarse_cols = ((PY_LONG_LONG)((__pyx_v_high_res_array->dimensions[1]) / __pyx_v_upscale_factor));
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":154
+ *     cdef long long cr, cc, fr_start, fr_end, fc_start, fc_end
+ * 
+ *     cdef np.ndarray[np.float64_t, ndim=2] output_array = np.empty([num_coarse_rows, num_coarse_cols], dtype=np.float64)             # <<<<<<<<<<<<<<
+ * 
+ *     for cr in range(num_coarse_rows):
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_empty); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_num_coarse_rows); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_num_coarse_cols); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = PyList_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyList_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyList_SET_ITEM(__pyx_t_4, 1, __pyx_t_3);
+  __pyx_t_1 = 0;
+  __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_float64); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_4); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 154, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 154, __pyx_L1_error)
+  __pyx_t_6 = ((PyArrayObject *)__pyx_t_5);
+  {
+    __Pyx_BufFmt_StackElem __pyx_stack[1];
+    if (unlikely(__Pyx_GetBufferAndValidate(&__pyx_pybuffernd_output_array.rcbuffer->pybuffer, (PyObject*)__pyx_t_6, &__Pyx_TypeInfo_nn___pyx_t_5numpy_float64_t, PyBUF_FORMAT| PyBUF_STRIDES| PyBUF_WRITABLE, 2, 0, __pyx_stack) == -1)) {
+      __pyx_v_output_array = ((PyArrayObject *)Py_None); __Pyx_INCREF(Py_None); __pyx_pybuffernd_output_array.rcbuffer->pybuffer.buf = NULL;
+      __PYX_ERR(0, 154, __pyx_L1_error)
+    } else {__pyx_pybuffernd_output_array.diminfo[0].strides = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.strides[0]; __pyx_pybuffernd_output_array.diminfo[0].shape = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.shape[0]; __pyx_pybuffernd_output_array.diminfo[1].strides = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.strides[1]; __pyx_pybuffernd_output_array.diminfo[1].shape = __pyx_pybuffernd_output_array.rcbuffer->pybuffer.shape[1];
+    }
+  }
+  __pyx_t_6 = 0;
+  __pyx_v_output_array = ((PyArrayObject *)__pyx_t_5);
+  __pyx_t_5 = 0;
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":156
+ *     cdef np.ndarray[np.float64_t, ndim=2] output_array = np.empty([num_coarse_rows, num_coarse_cols], dtype=np.float64)
+ * 
+ *     for cr in range(num_coarse_rows):             # <<<<<<<<<<<<<<
+ *         fr_start = cr * upscale_factor
+ *         fr_end = (cr + 1) * upscale_factor
+ */
+  __pyx_t_7 = __pyx_v_num_coarse_rows;
+  __pyx_t_8 = __pyx_t_7;
+  for (__pyx_t_9 = 0; __pyx_t_9 < __pyx_t_8; __pyx_t_9+=1) {
+    __pyx_v_cr = __pyx_t_9;
+
+    /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":157
+ * 
+ *     for cr in range(num_coarse_rows):
+ *         fr_start = cr * upscale_factor             # <<<<<<<<<<<<<<
+ *         fr_end = (cr + 1) * upscale_factor
+ *         for cc in range(num_coarse_cols):
+ */
+    __pyx_v_fr_start = (__pyx_v_cr * __pyx_v_upscale_factor);
+
+    /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":158
+ *     for cr in range(num_coarse_rows):
+ *         fr_start = cr * upscale_factor
+ *         fr_end = (cr + 1) * upscale_factor             # <<<<<<<<<<<<<<
+ *         for cc in range(num_coarse_cols):
+ * 
+ */
+    __pyx_v_fr_end = ((__pyx_v_cr + 1) * __pyx_v_upscale_factor);
+
+    /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":159
+ *         fr_start = cr * upscale_factor
+ *         fr_end = (cr + 1) * upscale_factor
+ *         for cc in range(num_coarse_cols):             # <<<<<<<<<<<<<<
+ * 
+ *             fc_start = cc * upscale_factor
+ */
+    __pyx_t_10 = __pyx_v_num_coarse_cols;
+    __pyx_t_11 = __pyx_t_10;
+    for (__pyx_t_12 = 0; __pyx_t_12 < __pyx_t_11; __pyx_t_12+=1) {
+      __pyx_v_cc = __pyx_t_12;
+
+      /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":161
+ *         for cc in range(num_coarse_cols):
+ * 
+ *             fc_start = cc * upscale_factor             # <<<<<<<<<<<<<<
+ *             fc_end = (cc + 1) * upscale_factor
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+ */
+      __pyx_v_fc_start = (__pyx_v_cc * __pyx_v_upscale_factor);
+
+      /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":162
+ * 
+ *             fc_start = cc * upscale_factor
+ *             fc_end = (cc + 1) * upscale_factor             # <<<<<<<<<<<<<<
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+ * 
+ */
+      __pyx_v_fc_end = ((__pyx_v_cc + 1) * __pyx_v_upscale_factor);
+
+      /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":163
+ *             fc_start = cc * upscale_factor
+ *             fc_end = (cc + 1) * upscale_factor
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])             # <<<<<<<<<<<<<<
+ * 
+ *     return output_array
+ */
+      __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_mean); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_3);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fr_start); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fr_end); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_1 = PySlice_New(__pyx_t_4, __pyx_t_2, Py_None); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_1);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __pyx_t_2 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fc_start); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_2);
+      __pyx_t_4 = __Pyx_PyInt_From_PY_LONG_LONG(__pyx_v_fc_end); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __pyx_t_13 = PySlice_New(__pyx_t_2, __pyx_t_4, Py_None); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_4);
+      __Pyx_GIVEREF(__pyx_t_1);
+      PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+      __Pyx_GIVEREF(__pyx_t_13);
+      PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_13);
+      __pyx_t_1 = 0;
+      __pyx_t_13 = 0;
+      __pyx_t_13 = __Pyx_PyObject_GetItem(((PyObject *)__pyx_v_high_res_array), __pyx_t_4); if (unlikely(!__pyx_t_13)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_13);
+      __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __pyx_t_4 = NULL;
+      if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_3))) {
+        __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+        if (likely(__pyx_t_4)) {
+          PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+          __Pyx_INCREF(__pyx_t_4);
+          __Pyx_INCREF(function);
+          __Pyx_DECREF_SET(__pyx_t_3, function);
+        }
+      }
+      __pyx_t_5 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_3, __pyx_t_4, __pyx_t_13) : __Pyx_PyObject_CallOneArg(__pyx_t_3, __pyx_t_13);
+      __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+      __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
+      if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_5);
+      __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+      __pyx_t_14 = __pyx_PyFloat_AsDouble(__pyx_t_5); if (unlikely((__pyx_t_14 == ((npy_float64)-1)) && PyErr_Occurred())) __PYX_ERR(0, 163, __pyx_L1_error)
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+      __pyx_t_15 = __pyx_v_cr;
+      __pyx_t_16 = __pyx_v_cc;
+      __pyx_t_17 = -1;
+      if (__pyx_t_15 < 0) {
+        __pyx_t_17 = 0;
+      } else if (unlikely(__pyx_t_15 >= __pyx_pybuffernd_output_array.diminfo[0].shape)) __pyx_t_17 = 0;
+      if (__pyx_t_16 < 0) {
+        __pyx_t_17 = 1;
+      } else if (unlikely(__pyx_t_16 >= __pyx_pybuffernd_output_array.diminfo[1].shape)) __pyx_t_17 = 1;
+      if (unlikely(__pyx_t_17 != -1)) {
+        __Pyx_RaiseBufferIndexError(__pyx_t_17);
+        __PYX_ERR(0, 163, __pyx_L1_error)
+      }
+      *__Pyx_BufPtrStrided2d(__pyx_t_5numpy_float64_t *, __pyx_pybuffernd_output_array.rcbuffer->pybuffer.buf, __pyx_t_15, __pyx_pybuffernd_output_array.diminfo[0].strides, __pyx_t_16, __pyx_pybuffernd_output_array.diminfo[1].strides) = __pyx_t_14;
+    }
+  }
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":165
+ *             output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+ * 
+ *     return output_array             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __Pyx_INCREF(((PyObject *)__pyx_v_output_array));
+  __pyx_r = ((PyObject *)__pyx_v_output_array);
+  goto __pyx_L0;
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_13);
+  { PyObject *__pyx_type, *__pyx_value, *__pyx_tb;
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&__pyx_type, &__pyx_value, &__pyx_tb);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer);
+    __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output_array.rcbuffer->pybuffer);
+  __Pyx_ErrRestore(__pyx_type, __pyx_value, __pyx_tb);}
+  __Pyx_AddTraceback("hazelbean.calculation_core.aspect_ratio_array_functions.upscale_using_mean", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  goto __pyx_L2;
+  __pyx_L0:;
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_high_res_array.rcbuffer->pybuffer);
+  __Pyx_SafeReleaseBuffer(&__pyx_pybuffernd_output_array.rcbuffer->pybuffer);
+  __pyx_L2:;
+  __Pyx_XDECREF((PyObject *)__pyx_v_output_array);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
 /* "C:/Users/jajohns/mambaforge/envs/env2023a/lib/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
@@ -4678,14 +5092,15 @@
   {&__pyx_n_s_hazelbean_calculation_core_aspec_2, __pyx_k_hazelbean_calculation_core_aspec_2, sizeof(__pyx_k_hazelbean_calculation_core_aspec_2), 0, 0, 1, 1},
   {&__pyx_n_s_high_res_array, __pyx_k_high_res_array, sizeof(__pyx_k_high_res_array), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_int32, __pyx_k_int32, sizeof(__pyx_k_int32), 0, 0, 1, 1},
   {&__pyx_n_s_int64, __pyx_k_int64, sizeof(__pyx_k_int64), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_math, __pyx_k_math, sizeof(__pyx_k_math), 0, 0, 1, 1},
+  {&__pyx_n_s_mean, __pyx_k_mean, sizeof(__pyx_k_mean), 0, 0, 1, 1},
   {&__pyx_n_s_naive_downscale, __pyx_k_naive_downscale, sizeof(__pyx_k_naive_downscale), 0, 0, 1, 1},
   {&__pyx_n_s_naive_downscale_byte, __pyx_k_naive_downscale_byte, sizeof(__pyx_k_naive_downscale_byte), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_num_coarse_cols, __pyx_k_num_coarse_cols, sizeof(__pyx_k_num_coarse_cols), 0, 0, 1, 1},
   {&__pyx_n_s_num_coarse_rows, __pyx_k_num_coarse_rows, sizeof(__pyx_k_num_coarse_rows), 0, 0, 1, 1},
   {&__pyx_n_s_num_fine_cols, __pyx_k_num_fine_cols, sizeof(__pyx_k_num_fine_cols), 0, 0, 1, 1},
@@ -4696,14 +5111,15 @@
   {&__pyx_n_s_output_array, __pyx_k_output_array, sizeof(__pyx_k_output_array), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_sum, __pyx_k_sum, sizeof(__pyx_k_sum), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_n_s_time, __pyx_k_time, sizeof(__pyx_k_time), 0, 0, 1, 1},
   {&__pyx_n_s_upscale_factor, __pyx_k_upscale_factor, sizeof(__pyx_k_upscale_factor), 0, 0, 1, 1},
   {&__pyx_n_s_upscale_retaining_sum, __pyx_k_upscale_retaining_sum, sizeof(__pyx_k_upscale_retaining_sum), 0, 0, 1, 1},
+  {&__pyx_n_s_upscale_using_mean, __pyx_k_upscale_using_mean, sizeof(__pyx_k_upscale_using_mean), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 60, __pyx_L1_error)
   __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
@@ -4772,21 +5188,33 @@
   __Pyx_GIVEREF(__pyx_tuple__7);
   __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hazelbean_calculation_core_aspec, __pyx_n_s_naive_downscale_byte, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 91, __pyx_L1_error)
 
   /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
   __pyx_tuple__9 = PyTuple_Pack(13, __pyx_n_s_high_res_array, __pyx_n_s_upscale_factor, __pyx_n_s_num_fine_rows, __pyx_n_s_num_fine_cols, __pyx_n_s_num_coarse_rows, __pyx_n_s_num_coarse_cols, __pyx_n_s_cr, __pyx_n_s_cc, __pyx_n_s_fr_start, __pyx_n_s_fr_end, __pyx_n_s_fc_start, __pyx_n_s_fc_end, __pyx_n_s_output_array); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
   __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hazelbean_calculation_core_aspec, __pyx_n_s_upscale_retaining_sum, 111, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(0, 111, __pyx_L1_error)
+
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+  __pyx_tuple__11 = PyTuple_Pack(13, __pyx_n_s_high_res_array, __pyx_n_s_upscale_factor, __pyx_n_s_num_fine_rows, __pyx_n_s_num_fine_cols, __pyx_n_s_num_coarse_rows, __pyx_n_s_num_coarse_cols, __pyx_n_s_cr, __pyx_n_s_cc, __pyx_n_s_fr_start, __pyx_n_s_fr_end, __pyx_n_s_fc_start, __pyx_n_s_fc_end, __pyx_n_s_output_array); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(2, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_hazelbean_calculation_core_aspec, __pyx_n_s_upscale_using_mean, 142, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 142, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -5293,22 +5721,34 @@
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_naive_downscale_byte, __pyx_t_2) < 0) __PYX_ERR(0, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":111
  * @cython.boundscheck(True)
  * @cython.wraparound(False)
  * def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
- *     """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
  * 
  */
   __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_9hazelbean_16calculation_core_28aspect_ratio_array_functions_7upscale_retaining_sum, NULL, __pyx_n_s_hazelbean_calculation_core_aspec_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_upscale_retaining_sum, __pyx_t_2) < 0) __PYX_ERR(0, 111, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
+  /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":142
+ * @cython.boundscheck(True)
+ * @cython.wraparound(False)
+ * def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):             # <<<<<<<<<<<<<<
+ *     """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+ * 
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_9hazelbean_16calculation_core_28aspect_ratio_array_functions_9upscale_using_mean, NULL, __pyx_n_s_hazelbean_calculation_core_aspec_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_upscale_using_mean, __pyx_t_2) < 0) __PYX_ERR(0, 142, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
   /* "hazelbean/calculation_core/aspect_ratio_array_functions.pyx":1
  * # cython: cdivision=True             # <<<<<<<<<<<<<<
  * # define NPY_NO_DEPRECATED_API NPY_1_7_API_VERSION
  * #cython: boundscheck=False, wraparound=False
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
```

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/aspect_ratio_array_functions.pyx` & `hazelbean-1.4.8/hazelbean/calculation_core/aspect_ratio_array_functions.pyx`

 * *Files 24% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     return output_array
 
 @cython.cdivision(True)
 @cython.embedsignature(True)
 @cython.boundscheck(True)
 @cython.wraparound(False)
 def upscale_retaining_sum(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):
-    """Return an array that makes n by m array into n / input_scalar by m * upscale_factor with the sum of the fine res cells in the coarse res."""
+    """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
 
     cdef long long num_fine_rows = high_res_array.shape[0]
     cdef long long num_fine_cols = high_res_array.shape[1]
 
     cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)
     cdef long long num_coarse_cols = <long long>(high_res_array.shape[1] / upscale_factor)
 
@@ -131,11 +131,42 @@
             fc_end = (cc + 1) * upscale_factor
             output_array[cr, cc] = np.sum(high_res_array[fr_start:fr_end, fc_start:fc_end])
 
     return output_array
 
 
 
+@cython.cdivision(True)
+@cython.embedsignature(True)
+@cython.boundscheck(True)
+@cython.wraparound(False)
+def upscale_using_mean(np.ndarray[np.float64_t, ndim=2] high_res_array, long long upscale_factor):
+    """Return an array that makes n by m array into n / input_scalar by m / upscale_factor with the sum of the fine res cells in the coarse res."""
+
+    cdef long long num_fine_rows = high_res_array.shape[0]
+    cdef long long num_fine_cols = high_res_array.shape[1]
+
+    cdef long long num_coarse_rows = <long long>(high_res_array.shape[0] / upscale_factor)
+    cdef long long num_coarse_cols = <long long>(high_res_array.shape[1] / upscale_factor)
+
+
+    cdef long long cr, cc, fr_start, fr_end, fc_start, fc_end
+
+    cdef np.ndarray[np.float64_t, ndim=2] output_array = np.empty([num_coarse_rows, num_coarse_cols], dtype=np.float64)
+
+    for cr in range(num_coarse_rows):
+        fr_start = cr * upscale_factor
+        fr_end = (cr + 1) * upscale_factor
+        for cc in range(num_coarse_cols):
+
+            fc_start = cc * upscale_factor
+            fc_end = (cc + 1) * upscale_factor
+            output_array[cr, cc] = np.mean(high_res_array[fr_start:fr_end, fc_start:fc_end])
+
+    return output_array
+
+
+
```

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/compile_cython_functions.py` & `hazelbean-1.4.8/hazelbean/calculation_core/compile_cython_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.c` & `hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.c`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.cpp` & `hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.cpp`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/calculation_core/cython_functions.pyx` & `hazelbean-1.4.8/hazelbean/calculation_core/cython_functions.pyx`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/cat_ears.py` & `hazelbean-1.4.8/hazelbean/cat_ears.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/cloud_utils.py` & `hazelbean-1.4.8/hazelbean/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/config.py` & `hazelbean-1.4.8/hazelbean/config.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/conventions.py` & `hazelbean-1.4.8/hazelbean/conventions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/core.py` & `hazelbean-1.4.8/hazelbean/core.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/data_structures.py` & `hazelbean-1.4.8/hazelbean/data_structures.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/file_io.py` & `hazelbean-1.4.8/hazelbean/file_io.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/geoprocessing.py` & `hazelbean-1.4.8/hazelbean/geoprocessing.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/geoprocessing_extension.py` & `hazelbean-1.4.8/hazelbean/geoprocessing_extension.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/globals.py` & `hazelbean-1.4.8/hazelbean/globals.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/netcdf.py` & `hazelbean-1.4.8/hazelbean/netcdf.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/os_utils.py` & `hazelbean-1.4.8/hazelbean/os_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/parallel.py` & `hazelbean-1.4.8/hazelbean/parallel.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/project_flow.py` & `hazelbean-1.4.8/hazelbean/project_flow.py`

 * *Files 0% similar despite different names*

```diff
@@ -756,15 +756,15 @@
             # Task is not an iterator, thus we just call it's child directly
             elif task.parent is not None:
                 if task.parent.type == 'iterator':
                     for child in task.children:
                         self.run_task(child)# Run the child found by iterating the task-node's children
             else:
                 for child in task.children:
-                    self.run_task(child)  # Run the child found by iterating the task-node's children
+                     self.run_task(child)  # Run the child found by iterating the task-node's children
 
                     # raise NameError('wtf')
          
         try:           
             if task.note is not None:
                 hb.write_to_file(task.note, os.path.join(task.task_dir, task.note + '.txt'))
             if task.documentation is not None:
```

### Comparing `hazelbean-1.4.7/hazelbean/pyramids.py` & `hazelbean-1.4.8/hazelbean/pyramids.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/raster_vector_interface.py` & `hazelbean-1.4.8/hazelbean/raster_vector_interface.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/spatial_projection.py` & `hazelbean-1.4.8/hazelbean/spatial_projection.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/spatial_utils.py` & `hazelbean-1.4.8/hazelbean/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/stats.py` & `hazelbean-1.4.8/hazelbean/stats.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/auto_ui.py` & `hazelbean-1.4.8/hazelbean/ui/auto_ui.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/auto_ui_tg.py` & `hazelbean-1.4.8/hazelbean/ui/auto_ui_tg.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/cli.py` & `hazelbean-1.4.8/hazelbean/ui/cli.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/datastack.py` & `hazelbean-1.4.8/hazelbean/ui/datastack.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/execution.py` & `hazelbean-1.4.8/hazelbean/ui/execution.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/inputs.py` & `hazelbean-1.4.8/hazelbean/ui/inputs.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/launcher.py` & `hazelbean-1.4.8/hazelbean/ui/launcher.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/model.py` & `hazelbean-1.4.8/hazelbean/ui/model.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/usage.py` & `hazelbean-1.4.8/hazelbean/ui/usage.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/usage_logger.py` & `hazelbean-1.4.8/hazelbean/ui/usage_logger.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/utils.py` & `hazelbean-1.4.8/hazelbean/ui/utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/ui/validation.py` & `hazelbean-1.4.8/hazelbean/ui/validation.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/utils.py` & `hazelbean-1.4.8/hazelbean/utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean/visualization.py` & `hazelbean-1.4.8/hazelbean/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1503,15 +1503,15 @@
         '''255,255,255
         220,66,69
         219,164,75
         227,227,34
         0,160,18
         111,232,94
         172,191,229
-        222,213,239
+        244,244,244
         228,228,228
         255,0,255
         255,255,255''',
 
     'seals_simplified_6_color':
         '''220,66,69
         219,164,75
```

### Comparing `hazelbean-1.4.7/hazelbean/watershed_processing.py` & `hazelbean-1.4.8/hazelbean/watershed_processing.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/hazelbean.egg-info/SOURCES.txt` & `hazelbean-1.4.8/hazelbean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.7/setup.py` & `hazelbean-1.4.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 packages=find_packages()
 include_package_data=True
 
 setup(
   name = 'hazelbean',
   packages = packages,
-  version = '1.4.7',
+  version = '1.4.8',
   description = 'Geospatial research tools',
   long_description = 'Geospatial research tools for economics and sustainability science.',
   author = 'Justin Andrew Johnson',
   url = 'https://github.com/jandrewjohnson/hazelbean',
   download_url = 'https://github.com/jandrewjohnson/hazelbean',
   keywords = ['geospatial', 'raster', 'shapefile', 'sustainability science'],
   classifiers = ["Programming Language :: Python :: 3"],
```


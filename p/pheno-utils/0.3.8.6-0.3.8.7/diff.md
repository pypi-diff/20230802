# Comparing `tmp/pheno-utils-0.3.8.6.tar.gz` & `tmp/pheno-utils-0.3.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pheno-utils-0.3.8.6.tar", last modified: Wed Aug  2 06:56:52 2023, max compression
+gzip compressed data, was "pheno-utils-0.3.8.7.tar", last modified: Wed Aug  2 07:45:06 2023, max compression
```

## Comparing `pheno-utils-0.3.8.6.tar` & `pheno-utils-0.3.8.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:56:52.450348 pheno-utils-0.3.8.6/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)      184 2023-08-02 06:29:57.000000 pheno-utils-0.3.8.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2361 2023-08-02 06:56:52.449395 pheno-utils-0.3.8.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:56:52.394825 pheno-utils-0.3.8.6/pheno_utils/
--rw-r--r--   0 root         (0) root         (0)      344 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19748 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/_modidx.py
--rw-r--r--   0 root         (0) root         (0)    16533 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/age_reference_plots.py
--rw-r--r--   0 root         (0) root         (0)     5530 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/basic_analysis.py
--rw-r--r--   0 root         (0) root         (0)    11559 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/basic_plots.py
--rw-r--r--   0 root         (0) root         (0)     2672 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/blandaltman_plots.py
--rw-r--r--   0 root         (0) root         (0)     7865 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/cgm_plots.py
--rw-r--r--   0 root         (0) root         (0)     3036 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/cohort_selector.py
--rw-r--r--   0 root         (0) root         (0)     4652 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:56:52.445128 pheno-utils-0.3.8.6/pheno_utils/config_setup/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/config_setup/__init__.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 08:54:34.000000 pheno-utils-0.3.8.6/pheno_utils/config_setup/config_tre.json
--rw-r--r--   0 root         (0) root         (0)     2696 2023-07-26 08:11:20.000000 pheno-utils-0.3.8.6/pheno_utils/config_setup/create_default_config.py
--rw-r--r--   0 root         (0) root         (0)      260 2023-07-20 12:24:23.000000 pheno-utils-0.3.8.6/pheno_utils/config_setup/example_config.json
--rw-r--r--   0 root         (0) root         (0)     2825 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/dates_plots.py
--rw-r--r--   0 root         (0) root         (0)     2113 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/ecg_analysis.py
--rw-r--r--   0 root         (0) root         (0)     7781 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/meta_loader.py
--rw-r--r--   0 root         (0) root         (0)    20194 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/pheno_loader.py
--rw-r--r--   0 root         (0) root         (0)     1444 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/questionnaires_handler.py
--rw-r--r--   0 root         (0) root         (0)    13188 2023-08-02 06:55:14.000000 pheno-utils-0.3.8.6/pheno_utils/sleep_plots.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 06:56:52.430670 pheno-utils-0.3.8.6/pheno_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2361 2023-08-02 06:56:52.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      895 2023-08-02 06:56:52.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 06:56:52.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-08-02 06:56:52.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      132 2023-08-02 06:56:52.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-08-02 06:56:52.000000 pheno-utils-0.3.8.6/pheno_utils.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-08-02 06:55:11.000000 pheno-utils-0.3.8.6/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 06:56:52.451091 pheno-utils-0.3.8.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2639 2023-08-02 06:44:56.000000 pheno-utils-0.3.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:45:06.621910 pheno-utils-0.3.8.7/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-06-21 16:13:16.000000 pheno-utils-0.3.8.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      184 2023-08-02 06:29:57.000000 pheno-utils-0.3.8.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-08-02 07:45:06.620959 pheno-utils-0.3.8.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1583 2023-07-26 07:07:45.000000 pheno-utils-0.3.8.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:45:06.549041 pheno-utils-0.3.8.7/pheno_utils/
+-rw-r--r--   0 root         (0) root         (0)      344 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19748 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)    16533 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/age_reference_plots.py
+-rw-r--r--   0 root         (0) root         (0)     5530 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/basic_analysis.py
+-rw-r--r--   0 root         (0) root         (0)    11559 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/basic_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2672 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/blandaltman_plots.py
+-rw-r--r--   0 root         (0) root         (0)     7865 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/cgm_plots.py
+-rw-r--r--   0 root         (0) root         (0)     3036 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/cohort_selector.py
+-rw-r--r--   0 root         (0) root         (0)     4649 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:45:06.615654 pheno-utils-0.3.8.7/pheno_utils/config_setup/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/config_setup/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-07-25 08:54:34.000000 pheno-utils-0.3.8.7/pheno_utils/config_setup/config_tre.json
+-rw-r--r--   0 root         (0) root         (0)     2696 2023-07-26 08:11:20.000000 pheno-utils-0.3.8.7/pheno_utils/config_setup/create_default_config.py
+-rw-r--r--   0 root         (0) root         (0)      260 2023-07-20 12:24:23.000000 pheno-utils-0.3.8.7/pheno_utils/config_setup/example_config.json
+-rw-r--r--   0 root         (0) root         (0)     2825 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/dates_plots.py
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/ecg_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     7781 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/meta_loader.py
+-rw-r--r--   0 root         (0) root         (0)    20194 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/pheno_loader.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/questionnaires_handler.py
+-rw-r--r--   0 root         (0) root         (0)    13188 2023-08-02 07:44:45.000000 pheno-utils-0.3.8.7/pheno_utils/sleep_plots.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:45:06.594001 pheno-utils-0.3.8.7/pheno_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-08-02 07:45:06.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      895 2023-08-02 07:45:06.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:45:06.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-02 07:45:06.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-21 16:16:15.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      132 2023-08-02 07:45:06.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-08-02 07:45:06.000000 pheno-utils-0.3.8.7/pheno_utils.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-08-02 07:42:42.000000 pheno-utils-0.3.8.7/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:45:06.622429 pheno-utils-0.3.8.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-08-02 06:44:56.000000 pheno-utils-0.3.8.7/setup.py
```

### Comparing `pheno-utils-0.3.8.6/LICENSE` & `pheno-utils-0.3.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/PKG-INFO` & `pheno-utils-0.3.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.8.6
+Version: 0.3.8.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.8.6/README.md` & `pheno-utils-0.3.8.7/README.md`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/_modidx.py` & `pheno-utils-0.3.8.7/pheno_utils/_modidx.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/age_reference_plots.py` & `pheno-utils-0.3.8.7/pheno_utils/age_reference_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/basic_analysis.py` & `pheno-utils-0.3.8.7/pheno_utils/basic_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/basic_plots.py` & `pheno-utils-0.3.8.7/pheno_utils/basic_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/blandaltman_plots.py` & `pheno-utils-0.3.8.7/pheno_utils/blandaltman_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/cgm_plots.py` & `pheno-utils-0.3.8.7/pheno_utils/cgm_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/cohort_selector.py` & `pheno-utils-0.3.8.7/pheno_utils/cohort_selector.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/config.py` & `pheno-utils-0.3.8.7/pheno_utils/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 
 
 # %% ../nbs/00_config.ipynb 5
 def copy_tre_config():
     tre_mode = False
     script_path = os.path.dirname(os.path.abspath(__file__))
-    absolute_config_path = os.path.join(script_path, '../config_setup/config_tre.json')
+    absolute_config_path = os.path.join(script_path, 'config_setup/config_tre.json')
     
     with open(absolute_config_path, 'r') as openfile:
         json_object = json.load(openfile)
                 
     datasets_full_path = json_object['DATASETS_PATH']
     if os.path.exists(datasets_full_path):
         print("TRE Mode")
```

### Comparing `pheno-utils-0.3.8.6/pheno_utils/config_setup/create_default_config.py` & `pheno-utils-0.3.8.7/pheno_utils/config_setup/create_default_config.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/dates_plots.py` & `pheno-utils-0.3.8.7/pheno_utils/dates_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/ecg_analysis.py` & `pheno-utils-0.3.8.7/pheno_utils/ecg_analysis.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/meta_loader.py` & `pheno-utils-0.3.8.7/pheno_utils/meta_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/pheno_loader.py` & `pheno-utils-0.3.8.7/pheno_utils/pheno_loader.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/questionnaires_handler.py` & `pheno-utils-0.3.8.7/pheno_utils/questionnaires_handler.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils/sleep_plots.py` & `pheno-utils-0.3.8.7/pheno_utils/sleep_plots.py`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/pheno_utils.egg-info/PKG-INFO` & `pheno-utils-0.3.8.7/pheno_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pheno-utils
-Version: 0.3.8.6
+Version: 0.3.8.7
 Summary: Pheno data utils - viz, loaders, mergers
 Home-page: https://github.com/pheno-ai/pheno-utils
 Author: pheno.ai
 Author-email: hagai@pheno.ai
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pheno-utils-0.3.8.6/pheno_utils.egg-info/SOURCES.txt` & `pheno-utils-0.3.8.7/pheno_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pheno-utils-0.3.8.6/settings.ini` & `pheno-utils-0.3.8.7/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = pheno-utils
 lib_name = pheno-utils
-version = 0.3.8.6
+version = 0.3.8.7
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = pheno_utils
 nbs_path = nbs
 recursive = True
```

### Comparing `pheno-utils-0.3.8.6/setup.py` & `pheno-utils-0.3.8.7/setup.py`

 * *Files identical despite different names*


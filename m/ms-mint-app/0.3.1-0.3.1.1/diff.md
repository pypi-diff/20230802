# Comparing `tmp/ms-mint-app-0.3.1.tar.gz` & `tmp/ms-mint-app-0.3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms-mint-app-0.3.1.tar", last modified: Fri Jul 14 21:12:04 2023, max compression
+gzip compressed data, was "ms-mint-app-0.3.1.1.tar", last modified: Wed Aug  2 19:33:29 2023, max compression
```

## Comparing `ms-mint-app-0.3.1.tar` & `ms-mint-app-0.3.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/ms_mint_app/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/ms_mint_app/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/filelock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugin_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.157940 ms-mint-app-0.3.1/ms_mint_app/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/add_metabolites.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.157940 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/distributions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/pca.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/ms_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/quality_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/target_optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/plugins/workspaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/ms_mint_app/static/
--rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Chem.parquet
--rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Groups.parquet
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/Standard_Peaklist.csv
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 21:11:51.000000 ms-mint-app-0.3.1/ms_mint_app/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/ms_mint_app/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.157940 ms-mint-app-0.3.1/ms_mint_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-14 21:12:04.000000 ms-mint-app-0.3.1/ms_mint_app.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/scripts/Mint.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-07-14 21:12:04.169942 ms-mint-app-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-07-14 21:11:53.000000 ms-mint-app-0.3.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/ms_mint_app/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/ms_mint_app/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8872 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13453 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/filelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugin_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.213349 ms-mint-app-0.3.1.1/ms_mint_app/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/add_metabolites.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.213349 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6225 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/distributions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4626 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/pca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/ms_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4144 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/quality_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20693 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/target_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/plugins/workspaces.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/ms_mint_app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)  9253590 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/static/ChEBI-Chem.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)  1058677 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/static/ChEBI-Groups.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/static/Standard_Peaklist.csv
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:18.000000 ms-mint-app-0.3.1.1/ms_mint_app/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23724 2023-08-02 19:33:19.000000 ms-mint-app-0.3.1.1/ms_mint_app/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.209349 ms-mint-app-0.3.1.1/ms_mint_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-02 19:33:29.000000 ms-mint-app-0.3.1.1/ms_mint_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-08-02 19:33:29.000000 ms-mint-app-0.3.1.1/ms_mint_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 19:33:29.000000 ms-mint-app-0.3.1.1/ms_mint_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-08-02 19:33:29.000000 ms-mint-app-0.3.1.1/ms_mint_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 19:33:29.000000 ms-mint-app-0.3.1.1/ms_mint_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-08-02 19:33:19.000000 ms-mint-app-0.3.1.1/scripts/Mint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-08-02 19:33:29.225350 ms-mint-app-0.3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-08-02 19:33:19.000000 ms-mint-app-0.3.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-08-02 19:33:19.000000 ms-mint-app-0.3.1.1/versioneer.py
```

### Comparing `ms-mint-app-0.3.1/LICENSE` & `ms-mint-app-0.3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/PKG-INFO` & `ms-mint-app-0.3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.3.1
+Version: 0.3.1.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-app-0.3.1/README.md` & `ms-mint-app-0.3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/app.py` & `ms-mint-app-0.3.1.1/ms_mint_app/app.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/auth.py` & `ms-mint-app-0.3.1.1/ms_mint_app/auth.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/database.py` & `ms-mint-app-0.3.1.1/ms_mint_app/database.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/filelock.py` & `ms-mint-app-0.3.1.1/ms_mint_app/filelock.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/messages.py` & `ms-mint-app-0.3.1.1/ms_mint_app/messages.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugin_manager.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/add_metabolites.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/add_metabolites.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/distributions.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/distributions.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/heatmap.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/heatmap.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/hierachical_clustering.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/pca.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/pca.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/analysis_tools/plotting.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/analysis_tools/plotting.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/metadata.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/metadata.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/ms_files.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/ms_files.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/processing.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/processing.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/quality_control.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/quality_control.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/target_optimization.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/target_optimization.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             dbc.Col(dbc.Button("Regenerate all figures", id="pko-peak-preview-from-scratch", style={'width': '100%'})),
             dbc.Col(dbc.Button("Detect rt_min,rt_max for all targets", id="pko-detect-rtmin-rtmax-for-all", color='danger', style={'width': '100%'})),
         ]),
         dcc.Markdown("---"),
 
         html.Div(
             id="pko-peak-preview-images",
-            style={"maxHeight": "600px", "overflowX": "scroll", "padding": "auto"},
+            style={"maxHeight": "700px", "overflowX": "scroll", "padding": "auto"},
 
         ),
         dcc.Markdown("---"),
         html.H4("Interactive Rt optimization"),
 
         html.Div(id="pko-controls"),
         dcc.Dropdown(id="pko-dropdown", options=[], value=None),
```

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/targets.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/targets.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/plugins/workspaces.py` & `ms-mint-app-0.3.1.1/ms_mint_app/plugins/workspaces.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Chem.parquet` & `ms-mint-app-0.3.1.1/ms_mint_app/static/ChEBI-Chem.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/static/ChEBI-Groups.parquet` & `ms-mint-app-0.3.1.1/ms_mint_app/static/ChEBI-Groups.parquet`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/ms_mint_app/tools.py` & `ms-mint-app-0.3.1.1/ms_mint_app/tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -769,15 +769,15 @@
     return buffer.getvalue
 
 
 def df_to_in_memory_excel_file(df):
     def to_xlsx(bytes_io):
         xslx_writer = pd.ExcelWriter(bytes_io, engine="xlsxwriter")
         df.to_excel(xslx_writer, index=True, sheet_name="sheet1")
-        xslx_writer.save()
+        xslx_writer.close()
 
     return to_xlsx
 
 
 def has_na(df):
     return df.isna().sum().sum() > 0
```

### Comparing `ms-mint-app-0.3.1/ms_mint_app.egg-info/PKG-INFO` & `ms-mint-app-0.3.1.1/ms_mint_app.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-mint-app
-Version: 0.3.1
+Version: 0.3.1.1
 Summary: Metabolomics Integrator (Mint)
 Home-page: https://github.com/LewisResearchGroup/ms-mint-app
 Author: Soren Wacker
 Author-email: swacker@ucalgary.ca
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ms-mint-app-0.3.1/ms_mint_app.egg-info/SOURCES.txt` & `ms-mint-app-0.3.1.1/ms_mint_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/scripts/Mint.py` & `ms-mint-app-0.3.1.1/scripts/Mint.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/setup.py` & `ms-mint-app-0.3.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `ms-mint-app-0.3.1/versioneer.py` & `ms-mint-app-0.3.1.1/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/featherplot-0.0.5.tar.gz` & `tmp/featherplot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featherplot-0.0.5.tar", last modified: Wed Aug  2 19:24:42 2023, max compression
+gzip compressed data, was "featherplot-0.0.6.tar", last modified: Wed Aug  2 19:42:05 2023, max compression
```

## Comparing `featherplot-0.0.5.tar` & `featherplot-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:24:42.535145 featherplot-0.0.5/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.5/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.5/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1850 2023-08-02 19:24:42.535012 featherplot-0.0.5/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.5/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:24:42.533606 featherplot-0.0.5/featherplot/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    17719 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1574 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/commands.py
--rw-r--r--   0 solst      (501) staff       (20)      190 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.5/featherplot/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)     4366 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/deepscatter.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-08-02 19:07:12.000000 featherplot-0.0.5/featherplot/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      241 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     6523 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/types.py
--rw-r--r--   0 solst      (501) staff       (20)    20880 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:24:42.534782 featherplot-0.0.5/featherplot.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1850 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      572 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)      115 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.5/featherplot.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       40 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      980 2023-08-02 19:24:31.000000 featherplot-0.0.5/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-08-02 19:24:42.535186 featherplot-0.0.5/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.5/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:42:05.579566 featherplot-0.0.6/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.6/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.6/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1879 2023-08-02 19:42:05.579443 featherplot-0.0.6/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1210 2023-08-02 19:41:47.000000 featherplot-0.0.6/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:42:05.578166 featherplot-0.0.6/featherplot/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    17719 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1574 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)      190 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.6/featherplot/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)     4366 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/deepscatter.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-08-02 19:07:12.000000 featherplot-0.0.6/featherplot/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      241 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     6523 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    20880 2023-08-02 19:41:44.000000 featherplot-0.0.6/featherplot/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:42:05.579267 featherplot-0.0.6/featherplot.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1879 2023-08-02 19:42:05.000000 featherplot-0.0.6/featherplot.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      572 2023-08-02 19:42:05.000000 featherplot-0.0.6/featherplot.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-02 19:42:05.000000 featherplot-0.0.6/featherplot.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)      115 2023-08-02 19:42:05.000000 featherplot-0.0.6/featherplot.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.6/featherplot.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       45 2023-08-02 19:42:05.000000 featherplot-0.0.6/featherplot.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-08-02 19:42:05.000000 featherplot-0.0.6/featherplot.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      985 2023-08-02 19:41:41.000000 featherplot-0.0.6/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-08-02 19:42:05.579602 featherplot-0.0.6/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2601 2023-08-02 19:29:43.000000 featherplot-0.0.6/setup.py
```

### Comparing `featherplot-0.0.5/LICENSE` & `featherplot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/PKG-INFO` & `featherplot-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.5
+Version: 0.0.6
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: featherplot feather pyarrow arrow feather-format parquet parquet-format anndata single cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-featherplot
-================
+# featherplot
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
 
 ### Setup
 
@@ -63,15 +62,15 @@
 ### Publishing
 
 ``` sh
 # publish to pypi
 $ nbdev_pypi
 
 # publish to conda
-$ nbdev_conda
+$ nbdev_conda --build_args '-c conda-forge'  --mambabuild
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
```

### Comparing `featherplot-0.0.5/README.md` & `featherplot-0.0.6/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-featherplot
-================
+# featherplot
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
 
 ### Setup
 
@@ -44,15 +43,15 @@
 ### Publishing
 
 ``` sh
 # publish to pypi
 $ nbdev_pypi
 
 # publish to conda
-$ nbdev_conda
+$ nbdev_conda --build_args '-c conda-forge'  --mambabuild
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
```

### Comparing `featherplot-0.0.5/featherplot/_modidx.py` & `featherplot-0.0.6/featherplot/_modidx.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/featherplot/commands.py` & `featherplot-0.0.6/featherplot/commands.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/featherplot/deepscatter.py` & `featherplot-0.0.6/featherplot/deepscatter.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/featherplot/paths.py` & `featherplot-0.0.6/featherplot/paths.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/featherplot/types.py` & `featherplot-0.0.6/featherplot/types.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/featherplot/utils.py` & `featherplot-0.0.6/featherplot/utils.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/featherplot.egg-info/PKG-INFO` & `featherplot-0.0.6/featherplot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.5
+Version: 0.0.6
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: featherplot feather pyarrow arrow feather-format parquet parquet-format anndata single cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.10
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-featherplot
-================
+# featherplot
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 ## Developer Guide
 
 ### Setup
 
@@ -63,15 +62,15 @@
 ### Publishing
 
 ``` sh
 # publish to pypi
 $ nbdev_pypi
 
 # publish to conda
-$ nbdev_conda
+$ nbdev_conda --build_args '-c conda-forge'  --mambabuild
 ```
 
 # Usage
 
 ## Installation
 
 Install latest from the GitHub
```

### Comparing `featherplot-0.0.5/featherplot.egg-info/SOURCES.txt` & `featherplot-0.0.6/featherplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.5/settings.ini` & `featherplot-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [DEFAULT]
 repo = featherplot-py
 lib_name = featherplot
-version = 0.0.5
-min_python = 3.10
+version = 0.0.6
+min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = featherplot
 nbs_path = nbs
 recursive = True
 tst_flags = notest
@@ -30,9 +30,9 @@
 console_scripts = featherplot=featherplot.commands:run_add_sidecars
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
-requirements = pyarrow rich typer numpy anndata
+requirements = pyarrow rich typer numpy>1.22 anndata
```

### Comparing `featherplot-0.0.5/setup.py` & `featherplot-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'mit': ('MIT License', 'OSI Approved :: MIT License'),
     'gpl2': ('GNU General Public License v2', 'OSI Approved :: GNU General Public License v2 (GPLv2)'),
     'gpl3': ('GNU General Public License v3', 'OSI Approved :: GNU General Public License v3 (GPLv3)'),
     'bsd3': ('BSD License', 'OSI Approved :: BSD License'),
 }
 statuses = [ '1 - Planning', '2 - Pre-Alpha', '3 - Alpha',
     '4 - Beta', '5 - Production/Stable', '6 - Mature', '7 - Inactive' ]
-py_versions = '3.6 3.7 3.8 3.9 3.10'.split()
+py_versions = '3.6 3.7 3.8 3.9 3.10 3.11'.split()
 
 requirements = shlex.split(cfg.get('requirements', ''))
 if cfg.get('pip_requirements'): requirements += shlex.split(cfg.get('pip_requirements', ''))
 min_python = cfg['min_python']
 lic = licenses.get(cfg['license'].lower(), (cfg['license'], None))
 dev_requirements = (cfg.get('dev_requirements') or '').split()
```


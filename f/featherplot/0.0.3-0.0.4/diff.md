# Comparing `tmp/featherplot-0.0.3.tar.gz` & `tmp/featherplot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featherplot-0.0.3.tar", last modified: Sun Jun 18 13:49:00 2023, max compression
+gzip compressed data, was "featherplot-0.0.4.tar", last modified: Wed Aug  2 19:07:14 2023, max compression
```

## Comparing `featherplot-0.0.3.tar` & `featherplot-0.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 13:49:00.494004 featherplot-0.0.3/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.3/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.3/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-18 13:49:00.493862 featherplot-0.0.3/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.3/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 13:49:00.491311 featherplot-0.0.3/featherplot/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    17489 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1574 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/commands.py
--rw-r--r--   0 solst      (501) staff       (20)      209 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.3/featherplot/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)     4366 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/deepscatter.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      241 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     6565 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/types.py
--rw-r--r--   0 solst      (501) staff       (20)    20393 2023-06-18 13:48:55.000000 featherplot-0.0.3/featherplot/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-06-18 13:49:00.493658 featherplot-0.0.3/featherplot.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      572 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)      115 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.3/featherplot.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-06-18 13:49:00.000000 featherplot-0.0.3/featherplot.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      870 2023-06-18 13:48:49.000000 featherplot-0.0.3/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-06-18 13:49:00.494045 featherplot-0.0.3/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.3/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:07:14.505150 featherplot-0.0.4/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.4/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.4/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1788 2023-08-02 19:07:14.504998 featherplot-0.0.4/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.4/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:07:14.503966 featherplot-0.0.4/featherplot/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    17719 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1574 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)      209 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.4/featherplot/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)     4366 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/deepscatter.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      241 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     6565 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    20880 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:07:14.504800 featherplot-0.0.4/featherplot.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1788 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      572 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)      115 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.4/featherplot.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)        7 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      870 2023-08-02 19:07:12.000000 featherplot-0.0.4/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-08-02 19:07:14.505194 featherplot-0.0.4/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.4/setup.py
```

### Comparing `featherplot-0.0.3/LICENSE` & `featherplot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/PKG-INFO` & `featherplot-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.3
+Version: 0.0.4
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `featherplot-0.0.3/README.md` & `featherplot-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/featherplot/_modidx.py` & `featherplot-0.0.4/featherplot/_modidx.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,8 +145,10 @@
                                    'featherplot.utils.create_conditional_channel': ( 'utils.html#create_conditional_channel',
                                                                                      'featherplot/utils.py'),
                                    'featherplot.utils.create_functional_channel': ( 'utils.html#create_functional_channel',
                                                                                     'featherplot/utils.py'),
                                    'featherplot.utils.create_lambda_channel': ('utils.html#create_lambda_channel', 'featherplot/utils.py'),
                                    'featherplot.utils.create_root_channel': ('utils.html#create_root_channel', 'featherplot/utils.py'),
                                    'featherplot.utils.get_user': ('utils.html#get_user', 'featherplot/utils.py'),
+                                   'featherplot.utils.handle_duplicate_columns': ( 'utils.html#handle_duplicate_columns',
+                                                                                   'featherplot/utils.py'),
                                    'featherplot.utils.make_temp_file': ('utils.html#make_temp_file', 'featherplot/utils.py')}}}
```

### Comparing `featherplot-0.0.3/featherplot/commands.py` & `featherplot-0.0.4/featherplot/commands.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/featherplot/deepscatter.py` & `featherplot-0.0.4/featherplot/deepscatter.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/featherplot/paths.py` & `featherplot-0.0.4/featherplot/paths.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/featherplot/types.py` & `featherplot-0.0.4/featherplot/types.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/featherplot/utils.py` & `featherplot-0.0.4/featherplot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/04_utils.ipynb.
 
 # %% auto 0
 __all__ = ['get_user', 'collapse_user', 'make_temp_file', 'QuadFeatherRenamer', 'create_lambda_channel',
            'create_conditional_channel', 'create_functional_channel', 'create_boolean_channel', 'create_color_channel',
-           'create_root_channel', 'SeriesToChannel', 'DataFrameToMetadata', 'MockSingleCellData', 'AnnDataProcessor']
+           'create_root_channel', 'SeriesToChannel', 'handle_duplicate_columns', 'DataFrameToMetadata',
+           'MockSingleCellData', 'AnnDataProcessor']
 
 # %% ../nbs/04_utils.ipynb 3
 import os, pwd, sys, json, yaml, atexit, tempfile, inspect
 
 import numpy as np, pandas as pd
 import anndata as ad
 
@@ -320,14 +321,30 @@
         return valids, errors
 
     def to_meta(self, **kwargs) -> dict:
         channel = self.convert()
         return channel.to_meta(**kwargs)
 
 # %% ../nbs/04_utils.ipynb 12
+def handle_duplicate_columns(df:pd.DataFrame) -> pd.DataFrame:
+    all_cols = df.columns.tolist()
+    uni_cols, col_cnts = np.unique(all_cols, return_counts=True)
+    
+    for n in uni_cols[col_cnts > 1]:
+        i = 0
+        for j, o in enumerate(all_cols):
+            if o != n:
+                continue
+            all_cols[j] = f'{n}_{i}'
+            i += 1
+            
+    df.columns = all_cols
+    return df
+
+# %% ../nbs/04_utils.ipynb 13
 @rich_auto
 @dataclass
 class DataFrameToMetadata:
     df: pd.DataFrame
     sidecars: Optional[List[str]] = field(default_factory=list)
     embedding: Optional[List[str]] = field(default_factory=lambda : ['x', 'y', 'z'])
     alt_names: Optional[Dict[str, str]] = field(default_factory=dict)
@@ -425,15 +442,15 @@
             sidecars=self.sidecars,
             columns_metadata=columns_metadata,
             tiles_dir=None
         )
         return d
 
 
-# %% ../nbs/04_utils.ipynb 15
+# %% ../nbs/04_utils.ipynb 16
 @rich_auto
 @dataclass
 class MockSingleCellData:
     label: Optional[str] = 'barcode'
     c_str: Optional[str] = 'condition'
     n_str: Optional[str] = 'norm'
     
@@ -569,15 +586,15 @@
                 layers = layers,
             )
             
             self._adata = adata
 
         return self._adata
 
-# %% ../nbs/04_utils.ipynb 17
+# %% ../nbs/04_utils.ipynb 18
 @rich_auto
 @dataclass
 class AnnDataProcessor:
     adata: ad.AnnData
     x_emb: str = 'X_phate'
     layer: Optional[str] = None
```

### Comparing `featherplot-0.0.3/featherplot.egg-info/PKG-INFO` & `featherplot-0.0.4/featherplot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.3
+Version: 0.0.4
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `featherplot-0.0.3/featherplot.egg-info/SOURCES.txt` & `featherplot-0.0.4/featherplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.3/settings.ini` & `featherplot-0.0.4/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = featherplot-py
 lib_name = featherplot
-version = 0.0.3
+version = 0.0.4
 min_python = 3.10
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = featherplot
 nbs_path = nbs
 recursive = True
```

### Comparing `featherplot-0.0.3/setup.py` & `featherplot-0.0.4/setup.py`

 * *Files identical despite different names*


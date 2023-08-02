# Comparing `tmp/featherplot-0.0.4.tar.gz` & `tmp/featherplot-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "featherplot-0.0.4.tar", last modified: Wed Aug  2 19:07:14 2023, max compression
+gzip compressed data, was "featherplot-0.0.5.tar", last modified: Wed Aug  2 19:24:42 2023, max compression
```

## Comparing `featherplot-0.0.4.tar` & `featherplot-0.0.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:07:14.505150 featherplot-0.0.4/
--rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.4/LICENSE
--rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.4/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-08-02 19:07:14.504998 featherplot-0.0.4/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.4/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:07:14.503966 featherplot-0.0.4/featherplot/
--rw-r--r--   0 solst      (501) staff       (20)       22 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)    17719 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     1574 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/commands.py
--rw-r--r--   0 solst      (501) staff       (20)      209 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/constants.py
--rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.4/featherplot/dataclasses.py
--rw-r--r--   0 solst      (501) staff       (20)     4366 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/deepscatter.py
--rw-r--r--   0 solst      (501) staff       (20)      134 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/files.py
--rw-r--r--   0 solst      (501) staff       (20)      890 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/paths.py
--rw-r--r--   0 solst      (501) staff       (20)      241 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/rich.py
--rw-r--r--   0 solst      (501) staff       (20)      191 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/typer.py
--rw-r--r--   0 solst      (501) staff       (20)     6565 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/types.py
--rw-r--r--   0 solst      (501) staff       (20)    20880 2023-08-02 19:07:12.000000 featherplot-0.0.4/featherplot/utils.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:07:14.504800 featherplot-0.0.4/featherplot.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     1788 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      572 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)      115 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.4/featherplot.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)        7 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)       12 2023-08-02 19:07:14.000000 featherplot-0.0.4/featherplot.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      870 2023-08-02 19:07:12.000000 featherplot-0.0.4/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2023-08-02 19:07:14.505194 featherplot-0.0.4/setup.cfg
--rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.4/setup.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:24:42.535145 featherplot-0.0.5/
+-rw-rw-r--   0 solst      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 featherplot-0.0.5/LICENSE
+-rw-rw-r--   0 solst      (501) staff       (20)      111 2023-04-27 10:12:58.000000 featherplot-0.0.5/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     1850 2023-08-02 19:24:42.535012 featherplot-0.0.5/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     1181 2023-06-16 13:10:42.000000 featherplot-0.0.5/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:24:42.533606 featherplot-0.0.5/featherplot/
+-rw-r--r--   0 solst      (501) staff       (20)       22 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)    17719 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     1574 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/commands.py
+-rw-r--r--   0 solst      (501) staff       (20)      190 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/constants.py
+-rw-r--r--   0 solst      (501) staff       (20)      406 2023-06-16 11:36:56.000000 featherplot-0.0.5/featherplot/dataclasses.py
+-rw-r--r--   0 solst      (501) staff       (20)     4366 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/deepscatter.py
+-rw-r--r--   0 solst      (501) staff       (20)      134 2023-08-02 19:07:12.000000 featherplot-0.0.5/featherplot/files.py
+-rw-r--r--   0 solst      (501) staff       (20)      890 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/paths.py
+-rw-r--r--   0 solst      (501) staff       (20)      241 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/rich.py
+-rw-r--r--   0 solst      (501) staff       (20)      191 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/typer.py
+-rw-r--r--   0 solst      (501) staff       (20)     6523 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/types.py
+-rw-r--r--   0 solst      (501) staff       (20)    20880 2023-08-02 19:24:31.000000 featherplot-0.0.5/featherplot/utils.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2023-08-02 19:24:42.534782 featherplot-0.0.5/featherplot.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     1850 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      572 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)      115 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2023-06-16 11:34:58.000000 featherplot-0.0.5/featherplot.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       40 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)       12 2023-08-02 19:24:42.000000 featherplot-0.0.5/featherplot.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      980 2023-08-02 19:24:31.000000 featherplot-0.0.5/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2023-08-02 19:24:42.535186 featherplot-0.0.5/setup.cfg
+-rw-rw-r--   0 solst      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 featherplot-0.0.5/setup.py
```

### Comparing `featherplot-0.0.4/LICENSE` & `featherplot-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/PKG-INFO` & `featherplot-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.4
+Version: 0.0.5
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
+Keywords: featherplot feather pyarrow arrow feather-format parquet parquet-format anndata single cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `featherplot-0.0.4/README.md` & `featherplot-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/featherplot/_modidx.py` & `featherplot-0.0.5/featherplot/_modidx.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/featherplot/commands.py` & `featherplot-0.0.5/featherplot/commands.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/featherplot/deepscatter.py` & `featherplot-0.0.5/featherplot/deepscatter.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/featherplot/paths.py` & `featherplot-0.0.5/featherplot/paths.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/featherplot/types.py` & `featherplot-0.0.5/featherplot/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,21 @@
 
 # %% ../nbs/03_types.ipynb 3
 from rich.repr import auto as rich_auto
 from dataclasses import dataclass, field, asdict
 from typing import Optional, Union, Any, List, TypeAlias, Literal, Tuple, get_args, Dict
 
 # %% ../nbs/03_types.ipynb 4
-#| export
-
-
-# %% ../nbs/03_types.ipynb 5
 QUADFEATHER_REQUIRED_COLUMNS: TypeAlias = Literal['x', 'y']
 QUADFEATHER_EXPECTED_COLUMNS: TypeAlias = Union[QUADFEATHER_REQUIRED_COLUMNS, Literal['z']]
 
-# %% ../nbs/03_types.ipynb 7
+# %% ../nbs/03_types.ipynb 6
 from typing import TypeVar
 
-# %% ../nbs/03_types.ipynb 8
+# %% ../nbs/03_types.ipynb 7
 Literals = TypeVar('Literals')
 
 @rich_auto
 @dataclass
 class TypeGuardError(TypeError):
     pass
 
@@ -102,15 +98,15 @@
 
 @rich_auto
 @dataclass
 class QuadFeatherColumnTypeGuard(LiteralTypeGuard):
     types: Optional[Literals] = field(default_factory=lambda : [QUADFEATHER_REQUIRED_COLUMNS, QUADFEATHER_EXPECTED_COLUMNS])
 
 
-# %% ../nbs/03_types.ipynb 10
+# %% ../nbs/03_types.ipynb 9
 Transform: TypeAlias = Literal['literal', 'linaer', 'log', 'sqrt']
 
 Range: TypeAlias = Tuple[Union[int, float], Union[int, float]]
 StringRange: TypeAlias = Union[str, List[str]]
 
 Domain: TypeAlias = Tuple[Union[int, float], Union[int, float]]
```

### Comparing `featherplot-0.0.4/featherplot/utils.py` & `featherplot-0.0.5/featherplot/utils.py`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/featherplot.egg-info/PKG-INFO` & `featherplot-0.0.5/featherplot.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: featherplot
-Version: 0.0.4
+Version: 0.0.5
 Summary: featherplot
 Home-page: https://github.com/dsm-72/featherplot-py
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
-Keywords: nbdev jupyter notebook python
+Keywords: featherplot feather pyarrow arrow feather-format parquet parquet-format anndata single cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `featherplot-0.0.4/featherplot.egg-info/SOURCES.txt` & `featherplot-0.0.5/featherplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `featherplot-0.0.4/settings.ini` & `featherplot-0.0.5/settings.ini`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = featherplot-py
 lib_name = featherplot
-version = 0.0.4
+version = 0.0.5
 min_python = 3.10
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = featherplot
 nbs_path = nbs
 recursive = True
@@ -18,20 +18,21 @@
 git_url = https://github.com/dsm-72/featherplot-py
 title = featherplot
 audience = Developers
 author = dsm-72
 author_email = sumner.magruder@yale.edu
 copyright = 2023 onwards, dsm-72
 description = featherplot
-keywords = nbdev jupyter notebook python
+keywords = featherplot feather pyarrow arrow feather-format parquet parquet-format anndata single cell
 language = English
 status = 3
 user = dsm-72
 conda_user = dsm-72
 console_scripts = featherplot=featherplot.commands:run_add_sidecars
 readme_nb = index.ipynb
 allowed_metadata_keys = 
 allowed_cell_metadata_keys = 
 jupyter_hooks = True
 clean_ids = True
 clear_all = False
+requirements = pyarrow rich typer numpy anndata
```

### Comparing `featherplot-0.0.4/setup.py` & `featherplot-0.0.5/setup.py`

 * *Files identical despite different names*


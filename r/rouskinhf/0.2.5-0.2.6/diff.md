# Comparing `tmp/rouskinhf-0.2.5.tar.gz` & `tmp/rouskinhf-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rouskinhf-0.2.5.tar", last modified: Fri Jul 28 05:17:19 2023, max compression
+gzip compressed data, was "rouskinhf-0.2.6.tar", last modified: Wed Aug  2 12:10:13 2023, max compression
```

## Comparing `rouskinhf-0.2.5.tar` & `rouskinhf-0.2.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 05:17:19.472392 rouskinhf-0.2.5/
--rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.2.5/LICENSE
--rw-r--r--   0 ymdt       (501) staff       (20)     7107 2023-07-28 05:17:19.472221 rouskinhf-0.2.5/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)     6656 2023-07-27 16:53:00.000000 rouskinhf-0.2.5/README.md
--rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-07-28 05:16:41.000000 rouskinhf-0.2.5/pyproject.toml
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 05:17:19.471206 rouskinhf-0.2.5/rouskinhf/
--rw-r--r--   0 ymdt       (501) staff       (20)      134 2023-07-28 00:54:40.000000 rouskinhf-0.2.5/rouskinhf/__init__.py
--rw-r--r--   0 ymdt       (501) staff       (20)    17391 2023-07-27 22:00:29.000000 rouskinhf-0.2.5/rouskinhf/datafolder.py
--rw-r--r--   0 ymdt       (501) staff       (20)    10786 2023-07-27 22:09:13.000000 rouskinhf-0.2.5/rouskinhf/datapoint.py
--rw-r--r--   0 ymdt       (501) staff       (20)      556 2023-07-20 03:42:13.000000 rouskinhf-0.2.5/rouskinhf/env.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2838 2023-07-27 04:57:54.000000 rouskinhf-0.2.5/rouskinhf/import_dataset_fun.py
--rw-r--r--   0 ymdt       (501) staff       (20)     4609 2023-07-26 22:55:50.000000 rouskinhf-0.2.5/rouskinhf/info_file.py
--rw-r--r--   0 ymdt       (501) staff       (20)    12498 2023-07-27 22:24:56.000000 rouskinhf-0.2.5/rouskinhf/list_datapoints.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3652 2023-07-25 20:41:22.000000 rouskinhf-0.2.5/rouskinhf/parsers.py
--rw-r--r--   0 ymdt       (501) staff       (20)     2503 2023-07-25 00:20:58.000000 rouskinhf-0.2.5/rouskinhf/path.py
--rw-r--r--   0 ymdt       (501) staff       (20)     6262 2023-07-25 18:54:46.000000 rouskinhf-0.2.5/rouskinhf/rnastructure.py
--rw-r--r--   0 ymdt       (501) staff       (20)     3681 2023-07-28 00:53:48.000000 rouskinhf-0.2.5/rouskinhf/util.py
-drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-07-28 05:17:19.471948 rouskinhf-0.2.5/rouskinhf.egg-info/
--rw-r--r--   0 ymdt       (501) staff       (20)     7107 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/PKG-INFO
--rw-r--r--   0 ymdt       (501) staff       (20)      458 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/SOURCES.txt
--rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/dependency_links.txt
--rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/requires.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-07-28 05:17:19.000000 rouskinhf-0.2.5/rouskinhf.egg-info/top_level.txt
--rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-07-28 05:17:19.472438 rouskinhf-0.2.5/setup.cfg
--rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.2.5/setup.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-08-02 12:10:13.652773 rouskinhf-0.2.6/
+-rw-r--r--   0 ymdt       (501) staff       (20)     1141 2023-06-30 22:14:56.000000 rouskinhf-0.2.6/LICENSE
+-rw-r--r--   0 ymdt       (501) staff       (20)     7297 2023-08-02 12:10:13.652647 rouskinhf-0.2.6/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)     6846 2023-08-02 12:09:36.000000 rouskinhf-0.2.6/README.md
+-rw-r--r--   0 ymdt       (501) staff       (20)      813 2023-08-02 12:05:39.000000 rouskinhf-0.2.6/pyproject.toml
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-08-02 12:10:13.651788 rouskinhf-0.2.6/rouskinhf/
+-rw-r--r--   0 ymdt       (501) staff       (20)      162 2023-08-02 11:32:59.000000 rouskinhf-0.2.6/rouskinhf/__init__.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    17314 2023-08-02 11:26:46.000000 rouskinhf-0.2.6/rouskinhf/datafolder.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    10757 2023-08-02 11:26:51.000000 rouskinhf-0.2.6/rouskinhf/datapoint.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2548 2023-08-02 12:00:47.000000 rouskinhf-0.2.6/rouskinhf/env.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2838 2023-07-27 04:57:54.000000 rouskinhf-0.2.6/rouskinhf/import_dataset_fun.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     4586 2023-08-02 11:26:59.000000 rouskinhf-0.2.6/rouskinhf/info_file.py
+-rw-r--r--   0 ymdt       (501) staff       (20)    12452 2023-08-02 11:27:06.000000 rouskinhf-0.2.6/rouskinhf/list_datapoints.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3652 2023-08-02 11:27:12.000000 rouskinhf-0.2.6/rouskinhf/parsers.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     2499 2023-08-02 11:27:24.000000 rouskinhf-0.2.6/rouskinhf/path.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     6543 2023-08-02 12:05:14.000000 rouskinhf-0.2.6/rouskinhf/rnastructure.py
+-rw-r--r--   0 ymdt       (501) staff       (20)     3111 2023-08-02 11:17:38.000000 rouskinhf-0.2.6/rouskinhf/util.py
+drwxr-xr-x   0 ymdt       (501) staff       (20)        0 2023-08-02 12:10:13.652470 rouskinhf-0.2.6/rouskinhf.egg-info/
+-rw-r--r--   0 ymdt       (501) staff       (20)     7297 2023-08-02 12:10:13.000000 rouskinhf-0.2.6/rouskinhf.egg-info/PKG-INFO
+-rw-r--r--   0 ymdt       (501) staff       (20)      458 2023-08-02 12:10:13.000000 rouskinhf-0.2.6/rouskinhf.egg-info/SOURCES.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)        1 2023-08-02 12:10:13.000000 rouskinhf-0.2.6/rouskinhf.egg-info/dependency_links.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)      152 2023-08-02 12:10:13.000000 rouskinhf-0.2.6/rouskinhf.egg-info/requires.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       10 2023-08-02 12:10:13.000000 rouskinhf-0.2.6/rouskinhf.egg-info/top_level.txt
+-rw-r--r--   0 ymdt       (501) staff       (20)       38 2023-08-02 12:10:13.652817 rouskinhf-0.2.6/setup.cfg
+-rw-r--r--   0 ymdt       (501) staff       (20)      468 2023-07-24 18:15:00.000000 rouskinhf-0.2.6/setup.py
```

### Comparing `rouskinhf-0.2.5/LICENSE` & `rouskinhf-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.5/PKG-INFO` & `rouskinhf-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: rouskinhf
-Version: 0.2.5
-Summary: A library to manipulate data for our DMS prediction models.
-Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
-License: MIT
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
 [![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
 ![PyPI](https://img.shields.io/pypi/v/rouskinhf)
 ![GitHub tag (with filter)](https://img.shields.io/github/v/tag/rouskinlab/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
@@ -106,14 +93,25 @@
 
 ```python
 !pip install python-dotenv
 %load_ext dotenv
 %dotenv env
 ```
 
+or, in a python script or Jupyter notebook:
+
+```python
+from rouskinhf import setup_env
+setup_env(
+    HUGGINGFACE_TOKEN="your token here",
+    DATA_FOLDER="data/datafolders",
+    ...
+)
+```
+
  The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
 
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
```

### Comparing `rouskinhf-0.2.5/README.md` & `rouskinhf-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: rouskinhf
+Version: 0.2.6
+Summary: A library to manipulate data for our DMS prediction models.
+Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
+License: MIT
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![Python CI](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/CI.yml)
 [![Publish distributions 📦 to PyPI](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml/badge.svg)](https://github.com/rouskinlab/rouskinhf/actions/workflows/release.yml)
 ![PyPI](https://img.shields.io/pypi/v/rouskinhf)
 ![GitHub tag (with filter)](https://img.shields.io/github/v/tag/rouskinlab/rouskinhf)
 
 # Download your RNA data from HuggingFace with rouskinhf!
 
@@ -93,14 +106,25 @@
 
 ```python
 !pip install python-dotenv
 %load_ext dotenv
 %dotenv env
 ```
 
+or, in a python script or Jupyter notebook:
+
+```python
+from rouskinhf import setup_env
+setup_env(
+    HUGGINGFACE_TOKEN="your token here",
+    DATA_FOLDER="data/datafolders",
+    ...
+)
+```
+
  The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
 
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
```

### Comparing `rouskinhf-0.2.5/pyproject.toml` & `rouskinhf-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 py-modules = ['rouskinhf']
 
 [project]
 name =  "rouskinhf"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
     {name = "Yves Martin", email = "yves@martin.yt"},
     {name = "Alberic de Lajarte", email = "albericlajarte@gmail.com"},
 ]
 description = "A library to manipulate data for our DMS prediction models."
 readme = "README.md"
 classifiers = [
```

### Comparing `rouskinhf-0.2.5/rouskinhf/datafolder.py` & `rouskinhf-0.2.6/rouskinhf/datafolder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,12 @@
-
-from typing import Any
-
-import json
-from .env import DATA_FOLDER
-
 from .path import PathDatafolder
-from .env import DATA_FOLDER, HUGGINGFACE_TOKEN
+from .env import env
 from .list_datapoints import ListofDatapoints
 from .info_file import infoFileWriter
 import os
-import numpy as np
 from huggingface_hub import HfApi
 from huggingface_hub import snapshot_download
 
 
 GENERATE_NPY = True
 PREDICT_STRUCTURE = False
 PREDICT_DMS = False
@@ -58,15 +51,15 @@
 
     def __init__(self, path_in, path_out, name, source, predict_structure, predict_dms) -> None:
         name = self._set_name(name, path_in)
         super().__init__(name, path_out)
         self.name = name
         self.path_in = path_in
         self.path_out = path_out
-        self.api = HfApi(token=HUGGINGFACE_TOKEN)
+        self.api = HfApi(token=env.HUGGINGFACE_TOKEN)
         self.predict_structure = predict_structure
         self.predict_dms = predict_dms
 
         # move path_in to source folder
         os.makedirs(self.get_source_folder(), exist_ok=True)
         os.system(f'cp -fr {path_in} {self.get_source_folder()}')
 
@@ -100,15 +93,15 @@
 
         >>> datafolder = DataFolder.from_dreem_output(path_in='data/input_files_for_testing/dreem_output.json', verbose=False)
         >>> datafolder.create_repo(exist_ok=True)
         """
 
         self.api.create_repo(
             repo_id=ROUSKINLAB+self.name,
-            token=HUGGINGFACE_TOKEN,
+            token=env.HUGGINGFACE_TOKEN,
             exist_ok=exist_ok,
             private=private,
             repo_type="dataset",
         )
 
     def upload_folder(self, revision = 'main', commit_message=None, commit_description=None, multi_commits=False, run_as_future=False, **kwargs):
 
@@ -145,15 +138,15 @@
         True
         """
 
         future = self.api.upload_folder(
             repo_id=ROUSKINLAB+self.name,
             folder_path=self.get_main_folder(),
             repo_type="dataset",
-            token=HUGGINGFACE_TOKEN,
+            token=env.HUGGINGFACE_TOKEN,
             revision=revision,
             commit_message=commit_message,
             commit_description=commit_description,
             multi_commits=multi_commits,
             run_as_future=run_as_future,
             allow_patterns=["source/*", "info.json", "data.json", "README.md"],
             **kwargs
@@ -360,15 +353,15 @@
 
         # Download the datafolder #TODO : check if the datafolder is already downloaded
         snapshot_download(
             repo_id = ROUSKINLAB+self.name,
             repo_type='dataset',
             local_dir=self.get_main_folder(),
             revision=revision,
-            token=HUGGINGFACE_TOKEN,
+            token=env.HUGGINGFACE_TOKEN,
             allow_patterns=['info.json', 'data.json']
             )
 
         assert os.path.isdir(self.get_main_folder()), f'No folder found in {self.get_main_folder()}'
         assert os.path.isfile(self.get_json()), f'No json file found in {self.get_main_folder()}'
 
         self.datapoints = ListofDatapoints.from_json(self.get_json(), tqdm=tqdm, verbose=verbose)
@@ -435,26 +428,26 @@
         If True, a progress bar is displayed. Default is True.
 
     verbose : bool, optional
         If True, the filtering report is displayed. Default is True.
 
     """
 
-    def from_fasta(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromFasta:
+    def from_fasta(path_in, path_out=env.DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromFasta:
         """Create a datafolder from a fasta file. See CreateDatafolderFromFasta for more details."""
         return CreateDatafolderFromFasta(path_in, path_out, name, predict_structure, predict_dms, generate_npy, tqdm=tqdm, verbose=verbose)
 
-    def from_dreem_output(path_in, path_out=DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromDreemOutput:
+    def from_dreem_output(path_in, path_out=env.DATA_FOLDER, name = None, predict_structure = PREDICT_STRUCTURE, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromDreemOutput:
         """Create a datafolder from a dreem output file. See CreateDatafolderFromDreemOutput for more details."""
         return CreateDatafolderFromDreemOutput(path_in, path_out, name, predict_structure, generate_npy, tqdm=tqdm, verbose= verbose)
 
-    def from_local(name, path=DATA_FOLDER, tqdm=True, verbose=True, generate_npy=False)->LoadDatafolderFromLocal:
+    def from_local(name, path=env.DATA_FOLDER, tqdm=True, verbose=True, generate_npy=False)->LoadDatafolderFromLocal:
         """Load a datafolder from local. See LoadDatafolderFromLocal for more details."""
         return LoadDatafolderFromLocal(name, path, tqdm=tqdm, verbose=verbose, generate_npy=generate_npy)
 
-    def from_ct_folder(path_in, path_out=DATA_FOLDER, name = None, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromCTfolder:
+    def from_ct_folder(path_in, path_out=env.DATA_FOLDER, name = None, predict_dms = PREDICT_DMS, generate_npy = GENERATE_NPY, tqdm=True, verbose=True)->CreateDatafolderFromCTfolder:
         """Create a datafolder from a folder of ct files. See CreateDatafolderFromCTfolder for more details."""
         return CreateDatafolderFromCTfolder(path_in, path_out, name, predict_dms, generate_npy, tqdm=tqdm, verbose= verbose)
 
-    def from_huggingface(name, path_out=DATA_FOLDER, tqdm=True, verbose=True)->LoadDatafolderFromHF:
+    def from_huggingface(name, path_out=env.DATA_FOLDER, tqdm=True, verbose=True)->LoadDatafolderFromHF:
         """Load a datafolder from HuggingFace. See LoadDatafolderFromHF for more details."""
         return LoadDatafolderFromHF(name, path_out, tqdm=tqdm, verbose=verbose)
```

### Comparing `rouskinhf-0.2.5/rouskinhf/datapoint.py` & `rouskinhf-0.2.6/rouskinhf/datapoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 
-from typing import Any, List
 from .parsers import *
 from .util import add_braces_if_no_braces, dot2int, int2dot, seq2int, standardize_sequence, sequence_has_regular_characters
 import numpy as np
 from .rnastructure import RNAstructure_singleton
 
 class Datapoint:
```

### Comparing `rouskinhf-0.2.5/rouskinhf/import_dataset_fun.py` & `rouskinhf-0.2.6/rouskinhf/import_dataset_fun.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.5/rouskinhf/info_file.py` & `rouskinhf-0.2.6/rouskinhf/info_file.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import datetime, os, json
-from typing import Any
 from .path import PathDatafolder
 
 STRUCTURE_FROM_RNASTRUCTURE = 'RNAstructure'
 STRUCTURE_FROM_SOURCE = 'source'
 DMS_FROM_RNASTRUCTURE = 'RNAstructure'
 DMS_FROM_SOURCE = 'source'
```

### Comparing `rouskinhf-0.2.5/rouskinhf/list_datapoints.py` & `rouskinhf-0.2.6/rouskinhf/list_datapoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 
 import os
 import numpy as np
-import json
-import re
 from .datapoint import Datapoint, DatapointFactory
-from typing import List, Tuple, Union, Optional
+from typing import List
 from .parsers import Fasta, DreemOutput
 import pandas as pd
 from tqdm import tqdm as tqdm_parser
 
 class ListofDatapoints:
 
     def __init__(self, datapoints=[], verbose=True):
```

### Comparing `rouskinhf-0.2.5/rouskinhf/parsers.py` & `rouskinhf-0.2.6/rouskinhf/parsers.py`

 * *Files identical despite different names*

### Comparing `rouskinhf-0.2.5/rouskinhf/path.py` & `rouskinhf-0.2.6/rouskinhf/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 
-from .env import DATA_FOLDER
+from .env import env
 import os
 from os.path import join
 
 class PathDatafolder:
     """Path to files and folders of a datafolder of name `name`. The path to the data folder is `DATA_FOLDER`, which is defined in `env`.
 
     Parameters
@@ -22,15 +22,15 @@
     >>> path = PathDatafolder(name='my_test_datafolder_pytest')
     >>> path.name
     'my_test_datafolder_pytest'
     >>> print(path)
     PathDatafolder(name='my_test_datafolder_pytest')
     """
 
-    def __init__(self, name, root = DATA_FOLDER) -> None:
+    def __init__(self, name, root = env.DATA_FOLDER) -> None:
         assert type(name) == str, f'name {name} is not a string'
         assert type(root) == str, f'root {root} is not a string'
         self.root = root
         self.name = name
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name='{self.name}')"
```

### Comparing `rouskinhf-0.2.5/rouskinhf/rnastructure.py` & `rouskinhf-0.2.6/rouskinhf/rnastructure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 import os
 import numpy as np
 import pandas as pd
-from .env import RNASTRUCTURE_PATH, RNASTRUCTURE_TEMP_FOLDER
+from .env import env
 
 def run_command(cmd):
     import subprocess
     process = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE)
     output, error = process.communicate()
     return output.decode('utf-8')
 
 class RNAstructure(object):
 
     """RNAstructure wrapper.
 
     Example
     -------
-
+    >>> from rouskinhf.rouskinhf import setup_env
+    >>> setup_env('env')
     >>> rnastructure = RNAstructure()
     >>> seq = 'TTAAACCGGCCAACATACCGCATATGAGGATCACCCATATGCTCAAGATATTCGAAAGAATATCTTTCCACAGTCGAAAGACTGTGTCTCTCTCTTCCTTTTTCTCTTCCTCTTTCTCTTTCTCTTTCTCTTCTCTTCTGTATTACGAGTTCGCTACTCGTTCCTTTCGA'
     >>> np.random.seed(seed=0)
     >>> dms = np.random.random(len(seq))
     >>> rnastructure.predictStructure(seq)
     '..............((((.(((((((.((....)))))))))..(((((((((....)))))))))..(((((((....))))))).....................................................)))).((((((.....)))))).........'
     >>> rnastructure.predictStructure(seq, dms)
     '.........................(((.............))).((((((...........((((((.......))))))..)))))).................................................................................'
     >>> len(rnastructure.predictPairingProbability(seq, dms))
     170
     """
 
     def __init__(self) -> None:
-        self.rnastructure_path = RNASTRUCTURE_PATH
-        self.directory = RNASTRUCTURE_TEMP_FOLDER
+        pass
 
     def predict_partition(self, temperature_k =None, dms = None):
         # predict the partition of rna structures
-        cmd = f"{os.path.join(self.rnastructure_path, 'partition')} {self.fasta_file} {self.pfs_file}"
+        cmd = f"{os.path.join(env.RNASTRUCTURE_PATH, 'partition')} {self.fasta_file} {self.pfs_file}"
         if temperature_k != None:
             cmd += ' --temperature '+str(temperature_k)
         if type(dms) != type(None):
             assert len(self.sequence) == len(dms), 'The length of the sequence is not the same as the length of the signal.'
             assert type(dms) in [list, tuple, np.ndarray], 'The dms signal should be a list of floats.'
             self.__write_dms_to_file(self.sequence, dms)
             cmd += ' --shape ' + self.dms_file
         run_command(cmd)
 
         # sum it into pairing probability
-        run_command(os.path.join(self.rnastructure_path,'ProbabilityPlot')+ ' ' +self.pfs_file + ' -t '+self.prob_file)
+        run_command(os.path.join(env.RNASTRUCTURE_PATH,'ProbabilityPlot')+ ' ' +self.pfs_file + ' -t '+self.prob_file)
 
         # read the probability file
         with open(self.prob_file,"r") as f:
             lines=f.readlines()
             pairingPrediction={'i':[],'j':[],'p':[]}
             for x in range(len(lines)):
                 if x>1:
@@ -87,26 +87,29 @@
         with open(self.dms_file, 'w') as f:
             for idx, (s, b) in enumerate(zip(signal, sequence)):
                 if b in 'AC':
                     f.write(f'{idx+1}\t{s}\n')
 
 
     def __make_temp_folder(self):
-        isExist = os.path.exists(self.directory)
-        if not isExist:
-            os.makedirs(self.directory)
-        return self.directory
+        """Remove content and make a new folder for temporary files."""
+        path = env.RNASTRUCTURE_TEMP_FOLDER
+        if os.path.exists(path):
+            import shutil
+            shutil.rmtree(path)
+        os.makedirs(path)
 
     def __make_files(self, temp_prefix='temp'):
-        self.pfs_file = f"{self.directory}/{temp_prefix}.pfs"
-        self.ct_file = f"{self.directory}/{temp_prefix}.ct"
-        self.dms_file = f"{self.directory}/{temp_prefix}.shape"
-        self.dot_file = f"{self.directory}/{temp_prefix}_dot.txt"
-        self.fasta_file = self.directory+'/'+temp_prefix+'.fasta'
-        self.prob_file = self.directory+'/'+temp_prefix+'_prob.txt'
+        this_file = lambda x: os.path.join(env.RNASTRUCTURE_TEMP_FOLDER, x)
+        self.pfs_file = this_file(f"{temp_prefix}.pfs")
+        self.ct_file = this_file(f"{temp_prefix}.ct")
+        self.dms_file = this_file(f"{temp_prefix}.shape")
+        self.dot_file = this_file(f"{temp_prefix}_dot.txt")
+        self.fasta_file = this_file(f"{temp_prefix}.fasta")
+        self.prob_file = this_file(f"{temp_prefix}_prob.txt")
 
     def __create_fasta_file(self, reference, sequence):
         # push the ref into a temp file
         temp_fasta = open(self.fasta_file, 'w')
         temp_fasta.write('>'+reference+'\n'+sequence)
         temp_fasta.close()
 
@@ -118,20 +121,21 @@
         return self.predict_partition(dms = dms)
 
     def predictStructure(self, sequence, dms = None):
         self.sequence = sequence
         self.__make_temp_folder()
         self.__make_files()
         self.__create_fasta_file('reference', sequence)
-        cmd = f"{os.path.join(self.rnastructure_path, 'Fold')} {self.fasta_file} {self.ct_file}"
+        cmd = f"{os.path.join(env.RNASTRUCTURE_PATH, 'Fold')} {self.fasta_file} {self.ct_file}"
         if type(dms) != type(None):
             assert len(sequence) == len(dms), 'The length of the sequence is not the same as the length of the signal.'
             assert type(dms) in [list, tuple, np.ndarray], 'The dms signal should be a list of floats.'
             self.__write_dms_to_file(sequence, dms)
             cmd += ' --dms ' + self.dms_file
         run_command(cmd)
-        cmd = f"{os.path.join(self.rnastructure_path, 'ct2dot')} {self.ct_file} 0 {self.dot_file}"
+        cmd = f"{os.path.join(env.RNASTRUCTURE_PATH, 'ct2dot')} {self.ct_file} 0 {self.dot_file}"
         run_command(cmd)
+        assert os.path.exists(self.dot_file), 'The dot file was not created. Check RNAstructure installation. If you use a Mac, make sure to run `setup_env(RNASTRUCTURE_PATH="abs/path/to/RNAstructure/exe")`.'
         with open(self.dot_file, 'r') as f:
             return f.readlines()[2].strip()
 
 RNAstructure_singleton = RNAstructure()
```

### Comparing `rouskinhf-0.2.5/rouskinhf/util.py` & `rouskinhf-0.2.6/rouskinhf/util.py`

 * *Files 13% similar despite different names*

```diff
@@ -54,32 +54,14 @@
 
 def add_braces_if_no_braces(s:str):
     if not s[0] == '{' or not s[-1] == '}':
         return '{' + s + '}'
     return s
 
 
-def source_env(path):
-    """
-    Source the environment variables from the file at path.
-
-    Args:
-        path (str): The path to the file to source.
-    """
-    out = {}
-    with open(path, 'r') as f:
-        for line in f.readlines():
-            line = line.split('#')[0].strip()
-            line = line.replace('export', '')
-            key, value = line.split('=')
-            key, value = key.replace(' ','').replace('"','').strip(), value.replace(' ','').replace('"','').strip()
-            os.environ[key] = value
-            out[key] = value
-
-    return out
 
 
 class DreemUtils:
     def flatten_json(data):
         out, row = [], {}
 
         for k,v in data.copy().items():
```

### Comparing `rouskinhf-0.2.5/rouskinhf.egg-info/PKG-INFO` & `rouskinhf-0.2.6/rouskinhf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rouskinhf
-Version: 0.2.5
+Version: 0.2.6
 Summary: A library to manipulate data for our DMS prediction models.
 Author-email: Yves Martin <yves@martin.yt>, Alberic de Lajarte <albericlajarte@gmail.com>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
@@ -106,14 +106,25 @@
 
 ```python
 !pip install python-dotenv
 %load_ext dotenv
 %dotenv env
 ```
 
+or, in a python script or Jupyter notebook:
+
+```python
+from rouskinhf import setup_env
+setup_env(
+    HUGGINGFACE_TOKEN="your token here",
+    DATA_FOLDER="data/datafolders",
+    ...
+)
+```
+
  The point of using environment variables is to ensure the privacy of your huggingface token. Make sure to add your `env` file to your `.gitignore`, so your HuggingFace token doesn't get pushed to any public repository.
 
 ### Import data with ``import_dataset``
 
 This repo provides a function ``import_dataset``, which allows your to pull a dataset from HuggingFace and store it locally. If the data is already stored locally, it will be loaded from the local folder. The type of data available is the DMS signal and the structure, under the shape of paired bases tuples. The function has the following signature:
 
 ```python
```


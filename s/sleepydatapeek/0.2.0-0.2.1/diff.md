# Comparing `tmp/sleepydatapeek-0.2.0.tar.gz` & `tmp/sleepydatapeek-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepydatapeek-0.2.0.tar", max compression
+gzip compressed data, was "sleepydatapeek-0.2.1.tar", max compression
```

## Comparing `sleepydatapeek-0.2.0.tar` & `sleepydatapeek-0.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.2.0/LICENSE
--rw-r--r--   0        0        0     1817 2023-08-01 22:30:32.920527 sleepydatapeek-0.2.0/README.md
--rw-r--r--   0        0        0      570 2023-08-01 22:33:33.036721 sleepydatapeek-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0     1118 2023-08-01 22:13:44.055991 sleepydatapeek-0.2.0/sleepydatapeek.py
--rw-r--r--   0        0        0     2016 2023-08-01 08:24:07.460864 sleepydatapeek-0.2.0/toolchain/commands.py
--rw-r--r--   0        0        0      421 2023-08-01 06:36:50.154356 sleepydatapeek-0.2.0/toolchain/utils.py
--rw-r--r--   0        0        0     2442 1970-01-01 00:00:00.000000 sleepydatapeek-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1817 2023-08-01 22:30:32.920527 sleepydatapeek-0.2.1/README.md
+-rw-r--r--   0        0        0      621 2023-08-02 17:58:03.679036 sleepydatapeek-0.2.1/pyproject.toml
+-rwxr-xr-x   0        0        0      929 2023-08-02 17:53:04.431941 sleepydatapeek-0.2.1/sleepydatapeek.py
+-rw-r--r--   0        0        0     1907 2023-08-02 17:53:14.924276 sleepydatapeek-0.2.1/toolchain/commands.py
+-rw-r--r--   0        0        0      247 2023-08-02 17:52:32.204969 sleepydatapeek-0.2.1/toolchain/utils.py
+-rw-r--r--   0        0        0     2553 1970-01-01 00:00:00.000000 sleepydatapeek-0.2.1/PKG-INFO
```

### Comparing `sleepydatapeek-0.2.0/LICENSE` & `sleepydatapeek-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.2.0/README.md` & `sleepydatapeek-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.2.0/pyproject.toml` & `sleepydatapeek-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepydatapeek"
-version = "0.2.0"
+version = "0.2.1"
 description = "Peek at local datafiles fast!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/datapeek"
 keywords = ["pandas", "data"]
 packages = [
@@ -12,11 +12,14 @@
     { include = "toolchain/commands.py" },
     { include = "toolchain/utils.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pandas = "^1.5.1"
+pyarrow = "^11.0"
+typer = "^0.9"
+tabulate = "^0.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sleepydatapeek-0.2.0/sleepydatapeek.py` & `sleepydatapeek-0.2.1/sleepydatapeek.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,25 +9,20 @@
   from sys import argv, exit
 
   sleepydatapeek(argv[1:])
   exit(0)
 '''
 
 # stdlib
-from os import path
-from pathlib import Path
-from typing import List, Dict, Union
-from sys import argv, exit, getsizeof
-from subprocess import call, check_output
-# custom modules
+from sys import exit
+# custom
 from toolchain.commands import datapeek_logic
 # 3rd party
 try:
   import typer
-  from yaml import safe_load, YAMLError
 except ModuleNotFoundError as e:
   print("Error: Missing one or more 3rd-party packages (pip install).")
   exit(1)
 
 
 def sleepydatapeek(input_path:str, output_path:str='') -> str:
   app = typer.Typer()
```

### Comparing `sleepydatapeek-0.2.0/toolchain/commands.py` & `sleepydatapeek-0.2.1/toolchain/commands.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 # stdlib
-from os import path
 from pathlib import Path, PurePosixPath
-from typing import List, Dict, Union
-from sys import argv, exit, getsizeof
+from sys import exit
 import pandas as pd
-from subprocess import call, check_output
-# custom modules
+# custom
 from toolchain.utils import *
 # 3rd party
 try:
   from yaml import safe_load, YAMLError
   from IPython.display import display
   from tabulate import tabulate
 except ModuleNotFoundError as e:
   print("Error: Missing one or more 3rd-party packages (pip install).")
   exit(1)
 
 
 #───Commands─────────────────
 def datapeek_logic(input_path:str, output_path:str='') -> str:
-  '''<brief-description>'''
+  '''builds and delivers payload string'''
 
   supported_formats = [
     'csv',
     'parquet',
     'json',
     'tsv'
   ]
```

### Comparing `sleepydatapeek-0.2.0/PKG-INFO` & `sleepydatapeek-0.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Metadata-Version: 2.1
 Name: sleepydatapeek
-Version: 0.2.0
+Version: 0.2.1
 Summary: Peek at local datafiles fast!
 Home-page: https://github.com/anthonybench/datapeek
 License: GNU GPL
 Keywords: pandas,data
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
+Requires-Dist: pyarrow (>=11.0,<12.0)
+Requires-Dist: tabulate (>=0.9,<0.10)
+Requires-Dist: typer (>=0.9,<0.10)
 Project-URL: Repository, https://github.com/anthonybench/datapeek
 Description-Content-Type: text/markdown
 
 # **DataPeek**
 *A quick way to peek at local datafiles.*
 
 <br />
```


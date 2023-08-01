# Comparing `tmp/quinten-cli-1.1.5.tar.gz` & `tmp/quinten-cli-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quinten-cli-1.1.5.tar", last modified: Thu Jul 13 10:21:49 2023, max compression
+gzip compressed data, was "quinten-cli-1.1.6.tar", last modified: Tue Aug  1 23:53:26 2023, max compression
```

## Comparing `quinten-cli-1.1.5.tar` & `quinten-cli-1.1.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/LICENSE
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/README.md
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.950682 quinten-cli-1.1.5/cli/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      925 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/__init__.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/env.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/input_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/install.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/output_interface.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1526 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/progress.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     5158 2023-07-13 10:21:37.000000 quinten-cli-1.1.5/cli/run.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/cli/status.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      586 2023-07-13 10:21:18.000000 quinten-cli-1.1.5/pyproject.toml
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/quinten_cli.egg-info/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/PKG-INFO
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      418 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/entry_points.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/requires.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-07-13 10:21:49.000000 quinten-cli-1.1.5/quinten_cli.egg-info/top_level.txt
--rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/setup.cfg
-drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-07-13 10:21:49.954682 quinten-cli-1.1.5/tests/
--rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/tests/test_api.py
--rw-rw-r--   0 quinten   (1000) quinten   (1000)     1249 2023-07-13 09:39:53.000000 quinten-cli-1.1.5/tests/test_progress_ui.py
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-08-01 23:53:26.664806 quinten-cli-1.1.6/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1069 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/LICENSE
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-08-01 23:53:26.664806 quinten-cli-1.1.6/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      294 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/README.md
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-08-01 23:53:26.660805 quinten-cli-1.1.6/cli/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      968 2023-08-01 23:44:54.000000 quinten-cli-1.1.6/cli/__init__.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      157 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/cli/env.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       46 2023-08-01 14:39:07.000000 quinten-cli-1.1.6/cli/exceptions.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      625 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/cli/input_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      741 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/cli/install.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1241 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/cli/output_interface.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1526 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/cli/progress.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     5219 2023-08-01 14:39:45.000000 quinten-cli-1.1.6/cli/run.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      366 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/cli/status.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      799 2023-08-01 23:49:23.000000 quinten-cli-1.1.6/pyproject.toml
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-08-01 23:53:26.664806 quinten-cli-1.1.6/quinten_cli.egg-info/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      603 2023-08-01 23:53:26.000000 quinten-cli-1.1.6/quinten_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      436 2023-08-01 23:53:26.000000 quinten-cli-1.1.6/quinten_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        1 2023-08-01 23:53:26.000000 quinten-cli-1.1.6/quinten_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       44 2023-08-01 23:53:26.000000 quinten-cli-1.1.6/quinten_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       74 2023-08-01 23:53:26.000000 quinten-cli-1.1.6/quinten_cli.egg-info/requires.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)        4 2023-08-01 23:53:26.000000 quinten-cli-1.1.6/quinten_cli.egg-info/top_level.txt
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)       38 2023-08-01 23:53:26.664806 quinten-cli-1.1.6/setup.cfg
+drwxrwxr-x   0 quinten   (1000) quinten   (1000)        0 2023-08-01 23:53:26.664806 quinten-cli-1.1.6/tests/
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)      322 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/tests/test_api.py
+-rw-rw-r--   0 quinten   (1000) quinten   (1000)     1249 2023-08-01 14:37:06.000000 quinten-cli-1.1.6/tests/test_progress_ui.py
```

### Comparing `quinten-cli-1.1.5/LICENSE` & `quinten-cli-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.5/PKG-INFO` & `quinten-cli-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.5
+Version: 1.1.6
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.5/cli/__init__.py` & `quinten-cli-1.1.6/cli/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import rich
 
+from .exceptions import CalledProcessError
 from .input_interface import ask, confirm, prompt
 from .install import get_install_command, install
 from .output_interface import Message as message
 from .progress import ProgressManager, progress
 from .run import (
     get,
     is_success,
```

### Comparing `quinten-cli-1.1.5/cli/input_interface.py` & `quinten-cli-1.1.6/cli/input_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.5/cli/install.py` & `quinten-cli-1.1.6/cli/install.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.5/cli/output_interface.py` & `quinten-cli-1.1.6/cli/output_interface.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.5/cli/progress.py` & `quinten-cli-1.1.6/cli/progress.py`

 * *Files identical despite different names*

### Comparing `quinten-cli-1.1.5/cli/run.py` & `quinten-cli-1.1.6/cli/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import shlex
 import subprocess
 import sys
 import types
 
 from plib import Path
 
+from . import exceptions
+
 
 def sh(*cmds, **kwargs):
     return run_commands(*cmds, shell=True, **kwargs)
 
 
 def run_commands(*cmds, **kwargs):
     for cmd in cmds:
@@ -107,15 +109,16 @@
             res = (
                 subprocess.run(args, text=text, check=check, shell=shell, **kwargs)
                 if wait
                 else subprocess.Popen(args, shell=shell, **kwargs)
             )
         except subprocess.CalledProcessError as error:
             if verbose_errors:
-                error = Exception(error.stderr or error)  # more verbose errors
+                # more verbose errors
+                error = exceptions.CalledProcessError(error.stderr or error)
             raise error
     return res
 
 
 def prepare_args(args, command=False, root=False):
     args = [str(arg) for arg in iterate_args(args, command)]
     if command:
```

### Comparing `quinten-cli-1.1.5/quinten_cli.egg-info/PKG-INFO` & `quinten-cli-1.1.6/quinten_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quinten-cli
-Version: 1.1.5
+Version: 1.1.6
 Author-email: Quinten Roets <qdr2104@columbia.edu>
 License: MIT
 Project-URL: Source Code, https://github.com/quintenroets/cli
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
```

### Comparing `quinten-cli-1.1.5/tests/test_progress_ui.py` & `quinten-cli-1.1.6/tests/test_progress_ui.py`

 * *Files identical despite different names*


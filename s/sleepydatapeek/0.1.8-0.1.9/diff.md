# Comparing `tmp/sleepydatapeek-0.1.8.tar.gz` & `tmp/sleepydatapeek-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepydatapeek-0.1.8.tar", max compression
+gzip compressed data, was "sleepydatapeek-0.1.9.tar", max compression
```

## Comparing `sleepydatapeek-0.1.8.tar` & `sleepydatapeek-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.1.8/LICENSE
--rw-r--r--   0        0        0     2157 2023-07-30 21:27:14.923444 sleepydatapeek-0.1.8/README.md
--rw-r--r--   0        0        0      570 2023-08-01 22:07:00.488256 sleepydatapeek-0.1.8/pyproject.toml
--rwxr-xr-x   0        0        0     1307 2023-08-01 08:21:08.446964 sleepydatapeek-0.1.8/sleepydatapeek.py
--rw-r--r--   0        0        0     2016 2023-08-01 08:24:07.460864 sleepydatapeek-0.1.8/toolchain/commands.py
--rw-r--r--   0        0        0      421 2023-08-01 06:36:50.154356 sleepydatapeek-0.1.8/toolchain/utils.py
--rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 sleepydatapeek-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-30 21:27:14.923251 sleepydatapeek-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2157 2023-07-30 21:27:14.923444 sleepydatapeek-0.1.9/README.md
+-rw-r--r--   0        0        0      570 2023-08-01 22:14:11.380149 sleepydatapeek-0.1.9/pyproject.toml
+-rwxr-xr-x   0        0        0     1118 2023-08-01 22:13:44.055991 sleepydatapeek-0.1.9/sleepydatapeek.py
+-rw-r--r--   0        0        0     2016 2023-08-01 08:24:07.460864 sleepydatapeek-0.1.9/toolchain/commands.py
+-rw-r--r--   0        0        0      421 2023-08-01 06:36:50.154356 sleepydatapeek-0.1.9/toolchain/utils.py
+-rw-r--r--   0        0        0     2782 1970-01-01 00:00:00.000000 sleepydatapeek-0.1.9/PKG-INFO
```

### Comparing `sleepydatapeek-0.1.8/LICENSE` & `sleepydatapeek-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.8/README.md` & `sleepydatapeek-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.8/pyproject.toml` & `sleepydatapeek-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sleepydatapeek"
-version = "0.1.8"
+version = "0.1.9"
 description = "Peek at local datafiles fast!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 repository = "https://github.com/anthonybench/datapeek"
 keywords = ["pandas", "data"]
 packages = [
```

### Comparing `sleepydatapeek-0.1.8/sleepydatapeek.py` & `sleepydatapeek-0.1.9/sleepydatapeek.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python
 
 '''README
-<readme-blurb>
+Usage:
+  # pip install sleepydatapeek
+  # pip install --upgrade sleepydatapeek
 
-❕ There is a CLIPME docstring at the bottom that serves a quick reference for useful python factoids that aren't particularly memorable, remove after development
-❕ Re-populate this README docstring with whatever makes sense
-❕ Remove unused imports
-❕ Remove example command
-❕ Run `poetry init` to generate basic pyproject.toml (consult existing examples)
+  from sleepydatapeek import sleepydatapeek
+  from sys import argv, exit
+
+  sleepydatapeek(argv[1:])
+  exit(0)
 '''
 
 # stdlib
 from os import path
 from pathlib import Path
 from typing import List, Dict, Union
 from sys import argv, exit, getsizeof
```

### Comparing `sleepydatapeek-0.1.8/toolchain/commands.py` & `sleepydatapeek-0.1.9/toolchain/commands.py`

 * *Files identical despite different names*

### Comparing `sleepydatapeek-0.1.8/PKG-INFO` & `sleepydatapeek-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sleepydatapeek
-Version: 0.1.8
+Version: 0.1.9
 Summary: Peek at local datafiles fast!
 Home-page: https://github.com/anthonybench/datapeek
 License: GNU GPL
 Keywords: pandas,data
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
```


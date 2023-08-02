# Comparing `tmp/sleepyemoji-3.5.tar.gz` & `tmp/sleepyemoji-3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleepyemoji-3.5.tar", max compression
+gzip compressed data, was "sleepyemoji-3.6.tar", max compression
```

## Comparing `sleepyemoji-3.5.tar` & `sleepyemoji-3.6.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.5/README.md
--rw-r--r--   0        0        0      568 2023-07-30 10:41:36.876291 sleepyemoji-3.5/pyproject.toml
--rwxr-xr-x   0        0        0     1372 2023-07-30 10:27:04.209058 sleepyemoji-3.5/sleepyemoji.py
--rw-r--r--   0        0        0     1143 2023-07-30 09:45:15.713124 sleepyemoji-3.5/toolchain/commands.py
--rw-r--r--   0        0        0     3186 2023-07-30 10:40:43.525787 sleepyemoji-3.5/toolchain/emojis.py
--rw-r--r--   0        0        0     2282 1970-01-01 00:00:00.000000 sleepyemoji-3.5/PKG-INFO
+-rw-r--r--   0        0        0     1676 2023-07-30 09:57:43.398987 sleepyemoji-3.6/README.md
+-rw-r--r--   0        0        0      603 2023-08-02 18:00:00.233706 sleepyemoji-3.6/pyproject.toml
+-rwxr-xr-x   0        0        0     1362 2023-08-02 17:54:30.955699 sleepyemoji-3.6/sleepyemoji.py
+-rw-r--r--   0        0        0     1137 2023-08-02 17:53:22.577136 sleepyemoji-3.6/toolchain/commands.py
+-rw-r--r--   0        0        0     3186 2023-07-30 10:40:43.525787 sleepyemoji-3.6/toolchain/emojis.py
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 sleepyemoji-3.6/PKG-INFO
```

### Comparing `sleepyemoji-3.5/README.md` & `sleepyemoji-3.6/README.md`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.5/pyproject.toml` & `sleepyemoji-3.6/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "sleepyemoji"
-version = "3.5"
+version = "3.6"
 description = "Print all the emojis that sleepyboy thinks are worthwhile!"
 authors = ["anthonybench <anythonybenchyep@gmail.com>"]
 license = "GNU GPL"
 readme = "README.md"
 keywords = ["emoji", "unicode"]
 repository = "https://github.com/anthonybench/emoji"
 packages = [
   { include = "sleepyemoji.py" },
   { include = "toolchain/commands.py" },
   { include = "toolchain/emojis.py" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-
+prettytable = "^3.8"
+typer = "^0.9"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `sleepyemoji-3.5/sleepyemoji.py` & `sleepyemoji-3.6/sleepyemoji.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,31 +15,30 @@
   1. New category? Update toolchain/commands.py
   2. Append lists in toolchain/emojis.py
   3. Update pypi package
   4. Update repository
 '''
 
 # stdlib
-import os
 from typing import List
-from sys import exit, argv
+from sys import exit
 # custom modules
-from toolchain.commands import run_logic
+from toolchain.commands import emoji_logic
 # 3rd party
 try:
   import typer
 except ModuleNotFoundError as e:
   print("Error: Missing one or more 3rd-party packages (pip install).")
   exit(1)
 
 
 def sleepyemoji(categories:List[str]) -> str:
   app = typer.Typer()
   @app.command()
-  def run(categories:List[str]) -> str:
+  def emoji(categories:List[str]) -> str:
     '''Another example command
 
     Prints emojis with some metadata, organized by category.
 
     ───Params\n
     categories:List[str] :: emoji categories to include (casing ignored)
 
@@ -54,14 +53,14 @@
 
     ───Example\n
       ./sleepyemoji.py a f h
 
     ───Return\n
     str :: prettytable string
     '''
-    return run_logic(categories)
+    return emoji_logic(categories)
   if (__name__ == "sleepyemoji") or (__name__ == '__main__'):
     app()
 
 
 ## Local Testing
 # sleepyemoji(argv)
```

### Comparing `sleepyemoji-3.5/toolchain/commands.py` & `sleepyemoji-3.6/toolchain/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # stdlib
 from typing import List
 from sys import exit
-# custom modules
+# custom
 from toolchain.emojis import *
 # 3rd party
 try:
   from prettytable import PrettyTable
 except ModuleNotFoundError as e:
   print("Error: Missing one or more 3rd-party packages (pip install).")
   exit(1)
 
 
 #───Commands─────────────────
-def run_logic(categories:List[str]) -> str:
+def emoji_logic(categories:List[str]) -> str:
   '''adds categories to output table provided in input array'''
 
   cats = [i.lower() for i in categories]
   res  = PrettyTable()
 
   res.field_names = [
     "Emoji", "Discord Value", "iOS Descriptor"
```

### Comparing `sleepyemoji-3.5/toolchain/emojis.py` & `sleepyemoji-3.6/toolchain/emojis.py`

 * *Files identical despite different names*

### Comparing `sleepyemoji-3.5/PKG-INFO` & `sleepyemoji-3.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: sleepyemoji
-Version: 3.5
+Version: 3.6
 Summary: Print all the emojis that sleepyboy thinks are worthwhile!
 Home-page: https://github.com/anthonybench/emoji
 License: GNU GPL
 Keywords: emoji,unicode
 Author: anthonybench
 Author-email: anythonybenchyep@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: prettytable (>=3.8,<4.0)
+Requires-Dist: typer (>=0.9,<0.10)
 Project-URL: Repository, https://github.com/anthonybench/emoji
 Description-Content-Type: text/markdown
 
 # **SleepyEmoji**
 *Fetch your favorite emojis fast!*
 
 <br />
```


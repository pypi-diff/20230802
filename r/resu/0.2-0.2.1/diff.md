# Comparing `tmp/resu-0.2.tar.gz` & `tmp/resu-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resu-0.2.tar", last modified: Sun May 15 13:29:45 2022, max compression
+gzip compressed data, was "resu-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `resu-0.2.tar` & `resu-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1101 2022-05-15 08:09:23.573397 resu-0.2/.github/workflows/build-checks.yml
--rw-r--r--   0        0        0     3134 2022-05-15 13:28:20.541812 resu-0.2/.gitignore
--rw-r--r--   0        0        0     1072 2022-05-15 07:12:25.704570 resu-0.2/LICENSE
--rw-r--r--   0        0        0     2559 2022-05-15 09:23:07.867270 resu-0.2/README.md
--rw-r--r--   0        0        0      403 2022-05-15 07:15:52.474313 resu-0.2/pyproject.toml
--rw-r--r--   0        0        0       27 2022-05-15 05:39:21.980043 resu-0.2/requirements.txt
--rw-r--r--   0        0        0      105 2022-05-15 13:28:33.995817 resu-0.2/resu/__init__.py
--rw-r--r--   0        0        0     4271 2022-05-15 13:27:17.234020 resu-0.2/resu/resu.py
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 resu-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1101 2022-05-15 08:09:23.573397 resu-0.2.1/.github/workflows/build-checks.yml
+-rw-r--r--   0        0        0     3105 2022-05-15 13:42:53.360968 resu-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1072 2022-05-15 07:12:25.704570 resu-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2559 2022-05-15 09:23:07.867270 resu-0.2.1/README.md
+-rw-r--r--   0        0        0      437 2023-08-02 19:14:24.664111 resu-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2022-05-15 05:39:21.980043 resu-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      107 2023-08-02 19:32:27.045979 resu-0.2.1/resu/__init__.py
+-rw-r--r--   0        0        0     6074 2022-10-24 16:52:06.880052 resu-0.2.1/resu/resu.py
+-rw-r--r--   0        0        0     2862 1970-01-01 00:00:00.000000 resu-0.2.1/PKG-INFO
```

### Comparing `resu-0.2/.github/workflows/build-checks.yml` & `resu-0.2.1/.github/workflows/build-checks.yml`

 * *Files identical despite different names*

### Comparing `resu-0.2/.gitignore` & `resu-0.2.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -158,12 +158,8 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Other
 .DS_Store
 .idea/
-*.ckpt
-*.json
-*.gz
-*.tgz
-*.7z
+
```

### Comparing `resu-0.2/LICENSE` & `resu-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `resu-0.2/README.md` & `resu-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `resu-0.2/resu/resu.py` & `resu-0.2.1/resu/resu.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 import base64
 import gzip
-import json
 import pickle
 import signal
 import sys
 import time
 from pathlib import Path
 from typing import Any, Callable, Iterable, Optional, Union
 
@@ -16,62 +15,110 @@
 try:
     import py7zr  # optional
 except ImportError:
     py7zr = False
 
 
 class Checkpoint:
+    """Checkpoint is a class that helps you to resume your progress from where
+    you left off in case of a keyboard interrupt (Ctrl+C) or a system crash.
+
+    Parameters
+    ----------
+    input_data : Optional[Union[Iterable, str]]
+        An iterable object or a path to a file containing the data to be
+        processed.
+    ckpt_file : Optional[str]
+        Path to the checkpoint file. If not provided, a checkpoint file will be
+        created automatically.
+
+    Attributes
+    ----------
+    input_data : Optional[Union[Iterable, str]]
+        An iterable object or a path to a file containing the data to be
+        processed.
+    ckpt_file : Optional[str]
+        Path to the checkpoint file. If not provided, a checkpoint file will be
+        created automatically.
+    progress : list
+        A list of completed entries.
+
+    Methods
+    -------
+    insert(input_data)
+        Inserts the input data.
+    resume(ckpt_file)
+        Resumes the progress from the checkpoint file.
+    ckpt_io(mode='read')
+        Reads or writes the progress to the checkpoint file.
+    keyboard_interrupt_handler(sig: int, _)
+        Handles the keyboard interrupt.
+    read_data() -> Iterable
+        Reads the input data from a file.
+    _encode(x: Any) -> bytes
+        Encodes the input data.
+    check_progress() -> list
+        Checks the progress.
+    record(func: Callable, checkpoint_every: int = 100, \
+        show_progress: bool = True, *args, **kwargs) -> list
+        Records the progress.
+    """
 
     def __init__(self,
                  input_data: Optional[Union[Iterable, str]] = None,
-                 ckpt_file: Optional[str] = None):
+                 ckpt_file: Optional[str] = None) -> None:
         self.input_data = input_data
         self.ckpt_file = ckpt_file
         self.progress = []
 
-    def insert(self, input_data):
+    def insert(self, input_data) -> None:
+        """Inserts the input data."""
         self.input_data = input_data
 
-    def resume(self, ckpt_file):
+    def resume(self, ckpt_file) -> None:
+        """Loads the progress from the checkpoint file."""
         self.ckpt_file = ckpt_file
 
-    def ckpt_io(self, mode='read'):
+    def ckpt_io(self, mode='read') -> Optional[list]:
+        """Reads or writes the progress to the checkpoint file."""
         if mode == 'write':
             with gzip.open(self.ckpt_file, 'wb') as j:
                 pickle.dump(self.progress, j)
         elif mode == 'read':
             with gzip.open(self.ckpt_file, 'rb') as j:
                 data = pickle.load(j)
             return data
 
     def keyboard_interrupt_handler(self, sig: int, _) -> None:
+        """Handles the keyboard interrupt."""
         print(f'KeyboardInterrupt (id: {sig}) has been caught...')
         print(f'Saving progress to checkpoint file `{self.ckpt_file}` before '
               'terminating the program gracefully...')
         self.ckpt_io(mode='write')
         sys.exit(1)
 
     def read_data(self) -> Iterable:
+        """Reads the input data from a file."""
         suffix = Path(self.input_data).suffix.lower()
         if suffix in ['.7z', '.7zip']:
             if not py7zr:
                 raise ImportError(
                     'py7zr is not installed! Install with: `pip install py7zr`'
                 )
             with py7zr.SevenZipFile(self.input_data, 'r') as z:
                 for j in z.readall().values():
-                    return json.load(j)
+                    return pickle.load(j)
 
         elif suffix == '.json':
             with open(self.input_data) as j:
-                return json.load(j)
+                return pickle.load(j)
 
         elif suffix in ['.gz', '.gzip']:
-            with gzip.open(self.input_data, 'rb') as j:
-                return json.load(j)
+            with gzip.open(self.ckpt_file, 'rb') as j:
+                return pickle.load(j)
 
         else:
             raise NotImplementedError(
                 'Input file format is not supported! Pass an iterable object '
                 'instead.\nSupported file formats for reading directly from '
                 'a file: (.json, .7zip|.7z, .gzip|.gz)')
```


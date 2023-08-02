# Comparing `tmp/bitrot-1.0.0.tar.gz` & `tmp/bitrot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bitrot-1.0.0.tar", last modified: Sun May 17 22:10:32 2020, max compression
+gzip compressed data, was "bitrot-1.0.1.tar", last modified: Wed Aug  2 11:03:44 2023, max compression
```

## Comparing `bitrot-1.0.0.tar` & `bitrot-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxr-xr-x   0 ambv       (502) staff       (20)        0 2020-05-17 22:10:32.215420 bitrot-1.0.0/
--rw-r--r--   0 ambv       (502) staff       (20)     8208 2020-05-17 22:10:32.215058 bitrot-1.0.0/PKG-INFO
--rw-r--r--   0 ambv       (502) staff       (20)     5658 2020-05-17 21:51:12.000000 bitrot-1.0.0/README.rst
-drwxr-xr-x   0 ambv       (502) staff       (20)        0 2020-05-17 22:10:32.211895 bitrot-1.0.0/bin/
--rw-r--r--   0 ambv       (502) staff       (20)     1454 2020-05-17 20:51:32.000000 bitrot-1.0.0/bin/bitrot
--rw-r--r--   0 ambv       (502) staff       (20)       38 2020-05-17 22:10:32.215522 bitrot-1.0.0/setup.cfg
--rw-r--r--   0 ambv       (502) staff       (20)     2997 2020-05-17 20:51:32.000000 bitrot-1.0.0/setup.py
-drwxr-xr-x   0 ambv       (502) staff       (20)        0 2020-05-17 22:10:32.212201 bitrot-1.0.0/src/
-drwxr-xr-x   0 ambv       (502) staff       (20)        0 2020-05-17 22:10:32.214522 bitrot-1.0.0/src/bitrot.egg-info/
--rw-r--r--   0 ambv       (502) staff       (20)     8208 2020-05-17 22:10:32.000000 bitrot-1.0.0/src/bitrot.egg-info/PKG-INFO
--rw-r--r--   0 ambv       (502) staff       (20)      246 2020-05-17 22:10:32.000000 bitrot-1.0.0/src/bitrot.egg-info/SOURCES.txt
--rw-r--r--   0 ambv       (502) staff       (20)        1 2020-05-17 22:10:32.000000 bitrot-1.0.0/src/bitrot.egg-info/dependency_links.txt
--rw-r--r--   0 ambv       (502) staff       (20)        1 2015-06-23 00:43:54.000000 bitrot-1.0.0/src/bitrot.egg-info/not-zip-safe
--rw-r--r--   0 ambv       (502) staff       (20)       36 2020-05-17 22:10:32.000000 bitrot-1.0.0/src/bitrot.egg-info/requires.txt
--rw-r--r--   0 ambv       (502) staff       (20)        7 2020-05-17 22:10:32.000000 bitrot-1.0.0/src/bitrot.egg-info/top_level.txt
--rwxr-xr-x   0 ambv       (502) staff       (20)    21373 2020-05-17 21:51:39.000000 bitrot-1.0.0/src/bitrot.py
+drwxr-xr-x   0 ambv       (501) staff       (20)        0 2023-08-02 11:03:44.996227 bitrot-1.0.1/
+-rw-r--r--   0 ambv       (501) staff       (20)      196 2023-08-02 07:58:49.000000 bitrot-1.0.1/.editorconfig
+-rw-r--r--   0 ambv       (501) staff       (20)       26 2023-08-02 07:58:49.000000 bitrot-1.0.1/.gitignore
+-rw-r--r--   0 ambv       (501) staff       (20)       45 2023-08-02 07:58:49.000000 bitrot-1.0.1/Ånnóying 𝚏Ⅰlęnąme by Łukasz
+-rw-r--r--   0 ambv       (501) staff       (20)     1080 2023-08-02 07:58:49.000000 bitrot-1.0.1/LICENSE
+-rw-r--r--   0 ambv       (501) staff       (20)     6951 2023-08-02 11:03:44.996067 bitrot-1.0.1/PKG-INFO
+-rw-r--r--   0 ambv       (501) staff       (20)     6285 2023-08-02 11:00:16.000000 bitrot-1.0.1/README.rst
+drwxr-xr-x   0 ambv       (501) staff       (20)        0 2023-08-02 11:03:44.994570 bitrot-1.0.1/bin/
+-rw-r--r--   0 ambv       (501) staff       (20)     1454 2023-08-02 07:58:49.000000 bitrot-1.0.1/bin/bitrot
+-rw-r--r--   0 ambv       (501) staff       (20)      993 2023-08-02 10:59:56.000000 bitrot-1.0.1/pyproject.toml
+-rw-r--r--   0 ambv       (501) staff       (20)       38 2023-08-02 11:03:44.996275 bitrot-1.0.1/setup.cfg
+drwxr-xr-x   0 ambv       (501) staff       (20)        0 2023-08-02 11:03:44.994706 bitrot-1.0.1/src/
+drwxr-xr-x   0 ambv       (501) staff       (20)        0 2023-08-02 11:03:44.995531 bitrot-1.0.1/src/bitrot.egg-info/
+-rw-r--r--   0 ambv       (501) staff       (20)     6951 2023-08-02 11:03:44.000000 bitrot-1.0.1/src/bitrot.egg-info/PKG-INFO
+-rw-r--r--   0 ambv       (501) staff       (20)      380 2023-08-02 11:03:44.000000 bitrot-1.0.1/src/bitrot.egg-info/SOURCES.txt
+-rw-r--r--   0 ambv       (501) staff       (20)        1 2023-08-02 11:03:44.000000 bitrot-1.0.1/src/bitrot.egg-info/dependency_links.txt
+-rw-r--r--   0 ambv       (501) staff       (20)       56 2023-08-02 11:03:44.000000 bitrot-1.0.1/src/bitrot.egg-info/entry_points.txt
+-rw-r--r--   0 ambv       (501) staff       (20)       28 2023-08-02 11:03:44.000000 bitrot-1.0.1/src/bitrot.egg-info/requires.txt
+-rw-r--r--   0 ambv       (501) staff       (20)        7 2023-08-02 11:03:44.000000 bitrot-1.0.1/src/bitrot.egg-info/top_level.txt
+-rwxr-xr-x   0 ambv       (501) staff       (20)    21224 2023-08-02 10:49:22.000000 bitrot-1.0.1/src/bitrot.py
+drwxr-xr-x   0 ambv       (501) staff       (20)        0 2023-08-02 11:03:44.995826 bitrot-1.0.1/tests/
+-rw-r--r--   0 ambv       (501) staff       (20)    11384 2023-08-02 10:49:22.000000 bitrot-1.0.1/tests/test_bitrot.py
+-rw-r--r--   0 ambv       (501) staff       (20)       20 2023-08-02 09:56:45.000000 bitrot-1.0.1/tests/test_requirements.txt
```

### Comparing `bitrot-1.0.0/README.rst` & `bitrot-1.0.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -45,20 +45,46 @@
 24 seconds.  Back in 2013, with a typical 5400 RPM laptop hard drive
 it took around 15 minutes.  How times have changed!
 
 Tests
 -----
 
 There's a simple but comprehensive test scenario using
-`BATS <https://github.com/sstephenson/bats>`.  Run the
-file in the `tests` directory to run it.
+`pytest <https://pypi.org/p/pytest>`_ and
+`pytest-order <https://pypi.org/p/pytest-order>`.
+
+Install::
+
+  $ python3 -m venv .venv
+  $ . .venv/bin/activate
+  (.venv)$ pip install -e .[test]
+
+Run::
+
+  (.venv)$ pytest -x
+  ==================== test session starts ====================
+  platform darwin -- Python 3.10.12, pytest-7.4.0, pluggy-1.2.0
+  rootdir: /Users/ambv/Documents/Python/bitrot
+  plugins: order-1.1.0
+  collected 12 items
+
+  tests/test_bitrot.py ............                      [100%]
+
+  ==================== 12 passed in 15.05s ====================
 
 Change Log
 ----------
 
+1.0.1
+~~~~~
+
+* officially remove Python 2 support that was broken since 1.0.0
+  anyway; now the package works with Python 3.8+ because of a few
+  features
+
 1.0.0
 ~~~~~
 
 * significantly sped up execution on solid state drives by using
   a process pool executor to calculate SHA1 hashes and perform `stat()`
   calls; use `-w1` if your runs on slow magnetic drives were
   negatively affected by this change
```

### Comparing `bitrot-1.0.0/bin/bitrot` & `bitrot-1.0.1/bin/bitrot`

 * *Files identical despite different names*

### Comparing `bitrot-1.0.0/src/bitrot.py` & `bitrot-1.0.1/src/bitrot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
+#!/usr/bin/env python3
 
 # Copyright (C) 2013 by Łukasz Langa
 
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -17,18 +16,15 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
-from __future__ import absolute_import
-from __future__ import division
-from __future__ import print_function
-from __future__ import unicode_literals
+from __future__ import annotations
 
 import argparse
 import atexit
 import datetime
 import errno
 import hashlib
 import os
@@ -36,27 +32,26 @@
 import sqlite3
 import stat
 import sys
 import tempfile
 import time
 import unicodedata
 
-from concurrent.futures import ProcessPoolExecutor, wait, as_completed
+from concurrent.futures import ProcessPoolExecutor, as_completed
+from importlib.metadata import version, PackageNotFoundError
 
 
 DEFAULT_CHUNK_SIZE = 16384  # block size in HFS+; 4X the block size in ext4
 DOT_THRESHOLD = 200
-VERSION = (1, 0, 0)
 IGNORED_FILE_SYSTEM_ERRORS = {errno.ENOENT, errno.EACCES}
 FSENCODING = sys.getfilesystemencoding()
-
-
-if sys.version[0] == '2':
-    str = type(u'text')
-    # use `bytes` for bytestrings
+try:
+    VERSION = version("bitrot")
+except PackageNotFoundError:
+    VERSION = "1.0.1"
 
 
 def normalize_path(path):
     path_uni = path.decode(FSENCODING)
     if FSENCODING in ('utf-8', 'UTF-8'):
         return unicodedata.normalize('NFKD', path_uni)
 
@@ -163,16 +158,14 @@
                 ),
                 file=sys.stderr,
             )
             raise BitrotException
 
         raise   # Not expected? https://github.com/ambv/bitrot/issues/
 
-    new_mtime = int(st.st_mtime)
-
     try:
         new_sha1 = sha1(path, chunk_size)
     except (IOError, OSError) as e:
         print(
             '\rwarning: cannot compute hash of {} [{}]'.format(
                 p_uni, errno.errorcode[e.args[0]],
             ),
@@ -543,15 +536,15 @@
         '-v', '--verbose', action='store_true',
         help='list new, updated and missing entries')
     parser.add_argument(
         '-t', '--test', action='store_true',
         help='just test against an existing database, don\'t update anything')
     parser.add_argument(
         '--version', action='version',
-        version='%(prog)s {}.{}.{}'.format(*VERSION))
+        version=f"%(prog)s {VERSION}")
     parser.add_argument(
         '--commit-interval', type=float, default=300,
         help='min time in seconds between commits '
              '(0 commits on every operation)')
     parser.add_argument(
         '-w', '--workers', type=int, default=os.cpu_count(),
         help='run this many workers (use -w1 for slow magnetic disks)')
```


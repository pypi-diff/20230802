# Comparing `tmp/kaydet-0.8.4.tar.gz` & `tmp/kaydet-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaydet-0.8.4.tar", last modified: Wed Aug  2 08:55:03 2023, max compression
+gzip compressed data, was "kaydet-0.8.5.tar", last modified: Wed Aug  2 10:39:33 2023, max compression
```

## Comparing `kaydet-0.8.4.tar` & `kaydet-0.8.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:55:03.637952 kaydet-0.8.4/
--rw-r--r--   0 mirat      (501) staff       (20)     1072 2023-08-02 07:26:21.000000 kaydet-0.8.4/LICENSE
--rw-r--r--   0 mirat      (501) staff       (20)     2294 2023-08-02 08:55:03.637843 kaydet-0.8.4/PKG-INFO
--rw-r--r--   0 mirat      (501) staff       (20)     1367 2023-08-02 08:54:21.000000 kaydet-0.8.4/README.md
--rw-r--r--   0 mirat      (501) staff       (20)       38 2023-08-02 08:55:03.637999 kaydet-0.8.4/setup.cfg
--rw-r--r--   0 mirat      (501) staff       (20)     1106 2023-08-02 08:52:52.000000 kaydet-0.8.4/setup.py
-drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:55:03.637102 kaydet-0.8.4/src/
--rw-r--r--   0 mirat      (501) staff       (20)        0 2023-08-02 07:27:04.000000 kaydet-0.8.4/src/__init__.py
-drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:55:03.637684 kaydet-0.8.4/src/kaydet.egg-info/
--rw-r--r--   0 mirat      (501) staff       (20)     2294 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/PKG-INFO
--rw-r--r--   0 mirat      (501) staff       (20)      229 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/SOURCES.txt
--rw-r--r--   0 mirat      (501) staff       (20)        1 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/dependency_links.txt
--rw-r--r--   0 mirat      (501) staff       (20)       39 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/entry_points.txt
--rw-r--r--   0 mirat      (501) staff       (20)       16 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/top_level.txt
--rwxr-xr-x   0 mirat      (501) staff       (20)     3398 2023-08-02 08:54:45.000000 kaydet-0.8.4/src/kaydet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:39:33.449740 kaydet-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-02 10:39:23.000000 kaydet-0.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-02 10:39:33.449740 kaydet-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-08-02 10:39:23.000000 kaydet-0.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 10:39:33.449740 kaydet-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-08-02 10:39:23.000000 kaydet-0.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:39:33.449740 kaydet-0.8.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 10:39:23.000000 kaydet-0.8.5/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 10:39:33.449740 kaydet-0.8.5/src/kaydet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-08-02 10:39:33.000000 kaydet-0.8.5/src/kaydet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-08-02 10:39:33.000000 kaydet-0.8.5/src/kaydet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 10:39:33.000000 kaydet-0.8.5/src/kaydet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 10:39:33.000000 kaydet-0.8.5/src/kaydet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 10:39:33.000000 kaydet-0.8.5/src/kaydet.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3369 2023-08-02 10:39:23.000000 kaydet-0.8.5/src/kaydet.py
```

### Comparing `kaydet-0.8.4/LICENSE` & `kaydet-0.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kaydet-0.8.4/PKG-INFO` & `kaydet-0.8.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kaydet
-Version: 0.8.4
-Summary: ('Simple and terminal-based personal diary app designed to help you preserve your daily thoughts, experiences, and memories.',)
+Version: 0.8.5
+Summary: Simple and terminal-based personal diary app designed to help you preserve your daily thoughts, experiences, and memories.
 Home-page: https://github.com/miratcan/logme
 Author: Mirat Can Bayrak
 License: MIT
 Keywords: diary tui
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,14 +25,18 @@
 
 # Kaydet is Your Personal Terminal Diary
 
 "kaydet" is a simple (112 lines if Python code) based diary app designed to
 help you preserve your daily thoughts, experiences, and memories without 
 leaving terminal.
 
+# How to Install?
+
+    $ pip3 install kaydet
+
 # Key Features:
 
 ## Short Entries
 
 Record your daily thoughts and experiences by typing them as a parameter in
 the terminal. "kaydet" automatically saves your entry to a file dedicated to
 the current day, along with a timestamp.
```

### Comparing `kaydet-0.8.4/README.md` & `kaydet-0.8.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Kaydet is Your Personal Terminal Diary
 
 "kaydet" is a simple (112 lines if Python code) based diary app designed to
 help you preserve your daily thoughts, experiences, and memories without 
 leaving terminal.
 
+# How to Install?
+
+    $ pip3 install kaydet
+
 # Key Features:
 
 ## Short Entries
 
 Record your daily thoughts and experiences by typing them as a parameter in
 the terminal. "kaydet" automatically saves your entry to a file dedicated to
 the current day, along with a timestamp.
```

### Comparing `kaydet-0.8.4/setup.py` & `kaydet-0.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `kaydet-0.8.4/src/kaydet.egg-info/PKG-INFO` & `kaydet-0.8.5/src/kaydet.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: kaydet
-Version: 0.8.4
-Summary: ('Simple and terminal-based personal diary app designed to help you preserve your daily thoughts, experiences, and memories.',)
+Version: 0.8.5
+Summary: Simple and terminal-based personal diary app designed to help you preserve your daily thoughts, experiences, and memories.
 Home-page: https://github.com/miratcan/logme
 Author: Mirat Can Bayrak
 License: MIT
 Keywords: diary tui
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -25,14 +25,18 @@
 
 # Kaydet is Your Personal Terminal Diary
 
 "kaydet" is a simple (112 lines if Python code) based diary app designed to
 help you preserve your daily thoughts, experiences, and memories without 
 leaving terminal.
 
+# How to Install?
+
+    $ pip3 install kaydet
+
 # Key Features:
 
 ## Short Entries
 
 Record your daily thoughts and experiences by typing them as a parameter in
 the terminal. "kaydet" automatically saves your entry to a file dedicated to
 the current day, along with a timestamp.
```

### Comparing `kaydet-0.8.4/src/kaydet.py` & `kaydet-0.8.5/src/kaydet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __author__ = "Mirat Can Bayrak"
 __copyright__ = "Copyright 2016, Planet Earth"
-__version__ = "0.8.4"
+__version__ = "0.8.5"
 __description__ = "Simple and terminal-based personal diary app designed " \
                   "to help you preserve your daily thoughts, experiences, " \
-                  "and memories.",
+                  "and memories."
 
 
 from datetime import datetime
 
 from os import mkdir, environ as env
 from os.path import expanduser, join, exists
 from configparser import ConfigParser
@@ -19,15 +19,15 @@
 
 def parse_args(config_path):
     parser = argparse.ArgumentParser(
         prog='kaydet',
         description=__description__,
         epilog="You can configure this by editing: %s" % config_path +
                "You can try these:\n\n"
-               "  $ kaydet 'I felt grateful when spending time with my kids.'\n"
+               "  $ kaydet 'I felt grateful now.'\n"
                "  $ kaydet \"When I'm typing this I felt that I need an "
                "editor\" --editor",
         formatter_class=argparse.RawTextHelpFormatter
     )
     parser.add_argument(
         'entry', type=str, nargs='?', metavar='Entry', action='store',
         help='Your one entry to be saved. If not given, editor will be '
```


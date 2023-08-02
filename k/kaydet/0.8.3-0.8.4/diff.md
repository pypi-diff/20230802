# Comparing `tmp/kaydet-0.8.3.tar.gz` & `tmp/kaydet-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaydet-0.8.3.tar", last modified: Wed Aug  2 08:52:57 2023, max compression
+gzip compressed data, was "kaydet-0.8.4.tar", last modified: Wed Aug  2 08:55:03 2023, max compression
```

## Comparing `kaydet-0.8.3.tar` & `kaydet-0.8.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:52:57.011558 kaydet-0.8.3/
--rw-r--r--   0 mirat      (501) staff       (20)     1072 2023-08-02 07:26:21.000000 kaydet-0.8.3/LICENSE
--rw-r--r--   0 mirat      (501) staff       (20)     2292 2023-08-02 08:52:57.011454 kaydet-0.8.3/PKG-INFO
--rw-r--r--   0 mirat      (501) staff       (20)     1365 2023-08-02 08:41:27.000000 kaydet-0.8.3/README.md
--rw-r--r--   0 mirat      (501) staff       (20)       38 2023-08-02 08:52:57.011595 kaydet-0.8.3/setup.cfg
--rw-r--r--   0 mirat      (501) staff       (20)     1106 2023-08-02 08:52:52.000000 kaydet-0.8.3/setup.py
-drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:52:57.010704 kaydet-0.8.3/src/
--rw-r--r--   0 mirat      (501) staff       (20)        0 2023-08-02 07:27:04.000000 kaydet-0.8.3/src/__init__.py
-drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:52:57.011291 kaydet-0.8.3/src/kaydet.egg-info/
--rw-r--r--   0 mirat      (501) staff       (20)     2292 2023-08-02 08:52:57.000000 kaydet-0.8.3/src/kaydet.egg-info/PKG-INFO
--rw-r--r--   0 mirat      (501) staff       (20)      229 2023-08-02 08:52:57.000000 kaydet-0.8.3/src/kaydet.egg-info/SOURCES.txt
--rw-r--r--   0 mirat      (501) staff       (20)        1 2023-08-02 08:52:57.000000 kaydet-0.8.3/src/kaydet.egg-info/dependency_links.txt
--rw-r--r--   0 mirat      (501) staff       (20)       39 2023-08-02 08:52:57.000000 kaydet-0.8.3/src/kaydet.egg-info/entry_points.txt
--rw-r--r--   0 mirat      (501) staff       (20)       16 2023-08-02 08:52:57.000000 kaydet-0.8.3/src/kaydet.egg-info/top_level.txt
--rwxr-xr-x   0 mirat      (501) staff       (20)     3398 2023-08-02 08:37:57.000000 kaydet-0.8.3/src/kaydet.py
+drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:55:03.637952 kaydet-0.8.4/
+-rw-r--r--   0 mirat      (501) staff       (20)     1072 2023-08-02 07:26:21.000000 kaydet-0.8.4/LICENSE
+-rw-r--r--   0 mirat      (501) staff       (20)     2294 2023-08-02 08:55:03.637843 kaydet-0.8.4/PKG-INFO
+-rw-r--r--   0 mirat      (501) staff       (20)     1367 2023-08-02 08:54:21.000000 kaydet-0.8.4/README.md
+-rw-r--r--   0 mirat      (501) staff       (20)       38 2023-08-02 08:55:03.637999 kaydet-0.8.4/setup.cfg
+-rw-r--r--   0 mirat      (501) staff       (20)     1106 2023-08-02 08:52:52.000000 kaydet-0.8.4/setup.py
+drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:55:03.637102 kaydet-0.8.4/src/
+-rw-r--r--   0 mirat      (501) staff       (20)        0 2023-08-02 07:27:04.000000 kaydet-0.8.4/src/__init__.py
+drwxr-xr-x   0 mirat      (501) staff       (20)        0 2023-08-02 08:55:03.637684 kaydet-0.8.4/src/kaydet.egg-info/
+-rw-r--r--   0 mirat      (501) staff       (20)     2294 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/PKG-INFO
+-rw-r--r--   0 mirat      (501) staff       (20)      229 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/SOURCES.txt
+-rw-r--r--   0 mirat      (501) staff       (20)        1 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/dependency_links.txt
+-rw-r--r--   0 mirat      (501) staff       (20)       39 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/entry_points.txt
+-rw-r--r--   0 mirat      (501) staff       (20)       16 2023-08-02 08:55:03.000000 kaydet-0.8.4/src/kaydet.egg-info/top_level.txt
+-rwxr-xr-x   0 mirat      (501) staff       (20)     3398 2023-08-02 08:54:45.000000 kaydet-0.8.4/src/kaydet.py
```

### Comparing `kaydet-0.8.3/LICENSE` & `kaydet-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `kaydet-0.8.3/PKG-INFO` & `kaydet-0.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaydet
-Version: 0.8.3
+Version: 0.8.4
 Summary: ('Simple and terminal-based personal diary app designed to help you preserve your daily thoughts, experiences, and memories.',)
 Home-page: https://github.com/miratcan/logme
 Author: Mirat Can Bayrak
 License: MIT
 Keywords: diary tui
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 Classifier: Topic :: Utilities
 Classifier: Topic :: Utilities
 Classifier: Topic :: Utilities
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Kaydet- Your Personal Terminal Diary
+# Kaydet is Your Personal Terminal Diary
 
 "kaydet" is a simple (112 lines if Python code) based diary app designed to
 help you preserve your daily thoughts, experiences, and memories without 
 leaving terminal.
 
 # Key Features:
```

### Comparing `kaydet-0.8.3/README.md` & `kaydet-0.8.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Kaydet- Your Personal Terminal Diary
+# Kaydet is Your Personal Terminal Diary
 
 "kaydet" is a simple (112 lines if Python code) based diary app designed to
 help you preserve your daily thoughts, experiences, and memories without 
 leaving terminal.
 
 # Key Features:
```

### Comparing `kaydet-0.8.3/setup.py` & `kaydet-0.8.4/setup.py`

 * *Files identical despite different names*

### Comparing `kaydet-0.8.3/src/kaydet.egg-info/PKG-INFO` & `kaydet-0.8.4/src/kaydet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaydet
-Version: 0.8.3
+Version: 0.8.4
 Summary: ('Simple and terminal-based personal diary app designed to help you preserve your daily thoughts, experiences, and memories.',)
 Home-page: https://github.com/miratcan/logme
 Author: Mirat Can Bayrak
 License: MIT
 Keywords: diary tui
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 Classifier: Topic :: Utilities
 Classifier: Topic :: Utilities
 Classifier: Topic :: Utilities
 Requires-Python: >=3.4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Kaydet- Your Personal Terminal Diary
+# Kaydet is Your Personal Terminal Diary
 
 "kaydet" is a simple (112 lines if Python code) based diary app designed to
 help you preserve your daily thoughts, experiences, and memories without 
 leaving terminal.
 
 # Key Features:
```

### Comparing `kaydet-0.8.3/src/kaydet.py` & `kaydet-0.8.4/src/kaydet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __author__ = "Mirat Can Bayrak"
 __copyright__ = "Copyright 2016, Planet Earth"
-__version__ = "0.8.3"
+__version__ = "0.8.4"
 __description__ = "Simple and terminal-based personal diary app designed " \
                   "to help you preserve your daily thoughts, experiences, " \
                   "and memories.",
 
 
 from datetime import datetime
```


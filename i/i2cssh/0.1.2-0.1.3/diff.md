# Comparing `tmp/i2cssh-0.1.2.tar.gz` & `tmp/i2cssh-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cssh-0.1.2.tar", last modified: Wed Aug  2 12:47:25 2023, max compression
+gzip compressed data, was "i2cssh-0.1.3.tar", last modified: Wed Aug  2 13:41:13 2023, max compression
```

## Comparing `i2cssh-0.1.2.tar` & `i2cssh-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:47:25.408818 i2cssh-0.1.2/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.2/LICENSE.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.2/MANIFEST.in
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:47:25.408010 i2cssh-0.1.2/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.2/README.md
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 12:47:25.409578 i2cssh-0.1.2/setup.cfg
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1059 2023-08-02 12:46:20.000000 i2cssh-0.1.2/setup.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:47:25.377415 i2cssh-0.1.2/src/
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:47:25.380406 i2cssh-0.1.2/src/i2cssh/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.2/src/i2cssh/__init__.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24134 2023-08-02 09:36:27.000000 i2cssh-0.1.2/src/i2cssh/lib.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:47:25.399138 i2cssh-0.1.2/src/i2cssh/tests/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.2/src/i2cssh/tests/__init__.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    23978 2023-08-02 09:50:11.000000 i2cssh-0.1.2/src/i2cssh/tests/test_i2cssh.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:47:25.393432 i2cssh-0.1.2/src/i2cssh.egg-info/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:47:25.000000 i2cssh-0.1.2/src/i2cssh.egg-info/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      373 2023-08-02 12:47:25.000000 i2cssh-0.1.2/src/i2cssh.egg-info/SOURCES.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 12:47:25.000000 i2cssh-0.1.2/src/i2cssh.egg-info/dependency_links.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       40 2023-08-02 12:47:25.000000 i2cssh-0.1.2/src/i2cssh.egg-info/entry_points.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 12:47:25.000000 i2cssh-0.1.2/src/i2cssh.egg-info/requires.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       12 2023-08-02 12:47:25.000000 i2cssh-0.1.2/src/i2cssh.egg-info/top_level.txt
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.2/src/main.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 12:46:57.000000 i2cssh-0.1.2/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.444801 i2cssh-0.1.3/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.3/LICENSE.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       13 2023-08-02 12:46:30.000000 i2cssh-0.1.3/MANIFEST.in
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 13:41:13.444156 i2cssh-0.1.3/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.3/README.md
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 13:41:13.445097 i2cssh-0.1.3/setup.cfg
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1067 2023-08-02 13:38:22.000000 i2cssh-0.1.3/setup.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.423007 i2cssh-0.1.3/src/
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.435063 i2cssh-0.1.3/src/i2cssh/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.3/src/i2cssh/__init__.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24141 2023-08-02 13:00:29.000000 i2cssh-0.1.3/src/i2cssh/lib.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      132 2023-08-02 12:43:08.000000 i2cssh-0.1.3/src/i2cssh/main.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.442199 i2cssh-0.1.3/src/i2cssh/tests/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.3/src/i2cssh/tests/__init__.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    23978 2023-08-02 09:50:11.000000 i2cssh-0.1.3/src/i2cssh/tests/test_i2cssh.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 13:39:20.000000 i2cssh-0.1.3/src/i2cssh/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 13:41:13.440528 i2cssh-0.1.3/src/i2cssh.egg-info/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      391 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       37 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/entry_points.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/requires.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        7 2023-08-02 13:41:13.000000 i2cssh-0.1.3/src/i2cssh.egg-info/top_level.txt
```

### Comparing `i2cssh-0.1.2/LICENSE.txt` & `i2cssh-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.2/PKG-INFO` & `i2cssh-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.2
+Version: 0.1.3
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.1.2/README.md` & `i2cssh-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.2/setup.py` & `i2cssh-0.1.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #! /usr/bin/env python3
 # -*- coding: utf-8 -*-
 from setuptools import setup
-from version import version
+from src.i2cssh.version import version
 
 
 setup(
     name="i2cssh",
     version=version(),
     author="Wouter de Bie",
     author_email="wouter@evenflow.nl",
     description="csshX like ssh tool for iTerm2",
     url="http://github.com/wouterdebie/i2cssh",
-    entry_points={"console_scripts": ["i2cssh=main.py:main"]},
+    entry_points={"console_scripts": ["i2cssh=main:main"]},
     license="MIT",
     keywords="ssh i2cssh csshX".split(),
     classifiers=[
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `i2cssh-0.1.2/src/i2cssh/lib.py` & `i2cssh-0.1.3/src/i2cssh/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import iterm2
 import yaml
 from click_option_group import MutuallyExclusiveOptionGroup, optgroup
 from iterm2 import Session
 from iterm2.color import Color
 from iterm2.profile import LocalWriteOnlyProfile
 
-from version import version
+from i2cssh.version import version
 
 
 @click.command()
 @optgroup.group("General options")
 @optgroup.option(
     "--clusters",
     "-c",
```

### Comparing `i2cssh-0.1.2/src/i2cssh/tests/test_i2cssh.py` & `i2cssh-0.1.3/src/i2cssh/tests/test_i2cssh.py`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.2/src/i2cssh.egg-info/PKG-INFO` & `i2cssh-0.1.3/src/i2cssh.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.2
+Version: 0.1.3
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```


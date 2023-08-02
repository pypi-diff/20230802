# Comparing `tmp/i2cssh-0.1.0.tar.gz` & `tmp/i2cssh-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "i2cssh-0.1.0.tar", last modified: Wed Aug  2 12:27:12 2023, max compression
+gzip compressed data, was "i2cssh-0.1.1.tar", last modified: Wed Aug  2 12:34:05 2023, max compression
```

## Comparing `i2cssh-0.1.0.tar` & `i2cssh-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.493567 i2cssh-0.1.0/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.0/LICENSE.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       32 2023-08-02 09:52:37.000000 i2cssh-0.1.0/MANIFEST.in
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:27:12.493083 i2cssh-0.1.0/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.0/README.md
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 12:27:12.493767 i2cssh-0.1.0/setup.cfg
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1024 2023-08-02 08:54:25.000000 i2cssh-0.1.0/setup.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.475193 i2cssh-0.1.0/src/
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.484842 i2cssh-0.1.0/src/i2cssh/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.0/src/i2cssh/__init__.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24134 2023-08-02 09:36:27.000000 i2cssh-0.1.0/src/i2cssh/lib.py
--rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      125 2023-07-31 14:19:43.000000 i2cssh-0.1.0/src/i2cssh/main.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.491386 i2cssh-0.1.0/src/i2cssh/tests/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.0/src/i2cssh/tests/__init__.py
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)    23978 2023-08-02 09:50:11.000000 i2cssh-0.1.0/src/i2cssh/tests/test_i2cssh.py
-drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:27:12.489809 i2cssh-0.1.0/src/i2cssh.egg-info/
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/PKG-INFO
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)      343 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/SOURCES.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/dependency_links.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/requires.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       11 2023-08-02 12:27:12.000000 i2cssh-0.1.0/src/i2cssh.egg-info/top_level.txt
--rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 09:53:53.000000 i2cssh-0.1.0/version.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:34:05.222259 i2cssh-0.1.1/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1057 2019-08-06 15:05:32.000000 i2cssh-0.1.1/LICENSE.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       32 2023-08-02 09:52:37.000000 i2cssh-0.1.1/MANIFEST.in
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:34:05.217324 i2cssh-0.1.1/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    13819 2023-07-31 18:43:06.000000 i2cssh-0.1.1/README.md
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       38 2023-08-02 12:34:05.222698 i2cssh-0.1.1/setup.cfg
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)     1028 2023-08-02 12:30:35.000000 i2cssh-0.1.1/setup.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:34:05.189103 i2cssh-0.1.1/src/
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:34:05.196117 i2cssh-0.1.1/src/bin/
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)       75 2023-07-31 13:43:27.000000 i2cssh-0.1.1/src/bin/i2cssh
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:34:05.199777 i2cssh-0.1.1/src/i2cssh/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:52:02.000000 i2cssh-0.1.1/src/i2cssh/__init__.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)    24134 2023-08-02 09:36:27.000000 i2cssh-0.1.1/src/i2cssh/lib.py
+-rwxr-xr-x   0 wouter.de.bie   (501) staff       (20)      125 2023-07-31 14:19:43.000000 i2cssh-0.1.1/src/i2cssh/main.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:34:05.214965 i2cssh-0.1.1/src/i2cssh/tests/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        0 2023-07-31 13:44:05.000000 i2cssh-0.1.1/src/i2cssh/tests/__init__.py
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)    23978 2023-08-02 09:50:11.000000 i2cssh-0.1.1/src/i2cssh/tests/test_i2cssh.py
+drwxr-xr-x   0 wouter.de.bie   (501) staff       (20)        0 2023-08-02 12:34:05.212945 i2cssh-0.1.1/src/i2cssh.egg-info/
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      711 2023-08-02 12:34:05.000000 i2cssh-0.1.1/src/i2cssh.egg-info/PKG-INFO
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)      358 2023-08-02 12:34:05.000000 i2cssh-0.1.1/src/i2cssh.egg-info/SOURCES.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)        1 2023-08-02 12:34:05.000000 i2cssh-0.1.1/src/i2cssh.egg-info/dependency_links.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       65 2023-08-02 12:34:05.000000 i2cssh-0.1.1/src/i2cssh.egg-info/requires.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       11 2023-08-02 12:34:05.000000 i2cssh-0.1.1/src/i2cssh.egg-info/top_level.txt
+-rw-r--r--   0 wouter.de.bie   (501) staff       (20)       34 2023-08-02 12:32:21.000000 i2cssh-0.1.1/version.py
```

### Comparing `i2cssh-0.1.0/LICENSE.txt` & `i2cssh-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.0/PKG-INFO` & `i2cssh-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.0
+Version: 0.1.1
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```

### Comparing `i2cssh-0.1.0/README.md` & `i2cssh-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.0/setup.py` & `i2cssh-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup(
     name="i2cssh",
     version=version(),
     author="Wouter de Bie",
     author_email="wouter@evenflow.nl",
     description="csshX like ssh tool for iTerm2",
     url="http://github.com/wouterdebie/i2cssh",
-    scripts=["bin/i2cssh"],
+    scripts=["src/bin/i2cssh"],
     license="MIT",
     keywords="ssh i2cssh csshX".split(),
     classifiers=[
         "Operating System :: MacOS",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
```

### Comparing `i2cssh-0.1.0/src/i2cssh/lib.py` & `i2cssh-0.1.1/src/i2cssh/lib.py`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.0/src/i2cssh/tests/test_i2cssh.py` & `i2cssh-0.1.1/src/i2cssh/tests/test_i2cssh.py`

 * *Files identical despite different names*

### Comparing `i2cssh-0.1.0/src/i2cssh.egg-info/PKG-INFO` & `i2cssh-0.1.1/src/i2cssh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: i2cssh
-Version: 0.1.0
+Version: 0.1.1
 Summary: csshX like ssh tool for iTerm2
 Home-page: http://github.com/wouterdebie/i2cssh
 Author: Wouter de Bie
 Author-email: wouter@evenflow.nl
 License: MIT
 Keywords: ssh,i2cssh,csshX
 Classifier: Operating System :: MacOS
```


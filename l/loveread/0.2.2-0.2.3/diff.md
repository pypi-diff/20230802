# Comparing `tmp/loveread-0.2.2.tar.gz` & `tmp/loveread-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loveread-0.2.2.tar", last modified: Wed Aug  2 20:13:03 2023, max compression
+gzip compressed data, was "loveread-0.2.3.tar", last modified: Wed Aug  2 20:16:31 2023, max compression
```

## Comparing `loveread-0.2.2.tar` & `loveread-0.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:13:03.390913 loveread-0.2.2/
--rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.2/LICENSE
--rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:13:03.390671 loveread-0.2.2/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      313 2023-08-02 20:04:30.000000 loveread-0.2.2/README.md
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:13:03.388485 loveread-0.2.2/loveread/
--rw-r--r--   0 shinsheel   (501) staff       (20)       22 2023-08-02 20:11:56.000000 loveread-0.2.2/loveread/__init__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)      271 2023-08-02 20:12:02.000000 loveread-0.2.2/loveread/__main__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.2/loveread/loveread.py
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:13:03.390066 loveread-0.2.2/loveread.egg-info/
--rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:13:03.000000 loveread-0.2.2/loveread.egg-info/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      217 2023-08-02 20:13:03.000000 loveread-0.2.2/loveread.egg-info/SOURCES.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 20:13:03.000000 loveread-0.2.2/loveread.egg-info/dependency_links.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 20:13:03.000000 loveread-0.2.2/loveread.egg-info/top_level.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 20:13:03.391144 loveread-0.2.2/setup.cfg
--rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 20:12:59.000000 loveread-0.2.2/setup.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:16:31.458116 loveread-0.2.3/
+-rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.3/LICENSE
+-rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:16:31.457946 loveread-0.2.3/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      313 2023-08-02 20:04:30.000000 loveread-0.2.3/README.md
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:16:31.456969 loveread-0.2.3/loveread/
+-rw-r--r--   0 shinsheel   (501) staff       (20)       17 2023-08-02 20:15:08.000000 loveread-0.2.3/loveread/__init__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)      266 2023-08-02 20:15:05.000000 loveread-0.2.3/loveread/__main__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.3/loveread/lib.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:16:31.457725 loveread-0.2.3/loveread.egg-info/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      212 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/SOURCES.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/dependency_links.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 20:16:31.000000 loveread-0.2.3/loveread.egg-info/top_level.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 20:16:31.458175 loveread-0.2.3/setup.cfg
+-rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 20:16:25.000000 loveread-0.2.3/setup.py
```

### Comparing `loveread-0.2.2/PKG-INFO` & `loveread-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.2
+Version: 0.2.3
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loveread-0.2.2/loveread/loveread.py` & `loveread-0.2.3/loveread/lib.py`

 * *Files identical despite different names*

### Comparing `loveread-0.2.2/loveread.egg-info/PKG-INFO` & `loveread-0.2.3/loveread.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loveread
-Version: 0.2.2
+Version: 0.2.3
 Summary: A brief description of your package
 Home-page: https://gitlab.com/wladgavrilov/loveread
 Author: Vlad Havrylov
 Author-email: wladgavrilov@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loveread-0.2.2/setup.py` & `loveread-0.2.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="loveread",
-    version="0.2.2",
+    version="0.2.3",
     author="Vlad Havrylov",
     author_email="wladgavrilov@gmail.com",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://gitlab.com/wladgavrilov/loveread",
     packages=['loveread'],
```


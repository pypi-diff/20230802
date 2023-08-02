# Comparing `tmp/loveread-0.2.tar.gz` & `tmp/loveread-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loveread-0.2.tar", last modified: Wed Aug  2 19:57:22 2023, max compression
+gzip compressed data, was "loveread-0.2.1.tar", last modified: Wed Aug  2 20:09:54 2023, max compression
```

## Comparing `loveread-0.2.tar` & `loveread-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 19:57:22.668636 loveread-0.2/
--rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2/LICENSE
--rw-r--r--   0 shinsheel   (501) staff       (20)     6636 2023-08-02 19:57:22.667510 loveread-0.2/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)     6175 2023-08-02 19:52:12.000000 loveread-0.2/README.md
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 19:57:22.665418 loveread-0.2/loveread/
--rw-r--r--   0 shinsheel   (501) staff       (20)      271 2023-08-02 19:47:35.000000 loveread-0.2/loveread/__init__.py
--rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2/loveread/loveread.py
-drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 19:57:22.666856 loveread-0.2/loveread.egg-info/
--rw-r--r--   0 shinsheel   (501) staff       (20)     6636 2023-08-02 19:57:22.000000 loveread-0.2/loveread.egg-info/PKG-INFO
--rw-r--r--   0 shinsheel   (501) staff       (20)      196 2023-08-02 19:57:22.000000 loveread-0.2/loveread.egg-info/SOURCES.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 19:57:22.000000 loveread-0.2/loveread.egg-info/dependency_links.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 19:57:22.000000 loveread-0.2/loveread.egg-info/top_level.txt
--rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 19:57:22.668748 loveread-0.2/setup.cfg
--rw-r--r--   0 shinsheel   (501) staff       (20)      594 2023-08-02 19:53:46.000000 loveread-0.2/setup.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:09:54.911196 loveread-0.2.1/
+-rw-r--r--   0 shinsheel   (501) staff       (20)        7 2023-08-02 19:55:40.000000 loveread-0.2.1/LICENSE
+-rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:09:54.910999 loveread-0.2.1/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      313 2023-08-02 20:04:30.000000 loveread-0.2.1/README.md
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:09:54.909882 loveread-0.2.1/loveread/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      271 2023-08-02 19:47:35.000000 loveread-0.2.1/loveread/__init__.py
+-rw-r--r--   0 shinsheel   (501) staff       (20)     1247 2023-08-02 19:48:30.000000 loveread-0.2.1/loveread/loveread.py
+drwxr-xr-x   0 shinsheel   (501) staff       (20)        0 2023-08-02 20:09:54.910773 loveread-0.2.1/loveread.egg-info/
+-rw-r--r--   0 shinsheel   (501) staff       (20)      777 2023-08-02 20:09:54.000000 loveread-0.2.1/loveread.egg-info/PKG-INFO
+-rw-r--r--   0 shinsheel   (501) staff       (20)      196 2023-08-02 20:09:54.000000 loveread-0.2.1/loveread.egg-info/SOURCES.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        1 2023-08-02 20:09:54.000000 loveread-0.2.1/loveread.egg-info/dependency_links.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)        9 2023-08-02 20:09:54.000000 loveread-0.2.1/loveread.egg-info/top_level.txt
+-rw-r--r--   0 shinsheel   (501) staff       (20)       38 2023-08-02 20:09:54.911257 loveread-0.2.1/setup.cfg
+-rw-r--r--   0 shinsheel   (501) staff       (20)      596 2023-08-02 20:09:52.000000 loveread-0.2.1/setup.py
```

### Comparing `loveread-0.2/loveread/loveread.py` & `loveread-0.2.1/loveread/loveread.py`

 * *Files identical despite different names*

### Comparing `loveread-0.2/setup.py` & `loveread-0.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="loveread",
-    version="0.2",
+    version="0.2.1",
     author="Vlad Havrylov",
     author_email="wladgavrilov@gmail.com",
     description="A brief description of your package",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://gitlab.com/wladgavrilov/loveread",
     packages=['loveread'],
```


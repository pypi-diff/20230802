# Comparing `tmp/pythonGPT-0.5.tar.gz` & `tmp/pythonGPT-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonGPT-0.5.tar", last modified: Wed Aug  2 15:53:15 2023, max compression
+gzip compressed data, was "pythonGPT-0.6.tar", last modified: Wed Aug  2 16:06:22 2023, max compression
```

## Comparing `pythonGPT-0.5.tar` & `pythonGPT-0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:53:15.477638 pythonGPT-0.5/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:53:15.477337 pythonGPT-0.5/PKG-INFO
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:53:15.474780 pythonGPT-0.5/pythonGPT/
--rw-r--r--   0 gregorykestin   (504) staff       (20)     4197 2023-08-02 15:51:58.000000 pythonGPT-0.5/pythonGPT/__init__.py
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:53:15.476979 pythonGPT-0.5/pythonGPT.egg-info/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:53:15.000000 pythonGPT-0.5/pythonGPT.egg-info/PKG-INFO
--rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 15:53:15.000000 pythonGPT-0.5/pythonGPT.egg-info/SOURCES.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 15:53:15.000000 pythonGPT-0.5/pythonGPT.egg-info/dependency_links.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 15:53:15.000000 pythonGPT-0.5/pythonGPT.egg-info/requires.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 15:53:15.000000 pythonGPT-0.5/pythonGPT.egg-info/top_level.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 15:53:15.477719 pythonGPT-0.5/setup.cfg
--rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 15:52:10.000000 pythonGPT-0.5/setup.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:06:22.435041 pythonGPT-0.6/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:06:22.434765 pythonGPT-0.6/PKG-INFO
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:06:22.432647 pythonGPT-0.6/pythonGPT/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)     4261 2023-08-02 16:05:41.000000 pythonGPT-0.6/pythonGPT/__init__.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:06:22.434390 pythonGPT-0.6/pythonGPT.egg-info/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:06:22.000000 pythonGPT-0.6/pythonGPT.egg-info/PKG-INFO
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 16:06:22.000000 pythonGPT-0.6/pythonGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 16:06:22.000000 pythonGPT-0.6/pythonGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 16:06:22.000000 pythonGPT-0.6/pythonGPT.egg-info/requires.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 16:06:22.000000 pythonGPT-0.6/pythonGPT.egg-info/top_level.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 16:06:22.435134 pythonGPT-0.6/setup.cfg
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 16:05:54.000000 pythonGPT-0.6/setup.py
```

### Comparing `pythonGPT-0.5/pythonGPT/__init__.py` & `pythonGPT-0.6/pythonGPT/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from IPython.display import display, Markdown
 from time import sleep
 
 #####security######
 import os
 import hashlib
 
-HASHED_ACCESS_CODE = hashlib.sha256(os.environ['PYTHON_GPT_ACCESS_CODE'].encode()).hexdigest()
+HASHED_ACCESS_CODE = hashlib.sha256(os.environ.get('PYTHON_GPT_ACCESS_CODE', '').encode()).hexdigest()
 initialized = False
 
 def initialize(user_code):
     global initialized
     hashed_user_code = hashlib.sha256(user_code.encode()).hexdigest()
-    if hashed_user_code != HASHED_ACCESS_CODE:
+    if hashed_user_code != HASHED_ACCESS_CODE or HASHED_ACCESS_CODE == hashlib.sha256('').hexdigest():
         raise PermissionError("Invalid access code!")
     initialized = True
 
 def _ensure_initialized():
     if not initialized:
         raise PermissionError("Module not initialized. Call `initialize()` with the access code first.")
 #####security######
```


# Comparing `tmp/pythonGPT-0.7.tar.gz` & `tmp/pythonGPT-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonGPT-0.7.tar", last modified: Wed Aug  2 16:24:43 2023, max compression
+gzip compressed data, was "pythonGPT-0.8.tar", last modified: Wed Aug  2 16:33:50 2023, max compression
```

## Comparing `pythonGPT-0.7.tar` & `pythonGPT-0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:24:43.382986 pythonGPT-0.7/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:24:43.382715 pythonGPT-0.7/PKG-INFO
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:24:43.359464 pythonGPT-0.7/pythonGPT/
--rw-r--r--   0 gregorykestin   (504) staff       (20)     4246 2023-08-02 16:23:52.000000 pythonGPT-0.7/pythonGPT/__init__.py
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:24:43.382347 pythonGPT-0.7/pythonGPT.egg-info/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:24:43.000000 pythonGPT-0.7/pythonGPT.egg-info/PKG-INFO
--rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 16:24:43.000000 pythonGPT-0.7/pythonGPT.egg-info/SOURCES.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 16:24:43.000000 pythonGPT-0.7/pythonGPT.egg-info/dependency_links.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 16:24:43.000000 pythonGPT-0.7/pythonGPT.egg-info/requires.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 16:24:43.000000 pythonGPT-0.7/pythonGPT.egg-info/top_level.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 16:24:43.383071 pythonGPT-0.7/setup.cfg
--rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 16:24:26.000000 pythonGPT-0.7/setup.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:33:50.379628 pythonGPT-0.8/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:33:50.379385 pythonGPT-0.8/PKG-INFO
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:33:50.377664 pythonGPT-0.8/pythonGPT/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)     4446 2023-08-02 16:33:39.000000 pythonGPT-0.8/pythonGPT/__init__.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:33:50.379047 pythonGPT-0.8/pythonGPT.egg-info/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/PKG-INFO
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/requires.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/top_level.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 16:33:50.379704 pythonGPT-0.8/setup.cfg
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 16:33:44.000000 pythonGPT-0.8/setup.py
```

### Comparing `pythonGPT-0.7/pythonGPT/__init__.py` & `pythonGPT-0.8/pythonGPT/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,16 +11,21 @@
 
 HASHED_ACCESS_CODE = "d99fb34fb491c5431038d8690b4ab83b0a4ec4fa40bcff872f0790261e0e752c"
 initialized = False
 
 def initialize(user_code):
     global initialized
     hashed_user_code = hashlib.sha256(user_code.encode()).hexdigest()
-    if hashed_user_code != HASHED_ACCESS_CODE or HASHED_ACCESS_CODE == hashlib.sha256('').hexdigest():
+    empty_hash = hashlib.sha256('').hexdigest()
+    print(f"User Hash: {hashed_user_code}")
+    print(f"Stored Hash: {HASHED_ACCESS_CODE}")
+    if hashed_user_code != HASHED_ACCESS_CODE:
         raise PermissionError("Invalid access code!")
+    if HASHED_ACCESS_CODE == empty_hash:
+        raise PermissionError("Access code was not properly initialized!")
     initialized = True
 
 def _ensure_initialized():
     if not initialized:
         raise PermissionError("Module not initialized. Call `initialize()` with the access code first.")
 #####security######
```


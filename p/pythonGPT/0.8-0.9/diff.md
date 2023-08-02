# Comparing `tmp/pythonGPT-0.8.tar.gz` & `tmp/pythonGPT-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonGPT-0.8.tar", last modified: Wed Aug  2 16:33:50 2023, max compression
+gzip compressed data, was "pythonGPT-0.9.tar", last modified: Wed Aug  2 16:37:21 2023, max compression
```

## Comparing `pythonGPT-0.8.tar` & `pythonGPT-0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:33:50.379628 pythonGPT-0.8/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:33:50.379385 pythonGPT-0.8/PKG-INFO
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:33:50.377664 pythonGPT-0.8/pythonGPT/
--rw-r--r--   0 gregorykestin   (504) staff       (20)     4446 2023-08-02 16:33:39.000000 pythonGPT-0.8/pythonGPT/__init__.py
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:33:50.379047 pythonGPT-0.8/pythonGPT.egg-info/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/PKG-INFO
--rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/SOURCES.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/dependency_links.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/requires.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 16:33:50.000000 pythonGPT-0.8/pythonGPT.egg-info/top_level.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 16:33:50.379704 pythonGPT-0.8/setup.cfg
--rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 16:33:44.000000 pythonGPT-0.8/setup.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:37:21.102286 pythonGPT-0.9/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:37:21.102005 pythonGPT-0.9/PKG-INFO
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:37:21.099846 pythonGPT-0.9/pythonGPT/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)     4363 2023-08-02 16:37:09.000000 pythonGPT-0.9/pythonGPT/__init__.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 16:37:21.101601 pythonGPT-0.9/pythonGPT.egg-info/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 16:37:21.000000 pythonGPT-0.9/pythonGPT.egg-info/PKG-INFO
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 16:37:21.000000 pythonGPT-0.9/pythonGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 16:37:21.000000 pythonGPT-0.9/pythonGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 16:37:21.000000 pythonGPT-0.9/pythonGPT.egg-info/requires.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 16:37:21.000000 pythonGPT-0.9/pythonGPT.egg-info/top_level.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 16:37:21.102382 pythonGPT-0.9/setup.cfg
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 16:37:16.000000 pythonGPT-0.9/setup.py
```

### Comparing `pythonGPT-0.8/pythonGPT/__init__.py` & `pythonGPT-0.9/pythonGPT/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 
 HASHED_ACCESS_CODE = "d99fb34fb491c5431038d8690b4ab83b0a4ec4fa40bcff872f0790261e0e752c"
 initialized = False
 
 def initialize(user_code):
     global initialized
     hashed_user_code = hashlib.sha256(user_code.encode()).hexdigest()
-    empty_hash = hashlib.sha256('').hexdigest()
-    print(f"User Hash: {hashed_user_code}")
-    print(f"Stored Hash: {HASHED_ACCESS_CODE}")
+    empty_hash = hashlib.sha256(''.encode()).hexdigest()
     if hashed_user_code != HASHED_ACCESS_CODE:
         raise PermissionError("Invalid access code!")
     if HASHED_ACCESS_CODE == empty_hash:
         raise PermissionError("Access code was not properly initialized!")
     initialized = True
 
 def _ensure_initialized():
```


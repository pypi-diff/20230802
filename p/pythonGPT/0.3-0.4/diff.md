# Comparing `tmp/pythonGPT-0.3.tar.gz` & `tmp/pythonGPT-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonGPT-0.3.tar", last modified: Wed Aug  2 15:02:50 2023, max compression
+gzip compressed data, was "pythonGPT-0.4.tar", last modified: Wed Aug  2 15:25:50 2023, max compression
```

## Comparing `pythonGPT-0.3.tar` & `pythonGPT-0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:02:50.034134 pythonGPT-0.3/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:02:50.033907 pythonGPT-0.3/PKG-INFO
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:02:50.031894 pythonGPT-0.3/pythonGPT/
--rw-r--r--   0 gregorykestin   (504) staff       (20)     3530 2023-08-02 15:01:11.000000 pythonGPT-0.3/pythonGPT/__init__.py
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:02:50.033475 pythonGPT-0.3/pythonGPT.egg-info/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/PKG-INFO
--rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/SOURCES.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/dependency_links.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/requires.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/top_level.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 15:02:50.034214 pythonGPT-0.3/setup.cfg
--rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 15:01:11.000000 pythonGPT-0.3/setup.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:25:50.232204 pythonGPT-0.4/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:25:50.231879 pythonGPT-0.4/PKG-INFO
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:25:50.229229 pythonGPT-0.4/pythonGPT/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)     4023 2023-08-02 15:25:13.000000 pythonGPT-0.4/pythonGPT/__init__.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:25:50.231493 pythonGPT-0.4/pythonGPT.egg-info/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:25:50.000000 pythonGPT-0.4/pythonGPT.egg-info/PKG-INFO
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 15:25:50.000000 pythonGPT-0.4/pythonGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 15:25:50.000000 pythonGPT-0.4/pythonGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 15:25:50.000000 pythonGPT-0.4/pythonGPT.egg-info/requires.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 15:25:50.000000 pythonGPT-0.4/pythonGPT.egg-info/top_level.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 15:25:50.232298 pythonGPT-0.4/setup.cfg
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 15:25:13.000000 pythonGPT-0.4/setup.py
```

### Comparing `pythonGPT-0.3/pythonGPT/__init__.py` & `pythonGPT-0.4/pythonGPT/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 # Below is version 1 of the client side pythonGPT code, which isn't optimized, but should hopefully serve as a proof of principle.
 
 import IPython
 import requests
 from IPython.display import display, Markdown
 from time import sleep
 
+#####security######
+ACCESS_CODE = "python@future!"
+initialized = False
+
+def initialize(user_code):
+    global initialized
+    if user_code != ACCESS_CODE:
+        raise PermissionError("Invalid access code!")
+    initialized = True
+
+def _ensure_initialized():
+    if not initialized:
+        raise PermissionError("Module not initialized. Call `initialize()` with the access code first.")
+#####security######
+
 current_cell_has_delayed_output = False  # Initialize the variable b/c it's used in two defs
 
 BASE_URL = 'https://pythongpt-de5fb0514677.herokuapp.com'
 ip = IPython.get_ipython()
 
 history = []
 
 
 def ask_gpt4(prompt):
+    _ensure_initialized()  # Make sure the module is initialized before proceeding
     try:
         # Initiate the request
         response = requests.post(f'{BASE_URL}/gpt-4', json={"prompt": prompt, "history": history})
         #print("HISTORY: " + str(history))
         response.raise_for_status()  # Check for HTTP errors.
         response_json = response.json()
```


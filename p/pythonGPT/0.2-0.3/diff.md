# Comparing `tmp/pythonGPT-0.2.tar.gz` & `tmp/pythonGPT-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pythonGPT-0.2.tar", last modified: Wed Aug  2 14:56:14 2023, max compression
+gzip compressed data, was "pythonGPT-0.3.tar", last modified: Wed Aug  2 15:02:50 2023, max compression
```

## Comparing `pythonGPT-0.2.tar` & `pythonGPT-0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 14:56:14.174451 pythonGPT-0.2/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 14:56:14.174150 pythonGPT-0.2/PKG-INFO
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 14:56:14.172021 pythonGPT-0.2/pythonGPT/
--rw-r--r--   0 gregorykestin   (504) staff       (20)     3529 2023-08-02 14:21:13.000000 pythonGPT-0.2/pythonGPT/__init__.py
-drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 14:56:14.173792 pythonGPT-0.2/pythonGPT.egg-info/
--rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 14:56:14.000000 pythonGPT-0.2/pythonGPT.egg-info/PKG-INFO
--rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 14:56:14.000000 pythonGPT-0.2/pythonGPT.egg-info/SOURCES.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 14:56:14.000000 pythonGPT-0.2/pythonGPT.egg-info/dependency_links.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 14:56:14.000000 pythonGPT-0.2/pythonGPT.egg-info/requires.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 14:56:14.000000 pythonGPT-0.2/pythonGPT.egg-info/top_level.txt
--rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 14:56:14.174529 pythonGPT-0.2/setup.cfg
--rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 14:53:40.000000 pythonGPT-0.2/setup.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:02:50.034134 pythonGPT-0.3/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:02:50.033907 pythonGPT-0.3/PKG-INFO
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:02:50.031894 pythonGPT-0.3/pythonGPT/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)     3530 2023-08-02 15:01:11.000000 pythonGPT-0.3/pythonGPT/__init__.py
+drwxr-xr-x   0 gregorykestin   (504) staff       (20)        0 2023-08-02 15:02:50.033475 pythonGPT-0.3/pythonGPT.egg-info/
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       51 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/PKG-INFO
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      194 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)        1 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       17 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/requires.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       10 2023-08-02 15:02:49.000000 pythonGPT-0.3/pythonGPT.egg-info/top_level.txt
+-rw-r--r--   0 gregorykestin   (504) staff       (20)       38 2023-08-02 15:02:50.034214 pythonGPT-0.3/setup.cfg
+-rw-r--r--   0 gregorykestin   (504) staff       (20)      192 2023-08-02 15:01:11.000000 pythonGPT-0.3/setup.py
```

### Comparing `pythonGPT-0.2/pythonGPT/__init__.py` & `pythonGPT-0.3/pythonGPT/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 history = []
 
 
 def ask_gpt4(prompt):
     try:
         # Initiate the request
         response = requests.post(f'{BASE_URL}/gpt-4', json={"prompt": prompt, "history": history})
-        print("HISTORY: " + str(history))
+        #print("HISTORY: " + str(history))
         response.raise_for_status()  # Check for HTTP errors.
         response_json = response.json()
 
         # Wait for the response from the threaded function
         while True:
             check_response = requests.get(f'{BASE_URL}/get-response/{response_json["id"]}')
             if check_response.json()["status"] == "completed":
```


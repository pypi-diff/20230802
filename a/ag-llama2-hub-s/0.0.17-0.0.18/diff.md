# Comparing `tmp/ag_llama2_hub_s-0.0.17.tar.gz` & `tmp/ag_llama2_hub_s-0.0.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama2_hub_s-0.0.17.tar", last modified: Wed Aug  2 10:47:26 2023, max compression
+gzip compressed data, was "dist\ag_llama2_hub_s-0.0.18.tar", last modified: Wed Aug  2 10:58:11 2023, max compression
```

## Comparing `ag_llama2_hub_s-0.0.17.tar` & `ag_llama2_hub_s-0.0.18.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.767189 ag_llama2_hub_s-0.0.17/
--rw-rw-rw-   0        0        0      837 2023-08-02 10:47:26.765055 ag_llama2_hub_s-0.0.17/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.751093 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/
--rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__init__.py
--rw-rw-rw-   0        0        0     3683 2023-08-02 10:47:01.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__main__.py
--rw-rw-rw-   0        0        0     5492 2023-08-02 08:40:31.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/model.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.759072 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/
--rw-rw-rw-   0        0        0      837 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 10:47:26.767189 ag_llama2_hub_s-0.0.17/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.17/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.763062 ag_llama2_hub_s-0.0.17/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.17/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.17/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.979029 ag_llama2_hub_s-0.0.18/
+-rw-rw-rw-   0        0        0      837 2023-08-02 10:58:11.977934 ag_llama2_hub_s-0.0.18/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.962964 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/
+-rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__init__.py
+-rw-rw-rw-   0        0        0     3677 2023-08-02 10:58:07.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__main__.py
+-rw-rw-rw-   0        0        0     5492 2023-08-02 08:40:31.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/model.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.971940 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:58:11.979029 ag_llama2_hub_s-0.0.18/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.975929 ag_llama2_hub_s-0.0.18/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.18/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.18/utils/render.py
```

### Comparing `ag_llama2_hub_s-0.0.17/PKG-INFO` & `ag_llama2_hub_s-0.0.18/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama2_hub_s
-Version: 0.0.17
+Version: 0.0.18
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__init__.py` & `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__main__.py` & `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
 # Load the language model to be served.
 stream_model = None
 def load_stream_model(model=MODEL,load_in_8bit=MODEL_LOAD_IN_8BIT):
     global stream_model
     logger.info(f"Loading model {MODEL} in 8bit: {load_in_8bit}")
     stream_model = load_model(
-        name_or_path=MODEL,
-        load_in_8bit=MODEL_LOAD_IN_8BIT,
+        name_or_path=model,
+        load_in_8bit=load_in_8bit,
         load_in_4bit=MODEL_LOAD_IN_4BIT,
     )
     logger.info(f"Model {MODEL} finished loading")
 
 # schema = {
 #         "prompt": str,
 #         "min_tokens": int,
```

### Comparing `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/model.py` & `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/PKG-INFO` & `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama2-hub-s
-Version: 0.0.17
+Version: 0.0.18
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.17/setup.py` & `ag_llama2_hub_s-0.0.18/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.17/utils/download.py` & `ag_llama2_hub_s-0.0.18/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.17/utils/render.py` & `ag_llama2_hub_s-0.0.18/utils/render.py`

 * *Files identical despite different names*


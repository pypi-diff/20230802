# Comparing `tmp/ag_llama2_hub_s-0.0.15.tar.gz` & `tmp/ag_llama2_hub_s-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama2_hub_s-0.0.15.tar", last modified: Tue Aug  1 15:48:52 2023, max compression
+gzip compressed data, was "dist\ag_llama2_hub_s-0.0.16.tar", last modified: Wed Aug  2 08:40:41 2023, max compression
```

## Comparing `ag_llama2_hub_s-0.0.15.tar` & `ag_llama2_hub_s-0.0.16.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 15:48:52.885789 ag_llama2_hub_s-0.0.15/
--rw-rw-rw-   0        0        0      837 2023-08-01 15:48:52.884819 ag_llama2_hub_s-0.0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 15:48:52.868551 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/
--rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-07-30 09:17:59.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/__main__.py
--rw-rw-rw-   0        0        0     5441 2023-08-01 15:48:09.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/model.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:48:52.878601 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/
--rw-rw-rw-   0        0        0      837 2023-08-01 15:48:52.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-08-01 15:48:52.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 15:48:52.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-08-01 15:48:52.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-01 15:48:52.000000 ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 15:48:52.885789 ag_llama2_hub_s-0.0.15/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.15/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 15:48:52.882846 ag_llama2_hub_s-0.0.15/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.15/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.15/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.114855 ag_llama2_hub_s-0.0.16/
+-rw-rw-rw-   0        0        0      837 2023-08-02 08:40:41.113882 ag_llama2_hub_s-0.0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.098897 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/
+-rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__init__.py
+-rw-rw-rw-   0        0        0     3643 2023-07-30 09:17:59.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__main__.py
+-rw-rw-rw-   0        0        0     5492 2023-08-02 08:40:31.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/model.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.107874 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:40:41.114855 ag_llama2_hub_s-0.0.16/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.16/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.111863 ag_llama2_hub_s-0.0.16/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.16/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.16/utils/render.py
```

### Comparing `ag_llama2_hub_s-0.0.15/PKG-INFO` & `ag_llama2_hub_s-0.0.16/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama2_hub_s
-Version: 0.0.15
+Version: 0.0.16
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/__init__.py` & `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/__main__.py` & `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.15/ag_llama2_hub_s/model.py` & `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def __init__(self, model, tokenizer,**kwargs):
         super().__init__()
         self.model = model
         self.tokenizer = tokenizer
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
         self.path=kwargs.get('path',None)
-        if self.path:
+        if self.path and os.path.exists(f"{self.path}/tokenizer.model"):
             self.s_tokenizer =SentencePieceProcessor(model_file=f"{self.path}/tokenizer.model")
 
     def __call__(
         self,
         prompt,
         max_tokens=16,
         temperature=1.0,
```

### Comparing `ag_llama2_hub_s-0.0.15/ag_llama2_hub_s.egg-info/PKG-INFO` & `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama2-hub-s
-Version: 0.0.15
+Version: 0.0.16
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.15/setup.py` & `ag_llama2_hub_s-0.0.16/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.15/utils/download.py` & `ag_llama2_hub_s-0.0.16/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.15/utils/render.py` & `ag_llama2_hub_s-0.0.16/utils/render.py`

 * *Files identical despite different names*


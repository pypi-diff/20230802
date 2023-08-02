# Comparing `tmp/ag_llama2_hub_s-0.0.18.tar.gz` & `tmp/ag_llama2_hub_s-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama2_hub_s-0.0.18.tar", last modified: Wed Aug  2 10:58:11 2023, max compression
+gzip compressed data, was "dist\ag_llama2_hub_s-0.0.19.tar", last modified: Wed Aug  2 11:22:59 2023, max compression
```

## Comparing `ag_llama2_hub_s-0.0.18.tar` & `ag_llama2_hub_s-0.0.19.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.979029 ag_llama2_hub_s-0.0.18/
--rw-rw-rw-   0        0        0      837 2023-08-02 10:58:11.977934 ag_llama2_hub_s-0.0.18/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.962964 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/
--rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__init__.py
--rw-rw-rw-   0        0        0     3677 2023-08-02 10:58:07.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__main__.py
--rw-rw-rw-   0        0        0     5492 2023-08-02 08:40:31.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/model.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.971940 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/
--rw-rw-rw-   0        0        0      837 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 10:58:11.000000 ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 10:58:11.979029 ag_llama2_hub_s-0.0.18/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.18/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:58:11.975929 ag_llama2_hub_s-0.0.18/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.18/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.18/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:22:59.279155 ag_llama2_hub_s-0.0.19/
+-rw-rw-rw-   0        0        0      837 2023-08-02 11:22:59.278158 ag_llama2_hub_s-0.0.19/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 11:22:59.262101 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/
+-rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/__init__.py
+-rw-rw-rw-   0        0        0     3677 2023-08-02 10:58:07.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/__main__.py
+-rw-rw-rw-   0        0        0     5522 2023-08-02 11:22:56.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/model.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:22:59.272174 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-08-02 11:22:59.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-08-02 11:22:59.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:22:59.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-08-02 11:22:59.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 11:22:59.000000 ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 11:22:59.280152 ag_llama2_hub_s-0.0.19/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:22:59.276163 ag_llama2_hub_s-0.0.19/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.19/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.19/utils/render.py
```

### Comparing `ag_llama2_hub_s-0.0.18/PKG-INFO` & `ag_llama2_hub_s-0.0.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag_llama2_hub_s
-Version: 0.0.18
+Version: 0.0.19
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__init__.py` & `ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/__main__.py` & `ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/__main__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s/model.py` & `ag_llama2_hub_s-0.0.19/ag_llama2_hub_s/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     def __init__(self, model, tokenizer,**kwargs):
         super().__init__()
         self.model = model
         self.tokenizer = tokenizer
         self.device = "cuda" if torch.cuda.is_available() else "cpu"
         self.path=kwargs.get('path',None)
+        self.s_tokenizer=None
         if self.path and os.path.exists(f"{self.path}/tokenizer.model"):
             self.s_tokenizer =SentencePieceProcessor(model_file=f"{self.path}/tokenizer.model")
 
     def __call__(
         self,
         prompt,
         max_tokens=16,
```

### Comparing `ag_llama2_hub_s-0.0.18/ag_llama2_hub_s.egg-info/PKG-INFO` & `ag_llama2_hub_s-0.0.19/ag_llama2_hub_s.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ag-llama2-hub-s
-Version: 0.0.18
+Version: 0.0.19
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.18/setup.py` & `ag_llama2_hub_s-0.0.19/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.18/utils/download.py` & `ag_llama2_hub_s-0.0.19/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.18/utils/render.py` & `ag_llama2_hub_s-0.0.19/utils/render.py`

 * *Files identical despite different names*


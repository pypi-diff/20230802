# Comparing `tmp/cybrex-1.1.8.tar.gz` & `tmp/cybrex-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cybrex-1.1.8.tar", last modified: Tue Aug  1 21:12:30 2023, max compression
+gzip compressed data, was "cybrex-1.1.9.tar", last modified: Wed Aug  2 08:54:10 2023, max compression
```

## Comparing `cybrex-1.1.8.tar` & `cybrex-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 21:12:30.302073 cybrex-1.1.8/
--rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.8/MANIFEST.in
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 21:12:30.301526 cybrex-1.1.8/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.8/README.md
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 21:12:30.298789 cybrex-1.1.8/cybrex/
--rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.8/cybrex/__init__.py
--rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 21:12:18.000000 cybrex-1.1.8/cybrex/cli.py
--rw-r--r--   0 pasha      (501) staff       (20)    11975 2023-08-01 21:12:18.000000 cybrex-1.1.8/cybrex/cybrex_ai.py
--rw-r--r--   0 pasha      (501) staff       (20)    13576 2023-08-01 19:57:40.000000 cybrex-1.1.8/cybrex/models.py
-drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-01 21:12:30.300902 cybrex-1.1.8/cybrex.egg-info/
--rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/PKG-INFO
--rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/SOURCES.txt
--rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/dependency_links.txt
--rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/entry_points.txt
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/requires.txt
--rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-01 21:12:30.000000 cybrex-1.1.8/cybrex.egg-info/top_level.txt
--rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-01 21:12:18.000000 cybrex-1.1.8/pyproject.toml
--rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.8/requirements.txt
--rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-01 21:12:30.302282 cybrex-1.1.8/setup.cfg
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 08:54:10.653321 cybrex-1.1.9/
+-rw-r--r--   0 pasha      (501) staff       (20)       24 2022-12-01 11:19:40.000000 cybrex-1.1.9/MANIFEST.in
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 08:54:10.652108 cybrex-1.1.9/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)    23862 2023-08-01 06:52:35.000000 cybrex-1.1.9/README.md
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 08:54:10.643014 cybrex-1.1.9/cybrex/
+-rw-r--r--   0 pasha      (501) staff       (20)        0 2023-07-12 12:59:05.000000 cybrex-1.1.9/cybrex/__init__.py
+-rw-r--r--   0 pasha      (501) staff       (20)     5637 2023-08-01 21:12:18.000000 cybrex-1.1.9/cybrex/cli.py
+-rw-r--r--   0 pasha      (501) staff       (20)    11975 2023-08-01 21:12:18.000000 cybrex-1.1.9/cybrex/cybrex_ai.py
+-rw-r--r--   0 pasha      (501) staff       (20)    13694 2023-08-02 08:53:55.000000 cybrex-1.1.9/cybrex/models.py
+drwxr-xr-x   0 pasha      (501) staff       (20)        0 2023-08-02 08:54:10.650039 cybrex-1.1.9/cybrex.egg-info/
+-rw-r--r--   0 pasha      (501) staff       (20)    24138 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/PKG-INFO
+-rw-r--r--   0 pasha      (501) staff       (20)      305 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/SOURCES.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        1 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/dependency_links.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       43 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/entry_points.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/requires.txt
+-rw-r--r--   0 pasha      (501) staff       (20)        7 2023-08-02 08:54:10.000000 cybrex-1.1.9/cybrex.egg-info/top_level.txt
+-rw-r--r--   0 pasha      (501) staff       (20)      531 2023-08-02 08:53:55.000000 cybrex-1.1.9/pyproject.toml
+-rw-r--r--   0 pasha      (501) staff       (20)      245 2023-08-01 20:22:19.000000 cybrex-1.1.9/requirements.txt
+-rw-r--r--   0 pasha      (501) staff       (20)       38 2023-08-02 08:54:10.653718 cybrex-1.1.9/setup.cfg
```

### Comparing `cybrex-1.1.8/PKG-INFO` & `cybrex-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.8
+Version: 1.1.9
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.8/README.md` & `cybrex-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.8/cybrex/cli.py` & `cybrex-1.1.9/cybrex/cli.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.8/cybrex/cybrex_ai.py` & `cybrex-1.1.9/cybrex/cybrex_ai.py`

 * *Files identical despite different names*

### Comparing `cybrex-1.1.8/cybrex/models.py` & `cybrex-1.1.9/cybrex/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import os
 from collections import OrderedDict
 from typing import List
 
 from ctransformers import AutoModelForCausalLM
 from keybert import KeyBERT
 from langchain import OpenAI
 from langchain.embeddings import HuggingFaceInstructEmbeddings, OpenAIEmbeddings
@@ -205,21 +206,24 @@
         else:
             raise ValueError("Unsupported embedding model")
 
     @lazy
     def llm(self):
         if self.config['llm']['model_type'] == 'llama':
             return LLM(
-                llm=AutoModelForCausalLM.from_pretrained(**self.config['llm']['config']),
+                llm=AutoModelForCausalLM.from_pretrained(
+                    **self.config['llm']['config'],
+                    cache_dir=os.environ.get('TRANSFORMERS_CACHE'),
+                ),
                 prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type'])
             )
         elif self.config['llm']['model_type'] == 'openai':
             return LLM(
                 llm=OpenAI(**self.config['llm']['config']),
-                prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type'])
+                prompter=BasePrompter.prompter_from_type(self.config['llm']['prompter']['type']),
             )
 
     def get_embeddings_id(self):
         text_splitter_id = f'{self.config["text_splitter"]["type"]}' \
                            f'-{self.config["text_splitter"]["chunk_size"]}' \
                            f'-{self.config["text_splitter"]["chunk_overlap"]}'
         embedder_id = self.config['embedder']['model_name'].replace('/', '-')
```

### Comparing `cybrex-1.1.8/cybrex.egg-info/PKG-INFO` & `cybrex-1.1.9/cybrex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cybrex
-Version: 1.1.8
+Version: 1.1.9
 Summary: Researching AI
 Author: Interdimensional Walker
 Project-URL: Homepage, https://github.com/nexus-stc/stc
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `cybrex-1.1.8/pyproject.toml` & `cybrex-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools<65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cybrex"
-version = "1.1.8"
+version = "1.1.9"
 authors = [{ name = "Interdimensional Walker" }]
 description = "Researching AI"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
```


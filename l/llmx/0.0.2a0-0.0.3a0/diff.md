# Comparing `tmp/llmx-0.0.2a0.tar.gz` & `tmp/llmx-0.0.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmx-0.0.2a0.tar", last modified: Sat Jul 29 02:18:55 2023, max compression
+gzip compressed data, was "llmx-0.0.3a0.tar", last modified: Wed Aug  2 21:25:29 2023, max compression
```

## Comparing `llmx-0.0.2a0.tar` & `llmx-0.0.3a0.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.249914 llmx-0.0.2a0/
--rw-r--r--   0 victordibia   (501) staff       (20)     3143 2023-07-28 03:18:55.000000 llmx-0.0.2a0/.gitignore
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-25 17:59:05.000000 llmx-0.0.2a0/MANIFEST.in
--rw-r--r--   0 victordibia   (501) staff       (20)     3590 2023-07-29 02:18:55.249470 llmx-0.0.2a0/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)     3058 2023-07-29 02:15:52.000000 llmx-0.0.2a0/README.md
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.177791 llmx-0.0.2a0/llmx/
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-28 02:07:41.000000 llmx-0.0.2a0/llmx/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     1322 2023-07-28 18:57:05.000000 llmx-0.0.2a0/llmx/datamodel.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.195789 llmx-0.0.2a0/llmx/generators/
--rw-r--r--   0 victordibia   (501) staff       (20)       40 2023-07-28 16:35:42.000000 llmx-0.0.2a0/llmx/generators/__init__.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.234660 llmx-0.0.2a0/llmx/generators/text/
--rw-r--r--   0 victordibia   (501) staff       (20)        0 2023-07-28 16:35:47.000000 llmx-0.0.2a0/llmx/generators/text/__init__.py
--rw-r--r--   0 victordibia   (501) staff       (20)     1080 2023-07-28 18:43:55.000000 llmx-0.0.2a0/llmx/generators/text/base_textgen.py
--rw-r--r--   0 victordibia   (501) staff       (20)     2777 2023-07-28 23:04:53.000000 llmx-0.0.2a0/llmx/generators/text/cohere_textgen.py
--rw-r--r--   0 victordibia   (501) staff       (20)     8804 2023-07-29 02:14:05.000000 llmx-0.0.2a0/llmx/generators/text/hf_textgen.py
--rw-r--r--   0 victordibia   (501) staff       (20)     2471 2023-07-28 18:44:52.000000 llmx-0.0.2a0/llmx/generators/text/openai_textgen.py
--rw-r--r--   0 victordibia   (501) staff       (20)     2990 2023-07-28 22:08:12.000000 llmx-0.0.2a0/llmx/generators/text/palm_textgen.py
--rw-r--r--   0 victordibia   (501) staff       (20)     1524 2023-07-28 23:03:28.000000 llmx-0.0.2a0/llmx/generators/text/textgen.py
--rw-r--r--   0 victordibia   (501) staff       (20)     2269 2023-07-28 18:51:21.000000 llmx-0.0.2a0/llmx/utils.py
--rw-r--r--   0 victordibia   (501) staff       (20)       37 2023-07-29 02:17:54.000000 llmx-0.0.2a0/llmx/version.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.192285 llmx-0.0.2a0/llmx.egg-info/
--rw-r--r--   0 victordibia   (501) staff       (20)     3590 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/PKG-INFO
--rw-r--r--   0 victordibia   (501) staff       (20)      621 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/SOURCES.txt
--rw-r--r--   0 victordibia   (501) staff       (20)        1 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/dependency_links.txt
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/entry_points.txt
--rw-r--r--   0 victordibia   (501) staff       (20)      120 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/requires.txt
--rw-r--r--   0 victordibia   (501) staff       (20)        5 2023-07-29 02:18:55.000000 llmx-0.0.2a0/llmx.egg-info/top_level.txt
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.243005 llmx-0.0.2a0/notebooks/
--rw-r--r--   0 victordibia   (501) staff       (20)     4324 2023-07-28 21:00:21.000000 llmx-0.0.2a0/notebooks/tutorial.ipynb
--rw-r--r--   0 victordibia   (501) staff       (20)     1385 2023-07-28 20:56:36.000000 llmx-0.0.2a0/pyproject.toml
--rw-r--r--   0 victordibia   (501) staff       (20)       38 2023-07-29 02:18:55.249998 llmx-0.0.2a0/setup.cfg
--rw-r--r--   0 victordibia   (501) staff       (20)       36 2023-07-25 17:59:05.000000 llmx-0.0.2a0/setup.py
-drwxr-xr-x   0 victordibia   (501) staff       (20)        0 2023-07-29 02:18:55.246690 llmx-0.0.2a0/tests/
--rw-r--r--   0 victordibia   (501) staff       (20)     1597 2023-07-28 23:01:30.000000 llmx-0.0.2a0/tests/test_generators.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3155 2023-08-02 21:22:10.000000 llmx-0.0.3a0/.gitignore
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       27 2023-08-02 21:17:22.000000 llmx-0.0.3a0/MANIFEST.in
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4944 2023-08-02 21:25:29.071923 llmx-0.0.3a0/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4405 2023-08-02 21:12:51.000000 llmx-0.0.3a0/README.md
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       52 2023-08-02 20:54:38.000000 llmx-0.0.3a0/llmx/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1286 2023-08-02 01:35:37.000000 llmx-0.0.3a0/llmx/datamodel.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx/generators/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       83 2023-08-02 20:55:20.000000 llmx-0.0.3a0/llmx/generators/__init__.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx/generators/text/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-02 20:54:42.000000 llmx-0.0.3a0/llmx/generators/text/__init__.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1024 2023-08-02 14:48:18.000000 llmx-0.0.3a0/llmx/generators/text/base_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2806 2023-08-02 19:51:36.000000 llmx-0.0.3a0/llmx/generators/text/cohere_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     8484 2023-08-02 21:08:19.000000 llmx-0.0.3a0/llmx/generators/text/hf_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2679 2023-08-02 20:14:24.000000 llmx-0.0.3a0/llmx/generators/text/openai_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     3188 2023-08-02 20:59:05.000000 llmx-0.0.3a0/llmx/generators/text/palm_textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1505 2023-08-02 20:54:21.000000 llmx-0.0.3a0/llmx/generators/text/textgen.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     2269 2023-08-01 22:45:11.000000 llmx-0.0.3a0/llmx/utils.py
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       37 2023-08-02 21:21:40.000000 llmx-0.0.3a0/llmx/version.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/llmx.egg-info/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     4944 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/PKG-INFO
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      662 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/SOURCES.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        1 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/dependency_links.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/entry_points.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      127 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/requires.txt
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        5 2023-08-02 21:25:29.000000 llmx-0.0.3a0/llmx.egg-info/top_level.txt
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/notebooks/
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/notebooks/research/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)      775 2023-08-01 22:45:11.000000 llmx-0.0.3a0/notebooks/research/travelbenchmark.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     5857 2023-08-02 21:14:31.000000 llmx-0.0.3a0/notebooks/tutorial.ipynb
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1392 2023-08-02 17:35:12.000000 llmx-0.0.3a0/pyproject.toml
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       38 2023-08-02 21:25:29.071923 llmx-0.0.3a0/setup.cfg
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)       36 2023-08-01 22:45:11.000000 llmx-0.0.3a0/setup.py
+drwxr-xr-x   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)        0 2023-08-02 21:25:29.071923 llmx-0.0.3a0/tests/
+-rw-r--r--   0 NORTHAMERICA.victordibia (302077204) NORTHAMERICA.domain users (300000513)     1970 2023-08-02 21:19:19.000000 llmx-0.0.3a0/tests/test_generators.py
```

### Comparing `llmx-0.0.2a0/.gitignore` & `llmx-0.0.3a0/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .vscode
+.release.sh
 llmx/generators/cache
 llmx.egg-info
 notebooks/test.ipynb
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `llmx-0.0.2a0/PKG-INFO` & `llmx-0.0.3a0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,41 @@
-Metadata-Version: 2.1
-Name: llmx
-Version: 0.0.2a0
-Summary: LLMX: A library for LLM Text Generation
-Author-email: Victor Dibia <victor.dibia@gmail.com>
-Project-URL: Homepage, https://github.com/victordibia/llmx
-Project-URL: Bug Tracker, https://github.com/victordibia/llmx/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: web
-Provides-Extra: local
-
 # LLMX - An API for Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
 A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
 
 There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
 
 - **Unified Model Interface**: Single interface to create LLM text generators with support for **multiple LLM providers**.
 
 ```python
+from llmx import  text_generator as generator
 
-openai_generator = TextGenerator(provider="openai")
-palm_generator = TextGenerator(provider="google") # or palm
-cohere_generator = TextGenerator(provider="cohere") # or palm
-hf_generator = TextGenerator(provider="huggingface") # run locally
+openai_generator = generator(provider="openai")
+palm_generator = generator(provider="google") # or palm
+cohere_generator = generator(provider="cohere") # or palm
+hf_generator = generator(provider="huggingface") # run locally
 ```
 
 - **Unified Messaging Interface**. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form. A single request is list one only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. For all models.
 
 ```python
 messages = [
     {"role": "user", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
 
 - **Good Utils (e.g., Caching etc)**: E.g. being able to use caching for faster responses. General policy is that cache is used if config (including messages) is the same. If you want to force a new response, set `use_cache=False` in the `generate` call.
 
 ```python
-response = gen.generate(config=config, use_cache=True)
+response = gen.generate(messages=messages, use_cache=True)
+
+# TextGenerationResponse(text=[Message(role='assistant', content="Gravity is like a magical force that pulls things towards each other. It's what keeps us on the ground and stops us from floating away into space. ... ")], config=TextGenerationConfig(n=1, temperature=0.1, max_tokens=8147, top_p=1.0, top_k=50, frequency_penalty=0.0, presence_penalty=0.0, model_type='openai', model='gpt-4', stop=None), logprobs=[], usage={'prompt_tokens': 34, 'completion_tokens': 69, 'total_tokens': 103})
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
 Install from pypi. Please use python3.9 or higher.
@@ -74,26 +62,36 @@
 ```bash
 export OPENAI_API_KEY=<your key>
 export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
 ```
 
 ```python
-from llmx.generators.text.textgen import TextGenerator
+from llmx import  text_generator as generator
 from llmx.datamodel import TextGenerationConfig
 
-gen = TextGenerator(provider="openai")
-config = TextGenerationConfig(messages=[
-        {"role": "user", "content": "What is the height of the Eiffel Tower?"},
-    ])
-response = gen.generate(config=config, use_cache=False)
-print(response.text)
-# [{'role': 'assistant', 'content': 'The height of the Eiffel Tower is 324 meters (1,063 feet).'}]
+messages =  messages = [
+    {"role": "system", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
+    {"role": "user", "content": "What is  gravity?"}
+]
+
+openai_gen = generator(provider="openai")
+openai_config = TextGenerationConfig(model="gpt-4", max_tokens=50)
+openai_response = openai_gen.generate(messages, config=openai_config, use_cache=True)
+print(openai_response.text[0].content)
+
 ```
 
+See the [tutorial](/notebooks/tutorial.ipynb) for more examples.
+
 ## Current Work
 
 - Supported models
   - [x] OpenAI
   - [x] PaLM
   - [x] Cohere
-  - [ ] HuggingFace (local)
+  - [x] HuggingFace (local)
+
+## Caveats
+
+- **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
+- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
```

### Comparing `llmx-0.0.2a0/llmx/datamodel.py` & `llmx-0.0.3a0/llmx/datamodel.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,24 +17,23 @@
     def to_dict(self):
         return self._fields_dict
 
 
 @dataclass
 class TextGenerationConfig:
     n: int = 1
-    temperature: float = 0.5
-    max_tokens: int = None
+    temperature: float = 0.1
+    max_tokens: Union[int, None] = None
     top_p: float = 1.0
     top_k: int = 50
     frequency_penalty: float = 0.0
     presence_penalty: float = 0.0
     model_type: str = "openai"
     model: str = None
-    stop: Union[list[str], str, None] = None
-    messages: Union[list[dict], str, None] = None
+    stop: Union[list[str], str, None] = None 
 
     def __post_init__(self):
         self._fields_dict = asdict(self)
 
     def __getitem__(self, key: Union[str, int]) -> Any:
         return self._fields_dict.get(key)
```

### Comparing `llmx-0.0.2a0/llmx/generators/text/base_textgen.py` & `llmx-0.0.3a0/llmx/generators/text/base_textgen.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,29 @@
 import os
+from typing import Union
 from diskcache import Cache
 from ...utils import get_user_cache_dir
 from ...datamodel import TextGenerationConfig, TextGenerationResponse
 from ...version import APP_NAME
+from abc import ABC, abstractmethod
 
+class BaseTextGenerator(ABC):
 
-class BaseTextGenerator:
     def __init__(self, provider: str = "openai", **kwargs):
         self.provider = provider
         self.model_name = kwargs.get("model_name", "gpt-3.5-turbo")
 
         app_name = APP_NAME
         cache_dir_default = get_user_cache_dir(app_name)
-        cache_dir_based_on_model = os.path.join(
-            cache_dir_default, self.provider, self.model_name
-        )
+        cache_dir_based_on_model = os.path.join(cache_dir_default, self.provider, self.model_name)
         self.cache_dir = kwargs.get("cache_dir", cache_dir_based_on_model)
         self.cache = Cache(self.cache_dir)
 
+    @abstractmethod
     def generate(
-        self, config: TextGenerationConfig, use_cache=True, **kwargs
+        self, messages: Union[list[dict], str], config: TextGenerationConfig = TextGenerationConfig(), use_cache=True, **kwargs
     ) -> TextGenerationResponse:
-        raise NotImplementedError(
-            "This method should be implemented by all subclasses."
-        )
+        pass
 
+    @abstractmethod
     def count_tokens(self, text) -> int:
-        raise NotImplementedError(
-            "This method should be implemented by all subclasses."
-        )
+        pass
```

### Comparing `llmx-0.0.2a0/llmx/generators/text/cohere_textgen.py` & `llmx-0.0.3a0/llmx/generators/text/cohere_textgen.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from .base_textgen import BaseTextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse, Message
 from ...utils import cache_request, num_tokens_from_messages
 import os
 import cohere
 from dataclasses import asdict
 
@@ -27,38 +28,36 @@
                 prompt += message["content"] + "\n"
             else:
                 prompt += message["role"] + ": " + message["content"] + "\n"
 
         return prompt
 
     def generate(
-        self, config: TextGenerationConfig, use_cache=True, **kwargs
+        self,  messages: Union[list[dict], str], config: TextGenerationConfig = TextGenerationConfig(), use_cache=True, **kwargs
     ) -> TextGenerationResponse:
-        config.model = config.model or "command"
-        config.messages = self.format_messages(config.messages)
-
+         
+        messages = self.format_messages(messages)
         self.model_name = config.model
 
         cohere_config = {
-            "model": config.model,
-            "prompt": config.messages,
+            "model": config.model or "command",
+            "prompt": messages,
             "max_tokens": config.max_tokens,
             "temperature": config.temperature,
             "k": config.top_k,
             "p": config.top_p,
             "num_generations": config.n,
             "stop_sequences": config.stop,
             "frequency_penalty": config.frequency_penalty,
             "presence_penalty": config.presence_penalty,
         }
-
-        print(cohere_config)
-
+ 
+        cache_key_params = cohere_config | {"messages": messages}
         if use_cache:
-            response = cache_request(cache=self.cache, params=(cohere_config))
+            response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
         co_response = self.client.generate(**cohere_config)
 
         response_text = [
             Message(
@@ -67,19 +66,16 @@
             )
             for x in co_response.generations
         ]
 
         response = TextGenerationResponse(
             text=response_text,
             logprobs=[],  # You may need to extract log probabilities from the response if needed
-            config=config,
+            config=cohere_config,
             usage={},  # You may need to extract usage metrics from the response if needed
         )
 
-        if use_cache:
-            cache_request(
-                cache=self.cache, params=asdict(config), values=(cohere_config)
-            )
+        cache_request(cache=self.cache, params=cache_key_params, values=asdict(response))
         return response
 
     def count_tokens(self, text) -> int:
         return num_tokens_from_messages(text)
```

### Comparing `llmx-0.0.2a0/llmx/generators/text/hf_textgen.py` & `llmx-0.0.3a0/llmx/generators/text/hf_textgen.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from typing import Union
+from dataclasses import asdict, dataclass
+from transformers import (AutoTokenizer, AutoModelForCausalLM, GenerationConfig)
+import torch
+
+
 from .base_textgen import BaseTextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse
 from ...utils import cache_request
-from dataclasses import asdict
-from dataclasses import asdict, dataclass
 
 
 @dataclass
 class DialogueTemplate:
     system: str = None
     dialogue_type: str = "default"
     messages: list[dict[str, str]] = None
@@ -63,14 +67,15 @@
             prompt = prompt + " " + self.assistant_token + "\n"
             # print(instruction)
             return prompt
         elif self.dialogue_type == "llama2":
             prompt = "[INST]"
             system_prompt = ""
             other_prompt = ""
+
             for message in self.messages:
                 if message["role"] == "system":
                     system_prompt += message["content"] + "\n"
                 elif message["role"] == "assistant":
                     other_prompt += message["content"] + "  \n"
                 else:
                     other_prompt += "[INST] " + message["content"] + "[/INST]\n"
@@ -81,40 +86,20 @@
                 + other_prompt
                 + "[/INST]"
             )
 
 
 class HFTextGenerator(BaseTextGenerator):
     def __init__(self, provider: str = "huggingface", device_map=None, **kwargs):
-        # Check if transformers package is installed
-        try:
-            import transformers
-            from transformers import (
-                AutoTokenizer,
-                AutoModelForCausalLM,
-                GenerationConfig,
-            )
-        except ImportError:
-            raise ImportError(
-                "Please install the `transformers` package to use the HFTextGenerator class."
-            )
-
-        # Check if torch package is installed
-        try:
-            import torch
-        except ImportError:
-            raise ImportError(
-                "Please install the `torch` package to use the HFTextGenerator class."
-            )
 
         super().__init__(provider=provider)
 
         self.dialogue_type = kwargs.get("dialogue_type", "alpaca")
 
-        self.model_name = kwargs.get("model_name", "TheBloke/Llama-2-7b-chat-fp16")
+        self.model_name = kwargs.get("model", "TheBloke/gpt4-x-vicuna-13B-HF")
         self.load_in_8bit = kwargs.get("load_in_8bit", False)
         self.device = kwargs.get("device", self.get_default_device())
         self.tokenizer = AutoTokenizer.from_pretrained(self.model_name)
         self.model = AutoModelForCausalLM.from_pretrained(
             self.model_name, device_map=device_map, load_in_8bit=self.load_in_8bit
         )
         if not device_map:
@@ -133,15 +118,15 @@
                 user_token="### Instruction:",
                 assistant_token="### Response:",
             )
             self.model.config.pad_token_id = self.tokenizer.pad_token_id = 0  # unk
             self.model.config.bos_token_id = 1
             self.model.config.eos_token_id = 2
         else:
-            self.dialogue_template = DialogueTemplate()
+            self.dialogue_template = DialogueTemplate(end_token=self.tokenizer.eos_token)
 
     def get_default_device(self):
         """Pick GPU if available, else CPU"""
         if torch.cuda.is_available():
             return torch.device("cuda")
         elif torch.backends.mps.is_available():
             return torch.device("mps")
@@ -162,24 +147,30 @@
         for message in messages:
             instruction += message["content"] + "\n"
         instruction = instruction + "### Response: "
         # print(instruction)
         return instruction
 
     def generate(
-        self, config: TextGenerationConfig, use_cache=True, **kwargs
-    ) -> TextGenerationResponse:
+            self, messages: Union[list[dict],
+                                  str],
+            config: TextGenerationConfig = TextGenerationConfig(),
+            use_cache=True, **kwargs) -> TextGenerationResponse:
         config.model = self.model_name
-        config_kwargs = {**asdict(config), **kwargs}
+        cache_key_params = {
+            **asdict(config),
+            **kwargs,
+            "messages": messages,
+            "dialogue_type": self.dialogue_type}
         if use_cache:
-            response = cache_request(cache=self.cache, params=(config_kwargs))
+            response = cache_request(cache=self.cache, params=(cache_key_params))
             if response:
                 return TextGenerationResponse(**response)
 
-        self.dialogue_template.messages = config.messages
+        self.dialogue_template.messages = messages
         prompt = self.dialogue_template.get_inference_prompt()
         batch = self.tokenizer(
             prompt, return_tensors="pt", return_token_type_ids=False
         ).to(self.model.device)
         input_ids = batch["input_ids"]
 
         max_new_tokens = kwargs.get(
@@ -230,12 +221,12 @@
         response = TextGenerationResponse(
             text=[self.post_process_response(x) for x in text_response],
             logprobs=[],
             config=config,
             usage=usage,
         )
         # if use_cache:
-        cache_request(cache=self.cache, params=(config_kwargs), values=asdict(response))
+        cache_request(cache=self.cache, params=(cache_key_params), values=asdict(response))
         return response
 
     def count_tokens(self, text: str):
         return len(self.tokenizer(text)["input_ids"])
```

### Comparing `llmx-0.0.2a0/llmx/generators/text/openai_textgen.py` & `llmx-0.0.3a0/llmx/generators/text/openai_textgen.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from typing import Union
 from .base_textgen import BaseTextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse
 from ...utils import cache_request, num_tokens_from_messages
 import os
 import openai
 from dataclasses import asdict
 
@@ -33,42 +34,47 @@
             )
         openai.api_key = api_key
         if organization:
             openai.organization = organization
         self.api_key = api_key
 
     def generate(
-        self, config: TextGenerationConfig, use_cache=True, **kwargs
+        self,  messages: Union[list[dict], str], config: TextGenerationConfig = TextGenerationConfig(), use_cache=True, **kwargs
     ) -> TextGenerationResponse:
-        config.model = config.model or "gpt-3.5-turbo-0301"
-        self.model_name = config.model
+
+        model = config.model  or "gpt-3.5-turbo-0301"
+        prompt_tokens = num_tokens_from_messages(messages)
+        max_tokens = max(context_lengths.get(model, 4096) - prompt_tokens - 10, 200)
+
+        oai_config = {
+            "model": model,
+            "temperature": config.temperature,
+            "max_tokens": max_tokens,
+            "top_p": config.top_p,
+            "frequency_penalty": config.frequency_penalty,
+            "presence_penalty": config.presence_penalty,
+            "n": config.n,
+            "messages": messages,
+        }
+         
+        self.model_name = model
+        cache_key_params = (oai_config) | {"messages": messages} 
         if use_cache:
-            response = cache_request(cache=self.cache, params=asdict(config))
+            response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
-        prompt_tokens = num_tokens_from_messages(config.messages)
-        max_tokens = max(context_lengths[config.model] - prompt_tokens - 10, 200)
-
-        oai_response = openai.ChatCompletion.create(
-            model=config.model,
-            messages=config.messages,
-            n=config.n,
-            temperature=config.temperature,
-            max_tokens=max_tokens,
-            top_p=config.top_p,
-            frequency_penalty=config.frequency_penalty,
-            presence_penalty=config.presence_penalty,
-        )
+        
+        oai_response = openai.ChatCompletion.create(**oai_config)
 
         response = TextGenerationResponse(
             text=[dict(x.message) for x in oai_response.choices],
             logprobs=[],
-            config=config,
+            config=oai_config,
             usage=dict(oai_response.usage),
         )
         # if use_cache:
-        cache_request(cache=self.cache, params=asdict(config), values=asdict(response))
+        cache_request(cache=self.cache, params=cache_key_params, values=asdict(response))
         return response
 
     def count_tokens(self, text) -> int:
         return num_tokens_from_messages(text)
```

### Comparing `llmx-0.0.2a0/llmx/generators/text/palm_textgen.py` & `llmx-0.0.3a0/llmx/generators/text/palm_textgen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import asdict
 import os
+from typing import Union
 import google.generativeai as palm
 from .base_textgen import BaseTextGenerator
 from ...datamodel import TextGenerationConfig, TextGenerationResponse, Message
 from ...utils import cache_request, num_tokens_from_messages
 
 
 class PalmTextGenerator(BaseTextGenerator):
@@ -33,34 +34,35 @@
                     "author": message["role"],
                     "content": message["content"],
                 }
                 palm_messages.append(palm_message)
         return system_messages, palm_messages
 
     def generate(
-        self, config: TextGenerationConfig, use_cache=True, **kwargs
-    ) -> TextGenerationResponse:
-        config.model = config.model or "models/chat-bison-001"
-        self.model_name = config.model
-        system_messages, messages = self.format_messages(config.messages)
+            self, messages: Union[list[dict],
+                                  str],
+            config: TextGenerationConfig = TextGenerationConfig(),
+            use_cache=True, **kwargs) -> TextGenerationResponse:
+        model = config.model or "models/chat-bison-001"
+        self.model_name = model
+        system_messages, messages = self.format_messages(messages)
         palm_config = {
-            "model": config.model,
+            "model": model,
             "context": system_messages,
             "examples": None,
             "candidate_count": max(1, min(8, config.n)),  # 1 <= n <= 8
             "temperature": config.temperature,
             "top_p": config.top_p,
             "top_k": config.top_k,
             "messages": messages,
         }
-
-        print(palm_config)
-
+        # print("*********", config)
+        cache_key_params = palm_config | {"messages": messages}
         if use_cache:
-            response = cache_request(cache=self.cache, params=(palm_config))
+            response = cache_request(cache=self.cache, params=cache_key_params)
             if response:
                 return TextGenerationResponse(**response)
 
         try:
             palm_response = palm.chat(**palm_config)
         except Exception as e:
             raise ValueError(f"Error generating text: {e}")
@@ -72,20 +74,20 @@
             )
             for x in palm_response.candidates
         ]
 
         response = TextGenerationResponse(
             text=response_text,
             logprobs=[],
-            config=config,
+            config=palm_config,
             usage={
                 "total_tokens": num_tokens_from_messages(
                     response_text, model=palm_config["model"]
                 )
             },
         )
 
-        cache_request(cache=self.cache, params=(palm_config), values=asdict(response))
+        cache_request(cache=self.cache, params=(cache_key_params), values=asdict(response))
         return response
 
     def count_tokens(self, text) -> int:
         return num_tokens_from_messages(text)
```

### Comparing `llmx-0.0.2a0/llmx/utils.py` & `llmx-0.0.3a0/llmx/utils.py`

 * *Files identical despite different names*

### Comparing `llmx-0.0.2a0/llmx.egg-info/PKG-INFO` & `llmx-0.0.3a0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 Metadata-Version: 2.1
 Name: llmx
-Version: 0.0.2a0
+Version: 0.0.3a0
 Summary: LLMX: A library for LLM Text Generation
 Author-email: Victor Dibia <victor.dibia@gmail.com>
 Project-URL: Homepage, https://github.com/victordibia/llmx
 Project-URL: Bug Tracker, https://github.com/victordibia/llmx/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: web
-Provides-Extra: local
+Provides-Extra: transformers
 
 # LLMX - An API for Language Models
 
 [![PyPI version](https://badge.fury.io/py/llmx.svg)](https://badge.fury.io/py/llmx)
 
 A simple python package that provides a unified interface to several LLM providers [ OpenAI (default), PaLM, Cohere and local HuggingFace Models ].
 
 There is nothing special about this library, but some of the requirements I needed when I startec building this (that other libraries did not have):
 
 - **Unified Model Interface**: Single interface to create LLM text generators with support for **multiple LLM providers**.
 
 ```python
+from llmx import  text_generator as generator
 
-openai_generator = TextGenerator(provider="openai")
-palm_generator = TextGenerator(provider="google") # or palm
-cohere_generator = TextGenerator(provider="cohere") # or palm
-hf_generator = TextGenerator(provider="huggingface") # run locally
+openai_generator = generator(provider="openai")
+palm_generator = generator(provider="google") # or palm
+cohere_generator = generator(provider="cohere") # or palm
+hf_generator = generator(provider="huggingface") # run locally
 ```
 
 - **Unified Messaging Interface**. Standardizes on the OpenAI ChatML format. For example, the standard prompt sent a model is formatted as an array of objects, where each object has a role (`system`, `user`, or `assistant`) and content of the form. A single request is list one only one message (e.g., write code to plot a cosine wave signal). A conversation is a list of messages e.g. write code for x, update the axis to y, etc. For all models.
 
 ```python
 messages = [
     {"role": "user", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
     {"role": "user", "content": "What is  gravity?"}
 ]
 ```
 
 - **Good Utils (e.g., Caching etc)**: E.g. being able to use caching for faster responses. General policy is that cache is used if config (including messages) is the same. If you want to force a new response, set `use_cache=False` in the `generate` call.
 
 ```python
-response = gen.generate(config=config, use_cache=True)
+response = gen.generate(messages=messages, use_cache=True)
+
+# TextGenerationResponse(text=[Message(role='assistant', content="Gravity is like a magical force that pulls things towards each other. It's what keeps us on the ground and stops us from floating away into space. ... ")], config=TextGenerationConfig(n=1, temperature=0.1, max_tokens=8147, top_p=1.0, top_k=50, frequency_penalty=0.0, presence_penalty=0.0, model_type='openai', model='gpt-4', stop=None), logprobs=[], usage={'prompt_tokens': 34, 'completion_tokens': 69, 'total_tokens': 103})
 ```
 
 Are there other libraries that do things like this really well? Yes! I'd recommend looking at [guidance](https://github.com/microsoft/guidance) which does a lot more. Interested in optimized inference? Try somthing like [vllm](https://github.com/vllm-project/vllm).
 
 ## Installation
 
 Install from pypi. Please use python3.9 or higher.
@@ -74,26 +77,36 @@
 ```bash
 export OPENAI_API_KEY=<your key>
 export PALM_API_KEY=<your key>
 export COHERE_API_KEY=<your key>
 ```
 
 ```python
-from llmx.generators.text.textgen import TextGenerator
+from llmx import  text_generator as generator
 from llmx.datamodel import TextGenerationConfig
 
-gen = TextGenerator(provider="openai")
-config = TextGenerationConfig(messages=[
-        {"role": "user", "content": "What is the height of the Eiffel Tower?"},
-    ])
-response = gen.generate(config=config, use_cache=False)
-print(response.text)
-# [{'role': 'assistant', 'content': 'The height of the Eiffel Tower is 324 meters (1,063 feet).'}]
+messages =  messages = [
+    {"role": "system", "content": "You are a helpful assistant that can explain concepts clearly to a 6 year old child."},
+    {"role": "user", "content": "What is  gravity?"}
+]
+
+openai_gen = generator(provider="openai")
+openai_config = TextGenerationConfig(model="gpt-4", max_tokens=50)
+openai_response = openai_gen.generate(messages, config=openai_config, use_cache=True)
+print(openai_response.text[0].content)
+
 ```
 
+See the [tutorial](/notebooks/tutorial.ipynb) for more examples.
+
 ## Current Work
 
 - Supported models
   - [x] OpenAI
   - [x] PaLM
   - [x] Cohere
-  - [ ] HuggingFace (local)
+  - [x] HuggingFace (local)
+
+## Caveats
+
+- **Prompting**. llmx makes some assumptions around how prompts are constructed e.g., how the chat message interface is assembled into a prompt for each model type. If your application or use case requires more control over the prompt, you may want to use a different library (ideally query the LLM models directly).
+- **Inference Optimization**. This library is not really designed for speed, but more for rapid experimentation using multiple models. If you are looking for a library that is optimized for inference, I'd recommend looking at [vllm](https://github.com/vllm-project/vllm) or [tgi](https://github.com/huggingface/text-generation-inference)
```

### Comparing `llmx-0.0.2a0/llmx.egg-info/SOURCES.txt` & `llmx-0.0.3a0/llmx.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 llmx/generators/text/base_textgen.py
 llmx/generators/text/cohere_textgen.py
 llmx/generators/text/hf_textgen.py
 llmx/generators/text/openai_textgen.py
 llmx/generators/text/palm_textgen.py
 llmx/generators/text/textgen.py
 notebooks/tutorial.ipynb
+notebooks/research/travelbenchmark.ipynb
 tests/test_generators.py
```

### Comparing `llmx-0.0.2a0/pyproject.toml` & `llmx-0.0.3a0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     "pydantic",
     "openai", 
     "google-generativeai",
     "tiktoken",
     "diskcache",
     "cohere", 
 ]
-optional-dependencies = {web = ["fastapi", "uvicorn"], local = ["transformers[torch]>=4.26"]}
+optional-dependencies = {web = ["fastapi", "uvicorn"], transformers = ["transformers[torch]>=4.26"]}
 
 dynamic = ["version"]
 
 [tool.setuptools]
 include-package-data = true
```

### Comparing `llmx-0.0.2a0/tests/test_generators.py` & `llmx-0.0.3a0/tests/test_generators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,54 +1,65 @@
-from llmx.generators.text.textgen import TextGenerator
+import pytest
+import os
+from llmx import text_generator as generator
 from llmx.datamodel import TextGenerationConfig
 
 
 config = TextGenerationConfig(
     n=2,
-    temperature=0.01,
+    temperature=0.4,
     max_tokens=100,
     top_p=1.0,
     top_k=50,
     frequency_penalty=0.0,
-    presence_penalty=0.0,
-    messages=[
-        {"role": "user", "content": "What is the height of the Eiffel Tower?"},
-    ],
+    presence_penalty=0.0
 )
 
+messages = [
+    {"role": "user",
+     "content": "What is the capital of France? Only respond with the exact answer"}]
+
 
 def test_openai():
-    openai_gen = TextGenerator(provider="openai")
-    openai_response = openai_gen.generate(config=config, use_cache=False)
+    openai_gen = generator(provider="openai")
+    openai_response = openai_gen.generate(messages, config=config, use_cache=False)
     answer = openai_response.text[0].content
     print(openai_response.text[0].content)
 
-    assert (
-        "324" in answer or "1,063" in answer or "1,063 ft" in answer or "1063" in answer
-    )
+    assert ("paris" in answer.lower())
     assert len(openai_response.text) == 2
 
 
 def test_google():
-    google_gen = TextGenerator(provider="google")
+    google_gen = generator(provider="google")
     config.model = "models/chat-bison-001"
-    google_response = google_gen.generate(config=config, use_cache=False)
+    google_response = google_gen.generate(messages, config=config, use_cache=False)
     answer = google_response.text[0].content
     print(google_response.text[0].content)
 
-    assert (
-        "324" in answer or "1,063" in answer or "1,063 ft" in answer or "1063" in answer
-    )
-    assert len(google_response.text) == 2
+    assert ("paris" in answer.lower())
+    # assert len(google_response.text) == 2 palm may chose to return 1 or 2 responses
 
 
 def test_cohere():
-    cohere_gen = TextGenerator(provider="cohere")
+    cohere_gen = generator(provider="cohere")
     config.model = "command"
-    cohere_response = cohere_gen.generate(config=config, use_cache=False)
+    cohere_response = cohere_gen.generate(messages, config=config, use_cache=False)
     answer = cohere_response.text[0].content
     print(cohere_response.text[0].content)
 
-    assert (
-        "324" in answer or "1,063" in answer or "1,063 ft" in answer or "1063" in answer
-    )
+    assert ("paris" in answer.lower())
     assert len(cohere_response.text) == 2
+
+
+@pytest.mark.skipif("RUNALL" not in os.environ, reason="takes too long")
+def test_hf_local():
+    hf_local_gen = generator(
+        provider="hf",
+        model="TheBloke/Llama-2-7b-chat-fp16",
+        device_map="auto")
+    hf_local_response = hf_local_gen.generate(messages, config=config, use_cache=False)
+    answer = hf_local_response.text[0].content
+    print(hf_local_response.text[0].content)
+
+    assert ("paris" in answer.lower())
+    assert len(hf_local_response.text) == 2
```


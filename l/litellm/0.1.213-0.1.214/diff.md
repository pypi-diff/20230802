# Comparing `tmp/litellm-0.1.213.tar.gz` & `tmp/litellm-0.1.214.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.213.tar", last modified: Wed Aug  2 03:14:59 2023, max compression
+gzip compressed data, was "litellm-0.1.214.tar", last modified: Wed Aug  2 19:37:59 2023, max compression
```

## Comparing `litellm-0.1.213.tar` & `litellm-0.1.214.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-02 03:14:59.260458 litellm-0.1.213/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     1065 2023-07-27 00:10:35.000000 litellm-0.1.213/LICENSE
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-02 03:14:59.260364 litellm-0.1.213/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2129 2023-08-02 03:09:05.000000 litellm-0.1.213/README.md
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-02 03:14:59.259564 litellm-0.1.213/litellm/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      626 2023-08-01 22:01:24.000000 litellm-0.1.213/litellm/__init__.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    10735 2023-08-02 00:06:25.000000 litellm-0.1.213/litellm/main.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)     2546 2023-08-01 22:01:24.000000 litellm-0.1.213/litellm/timeout.py
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)    12522 2023-08-01 22:01:24.000000 litellm-0.1.213/litellm/utils.py
-drwxr-xr-x   0 ishaanjaffer   (501) staff       (20)        0 2023-08-02 03:14:59.260197 litellm-0.1.213/litellm.egg-info/
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      215 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/PKG-INFO
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      252 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        1 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       71 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/requires.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)        8 2023-08-02 03:14:59.000000 litellm-0.1.213/litellm.egg-info/top_level.txt
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)       38 2023-08-02 03:14:59.260492 litellm-0.1.213/setup.cfg
--rw-r--r--   0 ishaanjaffer   (501) staff       (20)      407 2023-08-02 03:14:16.000000 litellm-0.1.213/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:59.048095 litellm-0.1.214/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1065 2023-08-02 19:37:46.000000 litellm-0.1.214/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-02 19:37:59.044094 litellm-0.1.214/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2230 2023-08-02 19:37:46.000000 litellm-0.1.214/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:59.044094 litellm-0.1.214/litellm/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      640 2023-08-02 19:37:46.000000 litellm-0.1.214/litellm/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11031 2023-08-02 19:37:46.000000 litellm-0.1.214/litellm/main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2546 2023-08-02 19:37:46.000000 litellm-0.1.214/litellm/timeout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14277 2023-08-02 19:37:46.000000 litellm-0.1.214/litellm/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-02 19:37:59.044094 litellm-0.1.214/litellm.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      151 2023-08-02 19:37:59.000000 litellm-0.1.214/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      267 2023-08-02 19:37:59.000000 litellm-0.1.214/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-02 19:37:59.000000 litellm-0.1.214/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       71 2023-08-02 19:37:59.000000 litellm-0.1.214/litellm.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-02 19:37:59.000000 litellm-0.1.214/litellm.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-08-02 19:37:46.000000 litellm-0.1.214/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-02 19:37:59.048095 litellm-0.1.214/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      407 2023-08-02 19:37:46.000000 litellm-0.1.214/setup.py
```

### Comparing `litellm-0.1.213/LICENSE` & `litellm-0.1.214/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.213/README.md` & `litellm-0.1.214/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # *🚅 litellm*
 [![PyPI Version](https://img.shields.io/pypi/v/litellm.svg)](https://pypi.org/project/litellm/)
 [![PyPI Version](https://img.shields.io/badge/stable%20version-v0.1.1-blue?color=green&link=https://pypi.org/project/litellm/0.1.1/)](https://pypi.org/project/litellm/0.1.1/)
 [![CircleCI](https://dl.circleci.com/status-badge/img/gh/BerriAI/litellm/tree/main.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/BerriAI/litellm/tree/main)
 ![Downloads](https://img.shields.io/pypi/dm/litellm)
+![https://github.com/BerriAI/litellm](https://img.shields.io/badge/%F0%9F%9A%85%20%20liteLLM-8A2BE2)
 
 [![](https://dcbadge.vercel.app/api/server/wuPM9dRgDw)](https://discord.gg/wuPM9dRgDw)
 
 a simple & light 100 line package to call OpenAI, Azure, Cohere, Anthropic API Endpoints 
 
 litellm manages:
 - translating inputs to completion and embedding endpoints
```

### Comparing `litellm-0.1.213/litellm/__init__.py` & `litellm-0.1.214/litellm/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 success_callback = []
 failure_callback = []
 set_verbose=False
-
+telemetry=True
 ####### COMPLETION MODELS ###################
 open_ai_chat_completion_models = [
   'gpt-3.5-turbo', 
   'gpt-4'
 ]
 open_ai_text_completion_models = [
     'text-davinci-003'
```

### Comparing `litellm-0.1.213/litellm/main.py` & `litellm-0.1.214/litellm/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -248,43 +248,48 @@
     raise exception_type(model=model, original_exception=e)
 
 
 ### EMBEDDING ENDPOINTS ####################
 @client
 @timeout(60) ## set timeouts, in case calls hang (e.g. Azure) - default is 60s, override with `force_timeout`
 def embedding(model, input=[], azure=False, force_timeout=60, logger_fn=None):
-  response = None
-  if azure == True:
-    # azure configs
-    openai.api_type = "azure"
-    openai.api_base = os.environ.get("AZURE_API_BASE")
-    openai.api_version = os.environ.get("AZURE_API_VERSION")
-    openai.api_key = os.environ.get("AZURE_API_KEY")
-    ## LOGGING
-    logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
-    ## EMBEDDING CALL
-    response = openai.Embedding.create(input=input, engine=model)
-    print_verbose(f"response_value: {str(response)[:50]}")
-  elif model in litellm.open_ai_embedding_models:
-    openai.api_type = "openai"
-    openai.api_base = "https://api.openai.com/v1"
-    openai.api_version = None
-    openai.api_key = os.environ.get("OPENAI_API_KEY")
-    ## LOGGING
-    logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
-    ## EMBEDDING CALL
-    response = openai.Embedding.create(input=input, model=model)
-    print_verbose(f"response_value: {str(response)[:50]}")
-  else: 
-    logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
-    args = locals()
-    raise ValueError(f"No valid embedding model args passed in - {args}")
-  
-  return response
-
+  try:
+    response = None
+    if azure == True:
+      # azure configs
+      openai.api_type = "azure"
+      openai.api_base = os.environ.get("AZURE_API_BASE")
+      openai.api_version = os.environ.get("AZURE_API_VERSION")
+      openai.api_key = os.environ.get("AZURE_API_KEY")
+      ## LOGGING
+      logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
+      ## EMBEDDING CALL
+      response = openai.Embedding.create(input=input, engine=model)
+      print_verbose(f"response_value: {str(response)[:50]}")
+    elif model in litellm.open_ai_embedding_models:
+      openai.api_type = "openai"
+      openai.api_base = "https://api.openai.com/v1"
+      openai.api_version = None
+      openai.api_key = os.environ.get("OPENAI_API_KEY")
+      ## LOGGING
+      logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
+      ## EMBEDDING CALL
+      response = openai.Embedding.create(input=input, model=model)
+      print_verbose(f"response_value: {str(response)[:50]}")
+    else: 
+      logging(model=model, input=input, azure=azure, logger_fn=logger_fn)
+      args = locals()
+      raise ValueError(f"No valid embedding model args passed in - {args}")
+    
+    return response
+  except Exception as e:
+    # log the original exception
+    logging(model=model, input=input, azure=azure, logger_fn=logger_fn, exception=e)
+    ## Map to OpenAI Exception
+    raise exception_type(model=model, original_exception=e)
 ####### HELPER FUNCTIONS ################
 ## Set verbose to true -> ```litellm.set_verbose = True```    
 def print_verbose(print_statement):
   if litellm.set_verbose:
     print(f"LiteLLM: {print_statement}")
     if random.random() <= 0.3:
       print("Get help - https://discord.com/invite/wuPM9dRgDw")
```

### Comparing `litellm-0.1.213/litellm/timeout.py` & `litellm-0.1.214/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.213/litellm/utils.py` & `litellm-0.1.214/litellm/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,11 @@
-import dotenv
-import json
-import traceback
-import threading
-import traceback
-import subprocess
-import uuid
-import litellm
-import os 
-import openai 
-import random
+import dotenv, json, traceback, threading
+import subprocess, os 
+import litellm, openai 
+import random, uuid, requests
 from openai.error import AuthenticationError, InvalidRequestError, RateLimitError, ServiceUnavailableError, OpenAIError
 ####### ENVIRONMENT VARIABLES ###################
 dotenv.load_dotenv() # Loading env variables using dotenv
 sentry_sdk_instance = None
 capture_exception = None
 add_breadcrumb = None
 posthog = None
@@ -30,19 +23,23 @@
 
 ####### LOGGING ###################
 #Logging function -> log the exact model details + what's being sent | Non-Blocking
 def logging(model, input, azure=False, additional_args={}, logger_fn=None, exception=None):
   try:
     model_call_details = {}
     model_call_details["model"] = model
-    model_call_details["input"] = input
     model_call_details["azure"] = azure
     # log exception details
     if exception:
       model_call_details["original_exception"] = exception
+
+    if litellm.telemetry:
+      safe_crash_reporting(model=model, exception=exception, azure=azure) # log usage-crash details. Do not log any user details. If you want to turn this off, set `litellm.telemetry=False`.
+
+    model_call_details["input"] = input
     # log additional call details -> api key, etc. 
     if azure == True or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_chat_completion_models or model in litellm.open_ai_embedding_models:
       model_call_details["api_type"] = openai.api_type
       model_call_details["api_base"] = openai.api_base
       model_call_details["api_version"] = openai.api_version
       model_call_details["api_key"] = openai.api_key
     elif "replicate" in model:
@@ -269,8 +266,52 @@
         elif "too many tokens" in error_str:
           raise InvalidRequestError(f"CohereException - {error_str}", f"{model}")
         elif "CohereConnectionError" in exception_type: # cohere seems to fire these errors when we load test it (1k+ messages / min)
           raise RateLimitError(f"CohereException - {original_exception.message}")
       raise original_exception # base case - return the original exception
     else:
       raise original_exception
-                        
+
+def safe_crash_reporting(model=None, exception=None, azure=None):
+    data = {
+      "model": model,
+      "exception": str(exception),
+      "azure": azure
+    }
+    print(f"data in crash reporting: {data}")
+    threading.Thread(target=litellm_telemetry, args=(data,), daemon=True).start()
+
+def litellm_telemetry(data):
+    print(f"data in in litellm telemetry: {data}")
+    # Load or generate the UUID
+    uuid_file = 'litellm_uuid.txt'
+    try:
+        # Try to open the file and load the UUID
+        with open(uuid_file, 'r') as file:
+            uuid_value = file.read()
+            if uuid_value:
+                uuid_value = uuid_value.strip()
+                print(f"Loaded UUID: {uuid_value}")
+            else:
+                raise FileNotFoundError
+    except FileNotFoundError:
+        # Generate a new UUID if the file doesn't exist or is empty
+        new_uuid = uuid.uuid4()
+        uuid_value = str(new_uuid)
+        with open(uuid_file, 'w') as file:
+            file.write(uuid_value)
+        print(f"Generated and stored UUID: {uuid_value}")
+
+    # Prepare the data to send to localhost:3000
+    payload = {
+        'uuid': uuid_value,
+        'data': data
+    }
+    print_verbose(f"payload: {payload}")
+    try:
+      # Make the POST request to localhost:3000
+      response = requests.post('https://litellm.berri.ai/logging', json=payload)
+      response.raise_for_status()  # Raise an exception for HTTP errors
+      print('Request successfully sent!')
+    except requests.exceptions.RequestException as e:
+        # Handle any errors in the request
+        print(f'Error: {e}')
```


# Comparing `tmp/litellm-0.1.217.tar.gz` & `tmp/litellm-0.1.218.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.217.tar", last modified: Wed Aug  2 20:52:03 2023, max compression
+gzip compressed data, was "litellm-0.1.218.tar", last modified: Wed Aug  2 21:55:06 2023, max compression
```

## Comparing `litellm-0.1.217.tar` & `litellm-0.1.218.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 20:52:03.681027 litellm-0.1.217/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.217/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 20:52:03.680900 litellm-0.1.217/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.217/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 20:52:03.679926 litellm-0.1.217/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      691 2023-08-02 20:51:39.000000 litellm-0.1.217/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11031 2023-08-02 19:34:49.000000 litellm-0.1.217/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.217/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.217/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 20:52:03.680693 litellm-0.1.217/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 20:52:03.000000 litellm-0.1.217/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-02 20:52:03.000000 litellm-0.1.217/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-02 20:52:03.000000 litellm-0.1.217/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-02 20:52:03.000000 litellm-0.1.217/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-02 20:52:03.000000 litellm-0.1.217/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.217/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-02 20:52:03.681073 litellm-0.1.217/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-02 20:51:45.000000 litellm-0.1.217/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 21:55:06.441280 litellm-0.1.218/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.218/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 21:55:06.441156 litellm-0.1.218/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2294 2023-08-02 20:27:13.000000 litellm-0.1.218/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 21:55:06.440140 litellm-0.1.218/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      691 2023-08-02 20:51:39.000000 litellm-0.1.218/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    10353 2023-08-02 21:49:41.000000 litellm-0.1.218/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.218/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:27:13.000000 litellm-0.1.218/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 21:55:06.440934 litellm-0.1.218/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-02 21:55:06.000000 litellm-0.1.218/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.218/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-02 21:55:06.441327 litellm-0.1.218/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-02 21:53:35.000000 litellm-0.1.218/setup.py
```

### Comparing `litellm-0.1.217/LICENSE` & `litellm-0.1.218/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.217/README.md` & `litellm-0.1.218/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.217/litellm/__init__.py` & `litellm-0.1.218/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.217/litellm/main.py` & `litellm-0.1.218/litellm/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,70 +59,71 @@
 def completion(
     model, messages, # required params
     # Optional OpenAI params: see https://platform.openai.com/docs/api-reference/chat/create
     functions=[], function_call="", # optional params
     temperature=1, top_p=1, n=1, stream=False, stop=None, max_tokens=float('inf'),
     presence_penalty=0, frequency_penalty=0, logit_bias={}, user="",
     # Optional liteLLM function params
-    *, force_timeout=60, azure=False, logger_fn=None, verbose=False
+    *, api_key=None, force_timeout=60, azure=False, logger_fn=None, verbose=False
   ):
   try:
     # check if user passed in any of the OpenAI optional params
     optional_params = get_optional_params(
       functions=functions, function_call=function_call, 
       temperature=temperature, top_p=top_p, n=n, stream=stream, stop=stop, max_tokens=max_tokens,
       presence_penalty=presence_penalty, frequency_penalty=frequency_penalty, logit_bias=logit_bias, user=user
     )
     if azure == True:
       # azure configs
       openai.api_type = "azure"
       openai.api_base = os.environ.get("AZURE_API_BASE")
       openai.api_version = os.environ.get("AZURE_API_VERSION")
-      openai.api_key = os.environ.get("AZURE_API_KEY")
+      openai.api_key = api_key if api_key is not None else os.environ.get("AZURE_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = openai.ChatCompletion.create(
         engine=model,
         messages = messages,
         **optional_params
       )
     elif model in litellm.open_ai_chat_completion_models:
       openai.api_type = "openai"
       openai.api_base = "https://api.openai.com/v1"
       openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
+      openai.api_key = api_key if api_key is not None else os.environ.get("OPENAI_API_KEY")
       ## LOGGING
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
-
       ## COMPLETION CALL
       response = openai.ChatCompletion.create(
         model=model,
         messages = messages,
         **optional_params
       )
     elif model in litellm.open_ai_text_completion_models:
       openai.api_type = "openai"
       openai.api_base = "https://api.openai.com/v1"
       openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
+      openai.api_key = api_key if api_key is not None else os.environ.get("OPENAI_API_KEY")
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = openai.Completion.create(
           model=model,
           prompt = prompt
       )
     elif "replicate" in model:
       # replicate defaults to os.environ.get("REPLICATE_API_TOKEN")
       # checking in case user set it to REPLICATE_API_KEY instead 
       if not os.environ.get("REPLICATE_API_TOKEN") and os.environ.get("REPLICATE_API_KEY"):
         replicate_api_token = os.environ.get("REPLICATE_API_KEY")
         os.environ["REPLICATE_API_TOKEN"] = replicate_api_token
+      elif api_key:
+         os.environ["REPLICATE_API_TOKEN"] = api_key
       prompt = " ".join([message["content"] for message in messages])
       input = {"prompt": prompt}
       if max_tokens != float('inf'):
         input["max_length"] = max_tokens # for t5 models 
         input["max_new_tokens"] = max_tokens # for llama2 models 
       ## LOGGING
       logging(model=model, input=input, azure=azure, additional_args={"max_tokens": max_tokens}, logger_fn=logger_fn)
@@ -144,14 +145,16 @@
             }
           }
         ]
       }
       response = new_response
     elif model in litellm.anthropic_models:
       #anthropic defaults to os.environ.get("ANTHROPIC_API_KEY")
+      if api_key:
+         os.environ["ANTHROPIC_API_KEY"] = api_key
       prompt = f"{HUMAN_PROMPT}" 
       for message in messages:
         if "role" in message:
           if message["role"] == "user":
             prompt += f"{HUMAN_PROMPT}{message['content']}"
           else:
             prompt += f"{AI_PROMPT}{message['content']}"
@@ -183,15 +186,15 @@
             }
           }
         ]
       }
       print_verbose(f"new response: {new_response}")
       response = new_response
     elif model in litellm.cohere_models:
-      cohere_key = os.environ.get("COHERE_API_KEY")
+      cohere_key = api_key if api_key is not None else os.environ.get("COHERE_API_KEY")
       co = cohere.Client(cohere_key)
       prompt = " ".join([message["content"] for message in messages])
       ## LOGGING
       logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
       ## COMPLETION CALL
       response = co.generate(  
         model=model,
@@ -206,40 +209,14 @@
                       "content": response[0].text,
                       "role": "assistant"
                   }
               }
           ],
       }
       response = new_response
-
-    elif model in litellm.open_ai_chat_completion_models:
-      openai.api_type = "openai"
-      openai.api_base = "https://api.openai.com/v1"
-      openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
-      ## LOGGING
-      logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
-      ## COMPLETION CALL
-      response = openai.ChatCompletion.create(
-          model=model,
-          messages = messages
-      )
-    elif model in litellm.open_ai_text_completion_models:
-      openai.api_type = "openai"
-      openai.api_base = "https://api.openai.com/v1"
-      openai.api_version = None
-      openai.api_key = os.environ.get("OPENAI_API_KEY")
-      prompt = " ".join([message["content"] for message in messages])
-      ## LOGGING
-      logging(model=model, input=prompt, azure=azure, logger_fn=logger_fn)
-      ## COMPLETION CALL
-      response = openai.Completion.create(
-          model=model,
-          prompt = prompt
-      )
     else: 
       logging(model=model, input=messages, azure=azure, logger_fn=logger_fn)
       args = locals()
       raise ValueError(f"No valid completion model args passed in - {args}")
     return response
   except Exception as e:
     # log the original exception
```

### Comparing `litellm-0.1.217/litellm/timeout.py` & `litellm-0.1.218/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.217/litellm/utils.py` & `litellm-0.1.218/litellm/utils.py`

 * *Files identical despite different names*


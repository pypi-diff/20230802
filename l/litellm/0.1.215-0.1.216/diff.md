# Comparing `tmp/litellm-0.1.215.tar.gz` & `tmp/litellm-0.1.216.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "litellm-0.1.215.tar", last modified: Wed Aug  2 19:50:12 2023, max compression
+gzip compressed data, was "litellm-0.1.216.tar", last modified: Wed Aug  2 20:07:46 2023, max compression
```

## Comparing `litellm-0.1.215.tar` & `litellm-0.1.216.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 19:50:12.329688 litellm-0.1.215/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.215/LICENSE
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 19:50:12.329572 litellm-0.1.215/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2230 2023-08-02 18:36:25.000000 litellm-0.1.215/README.md
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 19:50:12.328738 litellm-0.1.215/litellm/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      640 2023-08-02 19:34:49.000000 litellm-0.1.215/litellm/__init__.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    11031 2023-08-02 19:34:49.000000 litellm-0.1.215/litellm/main.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.215/litellm/timeout.py
--rw-r--r--   0 krrishdholakia   (501) staff       (20)    14277 2023-08-02 19:34:49.000000 litellm-0.1.215/litellm/utils.py
-drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 19:50:12.329381 litellm-0.1.215/litellm.egg-info/
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 19:50:12.000000 litellm-0.1.215/litellm.egg-info/PKG-INFO
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-02 19:50:12.000000 litellm-0.1.215/litellm.egg-info/SOURCES.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-02 19:50:12.000000 litellm-0.1.215/litellm.egg-info/dependency_links.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-02 19:50:12.000000 litellm-0.1.215/litellm.egg-info/requires.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-02 19:50:12.000000 litellm-0.1.215/litellm.egg-info/top_level.txt
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.215/pyproject.toml
--rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-02 19:50:12.329729 litellm-0.1.215/setup.cfg
--rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-02 19:50:10.000000 litellm-0.1.215/setup.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 20:07:46.149181 litellm-0.1.216/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     1065 2023-07-29 14:29:32.000000 litellm-0.1.216/LICENSE
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 20:07:46.148834 litellm-0.1.216/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2230 2023-08-02 18:36:25.000000 litellm-0.1.216/README.md
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 20:07:46.147843 litellm-0.1.216/litellm/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      640 2023-08-02 19:34:49.000000 litellm-0.1.216/litellm/__init__.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    11031 2023-08-02 19:34:49.000000 litellm-0.1.216/litellm/main.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)     2546 2023-08-02 18:36:25.000000 litellm-0.1.216/litellm/timeout.py
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)    14200 2023-08-02 20:06:21.000000 litellm-0.1.216/litellm/utils.py
+drwxr-xr-x   0 krrishdholakia   (501) staff       (20)        0 2023-08-02 20:07:46.148644 litellm-0.1.216/litellm.egg-info/
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      151 2023-08-02 20:07:46.000000 litellm-0.1.216/litellm.egg-info/PKG-INFO
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      267 2023-08-02 20:07:46.000000 litellm-0.1.216/litellm.egg-info/SOURCES.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        1 2023-08-02 20:07:46.000000 litellm-0.1.216/litellm.egg-info/dependency_links.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       71 2023-08-02 20:07:46.000000 litellm-0.1.216/litellm.egg-info/requires.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)        8 2023-08-02 20:07:46.000000 litellm-0.1.216/litellm.egg-info/top_level.txt
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      473 2023-08-02 19:34:49.000000 litellm-0.1.216/pyproject.toml
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)       38 2023-08-02 20:07:46.149240 litellm-0.1.216/setup.cfg
+-rw-r--r--   0 krrishdholakia   (501) staff       (20)      407 2023-08-02 20:07:13.000000 litellm-0.1.216/setup.py
```

### Comparing `litellm-0.1.215/LICENSE` & `litellm-0.1.216/LICENSE`

 * *Files identical despite different names*

### Comparing `litellm-0.1.215/README.md` & `litellm-0.1.216/README.md`

 * *Files identical despite different names*

### Comparing `litellm-0.1.215/litellm/__init__.py` & `litellm-0.1.216/litellm/__init__.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.215/litellm/main.py` & `litellm-0.1.216/litellm/main.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.215/litellm/timeout.py` & `litellm-0.1.216/litellm/timeout.py`

 * *Files identical despite different names*

### Comparing `litellm-0.1.215/litellm/utils.py` & `litellm-0.1.216/litellm/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,88 +230,87 @@
       success_handler(args, kwargs)
     pass
   except:
     pass
 
 
 def exception_type(model, original_exception):
-    if isinstance(original_exception, OpenAIError):
-        # Handle the OpenAIError
-        raise original_exception
-    elif model:
-      error_str = str(original_exception)
-      if isinstance(original_exception, BaseException):
-        exception_type = type(original_exception).__name__
+    try:
+      if isinstance(original_exception, OpenAIError):
+          # Handle the OpenAIError
+          raise original_exception
+      elif model:
+        error_str = str(original_exception)
+        if isinstance(original_exception, BaseException):
+          exception_type = type(original_exception).__name__
+        else:
+          exception_type = ""
+        if "claude" in model: #one of the anthropics
+          if "status_code" in original_exception:
+            print_verbose(f"status_code: {original_exception.status_code}")
+            if original_exception.status_code == 401:
+              raise AuthenticationError(f"AnthropicException - {original_exception.message}")
+            elif original_exception.status_code == 400:
+              raise InvalidRequestError(f"AnthropicException - {original_exception.message}", f"{model}")
+            elif original_exception.status_code == 429:
+              raise RateLimitError(f"AnthropicException - {original_exception.message}")
+        elif "replicate" in model:
+          if "Incorrect authentication token" in error_str:
+            raise AuthenticationError(f"ReplicateException - {error_str}")
+          elif exception_type == "ModelError":
+            raise InvalidRequestError(f"ReplicateException - {error_str}", f"{model}")
+          elif "Request was throttled" in error_str:
+            raise RateLimitError(f"ReplicateException - {error_str}")
+          elif exception_type == "ReplicateError": ## ReplicateError implies an error on Replicate server side, not user side
+            raise ServiceUnavailableError(f"ReplicateException - {error_str}")
+        elif model == "command-nightly": #Cohere
+          if "invalid api token" in error_str or "No API key provided." in error_str:
+            raise AuthenticationError(f"CohereException - {error_str}")
+          elif "too many tokens" in error_str:
+            raise InvalidRequestError(f"CohereException - {error_str}", f"{model}")
+          elif "CohereConnectionError" in exception_type: # cohere seems to fire these errors when we load test it (1k+ messages / min)
+            raise RateLimitError(f"CohereException - {original_exception.message}")
+        raise original_exception # base case - return the original exception
       else:
-        exception_type = ""
-      if "claude" in model: #one of the anthropics
-        print_verbose(f"status_code: {original_exception.status_code}")
-        if original_exception.status_code == 401:
-          raise AuthenticationError(f"AnthropicException - {original_exception.message}")
-        elif original_exception.status_code == 400:
-          raise InvalidRequestError(f"AnthropicException - {original_exception.message}", f"{model}")
-        elif original_exception.status_code == 429:
-          raise RateLimitError(f"AnthropicException - {original_exception.message}")
-      elif "replicate" in model:
-        if "Incorrect authentication token" in error_str:
-          raise AuthenticationError(f"ReplicateException - {error_str}")
-        elif exception_type == "ModelError":
-          raise InvalidRequestError(f"ReplicateException - {error_str}", f"{model}")
-        elif "Request was throttled" in error_str:
-          raise RateLimitError(f"ReplicateException - {error_str}")
-        elif exception_type == "ReplicateError": ## ReplicateError implies an error on Replicate server side, not user side
-          raise ServiceUnavailableError(f"ReplicateException - {error_str}")
-      elif model == "command-nightly": #Cohere
-        if "invalid api token" in error_str or "No API key provided." in error_str:
-          raise AuthenticationError(f"CohereException - {error_str}")
-        elif "too many tokens" in error_str:
-          raise InvalidRequestError(f"CohereException - {error_str}", f"{model}")
-        elif "CohereConnectionError" in exception_type: # cohere seems to fire these errors when we load test it (1k+ messages / min)
-          raise RateLimitError(f"CohereException - {original_exception.message}")
-      raise original_exception # base case - return the original exception
-    else:
+        raise original_exception
+    except:
       raise original_exception
 
 def safe_crash_reporting(model=None, exception=None, azure=None):
     data = {
       "model": model,
       "exception": str(exception),
       "azure": azure
     }
-    print(f"data in crash reporting: {data}")
     threading.Thread(target=litellm_telemetry, args=(data,), daemon=True).start()
 
 def litellm_telemetry(data):
-    print(f"data in in litellm telemetry: {data}")
     # Load or generate the UUID
     uuid_file = 'litellm_uuid.txt'
     try:
         # Try to open the file and load the UUID
         with open(uuid_file, 'r') as file:
             uuid_value = file.read()
             if uuid_value:
                 uuid_value = uuid_value.strip()
-                print(f"Loaded UUID: {uuid_value}")
             else:
                 raise FileNotFoundError
     except FileNotFoundError:
         # Generate a new UUID if the file doesn't exist or is empty
         new_uuid = uuid.uuid4()
         uuid_value = str(new_uuid)
         with open(uuid_file, 'w') as file:
             file.write(uuid_value)
-        print(f"Generated and stored UUID: {uuid_value}")
 
     # Prepare the data to send to localhost:3000
     payload = {
         'uuid': uuid_value,
         'data': data
     }
     print_verbose(f"payload: {payload}")
     try:
       # Make the POST request to localhost:3000
       response = requests.post('https://litellm.berri.ai/logging', json=payload)
       response.raise_for_status()  # Raise an exception for HTTP errors
-      print('Request successfully sent!')
     except requests.exceptions.RequestException as e:
         # Handle any errors in the request
-        print(f'Error: {e}')
+        pass
```


# Comparing `tmp/anthropic-0.3.7.tar.gz` & `tmp/anthropic-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthropic-0.3.7.tar", max compression
+gzip compressed data, was "anthropic-0.3.8.tar", max compression
```

## Comparing `anthropic-0.3.7.tar` & `anthropic-0.3.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.7/LICENSE
--rw-r--r--   0        0        0     9994 2023-07-31 16:20:19.817632 anthropic-0.3.7/README.md
--rw-r--r--   0        0        0     1925 2023-07-31 16:20:19.817881 anthropic-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.7/src/anthropic/__init__.py
--rw-r--r--   0        0        0    47846 2023-07-31 16:20:19.818281 anthropic-0.3.7/src/anthropic/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.7/src/anthropic/_base_exceptions.py
--rw-r--r--   0        0        0    15554 2023-07-31 16:20:19.818545 anthropic-0.3.7/src/anthropic/_client.py
--rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.7/src/anthropic/_constants.py
--rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.7/src/anthropic/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.7/src/anthropic/_models.py
--rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.7/src/anthropic/_qs.py
--rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.7/src/anthropic/_resource.py
--rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.7/src/anthropic/_streaming.py
--rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.7/src/anthropic/_tokenizers.py
--rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.7/src/anthropic/_types.py
--rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.7/src/anthropic/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.7/src/anthropic/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.7/src/anthropic/_utils/_utils.py
--rw-r--r--   0        0        0      128 2023-07-31 16:20:19.818825 anthropic-0.3.7/src/anthropic/_version.py
--rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.7/src/anthropic/pagination.py
--rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.7/src/anthropic/py.typed
--rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.7/src/anthropic/resources/__init__.py
--rw-r--r--   0        0        0    21781 2023-07-19 23:00:27.618209 anthropic-0.3.7/src/anthropic/resources/completions.py
--rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.7/src/anthropic/tokenizer.json
--rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.7/src/anthropic/types/__init__.py
--rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.7/src/anthropic/types/completion.py
--rw-r--r--   0        0        0     7111 2023-07-19 23:00:27.618522 anthropic-0.3.7/src/anthropic/types/completion_create_params.py
--rw-r--r--   0        0        0    10947 1970-01-01 00:00:00.000000 anthropic-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-06-26 21:50:36.624119 anthropic-0.3.8/LICENSE
+-rw-r--r--   0        0        0    10184 2023-08-02 20:24:32.279674 anthropic-0.3.8/README.md
+-rw-r--r--   0        0        0     1925 2023-08-02 20:24:32.282173 anthropic-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1999 2023-06-26 21:50:36.627612 anthropic-0.3.8/src/anthropic/__init__.py
+-rw-r--r--   0        0        0    47778 2023-08-02 20:24:32.282808 anthropic-0.3.8/src/anthropic/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-26 21:50:36.628324 anthropic-0.3.8/src/anthropic/_base_exceptions.py
+-rw-r--r--   0        0        0    15760 2023-08-02 20:24:32.283135 anthropic-0.3.8/src/anthropic/_client.py
+-rw-r--r--   0        0        0      112 2023-06-26 21:50:36.628774 anthropic-0.3.8/src/anthropic/_constants.py
+-rw-r--r--   0        0        0     1285 2023-06-26 21:50:36.628893 anthropic-0.3.8/src/anthropic/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-26 21:50:36.629012 anthropic-0.3.8/src/anthropic/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-26 21:50:36.629146 anthropic-0.3.8/src/anthropic/_qs.py
+-rw-r--r--   0        0        0      896 2023-06-26 21:50:36.629271 anthropic-0.3.8/src/anthropic/_resource.py
+-rw-r--r--   0        0        0     7126 2023-06-26 21:50:36.629400 anthropic-0.3.8/src/anthropic/_streaming.py
+-rw-r--r--   0        0        0     1186 2023-07-11 13:43:09.484957 anthropic-0.3.8/src/anthropic/_tokenizers.py
+-rw-r--r--   0        0        0     4230 2023-06-26 21:50:36.629650 anthropic-0.3.8/src/anthropic/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-26 21:50:36.629824 anthropic-0.3.8/src/anthropic/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-26 21:50:36.629952 anthropic-0.3.8/src/anthropic/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-26 21:50:36.630107 anthropic-0.3.8/src/anthropic/_utils/_utils.py
+-rw-r--r--   0        0        0      128 2023-08-02 20:24:32.283360 anthropic-0.3.8/src/anthropic/_version.py
+-rw-r--r--   0        0        0      168 2023-06-26 21:50:36.630485 anthropic-0.3.8/src/anthropic/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-26 21:50:36.630566 anthropic-0.3.8/src/anthropic/py.typed
+-rw-r--r--   0        0        0      156 2023-06-26 21:50:36.630819 anthropic-0.3.8/src/anthropic/resources/__init__.py
+-rw-r--r--   0        0        0    21781 2023-07-19 23:00:27.618209 anthropic-0.3.8/src/anthropic/resources/completions.py
+-rw-r--r--   0        0        0  1774213 2023-06-26 21:50:36.640575 anthropic-0.3.8/src/anthropic/tokenizer.json
+-rw-r--r--   0        0        0      226 2023-06-26 21:50:36.640828 anthropic-0.3.8/src/anthropic/types/__init__.py
+-rw-r--r--   0        0        0      664 2023-06-26 21:50:36.640952 anthropic-0.3.8/src/anthropic/types/completion.py
+-rw-r--r--   0        0        0     7111 2023-07-19 23:00:27.618522 anthropic-0.3.8/src/anthropic/types/completion_create_params.py
+-rw-r--r--   0        0        0    11137 1970-01-01 00:00:00.000000 anthropic-0.3.8/PKG-INFO
```

### Comparing `anthropic-0.3.7/LICENSE` & `anthropic-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/README.md` & `anthropic-0.3.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -166,14 +166,23 @@
 
 ## Using Types
 
 Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict), while responses are [Pydantic](https://pydantic-docs.helpmanual.io/) models. This helps provide autocomplete and documentation within your editor.
 
 If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `"basic"`.
 
+## Token counting
+
+You can estimate billing for a given request with the `client.count_tokens()` method, eg:
+
+```py
+client = Anthropic()
+client.count_tokens('Hello world!')  # 3
+```
+
 ## Handling errors
 
 When the library is unable to connect to the API (e.g., due to network connection problems or a timeout), a subclass of `anthropic.APIConnectionError` is raised.
 
 When the API returns a non-success status code (i.e., 4xx or 5xx
 response), a subclass of `anthropic.APIStatusError` will be raised, containing `status_code` and `response` properties.
 
@@ -237,23 +246,23 @@
     max_tokens_to_sample=300,
     model="claude-2",
 )
 ```
 
 ### Timeouts
 
-Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
+Requests time out after 10 minutes by default. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
 
 ```python
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 
 # Configure the default for all requests:
 anthropic = Anthropic(
-    # default is 60s
+    # default is 10 minutes
     timeout=20.0,
 )
 
 # More granular control:
 anthropic = Anthropic(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
```

### Comparing `anthropic-0.3.7/pyproject.toml` & `anthropic-0.3.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anthropic"
-version = "0.3.7"
+version = "0.3.8"
 description = "Client library for the anthropic API"
 readme = "README.md"
 authors = ["Anthropic <support@anthropic.com>"]
 license = "MIT"
 repository = "https://github.com/anthropics/anthropic-sdk-python"
 packages = [
   { include = "anthropic", from = "src" }
@@ -16,15 +16,15 @@
 pydantic = "^1.9.0"
 typing-extensions = ">= 4.1.1, < 5"
 anyio = ">= 3.5.0, < 4"
 distro = ">= 1.7.0, < 2"
 tokenizers = ">= 0.13.0"
 
 [tool.poetry.group.dev.dependencies]
-pyright = "1.1.297"
+pyright = "1.1.318"
 mypy = "1.1.1"
 black = "22.10.0"
 respx = "0.19.2"
 pytest = "7.1.1"
 pytest-asyncio = "0.18.3"
 ruff = "0.0.239"
 isort = "5.10.1"
```

### Comparing `anthropic-0.3.7/src/anthropic/__init__.py` & `anthropic-0.3.8/src/anthropic/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_base_client.py` & `anthropic-0.3.8/src/anthropic/_base_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -830,15 +830,15 @@
 
     def _request_api_list(
         self,
         model: Type[ModelT],
         page: Type[SyncPageT],
         options: FinalRequestOptions,
     ) -> SyncPageT:
-        resp = cast(SyncPageT, self.request(page, options, stream=False))
+        resp = self.request(page, options, stream=False)
         resp._set_private_attributes(  # pyright: ignore[reportPrivateUsage]
             client=self,
             model=model,
             options=options,
         )
         return resp
 
@@ -951,38 +951,38 @@
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="patch", url=path, json_data=body, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def put(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         files: RequestFiles | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="put", url=path, json_data=body, files=files, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def delete(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         body: Body | None = None,
         options: RequestOptions = {},
     ) -> ResponseT:
         opts = FinalRequestOptions.construct(method="delete", url=path, json_data=body, **options)
-        return cast(ResponseT, self.request(cast_to, opts))
+        return self.request(cast_to, opts)
 
     def get_api_list(
         self,
         path: str,
         *,
         model: Type[ModelT],
         page: Type[SyncPageT],
```

### Comparing `anthropic-0.3.7/src/anthropic/_base_exceptions.py` & `anthropic-0.3.8/src/anthropic/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_client.py` & `anthropic-0.3.8/src/anthropic/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import asyncio
 from typing import Union, Mapping, Optional
 
 import httpx
 from tokenizers import Tokenizer  # type: ignore[import]
 
-from . import resources
+from . import resources, _constants
 from ._qs import Querystring
 from ._types import (
     NOT_GIVEN,
     Omit,
     Headers,
     Timeout,
     NotGiven,
@@ -49,14 +49,18 @@
 class Anthropic(SyncAPIClient):
     completions: resources.Completions
 
     # client options
     api_key: str | None
     auth_token: str | None
 
+    # constants
+    HUMAN_PROMPT = _constants.HUMAN_PROMPT
+    AI_PROMPT = _constants.AI_PROMPT
+
     def __init__(
         self,
         *,
         auth_token: str | None = None,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         timeout: Union[float, Timeout, None] = DEFAULT_TIMEOUT,
@@ -236,14 +240,18 @@
 class AsyncAnthropic(AsyncAPIClient):
     completions: resources.AsyncCompletions
 
     # client options
     api_key: str | None
     auth_token: str | None
 
+    # constants
+    HUMAN_PROMPT = _constants.HUMAN_PROMPT
+    AI_PROMPT = _constants.AI_PROMPT
+
     def __init__(
         self,
         *,
         auth_token: str | None = None,
         base_url: Optional[str] = None,
         api_key: Optional[str] = None,
         timeout: Union[float, Timeout, None] = DEFAULT_TIMEOUT,
```

### Comparing `anthropic-0.3.7/src/anthropic/_exceptions.py` & `anthropic-0.3.8/src/anthropic/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_models.py` & `anthropic-0.3.8/src/anthropic/_models.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_qs.py` & `anthropic-0.3.8/src/anthropic/_qs.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_resource.py` & `anthropic-0.3.8/src/anthropic/_resource.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_streaming.py` & `anthropic-0.3.8/src/anthropic/_streaming.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_tokenizers.py` & `anthropic-0.3.8/src/anthropic/_tokenizers.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_types.py` & `anthropic-0.3.8/src/anthropic/_types.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_utils/__init__.py` & `anthropic-0.3.8/src/anthropic/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_utils/_transform.py` & `anthropic-0.3.8/src/anthropic/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/_utils/_utils.py` & `anthropic-0.3.8/src/anthropic/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/resources/completions.py` & `anthropic-0.3.8/src/anthropic/resources/completions.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/tokenizer.json` & `anthropic-0.3.8/src/anthropic/tokenizer.json`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/types/completion.py` & `anthropic-0.3.8/src/anthropic/types/completion.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/src/anthropic/types/completion_create_params.py` & `anthropic-0.3.8/src/anthropic/types/completion_create_params.py`

 * *Files identical despite different names*

### Comparing `anthropic-0.3.7/PKG-INFO` & `anthropic-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthropic
-Version: 0.3.7
+Version: 0.3.8
 Summary: Client library for the anthropic API
 Home-page: https://github.com/anthropics/anthropic-sdk-python
 License: MIT
 Author: Anthropic
 Author-email: support@anthropic.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -191,14 +191,23 @@
 
 ## Using Types
 
 Nested request parameters are [TypedDicts](https://docs.python.org/3/library/typing.html#typing.TypedDict), while responses are [Pydantic](https://pydantic-docs.helpmanual.io/) models. This helps provide autocomplete and documentation within your editor.
 
 If you would like to see type errors in VS Code to help catch bugs earlier, set `python.analysis.typeCheckingMode` to `"basic"`.
 
+## Token counting
+
+You can estimate billing for a given request with the `client.count_tokens()` method, eg:
+
+```py
+client = Anthropic()
+client.count_tokens('Hello world!')  # 3
+```
+
 ## Handling errors
 
 When the library is unable to connect to the API (e.g., due to network connection problems or a timeout), a subclass of `anthropic.APIConnectionError` is raised.
 
 When the API returns a non-success status code (i.e., 4xx or 5xx
 response), a subclass of `anthropic.APIStatusError` will be raised, containing `status_code` and `response` properties.
 
@@ -262,23 +271,23 @@
     max_tokens_to_sample=300,
     model="claude-2",
 )
 ```
 
 ### Timeouts
 
-Requests time out after 60 seconds by default. You can configure this with a `timeout` option,
+Requests time out after 10 minutes by default. You can configure this with a `timeout` option,
 which accepts a float or an [`httpx.Timeout`](https://www.python-httpx.org/advanced/#fine-tuning-the-configuration):
 
 ```python
 from anthropic import Anthropic, HUMAN_PROMPT, AI_PROMPT
 
 # Configure the default for all requests:
 anthropic = Anthropic(
-    # default is 60s
+    # default is 10 minutes
     timeout=20.0,
 )
 
 # More granular control:
 anthropic = Anthropic(
     timeout=httpx.Timeout(60.0, read=5.0, write=10.0, connect=2.0),
 )
```


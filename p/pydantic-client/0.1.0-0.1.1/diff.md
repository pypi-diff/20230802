# Comparing `tmp/pydantic_client-0.1.0.tar.gz` & `tmp/pydantic_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_client-0.1.0.tar", max compression
+gzip compressed data, was "pydantic_client-0.1.1.tar", max compression
```

## Comparing `pydantic_client-0.1.0.tar` & `pydantic_client-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-07-27 06:51:55.648483 pydantic_client-0.1.0/LICENSE
--rw-r--r--   0        0        0      716 2023-07-28 06:12:48.635050 pydantic_client-0.1.0/README.md
--rw-r--r--   0        0        0      201 2023-07-28 06:12:48.636548 pydantic_client-0.1.0/pydantic_client/__init__.py
--rw-r--r--   0        0        0        0 2023-07-28 06:12:48.636631 pydantic_client-0.1.0/pydantic_client/clients/__init__.py
--rw-r--r--   0        0        0      213 2023-07-28 06:12:48.636930 pydantic_client-0.1.0/pydantic_client/clients/abstract_client.py
--rw-r--r--   0        0        0     1185 2023-07-28 06:12:48.637113 pydantic_client-0.1.0/pydantic_client/clients/aiohttp_client.py
--rw-r--r--   0        0        0      948 2023-07-28 06:12:48.637293 pydantic_client-0.1.0/pydantic_client/clients/requests_client.py
--rw-r--r--   0        0        0      606 2023-07-28 06:12:48.637757 pydantic_client-0.1.0/pydantic_client/decorators.py
--rw-r--r--   0        0        0       78 2023-07-28 06:12:48.638209 pydantic_client-0.1.0/pydantic_client/errors.py
--rw-r--r--   0        0        0     2018 2023-07-28 06:12:48.638415 pydantic_client-0.1.0/pydantic_client/proxy.py
--rw-r--r--   0        0        0        0 2023-07-28 06:12:48.638486 pydantic_client-0.1.0/pydantic_client/schema/__init__.py
--rw-r--r--   0        0        0      192 2023-07-28 06:12:48.638876 pydantic_client-0.1.0/pydantic_client/schema/http_request.py
--rw-r--r--   0        0        0      435 2023-07-28 06:12:48.639183 pydantic_client-0.1.0/pydantic_client/schema/method_info.py
--rw-r--r--   0        0        0      621 2023-07-28 06:12:48.639642 pydantic_client-0.1.0/pydantic_client/utility.py
--rw-r--r--   0        0        0      581 2023-07-28 06:12:48.639886 pydantic_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 pydantic_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-27 06:51:55.648483 pydantic_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0      853 2023-08-02 10:15:45.513842 pydantic_client-0.1.1/README.md
+-rw-r--r--   0        0        0      272 2023-08-02 10:15:45.514567 pydantic_client-0.1.1/pydantic_client/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:12:48.636631 pydantic_client-0.1.1/pydantic_client/clients/__init__.py
+-rw-r--r--   0        0        0      213 2023-07-28 06:12:48.636930 pydantic_client-0.1.1/pydantic_client/clients/abstract_client.py
+-rw-r--r--   0        0        0     1185 2023-07-28 06:12:48.637113 pydantic_client-0.1.1/pydantic_client/clients/aiohttp_client.py
+-rw-r--r--   0        0        0      948 2023-07-28 06:12:48.637293 pydantic_client-0.1.1/pydantic_client/clients/requests_client.py
+-rw-r--r--   0        0        0      606 2023-07-28 06:12:48.637757 pydantic_client-0.1.1/pydantic_client/decorators.py
+-rw-r--r--   0        0        0       78 2023-07-28 06:12:48.638209 pydantic_client-0.1.1/pydantic_client/errors.py
+-rw-r--r--   0        0        0     2294 2023-08-02 10:15:45.515260 pydantic_client-0.1.1/pydantic_client/proxy.py
+-rw-r--r--   0        0        0        0 2023-07-28 06:12:48.638486 pydantic_client-0.1.1/pydantic_client/schema/__init__.py
+-rw-r--r--   0        0        0      192 2023-07-28 06:12:48.638876 pydantic_client-0.1.1/pydantic_client/schema/http_request.py
+-rw-r--r--   0        0        0      435 2023-07-28 06:12:48.639183 pydantic_client-0.1.1/pydantic_client/schema/method_info.py
+-rw-r--r--   0        0        0      621 2023-07-28 06:12:48.639642 pydantic_client-0.1.1/pydantic_client/utility.py
+-rw-r--r--   0        0        0      581 2023-08-02 10:15:45.516262 pydantic_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 pydantic_client-0.1.1/PKG-INFO
```

### Comparing `pydantic_client-0.1.0/LICENSE` & `pydantic_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.0/README.md` & `pydantic_client-0.1.1/pydantic_client/clients/requests_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,35 @@
-# pydantic-client
-Http client base pydantic, with requests or aiohttp
+from typing import Any
+from urllib.parse import urljoin
 
-### How to use
+from requests import Session
 
-```python
-from typing import List
-
-import requests
-from pydantic import BaseModel
-
-from pydantic_client import RequestsClient, rest
-
-
-class Book(BaseModel):
-    name: str
-    address: str
-
-
-class Books(BaseModel):
-    books: List[Book]
-
-
-class MyClient(RequestsClient):
-
-    @rest("/books?name={name}")
-    def get_books(self, name: str) -> Books:
-        ...
-
-    @rest("/books/{book_id}")
-    def get_book(self, book_id: int) -> Book:
-        ...
-
-    @rest("/books", method="POST")
-    def create_book(self, book: Book) -> Book:
-        ...
-
-
-my_client = MyClient(requests.Session())
-get_book: Book = my_client.get_book(1)
-```
+from pydantic_client.clients.abstract_client import AbstractClient
+from pydantic_client.proxy import ClientProxy
+from pydantic_client.schema.http_request import HttpRequest
+
+
+class RequestsClient(AbstractClient):
+
+    runner_class = ClientProxy
+
+    def __init__(self, base_url: str, session: Session = Session()):
+        self.session = session
+        self.base_url = base_url
+
+    def do_request(self, request: HttpRequest) -> Any:
+        if request.data:
+            data = request.data
+            json = {}
+        else:
+            data = {}
+            json = request.json_body
+
+        try:
+            return self.session.request(
+                url=urljoin(self.base_url, request.url),
+                method=request.method,
+                json=json,
+                data=data,
+            )
+        except BaseException as e:
+            raise e
```

### Comparing `pydantic_client-0.1.0/pydantic_client/clients/aiohttp_client.py` & `pydantic_client-0.1.1/pydantic_client/clients/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.0/pydantic_client/decorators.py` & `pydantic_client-0.1.1/pydantic_client/decorators.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.0/pydantic_client/proxy.py` & `pydantic_client-0.1.1/pydantic_client/proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import inspect
 import logging
 import re
 from typing import Any, Dict
+from urllib.parse import urlparse
 
 from pydantic_client.clients.abstract_client import AbstractClient
 from pydantic_client.schema.http_request import HttpRequest
 from pydantic_client.schema.method_info import MethodInfo
 
 logger = logging.getLogger(__name__)
 
@@ -22,24 +23,30 @@
             self.method_info.func, self.instance, *args, **kwargs,
         )
         f.pop("self", None)
         return f
 
     def _get_url(self, args) -> str:
         keys = self.querystring_pattern.findall(self.method_info.url)
-        query_args = {arg: val for arg, val in args.items() if arg in keys}
-        return self.method_info.url.format(**query_args)
+        query_args = {arg: val for arg, val in args.items() if arg in keys and val}
+        url = self.method_info.url.format(**query_args)
+
+        url_result = urlparse(url)
+        if "{" in url_result.path:
+            logger.warning(f"Not formatted args in url path: {url}")
+
+        querystring = "&".join(
+            f"{k}={v}" for k, v in url_result.query if "{" not in v
+        )
+        return url_result.path + "?" + querystring if querystring else url_result.path
 
     def get_request(self, *args, **kwargs):
         func_args: Dict[str, Any] = self._apply_args(*args, **kwargs)
 
         url: str = self._get_url(func_args)
-        if "{" in url and "}" in url:
-            logger.warning(f"Not formatted args in url: {url}")
-
         if self.method_info.form_body:
             data, json = func_args, {}
         else:
             data, json = {}, func_args
 
         return HttpRequest(
             url=url,
```

### Comparing `pydantic_client-0.1.0/pydantic_client/utility.py` & `pydantic_client-0.1.1/pydantic_client/utility.py`

 * *Files identical despite different names*

### Comparing `pydantic_client-0.1.0/pyproject.toml` & `pydantic_client-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "Http client base pydantic, with requests or aiohttp"
 authors = ["ponytailer <huangxiaohen2738@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "pydantic_client" }]
 homepage = "https://github.com/ponytailer/pydantic-client"
 
 [[tool.poetry.source]]
```


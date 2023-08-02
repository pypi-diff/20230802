# Comparing `tmp/starlette_logger-0.0.3.tar.gz` & `tmp/starlette_logger-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_logger-0.0.3.tar", last modified: Wed Aug  2 14:24:46 2023, max compression
+gzip compressed data, was "starlette_logger-0.0.4.tar", last modified: Wed Aug  2 14:52:18 2023, max compression
```

## Comparing `starlette_logger-0.0.3.tar` & `starlette_logger-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.3/.gitignore
--rw-r--r--   0        0        0      184 2023-08-02 14:19:41.852433 starlette_logger-0.0.3/Pipfile
--rw-r--r--   0        0        0     3414 2023-08-02 14:19:52.885032 starlette_logger-0.0.3/Pipfile.lock
--rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.3/README.md
--rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      293 2023-08-02 14:20:44.902643 starlette_logger-0.0.3/starlette_logger/__init__.py
--rw-r--r--   0        0        0     3140 2023-08-02 14:10:16.191678 starlette_logger-0.0.3/starlette_logger/middleware.py
--rw-r--r--   0        0        0        0 2023-08-02 14:12:26.620189 starlette_logger-0.0.3/tests/__init__.py
--rw-r--r--   0        0        0      325 2023-08-02 14:19:17.575597 starlette_logger-0.0.3/tests/test_request_id_middleware.py
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.4/.gitignore
+-rw-r--r--   0        0        0      196 2023-08-02 14:38:34.248701 starlette_logger-0.0.4/Pipfile
+-rw-r--r--   0        0        0     5733 2023-08-02 14:37:47.141456 starlette_logger-0.0.4/Pipfile.lock
+-rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.4/README.md
+-rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-08-02 14:52:11.129368 starlette_logger-0.0.4/starlette_logger/__init__.py
+-rw-r--r--   0        0        0     3504 2023-08-02 14:51:14.340113 starlette_logger-0.0.4/starlette_logger/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:12:26.620189 starlette_logger-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-02 14:47:00.858324 starlette_logger-0.0.4/tests/test_request_id_middleware.py
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.4/PKG-INFO
```

### Comparing `starlette_logger-0.0.3/.gitignore` & `starlette_logger-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `starlette_logger-0.0.3/Pipfile.lock` & `starlette_logger-0.0.4/Pipfile.lock`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8835227272727272%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'0296df2bb27909ad0b7b08d64dd9466fffea6addb592d1d5f6736ad7cb52fadc'}}",*

 * * "'develop'": "{'anyio': OrderedDict([('hashes', "*

 * *              "['sha256:44a3c9aba0f5defa43261a8b3efb97891f2bd7d804e0e1f56419befa1adfc780', "*

 * *              "'sha256:91dee416e570e92c64041bd18b900d1d6fa78dff7048769ce5ac5ddad004fbb5']), "*

 * *              '(\'markers\', "python_version >= \'3.7\'"), (\'version\', \'==3.7.1\')]), '*

 * *              "'certifi': OrderedDict([('hashes', "*

 * *             […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "c23bfeab0223d5657036d44bb2e0798a9407c7e1d20ecb4125390f4dbd82710d"
+            "sha256": "0296df2bb27909ad0b7b08d64dd9466fffea6addb592d1d5f6736ad7cb52fadc"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.11"
         },
         "sources": [
             {
@@ -54,14 +54,62 @@
                 "sha256:79b9e68e48b54e373441e130fa447944e6f87a05b35de23138e475c05d0f7e0e"
             ],
             "index": "pypi",
             "version": "==23.1.0"
         }
     },
     "develop": {
+        "anyio": {
+            "hashes": [
+                "sha256:44a3c9aba0f5defa43261a8b3efb97891f2bd7d804e0e1f56419befa1adfc780",
+                "sha256:91dee416e570e92c64041bd18b900d1d6fa78dff7048769ce5ac5ddad004fbb5"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==3.7.1"
+        },
+        "certifi": {
+            "hashes": [
+                "sha256:539cc1d13202e33ca466e88b2807e29f4c13049d6d87031a3c110744495cb082",
+                "sha256:92d6037539857d8206b8f6ae472e8b77db8058fec5937a1ef3f54304089edbb9"
+            ],
+            "markers": "python_version >= '3.6'",
+            "version": "==2023.7.22"
+        },
+        "h11": {
+            "hashes": [
+                "sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d",
+                "sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.14.0"
+        },
+        "httpcore": {
+            "hashes": [
+                "sha256:a6f30213335e34c1ade7be6ec7c47f19f50c56db36abef1a9dfa3815b1cb3888",
+                "sha256:c2789b767ddddfa2a5782e3199b2b7f6894540b17b16ec26b2c4d8e103510b87"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==0.17.3"
+        },
+        "httpx": {
+            "hashes": [
+                "sha256:06781eb9ac53cde990577af654bd990a4949de37a28bdb4a230d434f3a30b9bd",
+                "sha256:5853a43053df830c20f8110c5e69fe44d035d850b2dfe795e196f00fdb774bdd"
+            ],
+            "index": "pypi",
+            "version": "==0.24.1"
+        },
+        "idna": {
+            "hashes": [
+                "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
+                "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
+            ],
+            "markers": "python_version >= '3.5'",
+            "version": "==3.4"
+        },
         "iniconfig": {
             "hashes": [
                 "sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3",
                 "sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==2.0.0"
@@ -85,10 +133,18 @@
         "pytest": {
             "hashes": [
                 "sha256:78bf16451a2eb8c7a2ea98e32dc119fd2aa758f1d5d66dbf0a59d69a3969df32",
                 "sha256:b4bf8c45bd59934ed84001ad51e11b4ee40d40a1229d2c79f9c592b0a3f6bd8a"
             ],
             "index": "pypi",
             "version": "==7.4.0"
+        },
+        "sniffio": {
+            "hashes": [
+                "sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101",
+                "sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384"
+            ],
+            "markers": "python_version >= '3.7'",
+            "version": "==1.3.0"
         }
     }
 }
```

### Comparing `starlette_logger-0.0.3/starlette_logger/middleware.py` & `starlette_logger-0.0.4/starlette_logger/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import time
 import uuid
 from typing import Dict
 
+from starlette.datastructures import MutableHeaders
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from structlog import get_logger
 from structlog.contextvars import bind_contextvars, clear_contextvars, get_contextvars
 
 
 class ContextVars:
@@ -35,29 +36,34 @@
 
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> None:
         request_id = request.headers.get("x-request-id")
         if not request.headers.get("x-request-id"):
             request_id = str(uuid.uuid4())
-            self._logger.debug(
+            log_call = self._logger.debug(
                 "request id generated by application because none was provided",
                 reqId=request_id,
             )
-            request.headers["X-Request-Id"] = request_id
+            if log_call:
+                await log_call
+            mutable_headers = MutableHeaders(request._headers)
+            mutable_headers["X-Request-Id"] = request_id
+            request._headers = mutable_headers
+            request.scope.update(headers=request.headers.raw)
 
         inject_tracing_parameters = {"reqId": request_id}
 
         try:
             with ContextVars(**inject_tracing_parameters):
                 response = await call_next(request)
         except Exception as e:
             raise e
 
-        response.headers["X-Request-ID"] = request_id
+        response.headers["X-Request-Id"] = request_id
 
         return response
 
 
 class RequestLoggerMiddleware(BaseHTTPMiddleware):
     """
     Middleware that logs request information to structlog.
@@ -92,11 +98,13 @@
             raise error
         finally:
             end_time = time.perf_counter()
             request_metadata["duration"] = end_time - start_time
 
             if response:
                 request_metadata["status"] = response.status_code
-
-            await self._logger.info("http request", **request_metadata)
+            
+            log_call = self._logger.info("http request", **request_metadata)
+            if log_call:
+                await log_call
 
         return response
```


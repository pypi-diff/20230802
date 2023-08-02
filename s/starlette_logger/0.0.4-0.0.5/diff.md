# Comparing `tmp/starlette_logger-0.0.4.tar.gz` & `tmp/starlette_logger-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_logger-0.0.4.tar", last modified: Wed Aug  2 14:52:18 2023, max compression
+gzip compressed data, was "starlette_logger-0.0.5.tar", last modified: Wed Aug  2 15:41:01 2023, max compression
```

## Comparing `starlette_logger-0.0.4.tar` & `starlette_logger-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.4/.gitignore
--rw-r--r--   0        0        0      196 2023-08-02 14:38:34.248701 starlette_logger-0.0.4/Pipfile
--rw-r--r--   0        0        0     5733 2023-08-02 14:37:47.141456 starlette_logger-0.0.4/Pipfile.lock
--rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.4/README.md
--rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      293 2023-08-02 14:52:11.129368 starlette_logger-0.0.4/starlette_logger/__init__.py
--rw-r--r--   0        0        0     3504 2023-08-02 14:51:14.340113 starlette_logger-0.0.4/starlette_logger/middleware.py
--rw-r--r--   0        0        0        0 2023-08-02 14:12:26.620189 starlette_logger-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      873 2023-08-02 14:47:00.858324 starlette_logger-0.0.4/tests/test_request_id_middleware.py
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.5/.gitignore
+-rw-r--r--   0        0        0      196 2023-08-02 14:38:34.248701 starlette_logger-0.0.5/Pipfile
+-rw-r--r--   0        0        0     5733 2023-08-02 14:37:47.141456 starlette_logger-0.0.5/Pipfile.lock
+-rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.5/README.md
+-rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-08-02 15:39:44.526364 starlette_logger-0.0.5/starlette_logger/__init__.py
+-rw-r--r--   0        0        0     3479 2023-08-02 15:40:15.482205 starlette_logger-0.0.5/starlette_logger/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:12:26.620189 starlette_logger-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0      873 2023-08-02 14:47:00.858324 starlette_logger-0.0.5/tests/test_request_id_middleware.py
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.5/PKG-INFO
```

### Comparing `starlette_logger-0.0.4/.gitignore` & `starlette_logger-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `starlette_logger-0.0.4/Pipfile.lock` & `starlette_logger-0.0.5/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `starlette_logger-0.0.4/starlette_logger/middleware.py` & `starlette_logger-0.0.5/starlette_logger/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import time
 import uuid
 from typing import Dict
 
 from starlette.datastructures import MutableHeaders
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
-from structlog import get_logger
 from structlog.contextvars import bind_contextvars, clear_contextvars, get_contextvars
 
 
 class ContextVars:
     __original_context_vars: Dict
 
     def __init__(self, **kwargs):
@@ -27,16 +26,17 @@
 
 class RequestIdMiddleware(BaseHTTPMiddleware):
     """
     Middleware that injects a request id if none is set by caller.
     """
 
     def __init__(self, *args, **kwds) -> None:
+        self._logger = kwds["logger"]
+        del kwds["logger"]
         super().__init__(*args, **kwds)
-        self._logger = get_logger("middleware.request_id")
 
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> None:
         request_id = request.headers.get("x-request-id")
         if not request.headers.get("x-request-id"):
             request_id = str(uuid.uuid4())
@@ -66,16 +66,17 @@
 
 class RequestLoggerMiddleware(BaseHTTPMiddleware):
     """
     Middleware that logs request information to structlog.
     """
 
     def __init__(self, *args, **kwds) -> None:
+        self._logger = kwds["logger"]
+        del kwds["logger"]
         super().__init__(*args, **kwds)
-        self._logger = get_logger("middleware.request_logger")
 
     def _extract_request_metadata(self, request: Request) -> Dict:
         return {
             "agent": request.headers.get("user-agent"),
             "ip": str(request.client.host),
             "method": str(request.method),
             "path": str(request.url.path),
```

### Comparing `starlette_logger-0.0.4/tests/test_request_id_middleware.py` & `starlette_logger-0.0.5/tests/test_request_id_middleware.py`

 * *Files identical despite different names*


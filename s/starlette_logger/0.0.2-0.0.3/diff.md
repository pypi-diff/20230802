# Comparing `tmp/starlette_logger-0.0.2.tar.gz` & `tmp/starlette_logger-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_logger-0.0.2.tar", last modified: Wed Aug  2 11:35:17 2023, max compression
+gzip compressed data, was "starlette_logger-0.0.3.tar", last modified: Wed Aug  2 14:24:46 2023, max compression
```

## Comparing `starlette_logger-0.0.2.tar` & `starlette_logger-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.2/.gitignore
--rw-r--r--   0        0        0      171 2023-08-02 09:20:34.865349 starlette_logger-0.0.2/Pipfile
--rw-r--r--   0        0        0     2090 2023-08-02 09:20:35.615830 starlette_logger-0.0.2/Pipfile.lock
--rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.2/README.md
--rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      293 2023-08-02 11:34:41.374421 starlette_logger-0.0.2/starlette_logger/__init__.py
--rw-r--r--   0        0        0     3134 2023-08-02 08:28:11.427297 starlette_logger-0.0.2/starlette_logger/middleware.py
--rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3078 2023-08-02 06:03:28.269331 starlette_logger-0.0.3/.gitignore
+-rw-r--r--   0        0        0      184 2023-08-02 14:19:41.852433 starlette_logger-0.0.3/Pipfile
+-rw-r--r--   0        0        0     3414 2023-08-02 14:19:52.885032 starlette_logger-0.0.3/Pipfile.lock
+-rw-r--r--   0        0        0       75 2023-08-02 06:03:28.269458 starlette_logger-0.0.3/README.md
+-rw-r--r--   0        0        0      488 2023-08-02 11:31:48.594446 starlette_logger-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      293 2023-08-02 14:20:44.902643 starlette_logger-0.0.3/starlette_logger/__init__.py
+-rw-r--r--   0        0        0     3140 2023-08-02 14:10:16.191678 starlette_logger-0.0.3/starlette_logger/middleware.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:12:26.620189 starlette_logger-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0      325 2023-08-02 14:19:17.575597 starlette_logger-0.0.3/tests/test_request_id_middleware.py
+-rw-r--r--   0        0        0      491 1970-01-01 00:00:00.000000 starlette_logger-0.0.3/PKG-INFO
```

### Comparing `starlette_logger-0.0.2/.gitignore` & `starlette_logger-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `starlette_logger-0.0.2/starlette_logger/middleware.py` & `starlette_logger-0.0.3/starlette_logger/middleware.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class RequestIdMiddleware(BaseHTTPMiddleware):
     """
     Middleware that injects a request id if none is set by caller.
     """
 
     def __init__(self, *args, **kwds) -> None:
-        super().__init__(args, kwds)
+        super().__init__(*args, **kwds)
         self._logger = get_logger("middleware.request_id")
 
     async def dispatch(
         self, request: Request, call_next: RequestResponseEndpoint
     ) -> None:
         request_id = request.headers.get("x-request-id")
         if not request.headers.get("x-request-id"):
@@ -60,15 +60,15 @@
 
 class RequestLoggerMiddleware(BaseHTTPMiddleware):
     """
     Middleware that logs request information to structlog.
     """
 
     def __init__(self, *args, **kwds) -> None:
-        super().__init__(args, kwds)
+        super().__init__(*args, **kwds)
         self._logger = get_logger("middleware.request_logger")
 
     def _extract_request_metadata(self, request: Request) -> Dict:
         return {
             "agent": request.headers.get("user-agent"),
             "ip": str(request.client.host),
             "method": str(request.method),
```


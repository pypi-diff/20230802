# Comparing `tmp/jupyverse_api-0.2.0.tar.gz` & `tmp/jupyverse_api-0.2.1.tar.gz`

## Comparing `jupyverse_api-0.2.0.tar` & `jupyverse_api-0.2.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/cli.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/py.typed
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/README.md
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyverse_api-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5031 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2381 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/retrolab/__init__.py
+-rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/README.md
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 jupyverse_api-0.2.1/PKG-INFO
```

### Comparing `jupyverse_api-0.2.0/jupyverse_api/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse_api-0.2.0/jupyverse_api/cli.py` & `jupyverse_api-0.2.1/jupyverse_api/cli.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/app/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/app/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from collections import defaultdict
 from typing import Dict, List
 
 from fastapi import FastAPI
 
 from ..exceptions import RedirectException, _redirect_exception_handler
@@ -12,16 +14,21 @@
 
 class App:
     """A wrapper around FastAPI that checks for endpoint path conflicts."""
 
     _app: FastAPI
     _router_paths: Dict[str, List[str]]
 
-    def __init__(self, app: FastAPI):
-        self._app = app
+    def __init__(self, app: FastAPI, mount_path: str | None = None):
+        if mount_path is None:
+            self._app = app
+        else:
+            subapi = FastAPI()
+            app.mount(mount_path, subapi)
+            self._app = subapi
         app.add_exception_handler(RedirectException, _redirect_exception_handler)
         self._router_paths = defaultdict(list)
 
     @property
     def _paths(self):
         return [path for router, paths in self._router_paths.items() for path in paths]
```

### Comparing `jupyverse_api-0.2.0/jupyverse_api/auth/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/contents/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/contents/models.py` & `jupyverse_api-0.2.1/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/jupyterlab/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/kernels/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/kernels/models.py` & `jupyverse_api-0.2.1/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/lab/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/main/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/main/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,21 +9,29 @@
 from fastapi import FastAPI
 from pydantic import BaseModel
 
 from ..app import App
 
 
 class AppComponent(Component):
+    def __init__(
+        self,
+        *,
+        mount_path: str | None = None,
+    ) -> None:
+        super().__init__()
+        self.mount_path = mount_path
+
     async def start(
         self,
         ctx: Context,
     ) -> None:
         app = await ctx.request_resource(FastAPI)
 
-        _app = App(app)
+        _app = App(app, mount_path=self.mount_path)
         ctx.add_resource(_app)
 
 
 class JupyverseComponent(FastAPIComponent):
     def __init__(
         self,
         components: dict[str, dict[str, Any] | None] | None = None,
```

### Comparing `jupyverse_api-0.2.0/jupyverse_api/nbconvert/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/resource_usage/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/retrolab/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/retrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/terminals/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/jupyverse_api/yjs/__init__.py` & `jupyverse_api-0.2.1/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/.gitignore` & `jupyverse_api-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/COPYING.md` & `jupyverse_api-0.2.1/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/pyproject.toml` & `jupyverse_api-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse_api-0.2.0/PKG-INFO` & `jupyverse_api-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyverse_api
-Version: 0.2.0
+Version: 0.2.1
 Summary: The public API for Jupyverse
 Project-URL: Source, https://github.com/jupyter-server/jupyverse/jupyverse_api
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: api,jupyverse
 Classifier: Development Status :: 4 - Beta
```


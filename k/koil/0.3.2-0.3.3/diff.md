# Comparing `tmp/koil-0.3.2.tar.gz` & `tmp/koil-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "koil-0.3.2.tar", max compression
+gzip compressed data, was "koil-0.3.3.tar", max compression
```

## Comparing `koil-0.3.2.tar` & `koil-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3475 2022-03-02 12:09:12.548451 koil-0.3.2/README.md
--rw-r--r--   0        0        0      359 2022-04-12 08:39:04.407565 koil-0.3.2/koil/__init__.py
--rw-r--r--   0        0        0      116 2023-02-06 15:33:56.814184 koil-0.3.2/koil/composition/__init__.py
--rw-r--r--   0        0        0     2978 2023-07-26 13:35:45.096944 koil-0.3.2/koil/composition/base.py
--rw-r--r--   0        0        0     1052 2022-11-21 11:44:34.168046 koil-0.3.2/koil/composition/qt.py
--rw-r--r--   0        0        0     2980 2023-07-26 09:17:59.601113 koil-0.3.2/koil/decorators.py
--rw-r--r--   0        0        0      771 2023-07-19 16:54:53.430108 koil-0.3.2/koil/errors.py
--rw-r--r--   0        0        0    10113 2023-08-02 10:19:59.698656 koil-0.3.2/koil/helpers.py
--rw-r--r--   0        0        0     5131 2023-07-26 09:20:25.845722 koil-0.3.2/koil/koil.py
--rw-r--r--   0        0        0     1014 2023-07-19 14:15:35.493961 koil-0.3.2/koil/predicates.py
--rw-r--r--   0        0        0     8909 2023-08-02 09:46:40.942885 koil-0.3.2/koil/process.py
--rw-r--r--   0        0        0    10689 2023-07-26 09:17:59.909114 koil-0.3.2/koil/qt.py
--rw-r--r--   0        0        0     4501 2022-11-21 11:44:34.184046 koil-0.3.2/koil/task.py
--rw-r--r--   0        0        0      391 2022-03-28 11:51:32.994673 koil-0.3.2/koil/types.py
--rw-r--r--   0        0        0     6824 2022-03-25 16:39:20.667020 koil-0.3.2/koil/utils.py
--rw-r--r--   0        0        0     1164 2023-08-02 09:53:47.865048 koil-0.3.2/koil/vars.py
--rw-r--r--   0        0        0     1183 2023-08-02 12:01:14.266847 koil-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 koil-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3475 2022-03-02 12:09:12.548451 koil-0.3.3/README.md
+-rw-r--r--   0        0        0      359 2022-04-12 08:39:04.407565 koil-0.3.3/koil/__init__.py
+-rw-r--r--   0        0        0      116 2023-02-06 15:33:56.814184 koil-0.3.3/koil/composition/__init__.py
+-rw-r--r--   0        0        0     2978 2023-07-26 13:35:45.096944 koil-0.3.3/koil/composition/base.py
+-rw-r--r--   0        0        0     1052 2022-11-21 11:44:34.168046 koil-0.3.3/koil/composition/qt.py
+-rw-r--r--   0        0        0     2725 2023-08-02 12:39:51.924629 koil-0.3.3/koil/decorators.py
+-rw-r--r--   0        0        0      771 2023-07-19 16:54:53.430108 koil-0.3.3/koil/errors.py
+-rw-r--r--   0        0        0    10113 2023-08-02 10:19:59.698656 koil-0.3.3/koil/helpers.py
+-rw-r--r--   0        0        0     5033 2023-08-02 12:40:05.092706 koil-0.3.3/koil/koil.py
+-rw-r--r--   0        0        0     1014 2023-07-19 14:15:35.493961 koil-0.3.3/koil/predicates.py
+-rw-r--r--   0        0        0     8909 2023-08-02 09:46:40.942885 koil-0.3.3/koil/process.py
+-rw-r--r--   0        0        0    10689 2023-07-26 09:17:59.909114 koil-0.3.3/koil/qt.py
+-rw-r--r--   0        0        0     4501 2022-11-21 11:44:34.184046 koil-0.3.3/koil/task.py
+-rw-r--r--   0        0        0      391 2022-03-28 11:51:32.994673 koil-0.3.3/koil/types.py
+-rw-r--r--   0        0        0     6824 2022-03-25 16:39:20.667020 koil-0.3.3/koil/utils.py
+-rw-r--r--   0        0        0     1164 2023-08-02 09:53:47.865048 koil-0.3.3/koil/vars.py
+-rw-r--r--   0        0        0     1183 2023-08-02 12:40:09.716733 koil-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4301 1970-01-01 00:00:00.000000 koil-0.3.3/PKG-INFO
```

### Comparing `koil-0.3.2/README.md` & `koil-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/composition/base.py` & `koil-0.3.3/koil/composition/base.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/composition/qt.py` & `koil-0.3.3/koil/composition/qt.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/decorators.py` & `koil-0.3.3/koil/decorators.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,27 +40,23 @@
 
         def ___get_koiled_loop(self):
             return getattr(self, fieldname)
 
         def koiled_enter(self, *args, **kwargs):
             potential_koiled_loop = current_loop.get()
             if potential_koiled_loop is not None:
-                assert (
-                    getattr(self, fieldname, None) is None
-                ), f"You cannot enter a koil loop inside another koil loop. Do no set explicitly a Koil in {cls}. Found koiled loop {potential_koiled_loop}"
+                return unkoil(self.__aenter__, *args, **kwargs)
             else:
-                if getattr(self, fieldname, None) is None:
-                    setattr(
-                        self,
-                        fieldname,
-                        koil_class(creating_instance=self, **koilparams),
-                    )
+                setattr(
+                    self,
+                    fieldname,
+                    koil_class(name=f"{repr(self)}", **koilparams),
+                )
                 getattr(self, fieldname).__enter__()
-
-            return unkoil(self.__aenter__, *args, **kwargs)
+                return unkoil(self.__aenter__, *args, **kwargs)
 
         def koiled_exit(self, *args, **kwargs):
             unkoil(self.__aexit__, *args, **kwargs)
             koil = getattr(self, fieldname, None)
             if koil is not None:
                 koil.__exit__(None, None, None)
```

### Comparing `koil-0.3.2/koil/errors.py` & `koil-0.3.3/koil/errors.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/helpers.py` & `koil-0.3.3/koil/helpers.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/koil.py` & `koil-0.3.3/koil/koil.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 import os
 import sys
 import threading
 from typing import Any, Optional
 
 from koil.errors import ContextError
-from koil.vars import *
+from koil.vars import current_loop
 import time
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 try:
@@ -117,56 +117,55 @@
             if not hasattr(self, "sync_in_async") or self.sync_in_async is False:
                 raise ContextError(
                     "You are running in asyncio event loop already. Using koil makes no sense here, use asyncio instead. If this happens in a context manager, you probably forgot to use the `async with` syntax."
                 )
         except RuntimeError:
             pass
 
-        self._loop = current_loop.get()
-        assert (
-            self._loop is None
-        ), f"You are already in a koiled context. You can't nest koiled contexts. Omit creating a new Koil here {self._loop.name}"
-        # We are now creating a koiled loop for this context
-        self._loop = get_threaded_loop(
-            getattr(
-                self,
-                "name",
-                f"KoiledLoop {'governed by' + self.creating_instance.__class__.__name__ if getattr(self, 'creating_instance', None) else ''}",
-            ),
-            uvify=getattr(self, "uvify", True),
-        )
-        current_loop.set(self._loop)
+        self._loop = None
+        _loop = current_loop.get()
+        if _loop is None:
+            # We are now creating a koiled loop for this context
+            self._loop = get_threaded_loop(
+                getattr(
+                    self,
+                    "name",
+                    f"KoiledLoop {'governed by' + self.__class__.__name__ if getattr(self, 'creating_instance', None) else ''}",
+                ),
+                uvify=getattr(self, "uvify", True),
+            )
+            current_loop.set(self._loop)
         self.running = True
         return self
 
     async def __aloop_close(self):
         loop = asyncio.get_event_loop()
         logger.debug("Causing loop to stop")
         loop.stop()
 
     def __exit__(self, *args, **kwargs):
-        asyncio.run_coroutine_threadsafe(self.__aloop_close(), self._loop)
+        if self._loop:
+            self._loop.call_soon_threadsafe(self._loop.stop)
 
-        iterations = 0
+            iterations = 0
 
-        while self._loop.is_running():
-            time.sleep(0.001)
-            iterations += 1
-            if iterations == 100:
-                logger.warning(
-                    "Shutting Down takes longer than expected. Probably we are having loose Threads? Keyboard interrupt?"
-                )
+            while self._loop.is_running():
+                time.sleep(0.001)
+                iterations += 1
+                if iterations == 100:
+                    logger.warning(
+                        "Shutting Down takes longer than expected. Probably we are having loose Threads? Keyboard interrupt?"
+                    )
 
-        current_loop.set(None)
+            current_loop.set(None)
         self.running = False
 
 
 @dataclass
 class Koil(KoilMixin):
-    creating_instance: Optional[Any] = None
     "The instance that created this class through entering"
 
     uvify: bool = False
     """Shoul we run the loop with uvloop?"""
 
     name: str = "KoilLoop"
     """How would you like to name this loop"""
```

### Comparing `koil-0.3.2/koil/predicates.py` & `koil-0.3.3/koil/predicates.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/process.py` & `koil-0.3.3/koil/process.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/qt.py` & `koil-0.3.3/koil/qt.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/task.py` & `koil-0.3.3/koil/task.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/utils.py` & `koil-0.3.3/koil/utils.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/koil/vars.py` & `koil-0.3.3/koil/vars.py`

 * *Files identical despite different names*

### Comparing `koil-0.3.2/pyproject.toml` & `koil-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "koil"
-version = "0.3.2"
+version = "0.3.3"
 readme = "README.md"
 description = "Async for a sync world"
 authors = ["jhnnsrs <jhnnsrs@gmail.com>"]
 license = "CC BY-NC 3.0"
 packages = [{ include = "koil" }]
 
 [tool.poetry.dependencies]
```

### Comparing `koil-0.3.2/PKG-INFO` & `koil-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: koil
-Version: 0.3.2
+Version: 0.3.3
 Summary: Async for a sync world
 License: CC BY-NC 3.0
 Author: jhnnsrs
 Author-email: jhnnsrs@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


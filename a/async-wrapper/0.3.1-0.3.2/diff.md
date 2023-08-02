# Comparing `tmp/async_wrapper-0.3.1.tar.gz` & `tmp/async_wrapper-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.3.1.tar", max compression
+gzip compressed data, was "async_wrapper-0.3.2.tar", max compression
```

## Comparing `async_wrapper-0.3.1.tar` & `async_wrapper-0.3.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1070 2023-07-30 15:57:49.562929 async_wrapper-0.3.1/LICENSE
--rw-r--r--   0        0        0     1776 2023-07-30 15:57:49.562929 async_wrapper-0.3.1/README.md
--rw-r--r--   0        0        0     3535 2023-07-30 15:58:01.571217 async_wrapper-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      288 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-07-30 15:58:01.607218 async_wrapper-0.3.1/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      109 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/__init__.py
--rw-r--r--   0        0        0     1007 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_loky.py
--rw-r--r--   0        0        0      564 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_thread.py
--rw-r--r--   0        0        0      409 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/base.py
--rw-r--r--   0        0        0      654 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/main.py
--rw-r--r--   0        0        0     1721 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0      107 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/__init__.py
--rw-r--r--   0        0        0      983 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_loky.py
--rw-r--r--   0        0        0     1140 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_thread.py
--rw-r--r--   0        0        0     1136 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/base.py
--rw-r--r--   0        0        0      656 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/convert/synclib/main.py
--rw-r--r--   0        0        0        0 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      188 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0      104 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/exception.py
--rw-r--r--   0        0        0     8414 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/future.py
--rw-r--r--   0        0        0     5004 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0     2505 2023-07-30 15:57:49.566929 async_wrapper-0.3.1/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 async_wrapper-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/LICENSE
+-rw-r--r--   0        0        0     1776 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/README.md
+-rw-r--r--   0        0        0     3657 2023-08-02 13:23:50.142941 async_wrapper-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-02 13:23:50.210942 async_wrapper-0.3.2/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      109 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/__init__.py
+-rw-r--r--   0        0        0     1007 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_loky.py
+-rw-r--r--   0        0        0      564 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_thread.py
+-rw-r--r--   0        0        0      409 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/base.py
+-rw-r--r--   0        0        0      654 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/main.py
+-rw-r--r--   0        0        0     1721 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0      107 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/__init__.py
+-rw-r--r--   0        0        0      983 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_loky.py
+-rw-r--r--   0        0        0     1140 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_thread.py
+-rw-r--r--   0        0        0     1136 2023-08-02 13:23:32.758643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/base.py
+-rw-r--r--   0        0        0      656 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/convert/synclib/main.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      151 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0      104 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/exception.py
+-rw-r--r--   0        0        0     4440 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0     1354 2023-08-02 13:23:32.762643 async_wrapper-0.3.2/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0     2902 1970-01-01 00:00:00.000000 async_wrapper-0.3.2/PKG-INFO
```

### Comparing `async_wrapper-0.3.1/LICENSE` & `async_wrapper-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/README.md` & `async_wrapper-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/pyproject.toml` & `async_wrapper-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.3.1"
+version = "0.3.2"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
@@ -12,18 +12,20 @@
 [tool.poetry.dependencies]
 python = ">=3.8"
 typing-extensions = "^4.6.3"
 anyio = "^3.7.0"
 loky = { version = "^3.4.0", optional = true }
 cloudpickle = { version = "^2.2.1", optional = true }
 psutil = { version = "^5.9.5", optional = true }
+uvloop = { version = "^0.17.0", optional = true, markers = "platform_system != 'Windows'" }
 
 [tool.poetry.extras]
-all = ['loky', "cloudpickle", "psutil"]
+all = ['loky', "cloudpickle", "psutil", "uvloop"]
 loky = ['loky', "cloudpickle", "psutil"]
+uvloop = ['uvloop']
 
 [tool.poetry.group.dev.dependencies]
 ruff = "0.0.275"
 black = "23.3.0"
 ipykernel = "^6.23.3"
 pytest = "^7.4.0"
 pre-commit = "^3.3.3"
```

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_loky.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/_thread.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/asynclib/main.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/asynclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/main.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_loky.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_loky.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/_thread.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/synclib/_thread.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/base.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/synclib/base.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/convert/synclib/main.py` & `async_wrapper-0.3.2/src/async_wrapper/convert/synclib/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.3.1/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.3.2/src/async_wrapper/task_group/task_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 from __future__ import annotations
 
 from functools import partial, wraps
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Coroutine, Generic, TypeVar
-from weakref import WeakSet
 
 from anyio.abc import TaskGroup as _TaskGroup
-from typing_extensions import ParamSpec, Self, override
+from typing_extensions import Concatenate, ParamSpec, Self, override
 
-from async_wrapper.task_group.future import Future
 from async_wrapper.task_group.value import SoonValue
 
 if TYPE_CHECKING:
     from types import TracebackType
 
     from anyio.abc import CancelScope, Semaphore
 
-
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 
 class TaskGroupWrapper(_TaskGroup):
     def __init__(self, task_group: _TaskGroup) -> None:
         self._task_group = task_group
-        self._futures: WeakSet[Future[Any]] = WeakSet()
-
-    @property
-    def futures(self) -> WeakSet[Future[Any]]:
-        """futures using wrapper"""
-        return self._futures.copy()
 
     @property
     @override
     def cancel_scope(self) -> CancelScope:
         return self._task_group.cancel_scope
 
     @override
@@ -49,16 +40,15 @@
     @override
     def start_soon(
         self,
         func: Callable[..., Awaitable[Any]],
         *args: Any,
         name: Any = None,
     ) -> None:
-        future = self._as_future(func, *args)
-        return self._task_group.start_soon(future, name=name)
+        return self._task_group.start_soon(_as_coro, func, *args, name=name)
 
     @override
     async def start(
         self,
         func: Callable[..., Awaitable[Any]],
         *args: Any,
         name: Any = None,
@@ -93,26 +83,14 @@
             semaphore: anyio semaphore. Defaults to None.
 
         Returns:
             wrapped func
         """
         return SoonWrapper(func, self, semaphore)
 
-    def _as_future(
-        self,
-        func: Callable[ParamT, Awaitable[ValueT_co]],
-        *args: ParamT.args,
-        **kwargs: ParamT.kwargs,
-    ) -> Future[ValueT_co]:
-        coro = _as_coro(func, *args, **kwargs)
-        future = Future(coro)
-        self._futures.add(future)
-        future.add_done_callback(partial(_remove_future, task_group=self))
-        return future
-
 
 class SoonWrapper(Generic[ParamT, ValueT_co]):
     def __init__(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: _TaskGroup,
         semaphore: Semaphore | None = None,
@@ -124,32 +102,43 @@
 
     def __call__(  # noqa: D102
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
         value: SoonValue[ValueT_co] = SoonValue()
-        coro = self.wrapped(*args, **kwargs)
-        future = Future(coro)
-        value._set_future(future)  # noqa: SLF001
-        self.task_group.start_soon(future)
+        wrapped = partial(self.wrapped, value, *args, **kwargs)
+        self.task_group.start_soon(wrapped)
         return value
 
     @property
-    def wrapped(self) -> Callable[ParamT, Coroutine[Any, Any, ValueT_co]]:
+    def wrapped(
+        self,
+    ) -> Callable[
+        Concatenate[SoonValue[ValueT_co], ParamT],
+        Coroutine[Any, Any, ValueT_co],
+    ]:
         """wrapped func using semaphore"""
         if self._wrapped is not None:
             return self._wrapped
 
         @wraps(self.func)
-        async def wrapped(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
+        async def wrapped(
+            value: SoonValue[ValueT_co],
+            *args: ParamT.args,
+            **kwargs: ParamT.kwargs,
+        ) -> ValueT_co:
             if self.semaphore is None:
-                return await self.func(*args, **kwargs)
-            async with self.semaphore:
-                return await self.func(*args, **kwargs)
+                result = await self.func(*args, **kwargs)
+            else:
+                async with self.semaphore:
+                    result = await self.func(*args, **kwargs)
+            value._value = result  # noqa: SLF001
+            value._run_callbacks()  # noqa: SLF001
+            return result
 
         self._wrapped = wrapped
         return wrapped
 
     def copy(self, semaphore: Semaphore | None = None) -> Self:
         """copy self.
 
@@ -168,11 +157,7 @@
 
 async def _as_coro(
     func: Callable[ParamT, Awaitable[ValueT_co]],
     *args: ParamT.args,
     **kwargs: ParamT.kwargs,
 ) -> ValueT_co:
     return await func(*args, **kwargs)
-
-
-def _remove_future(future: Future[Any], task_group: TaskGroupWrapper) -> None:
-    task_group._futures.remove(future)  # noqa: SLF001
```

### Comparing `async_wrapper-0.3.1/PKG-INFO` & `async_wrapper-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.3.1
+Version: 0.3.2
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: loky
+Provides-Extra: uvloop
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: cloudpickle (>=2.2.1,<3.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: loky (>=3.4.0,<4.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: psutil (>=5.9.5,<6.0.0) ; extra == "all" or extra == "loky"
 Requires-Dist: typing-extensions (>=4.6.3,<5.0.0)
+Requires-Dist: uvloop (>=0.17.0,<0.18.0) ; (platform_system != "Windows") and (extra == "all" or extra == "uvloop")
 Project-URL: Repository, https://github.com/phi-friday/async-wrapper
 Description-Content-Type: text/markdown
 
 # async-wrapper
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=dev)](#)
```


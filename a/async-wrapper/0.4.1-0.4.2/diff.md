# Comparing `tmp/async_wrapper-0.4.1.tar.gz` & `tmp/async_wrapper-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_wrapper-0.4.1.tar", max compression
+gzip compressed data, was "async_wrapper-0.4.2.tar", max compression
```

## Comparing `async_wrapper-0.4.1.tar` & `async_wrapper-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/LICENSE
--rw-r--r--   0        0        0     1776 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/README.md
--rw-r--r--   0        0        0     3416 2023-08-02 13:46:17.846701 async_wrapper-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      288 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/__init__.py
--rw-r--r--   0        0        0       63 2023-08-02 13:46:17.890705 async_wrapper-0.4.1/src/async_wrapper/_version.py
--rw-r--r--   0        0        0      157 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/__init__.py
--rw-r--r--   0        0        0      564 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/_async.py
--rw-r--r--   0        0        0     1140 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/_sync.py
--rw-r--r--   0        0        0     1261 2023-08-02 13:46:03.957417 async_wrapper-0.4.1/src/async_wrapper/convert/abc.py
--rw-r--r--   0        0        0     1101 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/convert/main.py
--rw-r--r--   0        0        0        0 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/py.typed
--rw-r--r--   0        0        0      151 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/__init__.py
--rw-r--r--   0        0        0      104 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/exception.py
--rw-r--r--   0        0        0     4440 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/task_group.py
--rw-r--r--   0        0        0     1354 2023-08-02 13:46:03.961418 async_wrapper-0.4.1/src/async_wrapper/task_group/value.py
--rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 async_wrapper-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/LICENSE
+-rw-r--r--   0        0        0     1681 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/README.md
+-rw-r--r--   0        0        0     3416 2023-08-02 14:36:42.939421 async_wrapper-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/__init__.py
+-rw-r--r--   0        0        0       63 2023-08-02 14:36:42.975421 async_wrapper-0.4.2/src/async_wrapper/_version.py
+-rw-r--r--   0        0        0      157 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/__init__.py
+-rw-r--r--   0        0        0      595 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/_async.py
+-rw-r--r--   0        0        0     1186 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/_sync.py
+-rw-r--r--   0        0        0     1261 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/abc.py
+-rw-r--r--   0        0        0     1101 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/convert/main.py
+-rw-r--r--   0        0        0        0 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/py.typed
+-rw-r--r--   0        0        0      151 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/__init__.py
+-rw-r--r--   0        0        0      104 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/exception.py
+-rw-r--r--   0        0        0     5976 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/task_group.py
+-rw-r--r--   0        0        0      793 2023-08-02 14:36:30.947064 async_wrapper-0.4.2/src/async_wrapper/task_group/value.py
+-rw-r--r--   0        0        0     2520 1970-01-01 00:00:00.000000 async_wrapper-0.4.2/PKG-INFO
```

### Comparing `async_wrapper-0.4.1/LICENSE` & `async_wrapper-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.1/README.md` & `async_wrapper-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,32 +4,28 @@
 [![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=dev)](#)
 [![PyPI version](https://badge.fury.io/py/async-wrapper.svg)](https://badge.fury.io/py/async-wrapper)
 [![python version](https://img.shields.io/pypi/pyversions/async_wrapper.svg)](#)
 
 ## how to install
 ```shell
 $ pip install async_wrapper
-# or
-$ pip install "async_wrapper[all]"
-# or
-$ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
 
 import time
 
 import anyio
 
-from async_wrapper import TaskGroupWrapper, async_to_sync
+from async_wrapper import TaskGroupWrapper, toggle_func
 
 
-@async_to_sync("thread")
+@toggle_func
 async def sample_func() -> int:
     await anyio.sleep(1)
     return 1
 
 
 async def sample_func_2(x: int) -> int:
     await anyio.sleep(1)
```

### Comparing `async_wrapper-0.4.1/pyproject.toml` & `async_wrapper-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-wrapper"
-version = "0.4.1"
+version = "0.4.2"
 description = "async wrapper"
 authors = ["phi <phi.friday@gmail.com>"]
 readme = "README.md"
 license = "MIT License"
 homepage = "https://github.com/phi-friday/async-wrapper"
 repository = "https://github.com/phi-friday/async-wrapper"
 packages = [{ include = "async_wrapper", from = 'src' }]
```

### Comparing `async_wrapper-0.4.1/src/async_wrapper/convert/_sync.py` & `async_wrapper-0.4.2/src/async_wrapper/convert/_sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,44 +3,44 @@
 from concurrent.futures import ThreadPoolExecutor, wait
 from functools import partial, wraps
 from typing import Awaitable, Callable, TypeVar
 
 import anyio
 from typing_extensions import ParamSpec
 
-ValueT = TypeVar("ValueT")
+ValueT_co = TypeVar("ValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 
 __all__ = ["async_to_sync"]
 
 
 def async_to_sync(
-    func: Callable[ParamT, Awaitable[ValueT]],
-) -> Callable[ParamT, ValueT]:
+    func: Callable[ParamT, Awaitable[ValueT_co]],
+) -> Callable[ParamT, ValueT_co]:
     sync_func = _as_sync(func)
 
     @wraps(func)
-    def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
+    def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
         with ThreadPoolExecutor(1) as pool:
             future = pool.submit(sync_func, *args, **kwargs)
             wait([future])
             return future.result()
 
     return inner
 
 
 def _as_sync(
-    func: Callable[ParamT, Awaitable[ValueT]],
-) -> Callable[ParamT, ValueT]:
+    func: Callable[ParamT, Awaitable[ValueT_co]],
+) -> Callable[ParamT, ValueT_co]:
     @wraps(func)
-    def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT:
+    def inner(*args: ParamT.args, **kwargs: ParamT.kwargs) -> ValueT_co:
         return _run(func, *args, **kwargs)
 
     return inner
 
 
 def _run(
-    func: Callable[ParamT, Awaitable[ValueT]],
+    func: Callable[ParamT, Awaitable[ValueT_co]],
     *args: ParamT.args,
     **kwargs: ParamT.kwargs,
-) -> ValueT:
+) -> ValueT_co:
     return anyio.run(partial(func, *args, **kwargs))
```

### Comparing `async_wrapper-0.4.1/src/async_wrapper/convert/abc.py` & `async_wrapper-0.4.2/src/async_wrapper/convert/abc.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.1/src/async_wrapper/convert/main.py` & `async_wrapper-0.4.2/src/async_wrapper/convert/main.py`

 * *Files identical despite different names*

### Comparing `async_wrapper-0.4.1/src/async_wrapper/task_group/task_group.py` & `async_wrapper-0.4.2/src/async_wrapper/task_group/task_group.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from __future__ import annotations
 
+from contextlib import AsyncExitStack
 from functools import partial, wraps
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Coroutine, Generic, TypeVar
 
 from anyio.abc import TaskGroup as _TaskGroup
 from typing_extensions import Concatenate, ParamSpec, Self, override
 
 from async_wrapper.task_group.value import SoonValue
 
 if TYPE_CHECKING:
     from types import TracebackType
 
-    from anyio.abc import CancelScope, Semaphore
+    from anyio.abc import CancelScope, CapacityLimiter, Lock, Semaphore
 
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 OtherValueT_co = TypeVar("OtherValueT_co", covariant=True)
 ParamT = ParamSpec("ParamT")
 OtherParamT = ParamSpec("OtherParamT")
 
 
 class TaskGroupWrapper(_TaskGroup):
     def __init__(self, task_group: _TaskGroup) -> None:
         self._task_group = task_group
+        self._active_self = False
 
     @property
     @override
     def cancel_scope(self) -> CancelScope:
         return self._task_group.cancel_scope
 
     @override
@@ -53,55 +55,69 @@
         *args: Any,
         name: Any = None,
     ) -> Any:
         raise NotImplementedError
 
     @override
     async def __aenter__(self) -> Self:
+        if _is_active(self._task_group):
+            return self
         await self._task_group.__aenter__()
+        self._active_self = True
         return self
 
     @override
     async def __aexit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> bool | None:
-        return await self._task_group.__aexit__(exc_type, exc_val, exc_tb)
+        if self._active_self:
+            return await self._task_group.__aexit__(exc_type, exc_val, exc_tb)
+        return None
 
     def wrap(
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         semaphore: Semaphore | None = None,
+        limiter: CapacityLimiter | None = None,
+        lock: Lock | None = None,
     ) -> SoonWrapper[ParamT, ValueT_co]:
         """wrap function to use in wrapper.
 
         func will return soon value.
 
         Args:
             func: target func
             semaphore: anyio semaphore. Defaults to None.
+            limiter: anyio capacity limiter. defaults to None.
+            lock: anyio lock. defaults to None.
 
         Returns:
             wrapped func
         """
-        return SoonWrapper(func, self, semaphore)
+        return SoonWrapper(func, self, semaphore=semaphore, limiter=limiter, lock=lock)
 
 
 class SoonWrapper(Generic[ParamT, ValueT_co]):
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         func: Callable[ParamT, Awaitable[ValueT_co]],
         task_group: _TaskGroup,
         semaphore: Semaphore | None = None,
+        limiter: CapacityLimiter | None = None,
+        lock: Lock | None = None,
     ) -> None:
         self.func = func
         self.task_group = task_group
         self.semaphore = semaphore
+        self.limiter = limiter
+        self.lock = lock
+
         self._wrapped = None
 
     def __call__(  # noqa: D102
         self,
         *args: ParamT.args,
         **kwargs: ParamT.kwargs,
     ) -> SoonValue[ValueT_co]:
@@ -123,41 +139,71 @@
 
         @wraps(self.func)
         async def wrapped(
             value: SoonValue[ValueT_co],
             *args: ParamT.args,
             **kwargs: ParamT.kwargs,
         ) -> ValueT_co:
-            if self.semaphore is None:
+            async with AsyncExitStack() as stack:
+                if self.semaphore is not None:
+                    await stack.enter_async_context(self.semaphore)
+                if self.limiter is not None:
+                    await stack.enter_async_context(self.limiter)
+                if self.lock is not None:
+                    await stack.enter_async_context(self.lock)
+
                 result = await self.func(*args, **kwargs)
-            else:
-                async with self.semaphore:
-                    result = await self.func(*args, **kwargs)
-            value._value = result  # noqa: SLF001
-            value._run_callbacks()  # noqa: SLF001
-            return result
+                value._value = result  # noqa: SLF001
+                return result
+            raise RuntimeError("never")
 
         self._wrapped = wrapped
         return wrapped
 
-    def copy(self, semaphore: Semaphore | None = None) -> Self:
+    def copy(
+        self,
+        semaphore: Semaphore | None = None,
+        limiter: CapacityLimiter | None = None,
+        lock: Lock | None = None,
+    ) -> Self:
         """copy self.
 
         Args:
             semaphore: anyio semaphore.
                 Defaults to None.
                 if not None, overwrite.
+            limiter: anyio capacity limiter.
+                Defaults to None.
+                if not None, overwrite.
+            lock: anyio lock.
+                Defaults to None.
+                if not None, overwrite.
 
         Returns:
             self
         """
         if semaphore is None:
             semaphore = self.semaphore
-        return SoonWrapper(self.func, self.task_group, semaphore)
+        if limiter is None:
+            limiter = self.limiter
+        if lock is None:
+            lock = self.lock
+        return SoonWrapper(
+            self.func,
+            self.task_group,
+            semaphore=semaphore,
+            limiter=limiter,
+            lock=lock,
+        )
 
 
 async def _as_coro(
     func: Callable[ParamT, Awaitable[ValueT_co]],
     *args: ParamT.args,
     **kwargs: ParamT.kwargs,
 ) -> ValueT_co:
     return await func(*args, **kwargs)
+
+
+def _is_active(task_group: _TaskGroup) -> bool:
+    # trio, asyncio
+    return task_group._active  # type: ignore # noqa: SLF001
```

### Comparing `async_wrapper-0.4.1/src/async_wrapper/task_group/value.py` & `async_wrapper-0.4.2/src/async_wrapper/task_group/value.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 from __future__ import annotations
 
-from collections import deque
 from threading import local
-from typing import Any, Callable, Generic, TypeVar
+from typing import Generic, TypeVar
 
 from .exception import PendingError
 
 ValueT_co = TypeVar("ValueT_co", covariant=True)
 Pending = local()
 
 __all__ = ["SoonValue"]
 
 
 class SoonValue(Generic[ValueT_co]):
     def __init__(self) -> None:
         self._value: ValueT_co | local = Pending
-        self.done_callbacks: deque[Callable[[SoonValue[ValueT_co]], Any]] = deque()
 
     def __repr__(self) -> str:
         status = "pending" if self._value is Pending else "done"
         return f"<SoonValue: status={status}>"
 
     @property
     def value(self) -> ValueT_co:
@@ -28,25 +26,7 @@
             raise PendingError
         return self._value  # type: ignore
 
     @property
     def is_ready(self) -> bool:
         """value status"""
         return self._value is not Pending
-
-    def add_done_callback(
-        self,
-        callback: Callable[[SoonValue[ValueT_co]], Any],
-    ) -> None:
-        """add value callback.
-
-        run after set value.
-
-        Args:
-            callback: value callback.
-        """
-        self.done_callbacks.append(callback)
-
-    def _run_callbacks(self) -> None:
-        for callback in self.done_callbacks:
-            callback(self)
-        self.done_callbacks.clear()
```

### Comparing `async_wrapper-0.4.1/PKG-INFO` & `async_wrapper-0.4.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-wrapper
-Version: 0.4.1
+Version: 0.4.2
 Summary: async wrapper
 Home-page: https://github.com/phi-friday/async-wrapper
 License: MIT
 Author: phi
 Author-email: phi.friday@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
@@ -26,32 +26,28 @@
 [![github action](https://github.com/phi-friday/async-wrapper/actions/workflows/check.yaml/badge.svg?event=push&branch=dev)](#)
 [![PyPI version](https://badge.fury.io/py/async-wrapper.svg)](https://badge.fury.io/py/async-wrapper)
 [![python version](https://img.shields.io/pypi/pyversions/async_wrapper.svg)](#)
 
 ## how to install
 ```shell
 $ pip install async_wrapper
-# or
-$ pip install "async_wrapper[all]"
-# or
-$ pip install "async_wrapper[loky]"
 ```
 
 ## how to use
 ```python
 from __future__ import annotations
 
 import time
 
 import anyio
 
-from async_wrapper import TaskGroupWrapper, async_to_sync
+from async_wrapper import TaskGroupWrapper, toggle_func
 
 
-@async_to_sync("thread")
+@toggle_func
 async def sample_func() -> int:
     await anyio.sleep(1)
     return 1
 
 
 async def sample_func_2(x: int) -> int:
     await anyio.sleep(1)
```


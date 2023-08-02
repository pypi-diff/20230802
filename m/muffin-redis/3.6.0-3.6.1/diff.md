# Comparing `tmp/muffin_redis-3.6.0.tar.gz` & `tmp/muffin_redis-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_redis-3.6.0.tar", max compression
+gzip compressed data, was "muffin_redis-3.6.1.tar", max compression
```

## Comparing `muffin_redis-3.6.0.tar` & `muffin_redis-3.6.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3892 2023-08-02 06:55:55.803197 muffin_redis-3.6.0/README.rst
--rw-r--r--   0        0        0     3635 2023-08-02 06:55:55.803197 muffin_redis-3.6.0/muffin_redis/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 06:55:55.803197 muffin_redis-3.6.0/muffin_redis/py.typed
--rw-r--r--   0        0        0     1926 2023-08-02 06:55:55.803197 muffin_redis-3.6.0/pyproject.toml
--rw-r--r--   0        0        0     4893 1970-01-01 00:00:00.000000 muffin_redis-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     3775 2023-08-02 07:12:17.896410 muffin_redis-3.6.1/README.rst
+-rw-r--r--   0        0        0     3442 2023-08-02 07:12:17.896410 muffin_redis-3.6.1/muffin_redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:12:17.896410 muffin_redis-3.6.1/muffin_redis/py.typed
+-rw-r--r--   0        0        0     1926 2023-08-02 07:12:17.900410 muffin_redis-3.6.1/pyproject.toml
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 muffin_redis-3.6.1/PKG-INFO
```

### Comparing `muffin_redis-3.6.0/README.rst` & `muffin_redis-3.6.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -95,15 +95,14 @@
 **encoding**                ``"utf-8"``                             Connection encoding
 **poolsize**                ``10``                                  Connections pool size (set 0 to disable pooling)
 **decode_responses**        ``True``                                Decode binary responses
 **jsonify**                 ``False``                               Use json to store/read objects with get/set
 **blocking**                ``True``                                Wait for an available connection
 **timeout**                 ``20``                                  Timeout to get a connection
 **redislite**               ``False``                               Use redislite instead of redis
-**pytest**                  ``True``                                Pytest integration: flush redis before each test
 =========================== ======================================= ===========================
 
 .. _bugtracker:
 
 Bug tracker
 ===========
```

### Comparing `muffin_redis-3.6.0/muffin_redis/__init__.py` & `muffin_redis-3.6.1/muffin_redis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Redis support for Muffin framework."""
 
 from __future__ import annotations
 
-from contextlib import asynccontextmanager, suppress
+from contextlib import suppress
 from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional
 
 from asgi_tools._compat import json_dumps, json_loads
 from muffin.plugins import BasePlugin
 from redis.asyncio import BlockingConnectionPool, ConnectionPool, Redis, RedisError
 
 if TYPE_CHECKING:
@@ -26,15 +26,14 @@
         "decode_responses": True,
         "jsonify": False,
         "poolsize": 10,
         "blocking": True,
         "timeout": 20,
         # ===
         "redislite": False,
-        "pytest": True,
     }
 
     Error = RedisError
 
     def __init__(self, app: Optional[Application] = None, **options):
         """Initialize the plugin."""
         self.__client__: Optional[Redis] = None
@@ -116,13 +115,7 @@
             if isinstance(value, bytes):
                 value = value.decode("utf-8")
 
             with suppress(ValueError):
                 return json_loads(value)
 
         return value
-
-    @asynccontextmanager
-    async def conftest(self):
-        """Flush redis between tests."""
-        await self.client.flushall()
-        yield
```

### Comparing `muffin_redis-3.6.0/pyproject.toml` & `muffin_redis-3.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-redis"
-version = "3.6.0"
+version = "3.6.1"
 description = "Redis support for Muffin framework."
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 homepage = "https://github.com/klen/muffin-redis"
 repository = "https://github.com/klen/muffin-redis"
 keywords = ["redis", "muffin", "asgi", "asyncio"]
```

### Comparing `muffin_redis-3.6.0/PKG-INFO` & `muffin_redis-3.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-redis
-Version: 3.6.0
+Version: 3.6.1
 Summary: Redis support for Muffin framework.
 Home-page: https://github.com/klen/muffin-redis
 License: MIT
 Keywords: redis,muffin,asgi,asyncio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -122,15 +122,14 @@
 **encoding**                ``"utf-8"``                             Connection encoding
 **poolsize**                ``10``                                  Connections pool size (set 0 to disable pooling)
 **decode_responses**        ``True``                                Decode binary responses
 **jsonify**                 ``False``                               Use json to store/read objects with get/set
 **blocking**                ``True``                                Wait for an available connection
 **timeout**                 ``20``                                  Timeout to get a connection
 **redislite**               ``False``                               Use redislite instead of redis
-**pytest**                  ``True``                                Pytest integration: flush redis before each test
 =========================== ======================================= ===========================
 
 .. _bugtracker:
 
 Bug tracker
 ===========
```


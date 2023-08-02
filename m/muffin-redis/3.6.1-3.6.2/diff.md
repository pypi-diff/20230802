# Comparing `tmp/muffin_redis-3.6.1.tar.gz` & `tmp/muffin_redis-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "muffin_redis-3.6.1.tar", max compression
+gzip compressed data, was "muffin_redis-3.6.2.tar", max compression
```

## Comparing `muffin_redis-3.6.1.tar` & `muffin_redis-3.6.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3775 2023-08-02 07:12:17.896410 muffin_redis-3.6.1/README.rst
--rw-r--r--   0        0        0     3442 2023-08-02 07:12:17.896410 muffin_redis-3.6.1/muffin_redis/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 07:12:17.896410 muffin_redis-3.6.1/muffin_redis/py.typed
--rw-r--r--   0        0        0     1926 2023-08-02 07:12:17.900410 muffin_redis-3.6.1/pyproject.toml
--rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 muffin_redis-3.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3775 2023-08-02 07:22:07.909293 muffin_redis-3.6.2/README.rst
+-rw-r--r--   0        0        0     3442 2023-08-02 07:22:07.909293 muffin_redis-3.6.2/muffin_redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:22:07.909293 muffin_redis-3.6.2/muffin_redis/py.typed
+-rw-r--r--   0        0        0     1926 2023-08-02 07:22:07.909293 muffin_redis-3.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 muffin_redis-3.6.2/PKG-INFO
```

### Comparing `muffin_redis-3.6.1/README.rst` & `muffin_redis-3.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `muffin_redis-3.6.1/muffin_redis/__init__.py` & `muffin_redis-3.6.2/muffin_redis/__init__.py`

 * *Files identical despite different names*

### Comparing `muffin_redis-3.6.1/pyproject.toml` & `muffin_redis-3.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "muffin-redis"
-version = "3.6.1"
+version = "3.6.2"
 description = "Redis support for Muffin framework."
 readme = "README.rst"
 license = "MIT"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 homepage = "https://github.com/klen/muffin-redis"
 repository = "https://github.com/klen/muffin-redis"
 keywords = ["redis", "muffin", "asgi", "asyncio"]
```

### Comparing `muffin_redis-3.6.1/PKG-INFO` & `muffin_redis-3.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muffin-redis
-Version: 3.6.1
+Version: 3.6.2
 Summary: Redis support for Muffin framework.
 Home-page: https://github.com/klen/muffin-redis
 License: MIT
 Keywords: redis,muffin,asgi,asyncio
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```


# Comparing `tmp/aioworkers-pg-0.3.0a2.tar.gz` & `tmp/aioworkers_pg-0.4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioworkers-pg-0.3.0a2.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aioworkers-pg-0.3.0a2.tar` & `aioworkers_pg-0.4.0a1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0    11357 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/LICENSE
--rw-r--r--   0        0        0     1437 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/README.md
--rw-r--r--   0        0        0       24 2022-01-11 07:13:40.202796 aioworkers-pg-0.3.0a2/aioworkers_pg/__init__.py
--rw-r--r--   0        0        0     3558 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/aioworkers_pg/base.py
--rw-r--r--   0        0        0      707 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/aioworkers_pg/formatter.py
--rw-r--r--   0        0        0      922 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/aioworkers_pg/sa.py
--rw-r--r--   0        0        0     1895 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/aioworkers_pg/sql.py
--rw-r--r--   0        0        0     1067 2022-01-11 07:13:30.114740 aioworkers-pg-0.3.0a2/aioworkers_pg/storage.py
--rw-r--r--   0        0        0     1969 2022-01-11 07:13:40.198796 aioworkers-pg-0.3.0a2/pyproject.toml
--rw-r--r--   0        0        0     2212 2022-01-11 07:13:41.141983 aioworkers-pg-0.3.0a2/setup.py
--rw-r--r--   0        0        0     2435 2022-01-11 07:13:41.142278 aioworkers-pg-0.3.0a2/PKG-INFO
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/__init__.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/abc.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/base.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/formatter.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/sa.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/sql.py
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/aioworkers_pg/storage.py
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/LICENSE
+-rw-r--r--   0        0        0     2954 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/README.rst
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/pyproject.toml
+-rw-r--r--   0        0        0     5226 2020-02-02 00:00:00.000000 aioworkers_pg-0.4.0a1/PKG-INFO
```

### Comparing `aioworkers-pg-0.3.0a2/LICENSE` & `aioworkers_pg-0.4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioworkers-pg-0.3.0a2/aioworkers_pg/sql.py` & `aioworkers_pg-0.4.0a1/aioworkers_pg/sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import re
 from collections import ChainMap
 from typing import Any, Match, Sequence
 
-
 NAME = re.compile(r"[^:]:([\d\w_]+)")
 
 
 class Table:
     def __init__(self, name):
         self.name = name
```

### Comparing `aioworkers-pg-0.3.0a2/aioworkers_pg/storage.py` & `aioworkers_pg-0.4.0a1/aioworkers_pg/storage.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # true
 from .base import Connector
 from .formatter import PGFormattedEntity
 from .sql import SQL, Table
 
 
 class RoStorage(PGFormattedEntity, Connector, AbstractStorageReadOnly):
+    _get_sql: SQL
+
     def __init__(self, *args, **kwargs):
         self._key = ""
         self._table = None
-        self._get_sql = None
         super().__init__(*args, **kwargs)
 
     def set_config(self, config):
         super().set_config(config)
         self._key = self.config.key
         self._table = self.config.get("table") and Table(self.config.table)
         get_sql = self.config.get("get")
@@ -26,10 +27,10 @@
     async def init(self):
         await Connector.init(self)
 
     def raw_key(self, key):
         return self._get_sql.with_data({self._key: key})
 
     async def get(self, key):
-        result = await self._pool.fetchrow(*self.raw_key(key))
+        result = await self.pool.fetchrow(*self.raw_key(key))
         if result:
             return self.decode(result)
```


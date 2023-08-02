# Comparing `tmp/sqlx-exec-1.4.3.tar.gz` & `tmp/sqlx-exec-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-exec-1.4.3.tar", last modified: Tue Aug  1 10:46:56 2023, max compression
+gzip compressed data, was "dist\sqlx-exec-1.4.5.tar", last modified: Wed Aug  2 02:16:32 2023, max compression
```

## Comparing `sqlx-exec-1.4.3.tar` & `sqlx-exec-1.4.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/
--rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     3750 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     3163 2023-08-01 10:41:13.000000 sqlx-exec-1.4.3/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0     1232 2023-08-01 10:35:42.000000 sqlx-exec-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlexec/
--rw-rw-rw-   0        0        0      962 2023-07-30 16:50:50.000000 sqlx-exec-1.4.3/sqlexec/constant.py
--rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.3/sqlexec/engine.py
--rw-rw-rw-   0        0        0    13903 2023-08-01 03:53:45.000000 sqlx-exec-1.4.3/sqlexec/exec.py
--rw-rw-rw-   0        0        0     2025 2023-08-01 10:12:06.000000 sqlx-exec-1.4.3/sqlexec/init_import.py
--rw-rw-rw-   0        0        0      989 2023-07-30 14:49:13.000000 sqlx-exec-1.4.3/sqlexec/log_support.py
--rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.3/sqlexec/pooling.py
--rw-rw-rw-   0        0        0     1772 2023-07-30 15:17:09.000000 sqlx-exec-1.4.3/sqlexec/sql_support.py
--rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.3/sqlexec/support.py
--rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.3/sqlexec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     3750 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 10:46:56.000000 sqlx-exec-1.4.3/sqlx_exec.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/
+-rw-rw-rw-   0        0        0    11558 2023-07-21 06:24:32.000000 sqlx-exec-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0     3750 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3163 2023-08-01 10:41:13.000000 sqlx-exec-1.4.5/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1232 2023-08-02 02:15:55.000000 sqlx-exec-1.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlexec/
+-rw-rw-rw-   0        0        0      977 2023-08-01 15:23:57.000000 sqlx-exec-1.4.5/sqlexec/constant.py
+-rw-rw-rw-   0        0        0     2507 2023-07-29 10:31:40.000000 sqlx-exec-1.4.5/sqlexec/engine.py
+-rw-rw-rw-   0        0        0    13769 2023-08-01 16:09:28.000000 sqlx-exec-1.4.5/sqlexec/exec.py
+-rw-rw-rw-   0        0        0     2025 2023-08-01 10:12:06.000000 sqlx-exec-1.4.5/sqlexec/init_import.py
+-rw-rw-rw-   0        0        0      984 2023-08-01 15:30:49.000000 sqlx-exec-1.4.5/sqlexec/log_support.py
+-rw-rw-rw-   0        0        0     1508 2023-07-29 01:36:52.000000 sqlx-exec-1.4.5/sqlexec/pooling.py
+-rw-rw-rw-   0        0        0     2174 2023-08-01 15:23:57.000000 sqlx-exec-1.4.5/sqlexec/sql_support.py
+-rw-rw-rw-   0        0        0     4042 2023-07-25 15:24:05.000000 sqlx-exec-1.4.5/sqlexec/support.py
+-rw-rw-rw-   0        0        0      446 2023-07-30 15:33:50.000000 sqlx-exec-1.4.5/sqlexec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-29 03:34:26.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     3750 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 02:16:32.000000 sqlx-exec-1.4.5/sqlx_exec.egg-info/top_level.txt
```

### Comparing `sqlx-exec-1.4.3/LICENSE` & `sqlx-exec-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.3/PKG-INFO` & `sqlx-exec-1.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.3
+Version: 1.4.5
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```

### Comparing `sqlx-exec-1.4.3/README.rst` & `sqlx-exec-1.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.3/setup.py` & `sqlx-exec-1.4.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 setup(
     name='sqlx-exec',
     packages=['sqlexec'],
     description="A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='1.4.3',
+    version='1.4.5',
     url='https://gitee.com/summry/sql-exec',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['SQL', 'MySQL', 'PostgreSQL', 'SQLite', 'Oracle', 'SQL Server', 'Database', 'Python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-exec-1.4.3/sqlexec/constant.py` & `sqlx-exec-1.4.5/sqlexec/constant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LIMIT_1 = 1
+
 CACHE_SIZE = 256
 
 NAMED_REGEX = r':[\w|\d]*'
 
 MYSQL_PORT, POSTGRESQL_PORT = 3306, 5432
 
 MYSQL, POSTGRESQL, ORACLE, SQL_SERVER, SQLITE, UNKNOW = 'MySQL', 'PostgreSQL', 'Oracle', 'SQL Server', 'SQLite', 'Unknow'
```

### Comparing `sqlx-exec-1.4.3/sqlexec/engine.py` & `sqlx-exec-1.4.5/sqlexec/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.3/sqlexec/exec.py` & `sqlx-exec-1.4.5/sqlexec/exec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 from . import sql_support
 from .engine import Engine
 from .init_import import import_driver, get_engine
-from .log_support import logger, insert_log, save_log, get_log, sql_log
+from .log_support import logger, insert_log, save_log, do_sql_log, sql_log
 from .support import DBCtx, ConnectionCtx, Dict, MultiColumnsError, TransactionCtx, try_commit, DBError, DB_LOCK
 from .constant import MYSQL_CONNECTOR_DRIVER, SQLITE, PARAM_DRIVER, PARAM_SHOW_SQL, PARAM_TRANS_PLACEHOLDER, PARAM_DEBUG, PARAM_POOL_SIZE
 
 _DB_CTX = None
 
 
 def init_db(*args, **kwargs):
@@ -176,29 +176,29 @@
     """
     Batch insert
     :param table: table name
     :param args: All number must have same key. [{'name': '张三', 'age': 20}, {'name': '李四', 'age': 28}]
     :return: Effect row count
     """
     logger.debug("Exec func 'sqlexec.%s' \n\t Table: '%s', args: %s" % ('batch_insert', table, args))
-    assert len(args) > 0, 'args should not be empty.'
     sql, args = sql_support.batch_insert_sql_args(table, *args)
     return batch_execute(sql, *args)
 
 
 @with_connection
 def batch_execute(sql: str, *args):
     """
     Batch execute sql return effect rowcount
     :param sql: insert into person(name, age) values(?, ?)  -->  args: [('张三', 20), ('李四', 28)]
     :param args: All number must have same size.
     :return: Effect rowcount
     """
     global _DB_CTX
     cursor = None
+    assert args, "*args must not be empty."
     if isinstance(args[0], dict):
         sql, args = sql_support.batch_named_sql_args(sql, *args)
     sql = Engine.before_execute_intf('batch_execute', sql.strip(), *args)
     args = sql_support.get_batch_args(*args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.executemany(sql, args)
@@ -303,108 +303,103 @@
 
 def do_get(sql: str, *args):
     """
     Execute select SQL and expected one int and only one int result, SQL contain 'limit'.
     MultiColumnsError: Expect only one column.
     sql: SELECT count(1) FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    get_log('do_get', sql, *args)
-    result = do_select_one(sql, *args)
+    do_sql_log('sqlexec.do_get', sql, *args)
+    result, _ = _select_one(sql, *args)
     if result:
         if len(result) == 1:
             return result[0]
         msg = "Exec func 'sqlexec.%s' expect only one column but %d." % ('do_get', len(result))
         logger.error('%s  \n\t sql: %s \n\t args: %s' % (msg, sql, args))
         raise MultiColumnsError(msg)
     return None
 
 
-@with_connection
 def do_select(sql: str, *args):
     """
     execute select SQL and return unique result or list results(tuple).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    global _DB_CTX
-    cursor = None
-    sql = Engine.before_execute_intf('do_select', sql.strip(), *args)
-    try:
-        cursor = _DB_CTX.cursor()
-        cursor.execute(sql, args)
-        return cursor.fetchall()
-    finally:
-        if cursor:
-            cursor.close()
+    results, _ = _select(sql, *args)
+    return results
 
 
-@with_connection
 def do_select_one(sql: str, *args):
     """
     Execute select SQL and return unique result(tuple), SQL contain 'limit'.
     sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
     """
-    global _DB_CTX
-    cursor = None
-    sql = Engine.before_execute_intf('do_select_one', sql.strip(), *args)
-    try:
-        cursor = _DB_CTX.cursor()
-        cursor.execute(sql, args)
-        return cursor.fetchone()
-    finally:
-        if cursor:
-            cursor.close()
+    result, _ = _select_one(sql, *args)
+    return result
 
 
-@with_connection
 def do_query(sql: str, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM person WHERE name=? and age=?  -->  args: ('张三', 20)
     """
+    results, description = _select(sql, *args)
+    if results and description:
+        names = list(map(lambda x: x[0], description))
+        return list(map(lambda x: Dict(names, x), results))
+    return results
+
+
+def do_query_one(sql: str, *args):
+    """
+    execute select SQL and return unique result(dict), SQL contain 'limit'.
+    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
+    """
+    result, description = _select_one(sql, *args)
+    if result and description:
+        names = list(map(lambda x: x[0], description))
+        return Dict(names, result)
+    return result
+
+
+@with_connection
+def _select(sql: str, *args):
     global _DB_CTX
     cursor = None
-    sql = Engine.before_execute_intf('do_query', sql.strip(), *args)
+    sql = Engine.before_execute_intf('do_select', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
-        results = cursor.fetchall()
-        if results and cursor.description:
-            names = list(map(lambda x: x[0], cursor.description))
-            return list(map(lambda x: Dict(names, x), results))
-        else:
-            return results
+        return cursor.fetchall(), cursor.description
     finally:
         if cursor:
             cursor.close()
 
 
 @with_connection
-def do_query_one(sql: str, *args):
-    """
-    execute select SQL and return unique result(dict), SQL contain 'limit'.
-    sql: SELECT * FROM person WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
+def _select_one(sql: str, *args):
     global _DB_CTX
     cursor = None
-    sql = Engine.before_execute_intf('do_query_one', sql.strip(), *args)
+    sql, args = _do_limit_sql_args('sqlexec._select_one', sql, *args)
+    sql = Engine.before_execute_intf('_select_one', sql.strip(), *args)
     try:
         cursor = _DB_CTX.cursor()
         cursor.execute(sql, args)
-        result = cursor.fetchone()
-        if result and cursor.description:
-            names = [x[0] for x in cursor.description]
-            return Dict(names, result)
-        return result
+        return cursor.fetchone(), cursor.description
     finally:
         if cursor:
             cursor.close()
 
 
 def get_connection():
     global _DB_CTX
     _DB_CTX.try_init()
     return _DB_CTX.connection
 
 
 def try_mapping(function, sql, *args, **kwargs):
     sql_log(function, sql, *args, **kwargs)
     return sql_support.get_mapping_sql_args(sql, *args, **kwargs)
+
+
+def _do_limit_sql_args(function, sql, *args):
+    do_sql_log(function, sql, *args)
+    return sql_support.limit_one_sql_args(sql, *args)
```

### Comparing `sqlx-exec-1.4.3/sqlexec/init_import.py` & `sqlx-exec-1.4.5/sqlexec/init_import.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.3/sqlexec/log_support.py` & `sqlx-exec-1.4.5/sqlexec/log_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,14 @@
     logger.debug("Exec func 'sqlexec.%s', 'select_key': %s \n\t Table: '%s', kwargs: %s" % (function, select_key, table, kwargs))
 
 
 def sql_log(function: str, sql: str, *args, **kwargs):
     logger.debug("Exec func '%s' \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (function, sql.strip(), args, kwargs))
 
 
-def get_log(function: str, sql: str, *args):
-    logger.debug("Exec func 'sqlexec.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
+def do_sql_log(function: str, sql: str, *args):
+    logger.debug("Exec func '%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
 
 
 def db_ctx_log(action, connection):
     logger.debug('%s connection <%s>...' % (action, hex(id(connection))))
```

### Comparing `sqlx-exec-1.4.3/sqlexec/pooling.py` & `sqlx-exec-1.4.5/sqlexec/pooling.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.3/sqlexec/sql_support.py` & `sqlx-exec-1.4.5/sqlexec/sql_support.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 from .engine import Engine
 from typing import Sequence
 from .support import DBError
 from functools import lru_cache
-from .constant import CACHE_SIZE, NAMED_REGEX
+from .constant import CACHE_SIZE, NAMED_REGEX, LIMIT_1
 
 def insert_sql_args(table: str, **kwargs):
     cols, args = zip(*kwargs.items())
     sql = Engine.create_insert_sql_intf(table, cols)
     return sql, args
 
 
@@ -41,14 +41,30 @@
 
 
 def get_named_sql_args(sql: str, **kwargs):
     args = get_named_args(sql, **kwargs)
     return get_named_sql(sql), args
 
 
+def limit_one_sql_args(sql: str, *args):
+    if require_limit(sql):
+        return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
+    return sql, args
+
+
+def require_limit(sql: str):
+    lower_sql = sql.lower()
+    if 'limit' not in lower_sql:
+        return True
+    idx = lower_sql.rindex('limit')
+    if idx > 0 and ')' in lower_sql[idx:]:
+        return True
+    return False
+
+
 def is_mapping(sql: str):
     return ':' in sql
 
 
 def is_placeholder(sql: str):
     return '?' in sql
```

### Comparing `sqlx-exec-1.4.3/sqlexec/support.py` & `sqlx-exec-1.4.5/sqlexec/support.py`

 * *Files identical despite different names*

### Comparing `sqlx-exec-1.4.3/sqlx_exec.egg-info/PKG-INFO` & `sqlx-exec-1.4.5/sqlx_exec.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-exec
-Version: 1.4.3
+Version: 1.4.5
 Summary: A thread safe sql executor for Python with connection pool. It helps you automatically manage database connections and transactions.
 Home-page: https://gitee.com/summry/sql-exec
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: SQL,MySQL,PostgreSQL,SQLite,Oracle,SQL Server,Database,Python
 Platform: UNKNOWN
```


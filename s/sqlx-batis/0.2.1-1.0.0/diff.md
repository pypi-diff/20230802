# Comparing `tmp/sqlx-batis-0.2.1.tar.gz` & `tmp/sqlx-batis-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sqlx-batis-0.2.1.tar", last modified: Tue Aug  1 10:36:41 2023, max compression
+gzip compressed data, was "dist\sqlx-batis-1.0.0.tar", last modified: Wed Aug  2 02:17:13 2023, max compression
```

## Comparing `sqlx-batis-0.2.1.tar` & `sqlx-batis-1.0.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/
--rw-rw-rw-   0        0        0     5701 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-0.2.1/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1352 2023-08-01 10:36:35.000000 sqlx-batis-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlbatis/
--rw-rw-rw-   0        0        0      933 2023-08-01 10:18:34.000000 sqlx-batis-0.2.1/sqlbatis/constant.py
--rw-rw-rw-   0        0        0     8726 2023-08-01 10:31:42.000000 sqlx-batis-0.2.1/sqlbatis/db.py
--rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-0.2.1/sqlbatis/dbx.py
--rw-rw-rw-   0        0        0     6724 2023-07-30 16:13:17.000000 sqlx-batis-0.2.1/sqlbatis/engine.py
--rw-rw-rw-   0        0        0     3883 2023-07-31 11:35:56.000000 sqlx-batis-0.2.1/sqlbatis/log_support.py
--rw-rw-rw-   0        0        0    38928 2023-07-28 01:57:17.000000 sqlx-batis-0.2.1/sqlbatis/orm.py
--rw-rw-rw-   0        0        0     2409 2023-07-26 04:35:50.000000 sqlx-batis-0.2.1/sqlbatis/snowflake.py
--rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-0.2.1/sqlbatis/sql_holder.py
--rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-0.2.1/sqlbatis/sql_mapper.py
--rw-rw-rw-   0        0        0     1659 2023-08-01 10:31:42.000000 sqlx-batis-0.2.1/sqlbatis/sql_support.py
--rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-0.2.1/sqlbatis/support.py
--rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-0.2.1/sqlbatis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5701 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/requires.txt
--rw-rw-rw-   0        0        0      465 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-08-01 10:36:41.000000 sqlx-batis-0.2.1/sqlx_batis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/
+-rw-rw-rw-   0        0        0     5701 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5018 2023-07-30 08:42:44.000000 sqlx-batis-1.0.0/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1352 2023-08-02 02:16:25.000000 sqlx-batis-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlbatis/
+-rw-rw-rw-   0        0        0      927 2023-08-01 15:24:17.000000 sqlx-batis-1.0.0/sqlbatis/constant.py
+-rw-rw-rw-   0        0        0     6719 2023-08-01 15:51:50.000000 sqlx-batis-1.0.0/sqlbatis/db.py
+-rw-rw-rw-   0        0        0     6885 2023-07-30 15:46:56.000000 sqlx-batis-1.0.0/sqlbatis/dbx.py
+-rw-rw-rw-   0        0        0     6724 2023-07-30 16:13:17.000000 sqlx-batis-1.0.0/sqlbatis/engine.py
+-rw-rw-rw-   0        0        0     3731 2023-08-01 15:34:15.000000 sqlx-batis-1.0.0/sqlbatis/log_support.py
+-rw-rw-rw-   0        0        0    35069 2023-08-02 00:35:05.000000 sqlx-batis-1.0.0/sqlbatis/orm.py
+-rw-rw-rw-   0        0        0     4089 2023-08-02 00:22:16.000000 sqlx-batis-1.0.0/sqlbatis/orm_support.py
+-rw-rw-rw-   0        0        0     2539 2023-08-02 02:14:15.000000 sqlx-batis-1.0.0/sqlbatis/snowflake.py
+-rw-rw-rw-   0        0        0     7067 2023-07-23 23:51:27.000000 sqlx-batis-1.0.0/sqlbatis/sql_holder.py
+-rw-rw-rw-   0        0        0     5272 2023-07-30 15:49:36.000000 sqlx-batis-1.0.0/sqlbatis/sql_mapper.py
+-rw-rw-rw-   0        0        0     1216 2023-08-01 15:23:13.000000 sqlx-batis-1.0.0/sqlbatis/sql_support.py
+-rw-rw-rw-   0        0        0      333 2023-07-26 04:35:24.000000 sqlx-batis-1.0.0/sqlbatis/support.py
+-rw-rw-rw-   0        0        0     1662 2023-08-01 10:18:34.000000 sqlx-batis-1.0.0/sqlbatis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-30 06:47:24.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5701 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      489 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 02:17:13.000000 sqlx-batis-1.0.0/sqlx_batis.egg-info/top_level.txt
```

### Comparing `sqlx-batis-0.2.1/PKG-INFO` & `sqlx-batis-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.2.1
+Version: 1.0.0
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `sqlx-batis-0.2.1/README.rst` & `sqlx-batis-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.1/setup.py` & `sqlx-batis-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
     name='sqlx-batis',
     packages=['sqlbatis'],
     description="A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
-        'sqlx-exec>=1.4.2',
+        'sqlx-exec>=1.4.5',
     ],
-    version='0.2.1',
+    version='1.0.0',
     url='https://gitee.com/summry/sqlx-batis',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/constant.py` & `sqlx-batis-1.0.0/sqlbatis/constant.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-from sqlexec.constant import MYSQL, POSTGRESQL, SQLITE, ORACLE
-
-LIMIT_1 = 1
+from sqlexec.constant import MYSQL, POSTGRESQL, SQLITE, ORACLE, LIMIT_1
 
 NO_LIMIT = 0
 
 CACHE_SIZE = 256
 
 MAPPER_PATH = 'mapper_path'
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/db.py` & `sqlx-batis-1.0.0/sqlbatis/db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import sqlexec
 from sqlexec.exec import try_mapping
 from . import sql_support, Engine, DBError
-from .log_support import do_sql_log, save_log, do_page_log, page_log
+from .log_support import save_log, do_page_log, page_log
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec import insert, save as save_select_key, save_sql, do_save_sql, batch_insert, batch_execute
+from sqlexec import insert, save as save_select_key, save_sql, batch_insert, batch_execute, do_save_sql, do_execute, do_get, do_query, do_query_one, \
+    do_select, do_select_one
 
 
 def save(table: str, **kwargs):
     """
     Insert data into table, return primary key.
     :param table: table
     :param kwargs:
@@ -84,115 +84,60 @@
     sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age limit 1  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
     sql, args = _try_dynamic_sql('sqlbatis.db.select_one', sql, *args, **kwargs)
     return do_select_one(sql, *args)
 
 
-# ----------------------------------------------------------Do function------------------------------------------------------------------
-def do_execute(sql: str, *args):
-    """
-    Execute sql return effect rowcount
-    sql: insert into user(name, age) values(?, ?)  -->  args: ('张三', 20)
-    """
-    return sqlexec.do_execute(sql, *args)
-
-
-def do_get(sql: str, *args):
-    """
-    Execute select SQL and expected one int and only one int result. Automatically add 'limit ?' behind the sql statement if not.
-    MultiColumnsError: Expect only one column.
-    sql: SELECT count(1) FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
-    sql, args = _do_limit_sql_args('do_get', sql, *args)
-    return sqlexec.do_get(sql, *args)
-
-
-def do_query(sql: str, *args):
-    """
-    Execute select SQL and return list results(dict).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    return sqlexec.do_query(sql, *args)
-
-
-def do_select(sql: str, *args):
-    """
-    execute select SQL and return unique result or list results(tuple).
-    sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
-    """
-    return sqlexec.do_select(sql, *args)
-
-
-def do_query_one(sql: str, *args):
-    """
-    execute select SQL and return unique result(dict). Automatically add 'limit ?' behind the sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
-    sql, args = _do_limit_sql_args('do_query_one', sql, *args)
-    return sqlexec.do_query_one(sql, *args)
-
-
-def do_select_one(sql: str, *args):
-    """
-    Execute select SQL and return unique result(tuple). Automatically add 'limit ?' behind the sql statement if not.
-    sql: SELECT * FROM user WHERE name=? and age=? limit 1  -->  args: ('张三', 20)
-    """
-    sql, args = _do_limit_sql_args('do_select_one', sql, *args)
-    return sqlexec.do_select_one(sql, *args)
-
-
 # ----------------------------------------------------------Page function------------------------------------------------------------------
 def query_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age  -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    page_log('query_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = _try_mapping(sql, *args, **kwargs)
+    sql, args = _try_mapping('query_page', sql, page_num, page_size, *args, **kwargs)
     return do_query_page(sql, page_num, page_size, *args)
 
 
 def select_page(sql: str, page_num=1, page_size=10, *args, **kwargs):
     """
     Execute select SQL and return list(tuple) or empty list if no result. Automatically add 'limit ?,?' after sql statement if not.
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
          SELECT * FROM user WHERE name=:name and age=:age   -->  kwargs: ('张三', 20) --> kwargs: {'name': '张三', 'age': 20}
     """
-    page_log('select_page', sql, page_num, page_size, *args, **kwargs)
-    sql, args = _try_mapping(sql, *args, **kwargs)
+    sql, args = _try_mapping('select_page', sql, page_num, page_size, *args, **kwargs)
     return do_select_page(sql, page_num, page_size, *args)
 
 
 def do_query_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    do_page_log('select_page', sql.strip(), page_num, page_size, args)
-    sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
-    return sqlexec.do_query(sql, *args)
+    sql, args = _do_page_sql_args('do_query_page', sql, page_num, page_size, *args)
+    return do_query(sql, *args)
 
 
 def do_select_page(sql: str, page_num=1, page_size=10, *args):
     """
     Execute select SQL and return list results(dict).
     sql: SELECT * FROM user WHERE name=? and age=?  -->  args: ('张三', 20)
     """
-    do_page_log('do_select_page', sql.strip(), page_num, page_size, args)
-    sql, args = Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
-    return sqlexec.do_select(sql, *args)
+    sql, args = _do_page_sql_args('do_select_page', sql, page_num, page_size, *args)
+    return do_select(sql, *args)
 
 
 def _try_dynamic_sql(function, sql, *args, **kwargs):
     sql = sql_support.dynamic_sql(sql, **kwargs)
     return try_mapping(function, sql, *args, **kwargs)
 
 
-def _try_mapping(sql, *args, **kwargs):
+def _try_mapping(function, sql, page_num, page_size, *args, **kwargs):
+    page_log(function, sql, page_num, page_size, *args, **kwargs)
     sql = sql_support.dynamic_sql(sql, **kwargs)
     return sql_support.get_mapping_sql_args(sql, *args, **kwargs)
 
-def _do_limit_sql_args(function, sql, *args):
-    do_sql_log(function, sql, *args)
-    return sql_support.limit_one_sql_args(sql, *args)
+
+def _do_page_sql_args(function, sql, page_num, page_size, *args):
+    do_page_log(function, sql.strip(), page_num, page_size, *args)
+    return Engine.get_page_sql_args_intf(sql, page_num, page_size, *args)
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/dbx.py` & `sqlx-batis-1.0.0/sqlbatis/dbx.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.1/sqlbatis/engine.py` & `sqlx-batis-1.0.0/sqlbatis/engine.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.1/sqlbatis/log_support.py` & `sqlx-batis-1.0.0/sqlbatis/log_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 from sqlexec.log_support import logger
 
 
 def save_log(table, **kwargs):
     logger.debug("Exec func 'pgsqlx.db.save' \n\t Table: '%s', kwargs: %s" % (table, kwargs))
 
 
-def do_sql_log(function: str, sql: str, *args):
-    logger.debug("Exec func 'sqlbatis.db.%s' \n\t sql: %s \n\t args: %s" % (function, sql, args))
-
-
 def do_page_log(function: str, sql: str, page_num, page_size, *args):
     logger.debug(
         "Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\t sql: %s \n\t args: %s" % (function, page_num, page_size, sql.strip(), args))
 
 
 def page_log(function: str, sql: str, page_num, page_size, *args, **kwargs):
     logger.debug("Exec func 'sqlbatis.db.%s', page_num: %d, page_size: %d \n\tsql: %s \n\targs: %s \n\tkwargs: %s" % (
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/orm.py` & `sqlx-batis-1.0.0/sqlbatis/orm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import sys
 from .engine import Engine
 from datetime import datetime
 from enum import Enum, IntEnum
+from typing import Sequence, Union
 from .sql_support import simple_sql
 from .snowflake import get_snowflake_id
-from . import db, log_support, transaction
 from .support import DBError, NotFoundError
-from typing import Sequence, Union, List, Tuple
+from . import db, log_support, transaction, orm_support
 from .constant import LIMIT_1, NO_LIMIT, DEFAULT_KEY_FIELD, KEY, SELECT_KEY, TABLE, UPDATE_BY, UPDATE_TIME, DEL_FLAG, KEY_STRATEGY
 
 
 class DelFlag(IntEnum):
     UN_DELETE = 0
     DELETED = 1
 
@@ -145,27 +145,27 @@
         key = self._get_key()
         kv = self.__dict__
         _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
         return self.logical_delete_by_id(_id, update_by)
 
-    def un_logical_delete(self):
+    def logical_undelete(self):
         """
         Logic un delete only update the del flag
         person = Person(id=1)
-        rowcount = person.un_logical_delete()
+        rowcount = person.logical_undelete()
         """
-        log_support.orm_inst_log('un_logical_delete', self.__class__.__name__)
+        log_support.orm_inst_log('logical_undelete', self.__class__.__name__)
         key = self._get_key()
         kv = self.__dict__
         _id = kv.get(key)
         assert _id is not None, 'Primary key must not be None.'
         update_by = kv.get(self._get_update_by_field())
-        return self.un_logical_delete_by_id(_id, update_by)
+        return self.logical_undelete_by_id(_id, update_by)
 
     def delete(self):
         """
         Physical delete
         person = Person(id=1)
         rowcount = person.delete()
         """
@@ -249,41 +249,41 @@
         rowcount = Person.delete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
         log_support.orm_delete_by_id_log('logical_delete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.DELETED)
 
     @classmethod
-    def un_logical_delete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
+    def logical_undelete_by_id(cls, _id: Union[int, str], update_by: Union[int, str] = None):
         """
         Logic delete only update the del flag
-        rowcount = Person.un_logical_delete_by_id(id=1, update_by=100)
+        rowcount = Person.logical_undelete_by_id(id=1, update_by=100)
         return: Effect rowcount
         """
-        log_support.orm_delete_by_id_log('un_logical_delete_by_id', cls.__name__, _id, update_by)
+        log_support.orm_delete_by_id_log('logical_undelete_by_id', cls.__name__, _id, update_by)
         return cls._logical_delete_by_id_op(_id, update_by, DelFlag.UN_DELETE)
 
     @classmethod
     def logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
         rowcount = Person.logical_delete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
         log_support.orm_logical_delete_by_ids_log('logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.DELETED)
 
     @classmethod
-    def un_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
+    def logical_undelete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, batch_size=128):
         """
         Logic delete only update the del flag
-        rowcount = Person.un_logical_delete_by_ids(id=[1,2], update_by=100)
+        rowcount = Person.logical_undelete_by_ids(id=[1,2], update_by=100)
         return: Effect rowcount
         """
-        log_support.orm_logical_delete_by_ids_log('un_logical_delete_by_ids', cls.__name__, ids, update_by, batch_size)
+        log_support.orm_logical_delete_by_ids_log('logical_undelete_by_ids', cls.__name__, ids, update_by, batch_size)
         return cls._logical_delete_by_ids_op(ids, update_by=update_by, batch_size=batch_size, del_status=DelFlag.UN_DELETE)
 
     @classmethod
     def delete_by(cls, where: str, *args, **kwargs):
         """
         Physical delete
         rowcount = Person.delete_by('where name=? and age=?', '张三', 55)
@@ -319,17 +319,17 @@
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
         if ids_size == 1:
             return cls.delete_by_id(ids[0])
         elif ids_size <= batch_size:
             return cls.do_delete_by_ids(ids)
         else:
-            split_ids = _split_ids(ids, batch_size)
+            slices = orm_support.split_ids(ids, batch_size)
             with transaction():
-                results = list(map(cls.do_delete_by_ids, split_ids))
+                results = list(map(cls.do_delete_by_ids, slices))
             return sum(results)
 
     @classmethod
     def do_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]]):
         """
         Batch physical delete, please use delete_by_ids if there are too many
         rowcount = Person.do_delete_by_ids(id=[1,2])
@@ -363,17 +363,17 @@
     @classmethod
     def count(cls, **kwargs):
         """
         count = Person.count(name='张三', age=55)
         """
         log_support.orm_count_log('count', cls.__name__, **kwargs)
         table = cls._get_table()
-        where, args, _ = get_where_arg_limit(**kwargs)
+        where, args, _ = orm_support.get_where_arg_limit(**kwargs)
         fields = 'count(1)'
-        sql = select_sql(table, where, LIMIT_1, fields)
+        sql = orm_support.get_select_sql(table, where, LIMIT_1, fields)
         return db.do_get(sql, *args, LIMIT_1)
 
     @classmethod
     def count_by(cls, where: str, *args, **kwargs):
         """
         Automatically add 'limit ?' where if not.
         count = Person.count_by('where name=?', '李四')
@@ -385,15 +385,15 @@
         sql, args = simple_sql(sql, *args, **kwargs)
         return db.do_get(sql, *args)
 
     @classmethod
     def exists(cls, **kwargs):
         log_support.orm_count_log('exists', cls.__name__, **kwargs)
         table = cls._get_table()
-        where, args, _ = get_where_arg_limit(**kwargs)
+        where, args, _ = orm_support.get_where_arg_limit(**kwargs)
         sql = "SELECT 1 FROM {} {} limit ?".format(table, where)
         return db.do_get(sql, *args, LIMIT_1) == 1
 
     @classmethod
     def exists_by(cls, where: str, *args, **kwargs):
         log_support.orm_by_log(sys._getframe().f_code.co_name, cls.__name__, where, *args, **kwargs)
         assert where.lower().startswith('where'), "Must start with 'where' in the where parameter."
@@ -459,17 +459,17 @@
     def query(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('query', cls.__name__, *fields, **kwargs)
-        where, args, limit = get_where_arg_limit(**kwargs)
+        where, args, limit = orm_support.get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = select_sql(table, where, limit, *fields)
+        sql = orm_support.get_select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return db.do_query(sql, *args)
 
@@ -477,17 +477,17 @@
     def query_one(cls, *fields, **kwargs):
         """
         Return unique result(dict) or None if no result.
         persons = Person.query_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('query_one', cls.__name__, *fields, **kwargs)
-        where, args, _ = get_where_arg_limit(**kwargs)
+        where, args, _ = orm_support.get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = select_sql(table, where, LIMIT_1, *fields)
+        sql = orm_support.get_select_sql(table, where, LIMIT_1, *fields)
         return db.do_query_one(sql, *args, LIMIT_1)
 
     @classmethod
     def query_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.query_by('where name=?', '李四')
@@ -504,15 +504,15 @@
         person = Person.query_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('query_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
         where = 'WHERE {} = ?'.format(key)
-        sql = select_sql(table, where, LIMIT_1, *fields)
+        sql = orm_support.get_select_sql(table, where, LIMIT_1, *fields)
         return db.do_query_one(sql, _id, LIMIT_1)
 
     @classmethod
     def query_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         persons = Person.query_by_ids([1,2], 'id', 'name', 'age')
@@ -521,28 +521,28 @@
         """
         log_support.orm_find_by_ids_log('query_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
         where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
-        sql = select_sql(table, where, ids_size, *fields)
+        sql = orm_support.get_select_sql(table, where, ids_size, *fields)
         return db.do_query(sql, *ids, ids_size)
 
     @classmethod
     def select(cls, *fields, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('select', cls.__name__, *fields, **kwargs)
-        where, args, limit = get_where_arg_limit(**kwargs)
+        where, args, limit = orm_support.get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = select_sql(table, where, limit, *fields)
+        sql = orm_support.get_select_sql(table, where, limit, *fields)
         if limit:
             if isinstance(limit, int):
                 args = [*args, limit]
             else:
                 args = [*args, *limit]
         return db.do_select(sql, *args)
 
@@ -550,17 +550,17 @@
     def select_one(cls, *fields, **kwargs):
         """
         Return unique result(tuple) or None if no result.
         row = Person.select_one('id', 'name', 'age', name='张三', age=55)
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_log('select_one', cls.__name__, *fields, **kwargs)
-        where, args, _ = get_where_arg_limit(**kwargs)
+        where, args, _ = orm_support.get_where_arg_limit(**kwargs)
         table = cls._get_table()
-        sql = select_sql(table, where, LIMIT_1, *fields)
+        sql = orm_support.get_select_sql(table, where, LIMIT_1, *fields)
         return db.do_select_one(sql, *args, LIMIT_1)
 
     @classmethod
     def select_by(cls, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by('where name=?', '李四')
@@ -577,15 +577,15 @@
         row = Person.select_by_id(1, 'id', 'name', 'age')
         :param _id: key
         :param fields: Default select all fields if not set
         """
         log_support.orm_find_by_id_log('select_by_id', cls.__name__, _id, *fields)
         key, table = cls._get_key_and_table()
         where = 'WHERE {} = ?'.format(key)
-        sql = select_sql(table, where, LIMIT_1, *fields)
+        sql = orm_support.get_select_sql(table, where, LIMIT_1, *fields)
         return db.do_select_one(sql, _id, LIMIT_1)
 
     @classmethod
     def select_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], *fields):
         """
         Return list(dict) or empty list if no result.
         rows = Person.select_by_ids([1,2], 'id', 'name', 'age')
@@ -594,15 +594,15 @@
         """
         log_support.orm_find_by_ids_log('select_by_ids', cls.__name__, ids, *fields)
         ids_size = len(ids)
         assert ids_size > 0, 'ids must not be empty.'
 
         key, table = cls._get_key_and_table()
         where = 'WHERE {} in ({})'.format(key, ','.join(['?' for _ in range(ids_size)]))
-        sql = select_sql(table, where, ids_size, *fields)
+        sql = orm_support.get_select_sql(table, where, ids_size, *fields)
         return db.do_select(sql, *ids, ids_size)
 
     @classmethod
     def find_page(cls, page_num=1, page_size=10, *fields, **kwargs):
         """
         Return list(object) or empty list if no result.
         persons = Person.find_page(1, 10, 'name', 'age', name='张三', age=55)
@@ -630,16 +630,16 @@
         persons = Person.query_page(1, 10, 'id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         log_support.orm_page_log('query_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
-        where, args, _ = get_where_arg_limit(**kwargs)
-        sql = select_sql(table, where, NO_LIMIT, *fields)
+        where, args, _ = orm_support.get_where_arg_limit(**kwargs)
+        sql = orm_support.get_select_sql(table, where, NO_LIMIT, *fields)
         return db.do_query_page(sql, page_num, page_size, *args)
 
     @classmethod
     def query_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = Person.query_by_page(1, 10, 'where name=?', '李四')
@@ -656,16 +656,16 @@
         rows = Person.select_page('id', 'name', 'age', name='张三', age=55)
         :param page_num: page number
         :param page_size: page size
         :param fields: Default select all fields if not set
         """
         log_support.orm_page_log('select_page', page_num, page_size, cls.__name__, *fields, **kwargs)
         table = cls._get_table()
-        where, args, _ = get_where_arg_limit(**kwargs)
-        sql = select_sql(table, where, NO_LIMIT, *fields)
+        where, args, _ = orm_support.get_where_arg_limit(**kwargs)
+        sql = orm_support.get_select_sql(table, where, NO_LIMIT, *fields)
         return db.do_select_page(sql, page_num, page_size, *args)
 
     @classmethod
     def select_page_by(cls, page_num: int, page_size: int, where: str, *args, **kwargs):
         """
         Return list(dict) or empty list if no result. Automatically add 'limit ?,?' after where if not.
         rows = Person.select_by_page(1, 10, 'where name=?', '李四')
@@ -719,17 +719,17 @@
         assert ids_size > 0, 'ids must not be empty.'
 
         if ids_size == 1:
             return cls._logical_delete_by_id_op(ids[0], update_by, del_status)
         elif ids_size <= batch_size:
             return cls._do_logical_delete_by_ids(ids, update_by, del_status)
         else:
-            split_ids = _split_ids(ids, batch_size)
+            slices = orm_support.split_ids(ids, batch_size)
             with transaction():
-                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in split_ids]
+                results = [cls._do_logical_delete_by_ids(ids, update_by, del_status) for ids in slices]
             return sum(results)
 
     @classmethod
     def _do_logical_delete_by_ids(cls, ids: Union[Sequence[int], Sequence[str]], update_by: Union[int, str] = None, del_status=DelFlag.DELETED):
         key = cls._get_key()
         del_flag_field = cls._get_del_flag_field()
         update_by_field = cls._get_update_by_field()
@@ -760,15 +760,15 @@
         return None
 
     @classmethod
     def _get_table(cls):
         if hasattr(cls, TABLE):
             return cls.__table__
         log_support.logger.warning("%s not set attribute '%s'" % (cls.__name__, TABLE))
-        return _get_table_name(cls.__name__)
+        return orm_support.get_table_name(cls.__name__)
 
     @classmethod
     def _get_key_and_table(cls):
         return cls._get_key(), cls._get_table()
 
     @classmethod
     def _get_key_strategy(cls):
@@ -806,109 +806,11 @@
         return 'UPDATE {} SET {} WHERE {}'.format(table, update_fields, where), update_time_arg
 
     @classmethod
     def _where_sql(cls, where: str):
         low_where = where.lower()
         if low_where.startswith('where'):
             table = cls._get_table()
-            return select_sql(table, where, NO_LIMIT)
+            return orm_support.get_select_sql(table, where, NO_LIMIT)
         elif low_where.startswith('select'):
             return where
         raise DBError("The where parameter must be a complete SQL statement or conditions start with 'where'")
-
-
-# ----------------------------------------------------------Private function------------------------------------------------------------------
-def select_sql(table: str, where: str, limit: Union[int, Tuple[int], List[int]], *fields):
-    if fields:
-        fields = ','.join([col if '(' in col else '{}'.format(col) for col in fields])
-    else:
-        fields = Engine.get_table_columns_intf(table)
-
-    if limit:
-        if isinstance(limit, int):
-            return 'SELECT {} FROM {} {} LIMIT ?'.format(fields, table, where)
-        elif (isinstance(limit, Tuple) or isinstance(limit, List)) and len(limit) == 2:
-            return 'SELECT {} FROM {} {} LIMIT ? OFFSET ?'.format(fields, table, where)
-        else:
-            raise ValueError("The type of the parameter 'limit' must be 'int' or tuple, list, and it length is 2.")
-    else:
-        return 'SELECT {} FROM {} {}'.format(fields, table, where)
-
-
-def _get_condition_arg(k: str, v: object):
-    if k.endswith("__eq"):
-        return "{} = ?".format(k[:-4]), v
-    if k.endswith("__ne"):
-        return "{} != ?".format(k[:-4]), v
-    if k.endswith("__gt"):
-        return "{} > ?".format(k[:-4]), v
-    if k.endswith("__lt"):
-        return "{} < ?".format(k[:-4]), v
-    if k.endswith("__ge"):
-        return "{} >= ?".format(k[:-4]), v
-    if k.endswith("__gte"):
-        return "{} >= ?".format(k[:-5]), v
-    if k.endswith("__le"):
-        return "{} <= ?".format(k[:-4]), v
-    if k.endswith("__lte"):
-        return "{} <= ?".format(k[:-5]), v
-    if k.endswith("__isnull"):
-        return "{} is {}".format(k[:-8], 'null' if v else 'not null'), None
-    if k.endswith("__in") and isinstance(v, Sequence) and not isinstance(v, str):
-        return "{} in({})".format(k[:-4], ','.join(['?' for _ in v])), v
-    if k.endswith("__in"):
-        return "{} in({})".format(k[:-4], '?'), v
-    if k.endswith("__not_in") and isinstance(v, Sequence) and not isinstance(v, str):
-        return "{} not in({})".format(k[:-8], ','.join(['?' for _ in v])), v
-    if k.endswith("__not_in"):
-        return "{} not in({})".format(k[:-8], '?'), v
-    if k.endswith("__like"):
-        return "{} like ?".format(k[:-6], '?'), v
-    if k.endswith("__startswith"):
-        return "{} like ?".format(k[:-12]), '{}%'.format(v)
-    if k.endswith("__endswith"):
-        return "{} like ?".format(k[:-10]), '%{}'.format(v)
-    if k.endswith("__contains"):
-        return "{} like ?".format(k[:-10]), '%{}%'.format(v)
-    if k.endswith("__range") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
-        col = k[:-7]
-        return "{} >= ? and {} <= ?".format(col, col), v
-    if k.endswith("__between") and isinstance(v, Sequence) and 2 == len(v) and not isinstance(v, str):
-        return "{} between ? and ?".format(k[:-9]), v
-    if k.endswith("__range") or k.endswith("__between"):
-        return ValueError("Must is instance of Sequence with length 2 when use range or between statement")
-
-    return "{} = ?".format(k), v
-
-
-def get_where_arg_limit(**kwargs):
-    where, args, limit = '', [], 0
-    if 'limit' in kwargs:
-        limit = kwargs.pop('limit')
-
-    if kwargs:
-        conditions, tmp_args = zip(*[_get_condition_arg(k, v) for k, v in kwargs.items()])
-        tmp_args = [arg for arg in tmp_args if arg is not None]
-
-        for arg in tmp_args:
-            if arg:
-                if isinstance(arg, Sequence) and not isinstance(arg, str):
-                    args.extend(arg)
-                else:
-                    args.append(arg)
-        where = 'WHERE {}'.format(' and '.join(conditions))
-
-    return where, args, limit
-
-
-def _split_ids(ids: Sequence[int], batch_size):
-    ids_size = len(ids)
-    n = ids_size // batch_size
-    n += 0 if ids_size % batch_size == 0 else 1
-    return [ids[i:i + batch_size] for i in range(0, ids_size, batch_size)]
-
-
-def _get_table_name(class_name):
-    for i in range(1, len(class_name) - 1)[::-1]:
-        if class_name[i].isupper():
-            class_name = class_name[:i] + '_' + class_name[i:]
-    return class_name.lower()
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/snowflake.py` & `sqlx-batis-1.0.0/sqlbatis/snowflake.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,63 +1,65 @@
+"""
+默认worker_bits=3, sequence_bits=7。
+不区分数据中心，机器id最多2^3=8 台，每秒最大并发为2^7*1000=1024000，30年内id长度还是15位，javascript可以直接使用，不需转化为string
+"""
+
 import time
-from sqlexec.support import DB_LOCK
+from threading import RLock
 
 _SNOWFLAKE = None
-_WORKER_BITS = 10
-_SEQUENCE_BITS = 12
-_EPOCH = 1688140800000
 # _SEQUENCE_MASK = 4095
+_SNOWFLAKE_LOCK = RLock()
 
-
-def init_snowflake(machine_id=1, epoch=_EPOCH, worker_bits=_WORKER_BITS, sequence_bits=_SEQUENCE_BITS):
+def init_snowflake(epoch=1688140800000, machine_id=0, worker_bits=3, sequence_bits=7):
     global _SNOWFLAKE
-    _SNOWFLAKE = Snowflake(machine_id, epoch, worker_bits, sequence_bits)
+    with _SNOWFLAKE_LOCK:
+        _SNOWFLAKE = Snowflake(machine_id, epoch, worker_bits, sequence_bits)
 
 
 def get_snowflake_id():
     global _SNOWFLAKE
     try:
         return _SNOWFLAKE.generate_id()
     except AttributeError:
-        raise RuntimeError("Please init Snowflake first with: snowflake.init_snowflake(machine_id: int, epoch: int, worker_bits: int, sequence_bits: int)")
+        raise RuntimeError("Please init Snowflake first with: snowflake.init_snowflake(...)")
 
 
 def _get_timestamp():
     return int(time.time() * 1000)
 
 
+def _wait_next_millis(last_timestamp):
+    timestamp = _get_timestamp()
+    while timestamp <= last_timestamp:
+        timestamp = _get_timestamp()
+    return timestamp
+
+
 class Snowflake:
     def __init__(self, machine_id: int, epoch: int, worker_bits: int, sequence_bits: int):
         self.machine_id = machine_id
         self.epoch = epoch
         self.sequence = 0
         self.last_timestamp = -1
         self.worker_shift = sequence_bits
         self.sequence_mask = -1 ^ (-1 << sequence_bits)
         self.timestamp_left_shift = worker_bits + sequence_bits
 
         maxWorkerId = -1 ^ (-1 << worker_bits);
-        assert 0 < machine_id <= maxWorkerId, 'machine_id must ge 0 le %d' % maxWorkerId
-        assert 10 <= self.timestamp_left_shift <= 22, 'worker_bits add sequence_bits must between 10 and 20, but it is %d' % self.timestamp_left_shift
+        assert 0 <= machine_id < maxWorkerId, 'machine_id must ge 0 and lt %d, but it is %d' % (maxWorkerId, machine_id)
+        # assert 10 <= self.timestamp_left_shift <= 22, 'worker_bits add sequence_bits must between 10 and 20, but it is %d' % self.timestamp_left_shift
 
     def generate_id(self):
-        with DB_LOCK:
+        with _SNOWFLAKE_LOCK:
             timestamp = _get_timestamp()
             if timestamp < self.last_timestamp:
                 raise Exception("Clock moved backwards")
             if timestamp == self.last_timestamp:
                 self.sequence = (self.sequence + 1) & self.sequence_mask
                 if self.sequence == 0:
-                    timestamp = self._wait_next_millis(self.last_timestamp)
+                    timestamp = _wait_next_millis(self.last_timestamp)
             else:
                 self.sequence = 0
             self.last_timestamp = timestamp
             return ((timestamp - self.epoch) << self.timestamp_left_shift) | (self.machine_id << self.worker_shift) | self.sequence
             # return ((timestamp - 1288834974657) << 22) | (self.machine_id << 12) | self.sequence
-
-    @staticmethod
-    def _wait_next_millis(last_timestamp):
-        timestamp = _get_timestamp()
-        while timestamp <= last_timestamp:
-            timestamp = _get_timestamp()
-        return timestamp
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/sql_holder.py` & `sqlx-batis-1.0.0/sqlbatis/sql_holder.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.1/sqlbatis/sql_mapper.py` & `sqlx-batis-1.0.0/sqlbatis/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.1/sqlbatis/sql_support.py` & `sqlx-batis-1.0.0/sqlbatis/sql_support.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 from jinja2 import Template
 from functools import lru_cache
-from .support import MapperError
 from .constant import LIMIT_1, DYNAMIC_REGEX, CACHE_SIZE
 
 # Don't remove. Import for not repetitive implementation
-from sqlexec.sql_support import get_named_args, get_named_sql, get_batch_args, get_named_sql_args, is_mapping, get_mapping_sql_args
+from sqlexec.sql_support import get_batch_args, get_named_sql_args, is_mapping, get_mapping_sql_args, require_limit
 
 
 def simple_sql(sql: str, *args, **kwargs):
     return get_named_sql_args(sql, **kwargs) if kwargs else (sql, args)
 
 
 def dynamic_sql(sql: str, **kwargs):
@@ -20,35 +19,19 @@
 
 
 def get_page_start(page_num: int, page_size: int):
     assert page_num >= 1 and page_size >= 1, "'page_name' and 'page_size' should be higher or equal to 1"
     return (page_num - 1) * page_size
 
 
-def limit_one_sql_args(sql: str, *args):
-    if require_limit(sql):
-        return '{} LIMIT ?'.format(sql), [*args, LIMIT_1]
-    return sql, args
-
-
 @lru_cache(maxsize=2*CACHE_SIZE)
 def is_dynamic_sql(sql: str):
     return re.search(DYNAMIC_REGEX, sql)
 
 
-def require_limit(sql: str):
-    lower_sql = sql.lower()
-    if 'limit' not in lower_sql:
-        return True
-    idx = lower_sql.rindex('limit')
-    if idx > 0 and ')' in lower_sql[idx:]:
-        return True
-    return False
-
-
 @lru_cache(maxsize=2*CACHE_SIZE)
 def _get_sql_type(sql: str):
     """
     :return: 0: placeholder, 1: dynamic, 2: named mapping
     """
     if is_dynamic_sql(sql):
         return 1
```

### Comparing `sqlx-batis-0.2.1/sqlbatis/__init__.py` & `sqlx-batis-1.0.0/sqlbatis/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlx-batis-0.2.1/sqlx_batis.egg-info/PKG-INFO` & `sqlx-batis-1.0.0/sqlx_batis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlx-batis
-Version: 0.2.1
+Version: 1.0.0
 Summary: A thread safe sql executor for Python like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/sqlx-batis
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```


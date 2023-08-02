# Comparing `tmp/pgsqlx-1.7.5.tar.gz` & `tmp/pgsqlx-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pgsqlx-1.7.5.tar", last modified: Wed Aug  2 02:18:55 2023, max compression
+gzip compressed data, was "dist\pgsqlx-1.7.6.tar", last modified: Wed Aug  2 02:26:33 2023, max compression
```

## Comparing `pgsqlx-1.7.5.tar` & `pgsqlx-1.7.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/
-drwxrwxrwx   0        0        0        0 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx/
--rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.5/pgsqlx/constant.py
--rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.5/pgsqlx/db.py
--rw-rw-rw-   0        0        0     1259 2023-07-30 16:17:23.000000 pgsqlx-1.7.5/pgsqlx/dbx.py
--rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.5/pgsqlx/log_support.py
--rw-rw-rw-   0        0        0     2285 2023-07-28 02:02:00.000000 pgsqlx-1.7.5/pgsqlx/orm.py
--rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.5/pgsqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     1446 2023-07-30 16:16:26.000000 pgsqlx-1.7.5/pgsqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     5406 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      319 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/pgsqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     5406 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     4737 2023-07-30 08:43:39.000000 pgsqlx-1.7.5/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-02 02:18:55.000000 pgsqlx-1.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1370 2023-08-02 02:18:46.000000 pgsqlx-1.7.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/
+drwxrwxrwx   0        0        0        0 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx/
+-rw-rw-rw-   0        0        0      168 2023-07-29 08:25:34.000000 pgsqlx-1.7.6/pgsqlx/constant.py
+-rw-rw-rw-   0        0        0     1083 2023-07-28 02:02:26.000000 pgsqlx-1.7.6/pgsqlx/db.py
+-rw-rw-rw-   0        0        0     1259 2023-07-30 16:17:23.000000 pgsqlx-1.7.6/pgsqlx/dbx.py
+-rw-rw-rw-   0        0        0      956 2023-07-28 02:25:02.000000 pgsqlx-1.7.6/pgsqlx/log_support.py
+-rw-rw-rw-   0        0        0     2252 2023-08-02 02:25:20.000000 pgsqlx-1.7.6/pgsqlx/orm.py
+-rw-rw-rw-   0        0        0     3322 2023-07-28 02:02:00.000000 pgsqlx-1.7.6/pgsqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     1446 2023-07-30 16:16:26.000000 pgsqlx-1.7.6/pgsqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     5406 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      319 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/pgsqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5406 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4737 2023-07-30 08:43:39.000000 pgsqlx-1.7.6/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-02 02:26:33.000000 pgsqlx-1.7.6/setup.cfg
+-rw-rw-rw-   0        0        0     1370 2023-08-02 02:26:27.000000 pgsqlx-1.7.6/setup.py
```

### Comparing `pgsqlx-1.7.5/pgsqlx/db.py` & `pgsqlx-1.7.6/pgsqlx/db.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.5/pgsqlx/dbx.py` & `pgsqlx-1.7.6/pgsqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.5/pgsqlx/log_support.py` & `pgsqlx-1.7.6/pgsqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.5/pgsqlx/orm.py` & `pgsqlx-1.7.6/pgsqlx/orm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .constant import KEY_SEQ
 from .db import insert, save_key_seq
 from . import get_snowflake_id, PostgresEngine
 from .log_support import orm_insert_log, logger
 
 # Don't remove. Import for not repetitive implementation
-from sqlbatis.orm import DelFlag, KeyStrategy, Model as BaseModel, get_where_arg_limit, select_sql
+from sqlbatis.orm import DelFlag, KeyStrategy, Model as BaseModel
 
 
 class Model(BaseModel):
     """
     Create a class extends Model:
 
     class Person(Model):
```

### Comparing `pgsqlx-1.7.5/pgsqlx/sql_mapper.py` & `pgsqlx-1.7.6/pgsqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.5/pgsqlx/__init__.py` & `pgsqlx-1.7.6/pgsqlx/__init__.py`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.5/pgsqlx.egg-info/PKG-INFO` & `pgsqlx-1.7.6/pgsqlx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.7.5
+Version: 1.7.6
 Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.7.5/PKG-INFO` & `pgsqlx-1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pgsqlx
-Version: 1.7.5
+Version: 1.7.6
 Summary: A thread safe sql executor for PostgreSQL like MyBatis with connection pool. It helps you automatically manage database connections and transactions. It also provides ORM operations for single tables.
 Home-page: https://gitee.com/summry/pgsqlx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,PostgreSQL,MyBatis,python
 Platform: UNKNOWN
```

### Comparing `pgsqlx-1.7.5/README.rst` & `pgsqlx-1.7.6/README.rst`

 * *Files identical despite different names*

### Comparing `pgsqlx-1.7.5/setup.py` & `pgsqlx-1.7.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         # 'Jinja2>=2.7.0',
         # 'psycopg2>=2.7.4',
         'sqlx-batis>=1.0.0',
     ],
-    version='1.7.5',
+    version='1.7.6',
     url='https://gitee.com/summry/pgsqlx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'PostgreSQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```


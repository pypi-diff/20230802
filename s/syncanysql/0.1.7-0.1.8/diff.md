# Comparing `tmp/syncanysql-0.1.7.tar.gz` & `tmp/syncanysql-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.7.tar", last modified: Wed Jun  7 03:06:08 2023, max compression
+gzip compressed data, was "syncanysql-0.1.8.tar", last modified: Wed Aug  2 10:54:54 2023, max compression
```

## Comparing `syncanysql-0.1.7.tar` & `syncanysql-0.1.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:08.292360 syncanysql-0.1.7/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.7/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-07 03:06:08.294380 syncanysql-0.1.7/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3019 2023-05-30 02:47:03.000000 syncanysql-0.1.7/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-06-07 03:06:08.305385 syncanysql-0.1.7/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-06-03 11:38:53.000000 syncanysql-0.1.7/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:06.367979 syncanysql-0.1.7/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8803 2023-06-02 04:45:20.000000 syncanysql-0.1.7/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:07.124383 syncanysql-0.1.7/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3127 2023-06-02 03:47:10.000000 syncanysql-0.1.7/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11914 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.7/syncanysql/calculaters/env_variable_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      406 2023-05-30 02:50:43.000000 syncanysql-0.1.7/syncanysql/calculaters/generate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-06-05 09:23:36.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:07.639358 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    11491 2023-06-05 09:30:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6174 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3208 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/logical_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     5153 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6867 2023-06-05 06:30:27.000000 syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4291 2023-06-05 06:10:11.000000 syncanysql-0.1.7/syncanysql/calculaters/window_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   189228 2023-06-06 05:45:39.000000 syncanysql-0.1.7/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    13459 2023-05-27 14:11:29.000000 syncanysql-0.1.7/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      298 2023-06-02 03:32:36.000000 syncanysql-0.1.7/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8503 2023-06-02 04:45:20.000000 syncanysql-0.1.7/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4167 2023-06-02 04:35:38.000000 syncanysql-0.1.7/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.7/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     7050 2023-06-02 04:45:20.000000 syncanysql-0.1.7/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:08.243361 syncanysql-0.1.7/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.7/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.7/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1601 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.7/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4120 2023-06-02 04:35:38.000000 syncanysql-0.1.7/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    25444 2023-06-04 04:46:30.000000 syncanysql-0.1.7/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2886 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2139 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1217 2023-06-02 04:37:49.000000 syncanysql-0.1.7/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3805 2023-06-05 04:41:14.000000 syncanysql-0.1.7/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-06-03 05:28:09.000000 syncanysql-0.1.7/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-06-07 03:06:06.723362 syncanysql-0.1.7/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4346 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1311 2023-06-07 03:06:05.000000 syncanysql-0.1.7/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.7/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-06-07 03:06:04.000000 syncanysql-0.1.7/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-08-02 10:54:54.448666 syncanysql-0.1.8/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.8/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4390 2023-08-02 10:54:54.452664 syncanysql-0.1.8/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3055 2023-07-03 09:53:55.000000 syncanysql-0.1.8/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-08-02 10:54:54.466663 syncanysql-0.1.8/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-08-01 10:46:18.000000 syncanysql-0.1.8/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-08-02 10:54:52.597175 syncanysql-0.1.8/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8881 2023-08-01 09:50:44.000000 syncanysql-0.1.8/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-08-02 10:54:53.316218 syncanysql-0.1.8/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3127 2023-06-02 03:47:10.000000 syncanysql-0.1.8/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11914 2023-06-05 06:10:11.000000 syncanysql-0.1.8/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.8/syncanysql/calculaters/env_variable_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      406 2023-05-30 02:50:43.000000 syncanysql-0.1.8/syncanysql/calculaters/generate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-06-05 09:23:36.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-08-02 10:54:53.781786 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    11530 2023-08-01 10:19:50.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6174 2023-06-05 06:10:11.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3208 2023-06-05 06:10:11.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/logical_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     5153 2023-06-05 06:10:11.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6867 2023-06-05 06:30:27.000000 syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4291 2023-06-05 06:10:11.000000 syncanysql-0.1.8/syncanysql/calculaters/window_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   189228 2023-06-06 05:45:39.000000 syncanysql-0.1.8/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13919 2023-08-01 09:33:52.000000 syncanysql-0.1.8/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      298 2023-06-02 03:32:36.000000 syncanysql-0.1.8/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8503 2023-06-02 04:45:20.000000 syncanysql-0.1.8/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4238 2023-08-01 09:47:42.000000 syncanysql-0.1.8/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.8/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     7050 2023-06-02 04:45:20.000000 syncanysql-0.1.8/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-08-02 10:54:54.392664 syncanysql-0.1.8/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.8/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.8/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1601 2023-06-02 04:37:49.000000 syncanysql-0.1.8/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.8/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4120 2023-06-02 04:35:38.000000 syncanysql-0.1.8/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    25444 2023-06-04 04:46:30.000000 syncanysql-0.1.8/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2886 2023-06-02 04:37:49.000000 syncanysql-0.1.8/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2139 2023-06-02 04:37:49.000000 syncanysql-0.1.8/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1217 2023-06-02 04:37:49.000000 syncanysql-0.1.8/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3805 2023-06-05 04:41:14.000000 syncanysql-0.1.8/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-08-01 10:21:59.000000 syncanysql-0.1.8/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-08-02 10:54:52.948189 syncanysql-0.1.8/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4390 2023-08-02 10:54:51.000000 syncanysql-0.1.8/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1311 2023-08-02 10:54:51.000000 syncanysql-0.1.8/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-08-02 10:54:51.000000 syncanysql-0.1.8/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-08-02 10:54:51.000000 syncanysql-0.1.8/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.8/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-08-02 10:54:51.000000 syncanysql-0.1.8/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-08-02 10:54:51.000000 syncanysql-0.1.8/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.7/LICENSE` & `syncanysql-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/PKG-INFO` & `syncanysql-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
@@ -25,14 +25,15 @@
         -----
         
         - [安装](#安装)
         - [特性与限制](docs/feature-restrictions.md)
         - [配置详解](docs/configure.md)
         - [驱动依赖](docs/driver-dependency.md)
         - [示例详解](examples)
+        - [内置函数](docs/functions.md)
         
         ## 安装
         
         ```bash
         pip3 install syncanysql
         ```
```

### Comparing `syncanysql-0.1.7/README.md` & `syncanysql-0.1.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 -----
 
 - [安装](#安装)
 - [特性与限制](docs/feature-restrictions.md)
 - [配置详解](docs/configure.md)
 - [驱动依赖](docs/driver-dependency.md)
 - [示例详解](examples)
+- [内置函数](docs/functions.md)
 
 ## 安装
 
 ```bash
 pip3 install syncanysql
 ```
```

### Comparing `syncanysql-0.1.7/setup.py` & `syncanysql-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.7"
+version = "0.1.8"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=11.5.5,<12",
-        "syncany>=0.2.13",
+        "syncany>=0.2.14",
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
```

### Comparing `syncanysql-0.1.7/syncanysql/__init__.py` & `syncanysql-0.1.8/syncanysql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     TransformCalculater, register_calculater
 from syncany.taskers.config import Parser, ConfigReader, register_parser, register_reader
 from syncany.taskers.tasker import current_tasker
 from syncany.taskers.manager import TaskerManager
 from syncany.database import DatabaseManager, find_database
 from syncany.errors import DatabaseUnknownException
 from .version import version, version_info
-from .parser import SqlParser, SqlSegment
+from .parser import SqlParser, SqlSegment, FileParser
 from .config import GlobalConfig
 from .executor import Executor
 from .calculaters import GenerateCalculater, AggregateCalculater, StateAggregateCalculater, \
     WindowAggregateCalculater, WindowStateAggregateCalculater
 
 
 class ExecuterContext(object):
@@ -94,34 +94,35 @@
             cls.default_instance = ScriptEngine(config)
         return cls.default_instance
 
     @classmethod
     def current_context(cls):
         return ExecuterContext.current()
 
-    def __init__(self, config=None):
+    def __init__(self, custom_config=None):
+        self.custom_config = custom_config
         self.config = GlobalConfig()
-        self.config.load(config)
         self.manager = None
         self.databases = {}
         self.executor = None
 
     def setup(self):
         if self.manager is not None:
             return
-        init_execute_files = self.config.load()
+        init_execute_files = self.config.load(self.custom_config)
         self.config.config_logging()
         self.config.load_extensions()
         self.manager = TaskerManager(DatabaseManager())
         self.executor = Executor(self.manager, self.config.session())
         if init_execute_files:
-            self.executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in
-                                       range(len(init_execute_files))])
-            with self.executor as executor:
-                executor.execute()
+            for init_execute_file in init_execute_files:
+                file_parser = FileParser(init_execute_file)
+                self.executor.run("init " + init_execute_file, file_parser.load())
+                with self.executor as executor:
+                    executor.execute()
 
     def get_variable(self, name, default=None):
         if self.executor is None:
             self.setup()
         if name and name[0] != "@":
             name = "@" + name
         return self.executor.env_variables.get(name, default)
```

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.8/syncanysql/calculaters/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.8/syncanysql/calculaters/aggregate_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/env_variable_calculater.py` & `syncanysql-0.1.8/syncanysql/calculaters/env_variable_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.8/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def calculate(unit, value):
         if unit == "YEAR":
             return dt.replace(year=dt.year - value) if is_sub else dt.replace(year=dt.year + value)
         if unit in ("QUARTER", "MONTH"):
             months = value * 3 if unit == "QUARTER" else value
             if is_sub:
                 new_year = dt.year - int(months / 12) - (1 if dt.month - months % 12 < 1 else 0)
-                new_month = 12 + (dt.month - months % 12)
+                new_month = (dt.month - months % 12) + (12 if dt.month - months % 12 < 1 else 0)
             else:
                 new_year = dt.year + int(months / 12) + (1 if dt.month + months % 12 > 12 else 0)
                 new_month = (dt.month + months % 12) % 12
             return dt.replace(year=new_year, month=new_month)
         if unit in TIMEDELTA_UNITS:
             td = datetime.timedelta(seconds=TIMEDELTA_UNITS[unit] * value)
             return (dt - td) if is_sub else (dt + td)
```

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/logical_funcs.py` & `syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/logical_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.8/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/calculaters/window_calculater.py` & `syncanysql-0.1.8/syncanysql/calculaters/window_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/compiler.py` & `syncanysql-0.1.8/syncanysql/compiler.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/config.py` & `syncanysql-0.1.8/syncanysql/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -179,15 +179,24 @@
                 database["encoding"] = encoding
             if datetime_format:
                 database["datetime_format"] = datetime_format
             if date_format:
                 database["date_format"] = date_format
             if time_format:
                 database["time_format"] = time_format
-        return self.config.pop("executes", [])
+
+        init_execute_files = []
+        for init_execute_file in self.config.pop("executes", []):
+            if os.path.exists(init_execute_file):
+                init_execute_files.append(init_execute_file)
+            elif os.path.exists(os.path.join(home_config_path, init_execute_file)):
+                init_execute_files.append(os.path.join(home_config_path, init_execute_file))
+            else:
+                raise FileNotFoundError(init_execute_file)
+        return init_execute_files
 
     def load_config(self, filename=None):
         if filename is None:
             config, self.config = self.config, copy.deepcopy(CoreTasker.DEFAULT_CONFIG)
             for k, v in CoreTasker.DEFAULT_CONFIG.items():
                 if k in config and not config[k]:
                     config.pop(k)
```

### Comparing `syncanysql-0.1.7/syncanysql/executor.py` & `syncanysql-0.1.8/syncanysql/executor.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/main.py` & `syncanysql-0.1.8/syncanysql/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import traceback
 import time
 from syncany.logger import get_logger
 from syncany.taskers.manager import TaskerManager
 from syncany.database.database import DatabaseManager
 from .config import GlobalConfig
 from syncanysql.executor import Executor
-from .parser import SqlParser, FileParser, SqlSegment
+from .parser import SqlParser, FileParser
 from .prompt import CliPrompt
 
 def main():
     if os.getcwd() not in sys.path:
         sys.path.append(os.getcwd())
     if sys.stdin.isatty() and len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") \
             and not sys.argv[1].endswith(".sql"):
@@ -38,16 +38,18 @@
             global_config.config_logging(True)
         global_config.load_extensions()
         manager = TaskerManager(DatabaseManager())
 
         try:
             with Executor(manager, global_config.session()) as executor:
                 if init_execute_files:
-                    executor.run("init", [SqlSegment("execute `%s`" % init_execute_files[i], i + 1) for i in range(len(init_execute_files))])
-                    executor.execute()
+                    for init_execute_file in init_execute_files:
+                        file_parser = FileParser(init_execute_file)
+                        executor.run("init " + init_execute_file, file_parser.load())
+                        executor.execute()
 
                 if not sys.stdin.isatty() and (len(sys.argv) == 1 or (
                         len(sys.argv) >= 2 and not sys.argv[1].endswith(".sqlx") and not sys.argv[1].endswith(".sql"))):
                     start_time = time.time()
                     content = sys.stdin.read().strip()
                     if not content:
                         return
```

### Comparing `syncanysql-0.1.7/syncanysql/parser.py` & `syncanysql-0.1.8/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/prompt.py` & `syncanysql-0.1.8/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/delete.py` & `syncanysql-0.1.8/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/execute.py` & `syncanysql-0.1.8/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/explain.py` & `syncanysql-0.1.8/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/into.py` & `syncanysql-0.1.8/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/query.py` & `syncanysql-0.1.8/syncanysql/taskers/query.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/set.py` & `syncanysql-0.1.8/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/show.py` & `syncanysql-0.1.8/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/taskers/use.py` & `syncanysql-0.1.8/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql/utils.py` & `syncanysql-0.1.8/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.7/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.8/syncanysql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.7
+Version: 0.1.8
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
@@ -25,14 +25,15 @@
         -----
         
         - [安装](#安装)
         - [特性与限制](docs/feature-restrictions.md)
         - [配置详解](docs/configure.md)
         - [驱动依赖](docs/driver-dependency.md)
         - [示例详解](examples)
+        - [内置函数](docs/functions.md)
         
         ## 安装
         
         ```bash
         pip3 install syncanysql
         ```
```

### Comparing `syncanysql-0.1.7/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.8/syncanysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*


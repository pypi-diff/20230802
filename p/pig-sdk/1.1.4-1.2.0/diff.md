# Comparing `tmp/pig_sdk-1.1.4.tar.gz` & `tmp/pig_sdk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pig_sdk-1.1.4.tar", last modified: Wed Jul 26 12:16:05 2023, max compression
+gzip compressed data, was "pig_sdk-1.2.0.tar", last modified: Wed Aug  2 10:55:49 2023, max compression
```

## Comparing `pig_sdk-1.1.4.tar` & `pig_sdk-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.275679 pig_sdk-1.1.4/
--rw-rw-rw-   0        0        0      708 2023-07-26 12:16:05.275679 pig_sdk-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-07-06 00:36:30.000000 pig_sdk-1.1.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.227667 pig_sdk-1.1.4/pig_frame/
--rw-rw-rw-   0        0        0      495 2023-07-26 12:15:07.000000 pig_sdk-1.1.4/pig_frame/__init__.py
--rw-rw-rw-   0        0        0    22866 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/asserts.py
--rw-rw-rw-   0        0        0    22228 2023-07-07 06:39:23.000000 pig_sdk-1.1.4/pig_frame/common.py
--rw-rw-rw-   0        0        0     2119 2023-07-06 02:17:55.000000 pig_sdk-1.1.4/pig_frame/db.py
--rw-rw-rw-   0        0        0    10992 2023-07-07 06:23:37.000000 pig_sdk-1.1.4/pig_frame/ddt.py
--rw-rw-rw-   0        0        0     5928 2023-07-07 06:39:23.000000 pig_sdk-1.1.4/pig_frame/decorators.py
--rw-rw-rw-   0        0        0      549 2023-07-05 03:15:56.000000 pig_sdk-1.1.4/pig_frame/exceptions.py
--rw-rw-rw-   0        0        0     4685 2023-07-05 03:21:35.000000 pig_sdk-1.1.4/pig_frame/http_request.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.231668 pig_sdk-1.1.4/pig_frame/log/
--rw-rw-rw-   0        0        0    81066 2023-07-07 05:17:49.000000 pig_sdk-1.1.4/pig_frame/log/__init__.py
--rw-rw-rw-   0        0        0    35664 2023-07-06 03:53:05.000000 pig_sdk-1.1.4/pig_frame/log/config.py
--rw-rw-rw-   0        0        0    57386 2023-07-06 03:53:05.000000 pig_sdk-1.1.4/pig_frame/log/handlers.py
--rw-rw-rw-   0        0        0     1914 2023-07-05 02:55:17.000000 pig_sdk-1.1.4/pig_frame/mail.py
--rw-rw-rw-   0        0        0      840 2023-07-04 06:33:42.000000 pig_sdk-1.1.4/pig_frame/my_thread.py
--rw-rw-rw-   0        0        0      285 2023-07-04 06:33:42.000000 pig_sdk-1.1.4/pig_frame/num_util.py
--rw-rw-rw-   0        0        0     3036 2023-07-07 06:25:33.000000 pig_sdk-1.1.4/pig_frame/runner.py
--rw-rw-rw-   0        0        0    13972 2023-07-05 10:53:43.000000 pig_sdk-1.1.4/pig_frame/se_common.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.235669 pig_sdk-1.1.4/pig_frame/skeleton/
--rw-rw-rw-   0        0        0      466 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/README.md
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.243671 pig_sdk-1.1.4/pig_frame/skeleton/conf/
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.247672 pig_sdk-1.1.4/pig_frame/skeleton/conf/bbbb/
--rw-rw-rw-   0        0        0       81 2023-01-11 13:05:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/bbbb/demo2.json
--rw-rw-rw-   0        0        0       95 2023-07-07 05:34:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/global.json
--rw-rw-rw-   0        0        0       92 2023-01-11 13:05:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/pro.json
--rw-rw-rw-   0        0        0      446 2023-07-07 06:39:23.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/readme.md
--rw-rw-rw-   0        0        0     2167 2023-07-07 06:39:23.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/scheduler.json
--rw-rw-rw-   0        0        0       93 2023-07-07 05:34:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/test.json
--rw-rw-rw-   0        0        0       89 2023-07-07 05:34:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/conf/uat.json
--rw-rw-rw-   0        0        0        0 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.255674 pig_sdk-1.1.4/pig_frame/skeleton/testcases/
--rw-rw-rw-   0        0        0     2218 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/assert_demo.py
--rw-rw-rw-   0        0        0     1129 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/demo1.py
--rw-rw-rw-   0        0        0     1152 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/html_demo.py
--rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/idl_demo.py
--rw-rw-rw-   0        0        0      438 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/readme.md
--rw-rw-rw-   0        0        0      846 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/run_test_suite.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.259675 pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试场景/
--rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试场景/idl_demo.py
--rw-rw-rw-   0        0        0      151 2023-07-07 05:34:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试场景/readme.md
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.263676 pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试物料/
--rw-rw-rw-   0        0        0     1189 2023-07-07 06:19:26.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试物料/demo1.py
--rw-rw-rw-   0        0        0       59 2023-01-11 13:05:19.000000 pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试物料/readme.md
--rw-rw-rw-   0        0        0      902 2023-07-04 06:52:21.000000 pig_sdk-1.1.4/pig_frame/task_job.py
--rw-rw-rw-   0        0        0     7712 2023-07-07 04:41:20.000000 pig_sdk-1.1.4/pig_frame/task_scheduler.py
--rw-rw-rw-   0        0        0     1327 2023-07-06 02:15:41.000000 pig_sdk-1.1.4/pig_frame/template.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.267677 pig_sdk-1.1.4/pig_frame/templates/
--rw-rw-rw-   0        0        0     1128 2023-01-11 13:05:19.000000 pig_sdk-1.1.4/pig_frame/templates/idl.json
--rw-rw-rw-   0        0        0    17693 2023-07-07 05:34:19.000000 pig_sdk-1.1.4/pig_frame/templates/test_case_report.html
--rw-rw-rw-   0        0        0     3832 2023-07-07 05:27:10.000000 pig_sdk-1.1.4/pig_frame/templates/test_suite_report.html
--rw-rw-rw-   0        0        0    22801 2023-07-07 06:25:33.000000 pig_sdk-1.1.4/pig_frame/test_case.py
--rw-rw-rw-   0        0        0     5137 2023-07-07 04:44:56.000000 pig_sdk-1.1.4/pig_frame/test_suite.py
--rw-rw-rw-   0        0        0     3431 2023-07-05 10:21:49.000000 pig_sdk-1.1.4/pig_frame/utils.py
--rw-rw-rw-   0        0        0     2166 2023-07-04 06:52:22.000000 pig_sdk-1.1.4/pig_frame/xmind_util.py
-drwxrwxrwx   0        0        0        0 2023-07-26 12:16:05.275679 pig_sdk-1.1.4/pig_sdk.egg-info/
--rw-rw-rw-   0        0        0      708 2023-07-26 12:16:05.000000 pig_sdk-1.1.4/pig_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1615 2023-07-26 12:16:05.000000 pig_sdk-1.1.4/pig_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-26 12:16:05.000000 pig_sdk-1.1.4/pig_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-26 12:16:05.000000 pig_sdk-1.1.4/pig_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      314 2023-07-26 12:16:05.000000 pig_sdk-1.1.4/pig_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-26 12:16:05.000000 pig_sdk-1.1.4/pig_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-07-26 12:16:05.279682 pig_sdk-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0     2001 2023-07-26 12:12:53.000000 pig_sdk-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/
+-rw-rw-rw-   0        0        0      708 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-07-06 00:36:30.000000 pig_sdk-1.2.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.356442 pig_sdk-1.2.0/pig_frame/
+-rw-rw-rw-   0        0        0      495 2023-08-02 10:47:46.000000 pig_sdk-1.2.0/pig_frame/__init__.py
+-rw-rw-rw-   0        0        0    22866 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/asserts.py
+-rw-rw-rw-   0        0        0    22228 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/common.py
+-rw-rw-rw-   0        0        0     1859 2023-08-02 10:46:57.000000 pig_sdk-1.2.0/pig_frame/db.py
+-rw-rw-rw-   0        0        0    10992 2023-07-07 06:23:37.000000 pig_sdk-1.2.0/pig_frame/ddt.py
+-rw-rw-rw-   0        0        0     5928 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/decorators.py
+-rw-rw-rw-   0        0        0      549 2023-07-05 03:15:56.000000 pig_sdk-1.2.0/pig_frame/exceptions.py
+-rw-rw-rw-   0        0        0     4685 2023-07-05 03:21:35.000000 pig_sdk-1.2.0/pig_frame/http_request.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.356442 pig_sdk-1.2.0/pig_frame/log/
+-rw-rw-rw-   0        0        0    81066 2023-07-07 05:17:49.000000 pig_sdk-1.2.0/pig_frame/log/__init__.py
+-rw-rw-rw-   0        0        0    35664 2023-07-06 03:53:05.000000 pig_sdk-1.2.0/pig_frame/log/config.py
+-rw-rw-rw-   0        0        0    57386 2023-07-06 03:53:05.000000 pig_sdk-1.2.0/pig_frame/log/handlers.py
+-rw-rw-rw-   0        0        0     1914 2023-07-05 02:55:17.000000 pig_sdk-1.2.0/pig_frame/mail.py
+-rw-rw-rw-   0        0        0      840 2023-07-04 06:33:42.000000 pig_sdk-1.2.0/pig_frame/my_thread.py
+-rw-rw-rw-   0        0        0      285 2023-07-04 06:33:42.000000 pig_sdk-1.2.0/pig_frame/num_util.py
+-rw-rw-rw-   0        0        0     3036 2023-07-07 06:25:33.000000 pig_sdk-1.2.0/pig_frame/runner.py
+-rw-rw-rw-   0        0        0    13972 2023-07-05 10:53:43.000000 pig_sdk-1.2.0/pig_frame/se_common.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.356442 pig_sdk-1.2.0/pig_frame/skeleton/
+-rw-rw-rw-   0        0        0      466 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/conf/
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/conf/bbbb/
+-rw-rw-rw-   0        0        0       81 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/bbbb/demo2.json
+-rw-rw-rw-   0        0        0       95 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/global.json
+-rw-rw-rw-   0        0        0       92 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/pro.json
+-rw-rw-rw-   0        0        0      446 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/readme.md
+-rw-rw-rw-   0        0        0     2167 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/scheduler.json
+-rw-rw-rw-   0        0        0       93 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/test.json
+-rw-rw-rw-   0        0        0       89 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/uat.json
+-rw-rw-rw-   0        0        0        0 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/testcases/
+-rw-rw-rw-   0        0        0     2218 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/assert_demo.py
+-rw-rw-rw-   0        0        0     1129 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/demo1.py
+-rw-rw-rw-   0        0        0     1152 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/html_demo.py
+-rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/idl_demo.py
+-rw-rw-rw-   0        0        0      438 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/readme.md
+-rw-rw-rw-   0        0        0      846 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/run_test_suite.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/
+-rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/idl_demo.py
+-rw-rw-rw-   0        0        0      151 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/readme.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.387706 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/
+-rw-rw-rw-   0        0        0     1189 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/demo1.py
+-rw-rw-rw-   0        0        0       59 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/readme.md
+-rw-rw-rw-   0        0        0      902 2023-07-04 06:52:21.000000 pig_sdk-1.2.0/pig_frame/task_job.py
+-rw-rw-rw-   0        0        0     7799 2023-08-02 10:51:14.000000 pig_sdk-1.2.0/pig_frame/task_scheduler.py
+-rw-rw-rw-   0        0        0     1327 2023-07-06 02:15:41.000000 pig_sdk-1.2.0/pig_frame/template.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.387706 pig_sdk-1.2.0/pig_frame/templates/
+-rw-rw-rw-   0        0        0     1128 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/templates/idl.json
+-rw-rw-rw-   0        0        0    17693 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/templates/test_case_report.html
+-rw-rw-rw-   0        0        0     3832 2023-07-07 05:27:10.000000 pig_sdk-1.2.0/pig_frame/templates/test_suite_report.html
+-rw-rw-rw-   0        0        0    22800 2023-08-02 10:51:14.000000 pig_sdk-1.2.0/pig_frame/test_case.py
+-rw-rw-rw-   0        0        0     5137 2023-07-07 04:44:56.000000 pig_sdk-1.2.0/pig_frame/test_suite.py
+-rw-rw-rw-   0        0        0     3431 2023-07-05 10:21:49.000000 pig_sdk-1.2.0/pig_frame/utils.py
+-rw-rw-rw-   0        0        0     2166 2023-07-04 06:52:22.000000 pig_sdk-1.2.0/pig_frame/xmind_util.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/pig_sdk.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1615 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      298 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-08-02 10:47:46.000000 pig_sdk-1.2.0/setup.py
```

### Comparing `pig_sdk-1.1.4/PKG-INFO` & `pig_sdk-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pig_sdk
-Version: 1.1.4
+Version: 1.2.0
 Summary: 接口自动化框架
 Home-page: https://git.oak.net.cn/test_group/pigs_sdk/-/tree/master/pig_frame
 Author: chengwenping2
 Author-email: chengwenping2@newhope.cn
 Maintainer: chengwenping2
 Maintainer-email: chengwenping2@newhope.cn
 License: MIT
```

### Comparing `pig_sdk-1.1.4/pig_frame/asserts.py` & `pig_sdk-1.2.0/pig_frame/asserts.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/common.py` & `pig_sdk-1.2.0/pig_frame/common.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/db.py` & `pig_sdk-1.2.0/pig_frame/db.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,16 @@
 """
 文件说明：封装常用公共方法
 """
 
 import pymysql
 from sshtunnel import SSHTunnelForwarder
 from pymysql import converters, FIELD_TYPE
-import psycopg2
-from psycopg2 import extensions
 
-DEC2FLOAT = psycopg2.extensions.new_type(
-    psycopg2.extensions.DECIMAL.values,
-    'DEC2FLOAT',
-    lambda value, curs: float(value) if value is not None else None)
-psycopg2.extensions.register_type(DEC2FLOAT)
+
 conv = converters.conversions
 conv[FIELD_TYPE.NEWDECIMAL] = float  # convert decimals to float
 conv[FIELD_TYPE.DATE] = str  # convert dates to strings
 conv[FIELD_TYPE.TIMESTAMP] = str  # convert dates to strings
 conv[FIELD_TYPE.DATETIME] = str  # convert dates to strings
 conv[FIELD_TYPE.TIME] = str  # convert dates to strings
```

### Comparing `pig_sdk-1.1.4/pig_frame/ddt.py` & `pig_sdk-1.2.0/pig_frame/ddt.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/decorators.py` & `pig_sdk-1.2.0/pig_frame/decorators.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/exceptions.py` & `pig_sdk-1.2.0/pig_frame/exceptions.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/http_request.py` & `pig_sdk-1.2.0/pig_frame/http_request.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/log/__init__.py` & `pig_sdk-1.2.0/pig_frame/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/log/config.py` & `pig_sdk-1.2.0/pig_frame/log/config.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/log/handlers.py` & `pig_sdk-1.2.0/pig_frame/log/handlers.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/mail.py` & `pig_sdk-1.2.0/pig_frame/mail.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/my_thread.py` & `pig_sdk-1.2.0/pig_frame/my_thread.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/runner.py` & `pig_sdk-1.2.0/pig_frame/runner.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/se_common.py` & `pig_sdk-1.2.0/pig_frame/se_common.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/conf/scheduler.json` & `pig_sdk-1.2.0/pig_frame/skeleton/conf/scheduler.json`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/assert_demo.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/assert_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/demo1.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/demo1.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/html_demo.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/html_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/idl_demo.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/idl_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/run_test_suite.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/run_test_suite.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试场景/idl_demo.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/idl_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/skeleton/testcases/测试物料/demo1.py` & `pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/demo1.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/task_job.py` & `pig_sdk-1.2.0/pig_frame/task_job.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/task_scheduler.py` & `pig_sdk-1.2.0/pig_frame/task_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 def write_report(report_name, content):
     report_path = ""
     try:
         project_home = get_project_home()
         if not os.path.exists(f"{project_home}{os.sep}test_report"):
             os.mkdir(f"{project_home}{os.sep}test_report")
-        report_path = f'{project_home}{os.sep}test_report{os.sep}{report_name}_{datetime.now().strftime("%Y-%m-%d_%H%M%S_%f")[:-3]}.html'
+        report_path = f'{project_home}{os.sep}test_report{os.sep}{report_name}.html'
+        # report_path = f'{project_home}{os.sep}test_report{os.sep}{report_name}_{datetime.now().strftime("%Y-%m-%d_%H%M%S_%f")[:-3]}.html'
         log.info(f"{report_name}测试报告生成路径：{report_path}")
         f = open(report_path, "w", encoding="utf-8")
         f.write(content)
         f.close()
         return report_path
     except:
         return report_path
```

### Comparing `pig_sdk-1.1.4/pig_frame/template.py` & `pig_sdk-1.2.0/pig_frame/template.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/templates/idl.json` & `pig_sdk-1.2.0/pig_frame/templates/idl.json`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/templates/test_case_report.html` & `pig_sdk-1.2.0/pig_frame/templates/test_case_report.html`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/templates/test_suite_report.html` & `pig_sdk-1.2.0/pig_frame/templates/test_suite_report.html`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/test_case.py` & `pig_sdk-1.2.0/pig_frame/test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -389,15 +389,15 @@
             self.report.append(result)
 
             log.debug(f"{case_name} 验证结果：")
             log.debug(f'  断言结果:{case_assert.get("check_result")}')
         except Exception as e:
             log.error(f"添加测试用例失败:{traceback.format_exc()}\n{e}")
 
-    def output_report(self, file=None, unique=False, suite=None, task=None):
+    def output_report(self, file=None, unique=True, suite=None, task=None):
         """
         基线数据比对、测试报告生成、测试报告数据写入DB
         :return:
         :param file 调用方脚本名称
         :param unique 多次执行是否只生成一份报告
         """
         project_home = get_project_home()
```

### Comparing `pig_sdk-1.1.4/pig_frame/test_suite.py` & `pig_sdk-1.2.0/pig_frame/test_suite.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/utils.py` & `pig_sdk-1.2.0/pig_frame/utils.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_frame/xmind_util.py` & `pig_sdk-1.2.0/pig_frame/xmind_util.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/pig_sdk.egg-info/PKG-INFO` & `pig_sdk-1.2.0/pig_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pig-sdk
-Version: 1.1.4
+Version: 1.2.0
 Summary: 接口自动化框架
 Home-page: https://git.oak.net.cn/test_group/pigs_sdk/-/tree/master/pig_frame
 Author: chengwenping2
 Author-email: chengwenping2@newhope.cn
 Maintainer: chengwenping2
 Maintainer-email: chengwenping2@newhope.cn
 License: MIT
```

### Comparing `pig_sdk-1.1.4/pig_sdk.egg-info/SOURCES.txt` & `pig_sdk-1.2.0/pig_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.1.4/setup.py` & `pig_sdk-1.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,14 @@
         "psutil~=5.9.5",
         "XMind~=1.2.0",
         "APScheduler~=3.10.1",
         "pyjson5~=1.6.2",
         "json5~=0.9.14",
         "Faker~=18.10.1",
         "Jinja2~=3.1.2",
-        "psycopg2~=2.9.6",
         "termcolor~=2.3.0",
         "openpyxl~=3.1.2",
         "urllib3~=1.26.16",
         "beautifulsoup4~=4.12.2",
         "sshtunnel~=0.4.0",
     ],
     extras_require={
```


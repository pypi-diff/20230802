# Comparing `tmp/pig_sdk-1.2.0.tar.gz` & `tmp/pig_sdk-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pig_sdk-1.2.0.tar", last modified: Wed Aug  2 10:55:49 2023, max compression
+gzip compressed data, was "pig_sdk-1.2.1.tar", last modified: Wed Aug  2 11:44:35 2023, max compression
```

## Comparing `pig_sdk-1.2.0.tar` & `pig_sdk-1.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/
--rw-rw-rw-   0        0        0      708 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       49 2023-07-06 00:36:30.000000 pig_sdk-1.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.356442 pig_sdk-1.2.0/pig_frame/
--rw-rw-rw-   0        0        0      495 2023-08-02 10:47:46.000000 pig_sdk-1.2.0/pig_frame/__init__.py
--rw-rw-rw-   0        0        0    22866 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/asserts.py
--rw-rw-rw-   0        0        0    22228 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/common.py
--rw-rw-rw-   0        0        0     1859 2023-08-02 10:46:57.000000 pig_sdk-1.2.0/pig_frame/db.py
--rw-rw-rw-   0        0        0    10992 2023-07-07 06:23:37.000000 pig_sdk-1.2.0/pig_frame/ddt.py
--rw-rw-rw-   0        0        0     5928 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/decorators.py
--rw-rw-rw-   0        0        0      549 2023-07-05 03:15:56.000000 pig_sdk-1.2.0/pig_frame/exceptions.py
--rw-rw-rw-   0        0        0     4685 2023-07-05 03:21:35.000000 pig_sdk-1.2.0/pig_frame/http_request.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.356442 pig_sdk-1.2.0/pig_frame/log/
--rw-rw-rw-   0        0        0    81066 2023-07-07 05:17:49.000000 pig_sdk-1.2.0/pig_frame/log/__init__.py
--rw-rw-rw-   0        0        0    35664 2023-07-06 03:53:05.000000 pig_sdk-1.2.0/pig_frame/log/config.py
--rw-rw-rw-   0        0        0    57386 2023-07-06 03:53:05.000000 pig_sdk-1.2.0/pig_frame/log/handlers.py
--rw-rw-rw-   0        0        0     1914 2023-07-05 02:55:17.000000 pig_sdk-1.2.0/pig_frame/mail.py
--rw-rw-rw-   0        0        0      840 2023-07-04 06:33:42.000000 pig_sdk-1.2.0/pig_frame/my_thread.py
--rw-rw-rw-   0        0        0      285 2023-07-04 06:33:42.000000 pig_sdk-1.2.0/pig_frame/num_util.py
--rw-rw-rw-   0        0        0     3036 2023-07-07 06:25:33.000000 pig_sdk-1.2.0/pig_frame/runner.py
--rw-rw-rw-   0        0        0    13972 2023-07-05 10:53:43.000000 pig_sdk-1.2.0/pig_frame/se_common.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.356442 pig_sdk-1.2.0/pig_frame/skeleton/
--rw-rw-rw-   0        0        0      466 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/conf/
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/conf/bbbb/
--rw-rw-rw-   0        0        0       81 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/bbbb/demo2.json
--rw-rw-rw-   0        0        0       95 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/global.json
--rw-rw-rw-   0        0        0       92 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/pro.json
--rw-rw-rw-   0        0        0      446 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/readme.md
--rw-rw-rw-   0        0        0     2167 2023-07-07 06:39:23.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/scheduler.json
--rw-rw-rw-   0        0        0       93 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/test.json
--rw-rw-rw-   0        0        0       89 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/conf/uat.json
--rw-rw-rw-   0        0        0        0 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/testcases/
--rw-rw-rw-   0        0        0     2218 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/assert_demo.py
--rw-rw-rw-   0        0        0     1129 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/demo1.py
--rw-rw-rw-   0        0        0     1152 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/html_demo.py
--rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/idl_demo.py
--rw-rw-rw-   0        0        0      438 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/readme.md
--rw-rw-rw-   0        0        0      846 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/run_test_suite.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.372079 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/
--rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/idl_demo.py
--rw-rw-rw-   0        0        0      151 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/readme.md
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.387706 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/
--rw-rw-rw-   0        0        0     1189 2023-07-07 06:19:26.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/demo1.py
--rw-rw-rw-   0        0        0       59 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/readme.md
--rw-rw-rw-   0        0        0      902 2023-07-04 06:52:21.000000 pig_sdk-1.2.0/pig_frame/task_job.py
--rw-rw-rw-   0        0        0     7799 2023-08-02 10:51:14.000000 pig_sdk-1.2.0/pig_frame/task_scheduler.py
--rw-rw-rw-   0        0        0     1327 2023-07-06 02:15:41.000000 pig_sdk-1.2.0/pig_frame/template.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.387706 pig_sdk-1.2.0/pig_frame/templates/
--rw-rw-rw-   0        0        0     1128 2023-01-11 13:05:19.000000 pig_sdk-1.2.0/pig_frame/templates/idl.json
--rw-rw-rw-   0        0        0    17693 2023-07-07 05:34:19.000000 pig_sdk-1.2.0/pig_frame/templates/test_case_report.html
--rw-rw-rw-   0        0        0     3832 2023-07-07 05:27:10.000000 pig_sdk-1.2.0/pig_frame/templates/test_suite_report.html
--rw-rw-rw-   0        0        0    22800 2023-08-02 10:51:14.000000 pig_sdk-1.2.0/pig_frame/test_case.py
--rw-rw-rw-   0        0        0     5137 2023-07-07 04:44:56.000000 pig_sdk-1.2.0/pig_frame/test_suite.py
--rw-rw-rw-   0        0        0     3431 2023-07-05 10:21:49.000000 pig_sdk-1.2.0/pig_frame/utils.py
--rw-rw-rw-   0        0        0     2166 2023-07-04 06:52:22.000000 pig_sdk-1.2.0/pig_frame/xmind_util.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/pig_sdk.egg-info/
--rw-rw-rw-   0        0        0      708 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1615 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      298 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-08-02 10:55:49.000000 pig_sdk-1.2.0/pig_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-08-02 10:55:49.403332 pig_sdk-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1973 2023-08-02 10:47:46.000000 pig_sdk-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.722986 pig_sdk-1.2.1/
+-rw-rw-rw-   0        0        0      708 2023-08-02 11:44:35.722986 pig_sdk-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0       49 2023-07-06 00:36:30.000000 pig_sdk-1.2.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.672384 pig_sdk-1.2.1/pig_frame/
+-rw-rw-rw-   0        0        0      495 2023-08-02 11:40:30.000000 pig_sdk-1.2.1/pig_frame/__init__.py
+-rw-rw-rw-   0        0        0    22866 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/asserts.py
+-rw-rw-rw-   0        0        0    22228 2023-07-07 06:39:23.000000 pig_sdk-1.2.1/pig_frame/common.py
+-rw-rw-rw-   0        0        0     1859 2023-08-02 10:46:57.000000 pig_sdk-1.2.1/pig_frame/db.py
+-rw-rw-rw-   0        0        0    10992 2023-07-07 06:23:37.000000 pig_sdk-1.2.1/pig_frame/ddt.py
+-rw-rw-rw-   0        0        0     5928 2023-07-07 06:39:23.000000 pig_sdk-1.2.1/pig_frame/decorators.py
+-rw-rw-rw-   0        0        0      549 2023-07-05 03:15:56.000000 pig_sdk-1.2.1/pig_frame/exceptions.py
+-rw-rw-rw-   0        0        0     4685 2023-07-05 03:21:35.000000 pig_sdk-1.2.1/pig_frame/http_request.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.677384 pig_sdk-1.2.1/pig_frame/log/
+-rw-rw-rw-   0        0        0    81066 2023-07-07 05:17:49.000000 pig_sdk-1.2.1/pig_frame/log/__init__.py
+-rw-rw-rw-   0        0        0    35664 2023-07-06 03:53:05.000000 pig_sdk-1.2.1/pig_frame/log/config.py
+-rw-rw-rw-   0        0        0    57386 2023-07-06 03:53:05.000000 pig_sdk-1.2.1/pig_frame/log/handlers.py
+-rw-rw-rw-   0        0        0     1914 2023-07-05 02:55:17.000000 pig_sdk-1.2.1/pig_frame/mail.py
+-rw-rw-rw-   0        0        0      840 2023-07-04 06:33:42.000000 pig_sdk-1.2.1/pig_frame/my_thread.py
+-rw-rw-rw-   0        0        0      285 2023-07-04 06:33:42.000000 pig_sdk-1.2.1/pig_frame/num_util.py
+-rw-rw-rw-   0        0        0     3036 2023-07-07 06:25:33.000000 pig_sdk-1.2.1/pig_frame/runner.py
+-rw-rw-rw-   0        0        0    13972 2023-07-05 10:53:43.000000 pig_sdk-1.2.1/pig_frame/se_common.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.681385 pig_sdk-1.2.1/pig_frame/skeleton/
+-rw-rw-rw-   0        0        0      466 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.690121 pig_sdk-1.2.1/pig_frame/skeleton/conf/
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.691122 pig_sdk-1.2.1/pig_frame/skeleton/conf/bbbb/
+-rw-rw-rw-   0        0        0       81 2023-01-11 13:05:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/bbbb/demo2.json
+-rw-rw-rw-   0        0        0       95 2023-07-07 05:34:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/global.json
+-rw-rw-rw-   0        0        0       92 2023-01-11 13:05:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/pro.json
+-rw-rw-rw-   0        0        0      446 2023-07-07 06:39:23.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/readme.md
+-rw-rw-rw-   0        0        0     2167 2023-07-07 06:39:23.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/scheduler.json
+-rw-rw-rw-   0        0        0       93 2023-07-07 05:34:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/test.json
+-rw-rw-rw-   0        0        0       89 2023-07-07 05:34:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/conf/uat.json
+-rw-rw-rw-   0        0        0        0 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.700814 pig_sdk-1.2.1/pig_frame/skeleton/testcases/
+-rw-rw-rw-   0        0        0     2218 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/assert_demo.py
+-rw-rw-rw-   0        0        0     1129 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/demo1.py
+-rw-rw-rw-   0        0        0     1152 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/html_demo.py
+-rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/idl_demo.py
+-rw-rw-rw-   0        0        0      438 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/readme.md
+-rw-rw-rw-   0        0        0      846 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/run_test_suite.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.703814 pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试场景/
+-rw-rw-rw-   0        0        0     1323 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试场景/idl_demo.py
+-rw-rw-rw-   0        0        0      151 2023-07-07 05:34:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试场景/readme.md
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.706815 pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试物料/
+-rw-rw-rw-   0        0        0     1189 2023-07-07 06:19:26.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试物料/demo1.py
+-rw-rw-rw-   0        0        0       59 2023-01-11 13:05:19.000000 pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试物料/readme.md
+-rw-rw-rw-   0        0        0      902 2023-07-04 06:52:21.000000 pig_sdk-1.2.1/pig_frame/task_job.py
+-rw-rw-rw-   0        0        0     7882 2023-08-02 11:40:18.000000 pig_sdk-1.2.1/pig_frame/task_scheduler.py
+-rw-rw-rw-   0        0        0     1327 2023-07-06 02:15:41.000000 pig_sdk-1.2.1/pig_frame/template.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.711816 pig_sdk-1.2.1/pig_frame/templates/
+-rw-rw-rw-   0        0        0     1128 2023-01-11 13:05:19.000000 pig_sdk-1.2.1/pig_frame/templates/idl.json
+-rw-rw-rw-   0        0        0    17693 2023-07-07 05:34:19.000000 pig_sdk-1.2.1/pig_frame/templates/test_case_report.html
+-rw-rw-rw-   0        0        0     3832 2023-07-07 05:27:10.000000 pig_sdk-1.2.1/pig_frame/templates/test_suite_report.html
+-rw-rw-rw-   0        0        0    22800 2023-08-02 10:51:14.000000 pig_sdk-1.2.1/pig_frame/test_case.py
+-rw-rw-rw-   0        0        0     5137 2023-07-07 04:44:56.000000 pig_sdk-1.2.1/pig_frame/test_suite.py
+-rw-rw-rw-   0        0        0     3431 2023-07-05 10:21:49.000000 pig_sdk-1.2.1/pig_frame/utils.py
+-rw-rw-rw-   0        0        0     2166 2023-07-04 06:52:22.000000 pig_sdk-1.2.1/pig_frame/xmind_util.py
+drwxrwxrwx   0        0        0        0 2023-08-02 11:44:35.721984 pig_sdk-1.2.1/pig_sdk.egg-info/
+-rw-rw-rw-   0        0        0      708 2023-08-02 11:44:35.000000 pig_sdk-1.2.1/pig_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1615 2023-08-02 11:44:35.000000 pig_sdk-1.2.1/pig_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 11:44:35.000000 pig_sdk-1.2.1/pig_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 11:44:35.000000 pig_sdk-1.2.1/pig_sdk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      298 2023-08-02 11:44:35.000000 pig_sdk-1.2.1/pig_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-02 11:44:35.000000 pig_sdk-1.2.1/pig_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2023-08-02 11:44:35.723986 pig_sdk-1.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1973 2023-08-02 10:47:46.000000 pig_sdk-1.2.1/setup.py
```

### Comparing `pig_sdk-1.2.0/PKG-INFO` & `pig_sdk-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pig_sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: 接口自动化框架
 Home-page: https://git.oak.net.cn/test_group/pigs_sdk/-/tree/master/pig_frame
 Author: chengwenping2
 Author-email: chengwenping2@newhope.cn
 Maintainer: chengwenping2
 Maintainer-email: chengwenping2@newhope.cn
 License: MIT
```

### Comparing `pig_sdk-1.2.0/pig_frame/asserts.py` & `pig_sdk-1.2.1/pig_frame/asserts.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/common.py` & `pig_sdk-1.2.1/pig_frame/common.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/db.py` & `pig_sdk-1.2.1/pig_frame/db.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/ddt.py` & `pig_sdk-1.2.1/pig_frame/ddt.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/decorators.py` & `pig_sdk-1.2.1/pig_frame/decorators.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/exceptions.py` & `pig_sdk-1.2.1/pig_frame/exceptions.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/http_request.py` & `pig_sdk-1.2.1/pig_frame/http_request.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/log/__init__.py` & `pig_sdk-1.2.1/pig_frame/log/__init__.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/log/config.py` & `pig_sdk-1.2.1/pig_frame/log/config.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/log/handlers.py` & `pig_sdk-1.2.1/pig_frame/log/handlers.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/mail.py` & `pig_sdk-1.2.1/pig_frame/mail.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/my_thread.py` & `pig_sdk-1.2.1/pig_frame/my_thread.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/runner.py` & `pig_sdk-1.2.1/pig_frame/runner.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/se_common.py` & `pig_sdk-1.2.1/pig_frame/se_common.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/conf/scheduler.json` & `pig_sdk-1.2.1/pig_frame/skeleton/conf/scheduler.json`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/assert_demo.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/assert_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/demo1.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/demo1.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/html_demo.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/html_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/idl_demo.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/idl_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/run_test_suite.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/run_test_suite.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试场景/idl_demo.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试场景/idl_demo.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/skeleton/testcases/测试物料/demo1.py` & `pig_sdk-1.2.1/pig_frame/skeleton/testcases/测试物料/demo1.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/task_job.py` & `pig_sdk-1.2.1/pig_frame/task_job.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/task_scheduler.py` & `pig_sdk-1.2.1/pig_frame/task_scheduler.py`

 * *Files 4% similar despite different names*

```diff
@@ -78,20 +78,20 @@
     test_suite = TestSuite()
     test_suite.test_cases = testcase
     results = test_suite.run_cases()
 
     # 汇总执行结果发送报告
     sum_results = results.get("results") + suite_results
     report_content = report_overview(sum_results, upload=False)
+    report_name = task_detail.get("subject", "自动化用例执行报告")
     report_subject = task_detail.get("subject", "自动化用例执行报告") + datetime.now().strftime(
-        "%Y-%m-%d"
-    )
+        "%Y-%m-%d_%H%M%S_%f")[:-3]
 
     # 更新执行记录
-    suite_report_path = write_report(report_subject, report_content[0])
+    suite_report_path = write_report(report_name, report_content[0])
     sum_pass = 0
     sum_fail = 0
 
     for sub_result in sum_results:
         sum_pass += sub_result.pass_case
         sum_fail += sub_result.fail_case
```

### Comparing `pig_sdk-1.2.0/pig_frame/template.py` & `pig_sdk-1.2.1/pig_frame/template.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/templates/idl.json` & `pig_sdk-1.2.1/pig_frame/templates/idl.json`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/templates/test_case_report.html` & `pig_sdk-1.2.1/pig_frame/templates/test_case_report.html`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/templates/test_suite_report.html` & `pig_sdk-1.2.1/pig_frame/templates/test_suite_report.html`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/test_case.py` & `pig_sdk-1.2.1/pig_frame/test_case.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/test_suite.py` & `pig_sdk-1.2.1/pig_frame/test_suite.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/utils.py` & `pig_sdk-1.2.1/pig_frame/utils.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_frame/xmind_util.py` & `pig_sdk-1.2.1/pig_frame/xmind_util.py`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/pig_sdk.egg-info/PKG-INFO` & `pig_sdk-1.2.1/pig_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pig-sdk
-Version: 1.2.0
+Version: 1.2.1
 Summary: 接口自动化框架
 Home-page: https://git.oak.net.cn/test_group/pigs_sdk/-/tree/master/pig_frame
 Author: chengwenping2
 Author-email: chengwenping2@newhope.cn
 Maintainer: chengwenping2
 Maintainer-email: chengwenping2@newhope.cn
 License: MIT
```

### Comparing `pig_sdk-1.2.0/pig_sdk.egg-info/SOURCES.txt` & `pig_sdk-1.2.1/pig_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pig_sdk-1.2.0/setup.py` & `pig_sdk-1.2.1/setup.py`

 * *Files identical despite different names*


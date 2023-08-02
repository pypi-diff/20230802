# Comparing `tmp/apimeter-2.5.9.tar.gz` & `tmp/apimeter-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimeter-2.5.9.tar", max compression
+gzip compressed data, was "apimeter-2.6.0.tar", max compression
```

## Comparing `apimeter-2.5.9.tar` & `apimeter-2.6.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11338 2023-08-02 02:17:02.393026 apimeter-2.5.9/LICENSE
--rw-r--r--   0        0        0     1802 2023-08-02 02:42:35.294734 apimeter-2.5.9/README.md
--rw-r--r--   0        0        0      127 2023-08-02 02:20:26.667452 apimeter-2.5.9/apimeter/__init__.py
--rw-r--r--   0        0        0       70 2023-08-02 02:25:30.631590 apimeter-2.5.9/apimeter/__main__.py
--rw-r--r--   0        0        0    10437 2023-08-02 02:25:30.631783 apimeter-2.5.9/apimeter/api.py
--rw-r--r--   0        0        0       84 2023-08-02 02:25:30.918965 apimeter-2.5.9/apimeter/builtin/__init__.py
--rw-r--r--   0        0        0     3017 2023-08-02 02:25:30.920367 apimeter-2.5.9/apimeter/builtin/comparators.py
--rw-r--r--   0        0        0      925 2023-08-02 02:25:30.920584 apimeter-2.5.9/apimeter/builtin/functions.py
--rw-r--r--   0        0        0     4322 2023-08-02 02:44:16.736931 apimeter-2.5.9/apimeter/cli.py
--rw-r--r--   0        0        0     9351 2023-08-02 02:25:30.670264 apimeter-2.5.9/apimeter/client.py
--rw-r--r--   0        0        0      965 2023-08-02 02:20:26.669576 apimeter-2.5.9/apimeter/compat.py
--rw-r--r--   0        0        0     2666 2023-08-02 02:25:30.705540 apimeter-2.5.9/apimeter/context.py
--rw-r--r--   0        0        0     1142 2023-08-02 02:25:30.817485 apimeter-2.5.9/apimeter/exceptions.py
--rw-r--r--   0        0        0      114 2023-08-02 02:17:02.529002 apimeter-2.5.9/apimeter/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-08-02 02:20:26.671032 apimeter-2.5.9/apimeter/ext/har2case/__init__.py
--rw-r--r--   0        0        0     4808 2023-08-02 02:20:26.671419 apimeter-2.5.9/apimeter/ext/locusts/README.md
--rw-r--r--   0        0        0        0 2023-08-02 02:20:26.671540 apimeter-2.5.9/apimeter/ext/locusts/__init__.py
--rw-r--r--   0        0        0       81 2023-08-02 02:25:30.948807 apimeter-2.5.9/apimeter/ext/locusts/__main__.py
--rw-r--r--   0        0        0     5481 2023-08-02 02:25:30.950454 apimeter-2.5.9/apimeter/ext/locusts/cli.py
--rw-r--r--   0        0        0     1254 2023-08-02 02:25:31.206244 apimeter-2.5.9/apimeter/ext/locusts/locustfile_template.py
--rw-r--r--   0        0        0      627 2023-08-02 02:25:31.290728 apimeter-2.5.9/apimeter/ext/locusts/utils.py
--rw-r--r--   0        0        0     4148 2023-08-02 02:25:31.291005 apimeter-2.5.9/apimeter/ext/uploader/__init__.py
--rw-r--r--   0        0        0      924 2023-08-02 02:25:31.295623 apimeter-2.5.9/apimeter/loader/__init__.py
--rw-r--r--   0        0        0    15804 2023-08-02 02:25:31.299696 apimeter-2.5.9/apimeter/loader/buildup.py
--rw-r--r--   0        0        0     6455 2023-08-02 02:25:31.299883 apimeter-2.5.9/apimeter/loader/check.py
--rw-r--r--   0        0        0     5704 2023-08-02 02:25:31.355848 apimeter-2.5.9/apimeter/loader/load.py
--rw-r--r--   0        0        0     3536 2023-08-02 02:25:31.299950 apimeter-2.5.9/apimeter/loader/locate.py
--rw-r--r--   0        0        0     1607 2023-08-02 02:20:26.676961 apimeter-2.5.9/apimeter/loader/schemas/api.schema.json
--rw-r--r--   0        0        0    14880 2023-08-02 02:20:26.677353 apimeter-2.5.9/apimeter/loader/schemas/common.schema.json
--rw-r--r--   0        0        0     5187 2023-08-02 02:20:26.677757 apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v1.json
--rw-r--r--   0        0        0     6518 2023-08-02 02:20:26.679107 apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v2.json
--rw-r--r--   0        0        0     1994 2023-08-02 02:20:26.679520 apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v1.json
--rw-r--r--   0        0        0     2662 2023-08-02 02:20:26.679888 apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v2.json
--rw-r--r--   0        0        0     2367 2023-08-02 02:20:26.680214 apimeter-2.5.9/apimeter/logger.py
--rw-r--r--   0        0        0    50881 2023-08-02 02:25:30.832063 apimeter-2.5.9/apimeter/parser.py
--rw-r--r--   0        0        0      536 2023-08-02 02:25:31.498115 apimeter-2.5.9/apimeter/report/__init__.py
--rw-r--r--   0        0        0      309 2023-08-02 02:25:31.516575 apimeter-2.5.9/apimeter/report/html/__init__.py
--rw-r--r--   0        0        0     2627 2023-08-02 02:46:16.779127 apimeter-2.5.9/apimeter/report/html/gen_report.py
--rw-r--r--   0        0        0     2064 2023-08-02 02:25:31.516709 apimeter-2.5.9/apimeter/report/html/result.py
--rw-r--r--   0        0        0    10851 2023-08-02 02:20:26.683469 apimeter-2.5.9/apimeter/report/html/template.html
--rw-r--r--   0        0        0     1153 2023-08-02 02:25:31.500348 apimeter-2.5.9/apimeter/report/report.py
--rw-r--r--   0        0        0     6583 2023-08-02 02:25:31.501664 apimeter-2.5.9/apimeter/report/stringify.py
--rw-r--r--   0        0        0     2414 2023-08-02 02:25:31.502172 apimeter-2.5.9/apimeter/report/summarize.py
--rw-r--r--   0        0        0    10378 2023-08-02 02:25:30.866260 apimeter-2.5.9/apimeter/response.py
--rw-r--r--   0        0        0    14575 2023-08-02 02:25:30.866650 apimeter-2.5.9/apimeter/runner.py
--rw-r--r--   0        0        0    21296 2023-08-02 02:25:30.897029 apimeter-2.5.9/apimeter/utils.py
--rw-r--r--   0        0        0     7257 2023-08-02 02:25:30.918344 apimeter-2.5.9/apimeter/validator.py
--rw-r--r--   0        0        0    11026 2023-08-02 02:20:26.510919 apimeter-2.5.9/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1964 2023-08-02 02:35:45.851132 apimeter-2.5.9/pyproject.toml
--rw-r--r--   0        0        0     3707 2023-08-02 02:54:25.721357 apimeter-2.5.9/setup.py
--rw-r--r--   0        0        0     3891 2023-08-02 02:54:25.721848 apimeter-2.5.9/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-08-02 02:17:02.393026 apimeter-2.6.0/LICENSE
+-rw-r--r--   0        0        0     2122 2023-08-02 03:10:43.900504 apimeter-2.6.0/README.md
+-rw-r--r--   0        0        0      127 2023-08-02 02:20:26.667452 apimeter-2.6.0/apimeter/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-02 02:25:30.631590 apimeter-2.6.0/apimeter/__main__.py
+-rw-r--r--   0        0        0    10688 2023-08-02 04:24:12.353488 apimeter-2.6.0/apimeter/api.py
+-rw-r--r--   0        0        0       84 2023-08-02 02:25:30.918965 apimeter-2.6.0/apimeter/builtin/__init__.py
+-rw-r--r--   0        0        0     3017 2023-08-02 02:25:30.920367 apimeter-2.6.0/apimeter/builtin/comparators.py
+-rw-r--r--   0        0        0      925 2023-08-02 02:25:30.920584 apimeter-2.6.0/apimeter/builtin/functions.py
+-rw-r--r--   0        0        0     4361 2023-08-02 04:47:20.487140 apimeter-2.6.0/apimeter/cli.py
+-rw-r--r--   0        0        0     9351 2023-08-02 02:25:30.670264 apimeter-2.6.0/apimeter/client.py
+-rw-r--r--   0        0        0      965 2023-08-02 02:20:26.669576 apimeter-2.6.0/apimeter/compat.py
+-rw-r--r--   0        0        0     2666 2023-08-02 02:25:30.705540 apimeter-2.6.0/apimeter/context.py
+-rw-r--r--   0        0        0     1142 2023-08-02 02:25:30.817485 apimeter-2.6.0/apimeter/exceptions.py
+-rw-r--r--   0        0        0      114 2023-08-02 02:17:02.529002 apimeter-2.6.0/apimeter/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:20:26.671032 apimeter-2.6.0/apimeter/ext/har2case/__init__.py
+-rw-r--r--   0        0        0     4808 2023-08-02 02:20:26.671419 apimeter-2.6.0/apimeter/ext/locusts/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 02:20:26.671540 apimeter-2.6.0/apimeter/ext/locusts/__init__.py
+-rw-r--r--   0        0        0       81 2023-08-02 02:25:30.948807 apimeter-2.6.0/apimeter/ext/locusts/__main__.py
+-rw-r--r--   0        0        0     5481 2023-08-02 02:25:30.950454 apimeter-2.6.0/apimeter/ext/locusts/cli.py
+-rw-r--r--   0        0        0     1254 2023-08-02 02:25:31.206244 apimeter-2.6.0/apimeter/ext/locusts/locustfile_template.py
+-rw-r--r--   0        0        0      627 2023-08-02 02:25:31.290728 apimeter-2.6.0/apimeter/ext/locusts/utils.py
+-rw-r--r--   0        0        0     4148 2023-08-02 02:25:31.291005 apimeter-2.6.0/apimeter/ext/uploader/__init__.py
+-rw-r--r--   0        0        0      924 2023-08-02 02:25:31.295623 apimeter-2.6.0/apimeter/loader/__init__.py
+-rw-r--r--   0        0        0    15804 2023-08-02 02:25:31.299696 apimeter-2.6.0/apimeter/loader/buildup.py
+-rw-r--r--   0        0        0     6455 2023-08-02 02:25:31.299883 apimeter-2.6.0/apimeter/loader/check.py
+-rw-r--r--   0        0        0     5704 2023-08-02 02:25:31.355848 apimeter-2.6.0/apimeter/loader/load.py
+-rw-r--r--   0        0        0     3536 2023-08-02 02:25:31.299950 apimeter-2.6.0/apimeter/loader/locate.py
+-rw-r--r--   0        0        0     1607 2023-08-02 02:20:26.676961 apimeter-2.6.0/apimeter/loader/schemas/api.schema.json
+-rw-r--r--   0        0        0    14880 2023-08-02 02:20:26.677353 apimeter-2.6.0/apimeter/loader/schemas/common.schema.json
+-rw-r--r--   0        0        0     5187 2023-08-02 02:20:26.677757 apimeter-2.6.0/apimeter/loader/schemas/testcase.schema.v1.json
+-rw-r--r--   0        0        0     6518 2023-08-02 02:20:26.679107 apimeter-2.6.0/apimeter/loader/schemas/testcase.schema.v2.json
+-rw-r--r--   0        0        0     1994 2023-08-02 02:20:26.679520 apimeter-2.6.0/apimeter/loader/schemas/testsuite.schema.v1.json
+-rw-r--r--   0        0        0     2662 2023-08-02 02:20:26.679888 apimeter-2.6.0/apimeter/loader/schemas/testsuite.schema.v2.json
+-rw-r--r--   0        0        0     2367 2023-08-02 02:20:26.680214 apimeter-2.6.0/apimeter/logger.py
+-rw-r--r--   0        0        0    50881 2023-08-02 02:25:30.832063 apimeter-2.6.0/apimeter/parser.py
+-rw-r--r--   0        0        0      536 2023-08-02 02:25:31.498115 apimeter-2.6.0/apimeter/report/__init__.py
+-rw-r--r--   0        0        0      309 2023-08-02 02:25:31.516575 apimeter-2.6.0/apimeter/report/html/__init__.py
+-rw-r--r--   0        0        0     2633 2023-08-02 04:23:16.537473 apimeter-2.6.0/apimeter/report/html/gen_report.py
+-rw-r--r--   0        0        0     2064 2023-08-02 02:25:31.516709 apimeter-2.6.0/apimeter/report/html/result.py
+-rw-r--r--   0        0        0    10851 2023-08-02 02:20:26.683469 apimeter-2.6.0/apimeter/report/html/template.html
+-rw-r--r--   0        0        0     1153 2023-08-02 02:25:31.500348 apimeter-2.6.0/apimeter/report/report.py
+-rw-r--r--   0        0        0     6583 2023-08-02 02:25:31.501664 apimeter-2.6.0/apimeter/report/stringify.py
+-rw-r--r--   0        0        0     2414 2023-08-02 02:25:31.502172 apimeter-2.6.0/apimeter/report/summarize.py
+-rw-r--r--   0        0        0    10378 2023-08-02 02:25:30.866260 apimeter-2.6.0/apimeter/response.py
+-rw-r--r--   0        0        0    14575 2023-08-02 02:25:30.866650 apimeter-2.6.0/apimeter/runner.py
+-rw-r--r--   0        0        0    21296 2023-08-02 02:25:30.897029 apimeter-2.6.0/apimeter/utils.py
+-rw-r--r--   0        0        0     7257 2023-08-02 02:25:30.918344 apimeter-2.6.0/apimeter/validator.py
+-rw-r--r--   0        0        0    11026 2023-08-02 02:20:26.510919 apimeter-2.6.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1964 2023-08-02 04:48:00.442337 apimeter-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     4029 2023-08-02 04:50:12.806147 apimeter-2.6.0/setup.py
+-rw-r--r--   0        0        0     4211 2023-08-02 04:50:12.806768 apimeter-2.6.0/PKG-INFO
```

### Comparing `apimeter-2.5.9/LICENSE` & `apimeter-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/README.md` & `apimeter-2.6.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 
 - [`中文用户使用手册`][user-docs-zh]
 - [`开发历程记录博客`][development-blogs]
 - [CHANGELOG](docs/CHANGELOG.md)
 
 ## Usage
 ```python
-# 报告支持忽略成功用例数据
-apimeter xxx.yml --skip-success
-
-
+poetry install  # 安装依赖
+poetry run python -m apimeter /path/to/api  # 完整生成报告
+poetry run python -m apimeter /path/to/api --skip-success  # 报告忽略成功用例数据
+poetry build  # 打包
+poetry publish  # 发布，根据提示输入pypi账号密码
+pip install -i https://pypi.Python.org/simple/ apimeter  # 指定安装源，因为刚发布其他平台未及时同步
 ```
 
 
 [Requests]: http://docs.python-requests.org/en/master/
 [unittest]: https://docs.python.org/3/library/unittest.html
 [Locust]: http://locust.io/
 [har2case]: https://github.com/httprunner/har2case
```

### Comparing `apimeter-2.5.9/apimeter/api.py` & `apimeter-2.6.0/apimeter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             log_file="test.log"
         )
         summary = runner.run(path_or_tests)
 
     """
 
     def __init__(
-        self, failfast=False, save_tests=False, log_level="WARNING", log_file=None
+        self, failfast=False, save_tests=False, log_level="WARNING", log_file=None, skip_success=False
     ):
         """initialize HttpRunner.
 
         Args:
             failfast (bool): stop the test run on the first error or failure.
             save_tests (bool): save loaded/parsed tests to JSON file.
             log_level (str): logging level.
@@ -44,14 +44,15 @@
         logger.setup_logger(log_level, log_file)
 
         self.exception_stage = "initialize HttpRunner()"
         kwargs = {"failfast": failfast, "resultclass": report.HtmlTestResult}
         self.unittest_runner = unittest.TextTestRunner(**kwargs)
         self.test_loader = unittest.TestLoader()
         self.save_tests = save_tests
+        self.skip_success = skip_success
         self._summary = None
         self.project_working_directory = None
 
     def _add_tests(self, testcases):
         """initialize testcase with Runner() and add to test suite.
 
         Args:
@@ -138,14 +139,17 @@
 
         for testcase in test_suite:
             testcase_name = testcase.config.get("name")
             logger.log_info("Start to run testcase: {}".format(testcase_name))
 
             result = self.unittest_runner.run(testcase)
             if result.wasSuccessful():
+                # 测试用例执行成功，剔除执行成功的用例步骤数据，减少报告体积大小
+                if self.skip_success:
+                    result.records = []
                 tests_results.append((testcase, result))
             else:
                 tests_results.insert(0, (testcase, result))
 
         return tests_results
 
     def _aggregate(self, tests_results):
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `apimeter-2.5.9/apimeter/builtin/comparators.py` & `apimeter-2.6.0/apimeter/builtin/comparators.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/builtin/functions.py` & `apimeter-2.6.0/apimeter/builtin/functions.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/cli.py` & `apimeter-2.6.0/apimeter/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         sys.exit(0)
 
     runner = HttpRunner(
         failfast=args.failfast,
         save_tests=args.save_tests,
         log_level=args.log_level,
         log_file=args.log_file,
+        skip_success=args.skip_success
     )
 
     err_code = 0
     try:
         for path in args.testfile_paths:
             summary = runner.run(path, dot_env_path=args.dot_env_path)
             report_dir = args.report_dir or os.path.join(
```

### Comparing `apimeter-2.5.9/apimeter/client.py` & `apimeter-2.6.0/apimeter/client.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/compat.py` & `apimeter-2.6.0/apimeter/compat.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/context.py` & `apimeter-2.6.0/apimeter/context.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/exceptions.py` & `apimeter-2.6.0/apimeter/exceptions.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/ext/locusts/README.md` & `apimeter-2.6.0/apimeter/ext/locusts/README.md`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/ext/locusts/cli.py` & `apimeter-2.6.0/apimeter/ext/locusts/cli.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/ext/locusts/locustfile_template.py` & `apimeter-2.6.0/apimeter/ext/locusts/locustfile_template.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/ext/locusts/utils.py` & `apimeter-2.6.0/apimeter/ext/locusts/utils.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/ext/uploader/__init__.py` & `apimeter-2.6.0/apimeter/ext/uploader/__init__.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/__init__.py` & `apimeter-2.6.0/apimeter/loader/__init__.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/buildup.py` & `apimeter-2.6.0/apimeter/loader/buildup.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/check.py` & `apimeter-2.6.0/apimeter/loader/check.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/load.py` & `apimeter-2.6.0/apimeter/loader/load.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/locate.py` & `apimeter-2.6.0/apimeter/loader/locate.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/schemas/api.schema.json` & `apimeter-2.6.0/apimeter/loader/schemas/api.schema.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/schemas/common.schema.json` & `apimeter-2.6.0/apimeter/loader/schemas/common.schema.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v1.json` & `apimeter-2.6.0/apimeter/loader/schemas/testcase.schema.v1.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v2.json` & `apimeter-2.6.0/apimeter/loader/schemas/testcase.schema.v2.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v1.json` & `apimeter-2.6.0/apimeter/loader/schemas/testsuite.schema.v1.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v2.json` & `apimeter-2.6.0/apimeter/loader/schemas/testsuite.schema.v2.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/logger.py` & `apimeter-2.6.0/apimeter/logger.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/parser.py` & `apimeter-2.6.0/apimeter/parser.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/report/__init__.py` & `apimeter-2.6.0/apimeter/report/__init__.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/report/html/gen_report.py` & `apimeter-2.6.0/apimeter/report/html/gen_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     logger.log_info("Start to render Html report ...")
 
     start_at_timestamp = summary["time"]["start_at"]
     utc_time_iso_8601_str = datetime.utcfromtimestamp(start_at_timestamp).isoformat()
     summary["time"]["start_datetime"] = utc_time_iso_8601_str
 
     # skip success testcases in report
-    if skip_success:
-        for suite in summary["details"]:
-            suite['records'] = list(filter(lambda record: record['status'] != 'success', suite['records']))
+    # if skip_success:
+    #     for suite in summary["details"]:
+    #         suite['records'] = list(filter(lambda record: record['status'] != 'success', suite['records']))
 
     if report_file:
         report_dir = os.path.dirname(report_file)
         report_file_name = os.path.basename(report_file)
     else:
         report_dir = report_dir or os.path.join(os.getcwd(), "reports")
         # fix #826: Windows does not support file name include ":"
```

### Comparing `apimeter-2.5.9/apimeter/report/html/result.py` & `apimeter-2.6.0/apimeter/report/html/result.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/report/html/template.html` & `apimeter-2.6.0/apimeter/report/html/template.html`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/report/report.py` & `apimeter-2.6.0/apimeter/report/report.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/report/stringify.py` & `apimeter-2.6.0/apimeter/report/stringify.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/report/summarize.py` & `apimeter-2.6.0/apimeter/report/summarize.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/response.py` & `apimeter-2.6.0/apimeter/response.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/runner.py` & `apimeter-2.6.0/apimeter/runner.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/utils.py` & `apimeter-2.6.0/apimeter/utils.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/apimeter/validator.py` & `apimeter-2.6.0/apimeter/validator.py`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/docs/CHANGELOG.md` & `apimeter-2.6.0/docs/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.9/pyproject.toml` & `apimeter-2.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apimeter"
-version = "2.5.9"
+version = "2.6.0"
 description = "One-stop solution for HTTP(S) testing."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ["debugtalk <debugtalk@gmail.com>"]
 
 homepage = "https://github.com/httprunner/httprunner"
 repository = "https://github.com/httprunner/httprunner"
```

### Comparing `apimeter-2.5.9/setup.py` & `apimeter-2.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,17 +39,17 @@
                      'hrun = apimeter.cli:main',
                      'httprunner = apimeter.cli:main',
                      'locusts = apimeter.ext.locusts.cli:main',
                      'meter = apimeter.cli:main']}
 
 setup_kwargs = {
     'name': 'apimeter',
-    'version': '2.5.9',
+    'version': '2.6.0',
     'description': 'One-stop solution for HTTP(S) testing.',
-    'long_description': "\n# ApiMeter\n\n*ApiMeter* is a simple & elegant, yet powerful HTTP(S) testing framework. Enjoy! ✨ 🚀 ✨\n\n## Design Philosophy\n\n- Embrace open source, stand on giants' shoulders, like [`Requests`][Requests], [`unittest`][unittest] and [`Locust`][Locust].\n- Convention over configuration.\n- Pursuit of high rewards, write once and achieve a variety of testing needs\n\n## Key Features\n\n- Inherit all powerful features of [`Requests`][Requests], just have fun to handle HTTP(S) in human way.\n- Define testcases in YAML or JSON format in concise and elegant manner.\n- Record and generate testcases with [`HAR`][HAR] support. see [`har2case`][har2case].\n- Supports `variables`/`extract`/`validate` mechanisms to create full test scenarios.\n- Supports perfect hook mechanism.\n- With `debugtalk.py` plugin, very easy to implement complex logic in testcase.\n- Testcases can be run in diverse ways, with single testcase, multiple testcases, or entire project folder.\n- Test report is concise and clear, with detailed log records.\n- With reuse of [`Locust`][Locust], you can run performance test without extra work.\n- CLI command supported, perfect combination with `CI/CD`.\n\n## Documentation\n\nApiMeter is rich documented.\n\n- [`中文用户使用手册`][user-docs-zh]\n- [`开发历程记录博客`][development-blogs]\n- [CHANGELOG](docs/CHANGELOG.md)\n\n## Usage\n```python\n# 报告支持忽略成功用例数据\napimeter xxx.yml --skip-success\n\n\n```\n\n\n[Requests]: http://docs.python-requests.org/en/master/\n[unittest]: https://docs.python.org/3/library/unittest.html\n[Locust]: http://locust.io/\n[har2case]: https://github.com/httprunner/har2case\n[user-docs-zh]: http://docs.httprunner.org/\n[development-blogs]: http://debugtalk.com/tags/httprunner/\n[HAR]: http://httparchive.org/\n[Swagger]: https://swagger.io/\n\n",
+    'long_description': "\n# ApiMeter\n\n*ApiMeter* is a simple & elegant, yet powerful HTTP(S) testing framework. Enjoy! ✨ 🚀 ✨\n\n## Design Philosophy\n\n- Embrace open source, stand on giants' shoulders, like [`Requests`][Requests], [`unittest`][unittest] and [`Locust`][Locust].\n- Convention over configuration.\n- Pursuit of high rewards, write once and achieve a variety of testing needs\n\n## Key Features\n\n- Inherit all powerful features of [`Requests`][Requests], just have fun to handle HTTP(S) in human way.\n- Define testcases in YAML or JSON format in concise and elegant manner.\n- Record and generate testcases with [`HAR`][HAR] support. see [`har2case`][har2case].\n- Supports `variables`/`extract`/`validate` mechanisms to create full test scenarios.\n- Supports perfect hook mechanism.\n- With `debugtalk.py` plugin, very easy to implement complex logic in testcase.\n- Testcases can be run in diverse ways, with single testcase, multiple testcases, or entire project folder.\n- Test report is concise and clear, with detailed log records.\n- With reuse of [`Locust`][Locust], you can run performance test without extra work.\n- CLI command supported, perfect combination with `CI/CD`.\n\n## Documentation\n\nApiMeter is rich documented.\n\n- [`中文用户使用手册`][user-docs-zh]\n- [`开发历程记录博客`][development-blogs]\n- [CHANGELOG](docs/CHANGELOG.md)\n\n## Usage\n```python\npoetry install  # 安装依赖\npoetry run python -m apimeter /path/to/api  # 完整生成报告\npoetry run python -m apimeter /path/to/api --skip-success  # 报告忽略成功用例数据\npoetry build  # 打包\npoetry publish  # 发布，根据提示输入pypi账号密码\npip install -i https://pypi.Python.org/simple/ apimeter  # 指定安装源，因为刚发布其他平台未及时同步\n```\n\n\n[Requests]: http://docs.python-requests.org/en/master/\n[unittest]: https://docs.python.org/3/library/unittest.html\n[Locust]: http://locust.io/\n[har2case]: https://github.com/httprunner/har2case\n[user-docs-zh]: http://docs.httprunner.org/\n[development-blogs]: http://debugtalk.com/tags/httprunner/\n[HAR]: http://httparchive.org/\n[Swagger]: https://swagger.io/\n\n",
     'author': 'debugtalk',
     'author_email': 'debugtalk@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/httprunner/httprunner',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `apimeter-2.5.9/PKG-INFO` & `apimeter-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apimeter
-Version: 2.5.9
+Version: 2.6.0
 Summary: One-stop solution for HTTP(S) testing.
 Home-page: https://github.com/httprunner/httprunner
 License: Apache-2.0
 Keywords: HTTP,api,test,requests,locustio
 Author: debugtalk
 Author-email: debugtalk@gmail.com
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*
@@ -73,18 +73,20 @@
 
 - [`中文用户使用手册`][user-docs-zh]
 - [`开发历程记录博客`][development-blogs]
 - [CHANGELOG](docs/CHANGELOG.md)
 
 ## Usage
 ```python
-# 报告支持忽略成功用例数据
-apimeter xxx.yml --skip-success
-
-
+poetry install  # 安装依赖
+poetry run python -m apimeter /path/to/api  # 完整生成报告
+poetry run python -m apimeter /path/to/api --skip-success  # 报告忽略成功用例数据
+poetry build  # 打包
+poetry publish  # 发布，根据提示输入pypi账号密码
+pip install -i https://pypi.Python.org/simple/ apimeter  # 指定安装源，因为刚发布其他平台未及时同步
 ```
 
 
 [Requests]: http://docs.python-requests.org/en/master/
 [unittest]: https://docs.python.org/3/library/unittest.html
 [Locust]: http://locust.io/
 [har2case]: https://github.com/httprunner/har2case
```


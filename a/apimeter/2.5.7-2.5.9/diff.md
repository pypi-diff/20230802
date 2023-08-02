# Comparing `tmp/apimeter-2.5.7.tar.gz` & `tmp/apimeter-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apimeter-2.5.7.tar", max compression
+gzip compressed data, was "apimeter-2.5.9.tar", max compression
```

## Comparing `apimeter-2.5.7.tar` & `apimeter-2.5.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11338 2022-03-24 09:54:48.862432 apimeter-2.5.7/LICENSE
--rw-r--r--   0        0        0     4423 2023-08-01 03:09:55.673206 apimeter-2.5.7/README.md
--rw-r--r--   0        0        0      127 2023-08-01 03:09:55.899513 apimeter-2.5.7/apimeter/__init__.py
--rw-r--r--   0        0        0       70 2023-08-01 08:22:03.518051 apimeter-2.5.7/apimeter/__main__.py
--rw-r--r--   0        0        0    10507 2023-08-01 08:22:03.466263 apimeter-2.5.7/apimeter/api.py
--rw-r--r--   0        0        0       84 2023-08-01 08:22:03.729523 apimeter-2.5.7/apimeter/builtin/__init__.py
--rw-r--r--   0        0        0     3016 2023-08-01 08:22:03.730004 apimeter-2.5.7/apimeter/builtin/comparators.py
--rw-r--r--   0        0        0      945 2023-08-01 08:22:03.742572 apimeter-2.5.7/apimeter/builtin/functions.py
--rw-r--r--   0        0        0     4084 2023-08-01 08:22:03.205269 apimeter-2.5.7/apimeter/cli.py
--rw-r--r--   0        0        0     9545 2023-08-01 08:22:03.536295 apimeter-2.5.7/apimeter/client.py
--rw-r--r--   0        0        0      969 2023-08-01 03:09:55.903562 apimeter-2.5.7/apimeter/compat.py
--rw-r--r--   0        0        0     2666 2023-08-01 08:22:03.552596 apimeter-2.5.7/apimeter/context.py
--rw-r--r--   0        0        0     1148 2023-08-01 08:22:03.570430 apimeter-2.5.7/apimeter/exceptions.py
--rw-r--r--   0        0        0      114 2022-03-24 09:54:48.912883 apimeter-2.5.7/apimeter/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 03:09:55.904830 apimeter-2.5.7/apimeter/ext/har2case/__init__.py
--rw-r--r--   0        0        0     4808 2023-08-01 03:09:55.905290 apimeter-2.5.7/apimeter/ext/locusts/README.md
--rw-r--r--   0        0        0        0 2023-08-01 03:09:55.905462 apimeter-2.5.7/apimeter/ext/locusts/__init__.py
--rw-r--r--   0        0        0       81 2023-08-01 08:22:03.742442 apimeter-2.5.7/apimeter/ext/locusts/__main__.py
--rw-r--r--   0        0        0     5250 2023-08-01 08:22:03.765674 apimeter-2.5.7/apimeter/ext/locusts/cli.py
--rw-r--r--   0        0        0     1253 2023-08-01 08:22:03.793873 apimeter-2.5.7/apimeter/ext/locusts/locustfile_template.py
--rw-r--r--   0        0        0      628 2023-08-01 08:22:03.859718 apimeter-2.5.7/apimeter/ext/locusts/utils.py
--rw-r--r--   0        0        0     4146 2023-08-01 08:22:04.010928 apimeter-2.5.7/apimeter/ext/uploader/__init__.py
--rw-r--r--   0        0        0      916 2023-08-01 08:22:04.013422 apimeter-2.5.7/apimeter/loader/__init__.py
--rw-r--r--   0        0        0    15600 2023-08-01 08:22:04.022297 apimeter-2.5.7/apimeter/loader/buildup.py
--rw-r--r--   0        0        0     6494 2023-08-01 08:22:04.133339 apimeter-2.5.7/apimeter/loader/check.py
--rw-r--r--   0        0        0     5729 2023-08-01 08:22:04.167408 apimeter-2.5.7/apimeter/loader/load.py
--rw-r--r--   0        0        0     3495 2023-08-01 08:22:04.168809 apimeter-2.5.7/apimeter/loader/locate.py
--rw-r--r--   0        0        0     1607 2023-08-01 03:09:55.909825 apimeter-2.5.7/apimeter/loader/schemas/api.schema.json
--rw-r--r--   0        0        0    14880 2023-08-01 03:09:55.910232 apimeter-2.5.7/apimeter/loader/schemas/common.schema.json
--rw-r--r--   0        0        0     5187 2023-08-01 03:09:55.910867 apimeter-2.5.7/apimeter/loader/schemas/testcase.schema.v1.json
--rw-r--r--   0        0        0     6518 2023-08-01 03:09:55.911363 apimeter-2.5.7/apimeter/loader/schemas/testcase.schema.v2.json
--rw-r--r--   0        0        0     1994 2023-08-01 03:09:55.911695 apimeter-2.5.7/apimeter/loader/schemas/testsuite.schema.v1.json
--rw-r--r--   0        0        0     2662 2023-08-01 03:09:55.912091 apimeter-2.5.7/apimeter/loader/schemas/testsuite.schema.v2.json
--rw-r--r--   0        0        0     2383 2023-08-01 03:09:55.912843 apimeter-2.5.7/apimeter/logger.py
--rw-r--r--   0        0        0    51426 2023-08-01 08:22:03.582092 apimeter-2.5.7/apimeter/parser.py
--rw-r--r--   0        0        0      535 2023-08-01 08:22:04.218023 apimeter-2.5.7/apimeter/report/__init__.py
--rw-r--r--   0        0        0      318 2023-08-01 08:22:04.229490 apimeter-2.5.7/apimeter/report/html/__init__.py
--rw-r--r--   0        0        0     2547 2023-08-01 08:22:03.492831 apimeter-2.5.7/apimeter/report/html/gen_report.py
--rw-r--r--   0        0        0     2069 2023-08-01 08:22:04.229940 apimeter-2.5.7/apimeter/report/html/result.py
--rw-r--r--   0        0        0    10851 2023-08-01 03:09:55.915410 apimeter-2.5.7/apimeter/report/html/template.html
--rw-r--r--   0        0        0     1216 2023-08-01 08:22:04.218259 apimeter-2.5.7/apimeter/report/report.py
--rw-r--r--   0        0        0     6623 2023-08-01 08:22:03.473242 apimeter-2.5.7/apimeter/report/stringify.py
--rw-r--r--   0        0        0     2560 2023-08-01 08:22:04.229747 apimeter-2.5.7/apimeter/report/summarize.py
--rw-r--r--   0        0        0    10207 2023-08-01 08:22:03.659043 apimeter-2.5.7/apimeter/response.py
--rw-r--r--   0        0        0    14709 2023-08-01 08:22:03.684423 apimeter-2.5.7/apimeter/runner.py
--rw-r--r--   0        0        0    19207 2023-08-01 08:22:03.698958 apimeter-2.5.7/apimeter/utils.py
--rw-r--r--   0        0        0     7191 2023-08-01 08:22:03.700026 apimeter-2.5.7/apimeter/validator.py
--rw-r--r--   0        0        0    10777 2023-08-01 03:09:55.674220 apimeter-2.5.7/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1832 2023-08-01 08:25:18.279983 apimeter-2.5.7/pyproject.toml
--rw-r--r--   0        0        0     6145 2023-08-01 08:25:30.288379 apimeter-2.5.7/setup.py
--rw-r--r--   0        0        0     6512 2023-08-01 08:25:30.289146 apimeter-2.5.7/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-08-02 02:17:02.393026 apimeter-2.5.9/LICENSE
+-rw-r--r--   0        0        0     1802 2023-08-02 02:42:35.294734 apimeter-2.5.9/README.md
+-rw-r--r--   0        0        0      127 2023-08-02 02:20:26.667452 apimeter-2.5.9/apimeter/__init__.py
+-rw-r--r--   0        0        0       70 2023-08-02 02:25:30.631590 apimeter-2.5.9/apimeter/__main__.py
+-rw-r--r--   0        0        0    10437 2023-08-02 02:25:30.631783 apimeter-2.5.9/apimeter/api.py
+-rw-r--r--   0        0        0       84 2023-08-02 02:25:30.918965 apimeter-2.5.9/apimeter/builtin/__init__.py
+-rw-r--r--   0        0        0     3017 2023-08-02 02:25:30.920367 apimeter-2.5.9/apimeter/builtin/comparators.py
+-rw-r--r--   0        0        0      925 2023-08-02 02:25:30.920584 apimeter-2.5.9/apimeter/builtin/functions.py
+-rw-r--r--   0        0        0     4322 2023-08-02 02:44:16.736931 apimeter-2.5.9/apimeter/cli.py
+-rw-r--r--   0        0        0     9351 2023-08-02 02:25:30.670264 apimeter-2.5.9/apimeter/client.py
+-rw-r--r--   0        0        0      965 2023-08-02 02:20:26.669576 apimeter-2.5.9/apimeter/compat.py
+-rw-r--r--   0        0        0     2666 2023-08-02 02:25:30.705540 apimeter-2.5.9/apimeter/context.py
+-rw-r--r--   0        0        0     1142 2023-08-02 02:25:30.817485 apimeter-2.5.9/apimeter/exceptions.py
+-rw-r--r--   0        0        0      114 2023-08-02 02:17:02.529002 apimeter-2.5.9/apimeter/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 02:20:26.671032 apimeter-2.5.9/apimeter/ext/har2case/__init__.py
+-rw-r--r--   0        0        0     4808 2023-08-02 02:20:26.671419 apimeter-2.5.9/apimeter/ext/locusts/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 02:20:26.671540 apimeter-2.5.9/apimeter/ext/locusts/__init__.py
+-rw-r--r--   0        0        0       81 2023-08-02 02:25:30.948807 apimeter-2.5.9/apimeter/ext/locusts/__main__.py
+-rw-r--r--   0        0        0     5481 2023-08-02 02:25:30.950454 apimeter-2.5.9/apimeter/ext/locusts/cli.py
+-rw-r--r--   0        0        0     1254 2023-08-02 02:25:31.206244 apimeter-2.5.9/apimeter/ext/locusts/locustfile_template.py
+-rw-r--r--   0        0        0      627 2023-08-02 02:25:31.290728 apimeter-2.5.9/apimeter/ext/locusts/utils.py
+-rw-r--r--   0        0        0     4148 2023-08-02 02:25:31.291005 apimeter-2.5.9/apimeter/ext/uploader/__init__.py
+-rw-r--r--   0        0        0      924 2023-08-02 02:25:31.295623 apimeter-2.5.9/apimeter/loader/__init__.py
+-rw-r--r--   0        0        0    15804 2023-08-02 02:25:31.299696 apimeter-2.5.9/apimeter/loader/buildup.py
+-rw-r--r--   0        0        0     6455 2023-08-02 02:25:31.299883 apimeter-2.5.9/apimeter/loader/check.py
+-rw-r--r--   0        0        0     5704 2023-08-02 02:25:31.355848 apimeter-2.5.9/apimeter/loader/load.py
+-rw-r--r--   0        0        0     3536 2023-08-02 02:25:31.299950 apimeter-2.5.9/apimeter/loader/locate.py
+-rw-r--r--   0        0        0     1607 2023-08-02 02:20:26.676961 apimeter-2.5.9/apimeter/loader/schemas/api.schema.json
+-rw-r--r--   0        0        0    14880 2023-08-02 02:20:26.677353 apimeter-2.5.9/apimeter/loader/schemas/common.schema.json
+-rw-r--r--   0        0        0     5187 2023-08-02 02:20:26.677757 apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v1.json
+-rw-r--r--   0        0        0     6518 2023-08-02 02:20:26.679107 apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v2.json
+-rw-r--r--   0        0        0     1994 2023-08-02 02:20:26.679520 apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v1.json
+-rw-r--r--   0        0        0     2662 2023-08-02 02:20:26.679888 apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v2.json
+-rw-r--r--   0        0        0     2367 2023-08-02 02:20:26.680214 apimeter-2.5.9/apimeter/logger.py
+-rw-r--r--   0        0        0    50881 2023-08-02 02:25:30.832063 apimeter-2.5.9/apimeter/parser.py
+-rw-r--r--   0        0        0      536 2023-08-02 02:25:31.498115 apimeter-2.5.9/apimeter/report/__init__.py
+-rw-r--r--   0        0        0      309 2023-08-02 02:25:31.516575 apimeter-2.5.9/apimeter/report/html/__init__.py
+-rw-r--r--   0        0        0     2627 2023-08-02 02:46:16.779127 apimeter-2.5.9/apimeter/report/html/gen_report.py
+-rw-r--r--   0        0        0     2064 2023-08-02 02:25:31.516709 apimeter-2.5.9/apimeter/report/html/result.py
+-rw-r--r--   0        0        0    10851 2023-08-02 02:20:26.683469 apimeter-2.5.9/apimeter/report/html/template.html
+-rw-r--r--   0        0        0     1153 2023-08-02 02:25:31.500348 apimeter-2.5.9/apimeter/report/report.py
+-rw-r--r--   0        0        0     6583 2023-08-02 02:25:31.501664 apimeter-2.5.9/apimeter/report/stringify.py
+-rw-r--r--   0        0        0     2414 2023-08-02 02:25:31.502172 apimeter-2.5.9/apimeter/report/summarize.py
+-rw-r--r--   0        0        0    10378 2023-08-02 02:25:30.866260 apimeter-2.5.9/apimeter/response.py
+-rw-r--r--   0        0        0    14575 2023-08-02 02:25:30.866650 apimeter-2.5.9/apimeter/runner.py
+-rw-r--r--   0        0        0    21296 2023-08-02 02:25:30.897029 apimeter-2.5.9/apimeter/utils.py
+-rw-r--r--   0        0        0     7257 2023-08-02 02:25:30.918344 apimeter-2.5.9/apimeter/validator.py
+-rw-r--r--   0        0        0    11026 2023-08-02 02:20:26.510919 apimeter-2.5.9/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1964 2023-08-02 02:35:45.851132 apimeter-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3707 2023-08-02 02:54:25.721357 apimeter-2.5.9/setup.py
+-rw-r--r--   0        0        0     3891 2023-08-02 02:54:25.721848 apimeter-2.5.9/PKG-INFO
```

### Comparing `apimeter-2.5.7/LICENSE` & `apimeter-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/api.py` & `apimeter-2.5.9/apimeter/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,67 +1,74 @@
 import os
 import unittest
 
-from sentry_sdk import capture_message
-
-from apimeter import (__version__, exceptions, loader, logger, parser,
-                        report, runner, utils)
+from apimeter import (
+    __version__,
+    exceptions,
+    loader,
+    logger,
+    parser,
+    report,
+    runner,
+    utils,
+)
+from apimeter.utils import ga_client
 
 
 class HttpRunner(object):
-    """ Developer Interface: Main Interface
-        Usage:
+    """Developer Interface: Main Interface
+    Usage:
 
-            from httprunner.api import HttpRunner
-            runner = HttpRunner(
-                failfast=True,
-                save_tests=True,
-                log_level="INFO",
-                log_file="test.log"
-            )
-            summary = runner.run(path_or_tests)
+        from httprunner.api import HttpRunner
+        runner = HttpRunner(
+            failfast=True,
+            save_tests=True,
+            log_level="INFO",
+            log_file="test.log"
+        )
+        summary = runner.run(path_or_tests)
 
     """
 
-    def __init__(self, failfast=False, save_tests=False, log_level="WARNING", log_file=None):
-        """ initialize HttpRunner.
+    def __init__(
+        self, failfast=False, save_tests=False, log_level="WARNING", log_file=None
+    ):
+        """initialize HttpRunner.
 
         Args:
             failfast (bool): stop the test run on the first error or failure.
             save_tests (bool): save loaded/parsed tests to JSON file.
             log_level (str): logging level.
             log_file (str): log file path.
 
         """
         logger.setup_logger(log_level, log_file)
 
         self.exception_stage = "initialize HttpRunner()"
-        kwargs = {
-            "failfast": failfast,
-            "resultclass": report.HtmlTestResult
-        }
+        kwargs = {"failfast": failfast, "resultclass": report.HtmlTestResult}
         self.unittest_runner = unittest.TextTestRunner(**kwargs)
         self.test_loader = unittest.TestLoader()
         self.save_tests = save_tests
         self._summary = None
         self.project_working_directory = None
 
     def _add_tests(self, testcases):
-        """ initialize testcase with Runner() and add to test suite.
+        """initialize testcase with Runner() and add to test suite.
 
         Args:
             testcases (list): testcases list.
 
         Returns:
             unittest.TestSuite()
 
         """
+
         def _add_test(test_runner, test_dict):
-            """ add test to testcase.
-            """
+            """add test to testcase."""
+
             def test(self):
                 try:
                     test_runner.run_test(test_dict)
                 except exceptions.MyBaseFailure as ex:
                     self.fail(str(ex))
                 finally:
                     self.meta_datas = test_runner.meta_datas
@@ -86,42 +93,43 @@
 
             return test
 
         test_suite = unittest.TestSuite()
         for testcase in testcases:
             config = testcase.get("config", {})
             test_runner = runner.Runner(config)
-            TestSequense = type('TestSequense', (unittest.TestCase,), {})
+            TestSequense = type("TestSequense", (unittest.TestCase,), {})
 
             tests = testcase.get("teststeps", [])
             for index, test_dict in enumerate(tests):
                 times = test_dict.get("times", 1)
                 try:
                     times = int(times)
                 except ValueError:
                     raise exceptions.ParamsError(
-                        "times should be digit, given: {}".format(times))
+                        "times should be digit, given: {}".format(times)
+                    )
 
                 for times_index in range(times):
                     # suppose one testcase should not have more than 9999 steps,
                     # and one step should not run more than 999 times.
-                    test_method_name = 'test_{:04}_{:03}'.format(index, times_index)
+                    test_method_name = "test_{:04}_{:03}".format(index, times_index)
                     test_method = _add_test(test_runner, test_dict)
                     setattr(TestSequense, test_method_name, test_method)
 
             loaded_testcase = self.test_loader.loadTestsFromTestCase(TestSequense)
             setattr(loaded_testcase, "config", config)
             setattr(loaded_testcase, "teststeps", tests)
             setattr(loaded_testcase, "runner", test_runner)
             test_suite.addTest(loaded_testcase)
 
         return test_suite
 
     def _run_suite(self, test_suite):
-        """ run tests in test_suite
+        """run tests in test_suite
 
         Args:
             test_suite: unittest.TestSuite()
 
         Returns:
             list: tests_results
 
@@ -137,33 +145,29 @@
                 tests_results.append((testcase, result))
             else:
                 tests_results.insert(0, (testcase, result))
 
         return tests_results
 
     def _aggregate(self, tests_results):
-        """ aggregate results
+        """aggregate results
 
         Args:
             tests_results (list): list of (testcase, result)
 
         """
         summary = {
             "success": True,
             "stat": {
-                "testcases": {
-                    "total": len(tests_results),
-                    "success": 0,
-                    "fail": 0
-                },
-                "teststeps": {}
+                "testcases": {"total": len(tests_results), "success": 0, "fail": 0},
+                "teststeps": {},
             },
             "time": {},
             "platform": report.get_platform(),
-            "details": []
+            "details": [],
         }
 
         for tests_result in tests_results:
             testcase, result = tests_result
             testcase_summary = report.get_summary(result)
 
             if testcase_summary["success"]:
@@ -171,25 +175,26 @@
             else:
                 summary["stat"]["testcases"]["fail"] += 1
 
             summary["success"] &= testcase_summary["success"]
             testcase_summary["name"] = testcase.config.get("name")
             testcase_summary["in_out"] = utils.get_testcase_io(testcase)
 
-            report.aggregate_stat(summary["stat"]["teststeps"], testcase_summary["stat"])
+            report.aggregate_stat(
+                summary["stat"]["teststeps"], testcase_summary["stat"]
+            )
             report.aggregate_stat(summary["time"], testcase_summary["time"])
 
             summary["details"].append(testcase_summary)
 
         return summary
 
     def run_tests(self, tests_mapping):
-        """ run testcase/testsuite data
-        """
-        capture_message("start to run tests")
+        """run testcase/testsuite data"""
+        ga_client.track_event("RunAPITests", "hrun")
         project_mapping = tests_mapping.get("project_mapping", {})
         self.project_working_directory = project_mapping.get("PWD", os.getcwd())
 
         if self.save_tests:
             utils.dump_logs(tests_mapping, project_mapping, "loaded")
 
         # parse tests
@@ -228,15 +233,15 @@
             # save variables and export data
             vars_out = self.get_vars_out()
             utils.dump_logs(vars_out, project_mapping, "io")
 
         return self._summary
 
     def get_vars_out(self):
-        """ get variables and output
+        """get variables and output
         Returns:
             list: list of variables and output.
                 if tests are parameterized, list items are corresponded to parameters.
 
                 [
                     {
                         "in": {
@@ -251,21 +256,18 @@
 
             None: returns None if tests not started or finished or corrupted.
 
         """
         if not self._summary:
             return None
 
-        return [
-            summary["in_out"]
-            for summary in self._summary["details"]
-        ]
+        return [summary["in_out"] for summary in self._summary["details"]]
 
     def run_path(self, path, dot_env_path=None, mapping=None):
-        """ run testcase/testsuite file or folder.
+        """run testcase/testsuite file or folder.
 
         Args:
             path (str): testcase/testsuite file/foler path.
             dot_env_path (str): specified .env file path.
             mapping (dict): if mapping is specified, it will override variables in config block.
 
         Returns:
@@ -278,15 +280,15 @@
 
         if mapping:
             tests_mapping["project_mapping"]["variables"] = mapping
 
         return self.run_tests(tests_mapping)
 
     def run(self, path_or_tests, dot_env_path=None, mapping=None):
-        """ main interface.
+        """main interface.
 
         Args:
             path_or_tests:
                 str: testcase/testsuite file/foler path
                 dict: valid testcase/testsuite data
             dot_env_path (str): specified .env file path.
             mapping (dict): if mapping is specified, it will override variables in config block.
@@ -295,12 +297,16 @@
             dict: result summary
 
         """
         logger.log_info("HttpRunner version: {}".format(__version__))
         if loader.is_test_path(path_or_tests):
             return self.run_path(path_or_tests, dot_env_path, mapping)
         elif loader.is_test_content(path_or_tests):
-            project_working_directory = path_or_tests.get("project_mapping", {}).get("PWD", os.getcwd())
+            project_working_directory = path_or_tests.get("project_mapping", {}).get(
+                "PWD", os.getcwd()
+            )
             loader.init_pwd(project_working_directory)
             return self.run_tests(path_or_tests)
         else:
-            raise exceptions.ParamsError("Invalid testcase path or testcases: {}".format(path_or_tests))
+            raise exceptions.ParamsError(
+                "Invalid testcase path or testcases: {}".format(path_or_tests)
+            )
```

### Comparing `apimeter-2.5.7/apimeter/builtin/comparators.py` & `apimeter-2.5.9/apimeter/builtin/comparators.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -104,8 +104,8 @@
     assert builtin_str(check_value).endswith(builtin_str(expect_value))
 
 
 def _cast_to_int(expect_value):
     try:
         return int(expect_value)
     except Exception:
-        raise AssertionError("%r can't cast to int" % str(expect_value))
+        raise AssertionError("%r can't cast to int" % str(expect_value))
```

### Comparing `apimeter-2.5.7/apimeter/builtin/functions.py` & `apimeter-2.5.9/apimeter/builtin/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,33 +8,29 @@
 import time
 
 from apimeter.compat import builtin_str, integer_types
 from apimeter.exceptions import ParamsError
 
 
 def gen_random_string(str_len):
-    """ generate random string with specified length
-    """
-    return ''.join(
-        random.choice(string.ascii_letters + string.digits) for _ in range(str_len))
+    """generate random string with specified length"""
+    return "".join(
+        random.choice(string.ascii_letters + string.digits) for _ in range(str_len)
+    )
 
 
 def get_timestamp(str_len=13):
-    """ get timestamp string, length can only between 0 and 16
-    """
+    """get timestamp string, length can only between 0 and 16"""
     if isinstance(str_len, integer_types) and 0 < str_len < 17:
         return builtin_str(time.time()).replace(".", "")[:str_len]
 
     raise ParamsError("timestamp length can only between 0 and 16.")
 
 
 def get_current_date(fmt="%Y-%m-%d"):
-    """ get current date, default format is %Y-%m-%d
-    """
+    """get current date, default format is %Y-%m-%d"""
     return datetime.datetime.now().strftime(fmt)
 
 
 def sleep(n_secs):
-    """ sleep n seconds
-    """
+    """sleep n seconds"""
     time.sleep(n_secs)
-
```

### Comparing `apimeter-2.5.7/apimeter/cli.py` & `apimeter-2.5.9/apimeter/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,66 +6,74 @@
 
 from apimeter import __description__, __version__, exceptions
 from apimeter.api import HttpRunner
 from apimeter.compat import is_py2
 from apimeter.loader import load_cases
 from apimeter.logger import color_print, log_error
 from apimeter.report import gen_html_report
-from apimeter.utils import (create_scaffold, get_python2_retire_msg,
-                              prettify_json_file, init_sentry_sdk)
+from apimeter.utils import (
+    create_scaffold,
+    get_python2_retire_msg,
+    prettify_json_file,
+    init_sentry_sdk,
+)
 
 init_sentry_sdk()
 
 
 def main():
-    """ API test: parse command line options and run commands.
-    """
+    """API test: parse command line options and run commands."""
     if is_py2:
         color_print(get_python2_retire_msg(), "YELLOW")
 
     parser = argparse.ArgumentParser(description=__description__)
     parser.add_argument(
-        '-V', '--version', dest='version', action='store_true',
-        help="show version")
-    parser.add_argument(
-        'testfile_paths', nargs='*',
-        help="Specify api/testcase/testsuite file paths to run.")
-    parser.add_argument(
-        '--log-level', default='INFO',
-        help="Specify logging level, default is INFO.")
-    parser.add_argument(
-        '--log-file',
-        help="Write logs to specified file path.")
-    parser.add_argument(
-        '--dot-env-path',
-        help="Specify .env file path, which is useful for keeping sensitive data.")
+        "-V", "--version", dest="version", action="store_true", help="show version"
+    )
     parser.add_argument(
-        '--report-template',
-        help="Specify report template path.")
+        "testfile_paths",
+        nargs="*",
+        help="Specify api/testcase/testsuite file paths to run.",
+    )
     parser.add_argument(
-        '--report-dir',
-        help="Specify report save directory.")
+        "--log-level", default="INFO", help="Specify logging level, default is INFO."
+    )
+    parser.add_argument("--log-file", help="Write logs to specified file path.")
     parser.add_argument(
-        '--report-file',
-        help="Specify report file path, this has higher priority than specifying report dir.")
+        "--dot-env-path",
+        help="Specify .env file path, which is useful for keeping sensitive data.",
+    )
+    parser.add_argument("--report-template", help="Specify report template path.")
+    parser.add_argument("--report-dir", help="Specify report save directory.")
     parser.add_argument(
-        '--save-tests', action='store_true', default=False,
-        help="Save loaded/parsed/vars_out/summary json data to JSON files.")
+        "--report-file",
+        help="Specify report file path, this has higher priority than specifying report dir.",
+    )
     parser.add_argument(
-        '--failfast', action='store_true', default=False,
-        help="Stop the test run on the first error or failure.")
+        '--skip-success', action='store_true', default=False,
+        help="Specify skip success testcases in report.")    
     parser.add_argument(
-        '--startproject',
-        help="Specify new project name.")
+        "--save-tests",
+        action="store_true",
+        default=False,
+        help="Save loaded/parsed/vars_out/summary json data to JSON files.",
+    )
     parser.add_argument(
-        '--validate', nargs='*',
-        help="Validate YAML/JSON api/testcase/testsuite format.")
+        "--failfast",
+        action="store_true",
+        default=False,
+        help="Stop the test run on the first error or failure.",
+    )
+    parser.add_argument("--startproject", help="Specify new project name.")
     parser.add_argument(
-        '--prettify', nargs='*',
-        help="Prettify JSON testcase format.")
+        "--validate",
+        nargs="*",
+        help="Validate YAML/JSON api/testcase/testsuite format.",
+    )
+    parser.add_argument("--prettify", nargs="*", help="Prettify JSON testcase format.")
 
     args = parser.parse_args()
 
     if len(sys.argv) == 1:
         # no argument passed
         parser.print_help()
         sys.exit(0)
@@ -95,33 +103,39 @@
         create_scaffold(project_name)
         sys.exit(0)
 
     runner = HttpRunner(
         failfast=args.failfast,
         save_tests=args.save_tests,
         log_level=args.log_level,
-        log_file=args.log_file
+        log_file=args.log_file,
     )
 
     err_code = 0
     try:
         for path in args.testfile_paths:
             summary = runner.run(path, dot_env_path=args.dot_env_path)
-            report_dir = args.report_dir or os.path.join(runner.project_working_directory, "reports")
+            report_dir = args.report_dir or os.path.join(
+                runner.project_working_directory, "reports"
+            )
             gen_html_report(
                 summary,
                 report_template=args.report_template,
                 report_dir=report_dir,
-                report_file=args.report_file
+                report_file=args.report_file,
+                skip_success=args.skip_success,
             )
-            err_code |= (0 if summary and summary["success"] else 1)
+            err_code |= 0 if summary and summary["success"] else 1
     except Exception as ex:
-        color_print("!!!!!!!!!! exception stage: {} !!!!!!!!!!".format(runner.exception_stage), "YELLOW")
+        color_print(
+            "!!!!!!!!!! exception stage: {} !!!!!!!!!!".format(runner.exception_stage),
+            "YELLOW",
+        )
         color_print(str(ex), "RED")
         sentry_sdk.capture_exception(ex)
         err_code = 1
 
     sys.exit(err_code)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `apimeter-2.5.7/apimeter/client.py` & `apimeter-2.5.9/apimeter/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 # encoding: utf-8
 
 import time
 
 import requests
 import urllib3
 from requests import Request, Response
-from requests.exceptions import (InvalidSchema, InvalidURL, MissingSchema,
-                                 RequestException)
+from requests.exceptions import (
+    InvalidSchema,
+    InvalidURL,
+    MissingSchema,
+    RequestException,
+)
 
 from apimeter import logger, response
 from apimeter.utils import lower_dict_keys, omit_long_data
 
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 def get_req_resp_record(resp_obj):
-    """ get request and response info from Response() object.
-    """
+    """get request and response info from Response() object."""
+
     def log_print(req_resp_dict, r_type):
         msg = "\n================== {} details ==================\n".format(r_type)
         for key, value in req_resp_dict[r_type].items():
             msg += "{:<16} : {}\n".format(key, repr(value))
         logger.log_debug(msg)
 
-    req_resp_dict = {
-        "request": {},
-        "response": {}
-    }
+    req_resp_dict = {"request": {}, "response": {}}
 
     # record actual request info
     req_resp_dict["request"]["url"] = resp_obj.request.url
     req_resp_dict["request"]["method"] = resp_obj.request.method
     req_resp_dict["request"]["headers"] = dict(resp_obj.request.headers)
 
     request_body = resp_obj.request.body
     if request_body:
-        request_content_type = lower_dict_keys(
-            req_resp_dict["request"]["headers"]
-        ).get("content-type")
+        request_content_type = lower_dict_keys(req_resp_dict["request"]["headers"]).get(
+            "content-type"
+        )
         if request_content_type and "multipart/form-data" in request_content_type:
             # upload file type
             req_resp_dict["request"]["body"] = "upload file stream (OMITTED)"
         else:
             req_resp_dict["request"]["body"] = request_body
 
     # log request details in debug mode
@@ -79,59 +80,54 @@
     # log response details in debug mode
     log_print(req_resp_dict, "response")
 
     return req_resp_dict
 
 
 class ApiResponse(Response):
-
     def raise_for_status(self):
-        if hasattr(self, 'error') and self.error:
+        if hasattr(self, "error") and self.error:
             raise self.error
         Response.raise_for_status(self)
 
 
 class HttpSession(requests.Session):
     """
     Class for performing HTTP requests and holding (session-) cookies between requests (in order
     to be able to log in and out of websites). Each request is logged so that HttpRunner can
     display statistics.
 
     This is a slightly extended version of `python-request <http://python-requests.org>`_'s
     :py:class:`requests.Session` class and mostly this class works exactly the same.
     """
+
     def __init__(self):
         super(HttpSession, self).__init__()
         self.init_meta_data()
 
     def init_meta_data(self):
-        """ initialize meta_data, it will store detail data of request and response
-        """
+        """initialize meta_data, it will store detail data of request and response"""
         self.meta_data = {
             "name": "",
             "data": [
                 {
-                    "request": {
-                        "url": "N/A",
-                        "method": "N/A",
-                        "headers": {}
-                    },
+                    "request": {"url": "N/A", "method": "N/A", "headers": {}},
                     "response": {
                         "status_code": "N/A",
                         "headers": {},
                         "encoding": None,
-                        "content_type": ""
-                    }
+                        "content_type": "",
+                    },
                 }
             ],
             "stat": {
                 "content_size": "N/A",
                 "response_time_ms": "N/A",
                 "elapsed_ms": "N/A",
-            }
+            },
         }
 
     def update_last_req_resp_record(self, resp_obj):
         """
         update request and response info from Response() object.
         """
         self.meta_data["data"].pop()
@@ -198,34 +194,31 @@
         else:
             content_size = len(response.content or "")
 
         # record the consumed time
         self.meta_data["stat"] = {
             "response_time_ms": response_time_ms,
             "elapsed_ms": response.elapsed.microseconds / 1000.0,
-            "content_size": content_size
+            "content_size": content_size,
         }
 
         # record request and response histories, include 30X redirection
         response_list = response.history + [response]
         self.meta_data["data"] = [
-            get_req_resp_record(resp_obj)
-            for resp_obj in response_list
+            get_req_resp_record(resp_obj) for resp_obj in response_list
         ]
 
         try:
             response.raise_for_status()
         except RequestException as e:
-            logger.log_error(u"{exception}".format(exception=str(e)))
+            logger.log_error("{exception}".format(exception=str(e)))
         else:
             logger.log_info(
                 """status_code: {}, response_time(ms): {} ms, response_length: {} bytes\n""".format(
-                    response.status_code,
-                    response_time_ms,
-                    content_size
+                    response.status_code, response_time_ms, content_size
                 )
             )
 
         return response
 
     def _send_request_safe_mode(self, method, url, **kwargs):
         """
```

### Comparing `apimeter-2.5.7/apimeter/compat.py` & `apimeter-2.5.9/apimeter/compat.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 # Pythons
 # -------
 
 # Syntax sugar.
 _ver = sys.version_info
 
 #: Python 2.x?
-is_py2 = (_ver[0] == 2)
+is_py2 = _ver[0] == 2
 
 #: Python 3.x?
-is_py3 = (_ver[0] == 3)
+is_py3 = _ver[0] == 3
 
 
 # ---------
 # Specifics
 # ---------
 
 try:
```

### Comparing `apimeter-2.5.7/apimeter/context.py` & `apimeter-2.5.9/apimeter/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from apimeter import parser, utils
 
 
 class SessionContext(object):
-    """ HttpRunner session, store runtime variables.
+    """HttpRunner session, store runtime variables.
 
     Examples:
         >>> variables = {"SECRET_KEY": "DebugTalk"}
         >>> context = SessionContext(variables)
 
         Equivalent to:
         >>> context = SessionContext()
         >>> context.update_session_variables(variables)
 
     """
 
     def __init__(self, variables=None):
         variables_mapping = utils.ensure_mapping_format(variables or {})
-        self.session_variables_mapping = parser.parse_variables_mapping(variables_mapping)
+        self.session_variables_mapping = parser.parse_variables_mapping(
+            variables_mapping
+        )
         self.test_variables_mapping = {}
         self.init_test_variables()
 
     def init_test_variables(self, variables_mapping=None):
-        """ init test variables, called when each test(api) starts.
+        """init test variables, called when each test(api) starts.
             variables_mapping will be evaluated first.
 
         Args:
             variables_mapping (dict)
                 {
                     "random": "${gen_random_string(5)}",
                     "authorization": "${gen_md5($TOKEN, $data, $random)}",
@@ -41,24 +43,23 @@
 
         self.test_variables_mapping = {}
         # priority: extracted variable > teststep variable
         self.test_variables_mapping.update(parsed_variables_mapping)
         self.test_variables_mapping.update(self.session_variables_mapping)
 
     def update_test_variables(self, variable_name, variable_value):
-        """ update test variables, these variables are only valid in the current test.
-        """
+        """update test variables, these variables are only valid in the current test."""
         self.test_variables_mapping[variable_name] = variable_value
 
     def update_session_variables(self, variables_mapping):
-        """ update session with extracted variables mapping.
-            these variables are valid in the whole running session.
+        """update session with extracted variables mapping.
+        these variables are valid in the whole running session.
         """
         variables_mapping = utils.ensure_mapping_format(variables_mapping)
         self.session_variables_mapping.update(variables_mapping)
         self.test_variables_mapping.update(self.session_variables_mapping)
 
     def eval_content(self, content):
-        """ evaluate content recursively, take effect on each variable and function in content.
-            content may be in any data structure, include dict, list, tuple, number, string, etc.
+        """evaluate content recursively, take effect on each variable and function in content.
+        content may be in any data structure, include dict, list, tuple, number, string, etc.
         """
         return parser.parse_lazy_data(content, self.test_variables_mapping)
```

### Comparing `apimeter-2.5.7/apimeter/exceptions.py` & `apimeter-2.5.9/apimeter/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -77,9 +77,8 @@
 
 
 class TestcaseNotFound(NotFoundError):
     pass
 
 
 class SummaryEmpty(MyBaseError):
-    """ test result summary data is empty
-    """
+    """test result summary data is empty"""
```

### Comparing `apimeter-2.5.7/apimeter/ext/locusts/README.md` & `apimeter-2.5.9/apimeter/ext/locusts/README.md`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/ext/locusts/cli.py` & `apimeter-2.5.9/apimeter/ext/locusts/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 try:
     # monkey patch ssl at beginning to avoid RecursionError when running locust.
     from gevent import monkey
+
     monkey.patch_ssl()
     from locust import main as locust_main
 except ImportError:
     msg = """
 Locust is not installed, install first and try again.
 install with pip:
 $ pip install locustio
 """
     print(msg)
     import sys
+
     sys.exit(0)
 
 import io
 import multiprocessing
 import os
 import sys
 
@@ -22,54 +24,58 @@
 from apimeter import logger
 from apimeter.utils import init_sentry_sdk
 
 init_sentry_sdk()
 
 
 def parse_locustfile(file_path):
-    """ parse testcase file and return locustfile path.
-        if file_path is a Python file, assume it is a locustfile
-        if file_path is a YAML/JSON file, convert it to locustfile
+    """parse testcase file and return locustfile path.
+    if file_path is a Python file, assume it is a locustfile
+    if file_path is a YAML/JSON file, convert it to locustfile
     """
     if not os.path.isfile(file_path):
         logger.color_print("file path invalid, exit.", "RED")
         sys.exit(1)
 
     file_suffix = os.path.splitext(file_path)[1]
     if file_suffix == ".py":
         locustfile_path = file_path
-    elif file_suffix in ['.yaml', '.yml', '.json']:
+    elif file_suffix in [".yaml", ".yml", ".json"]:
         locustfile_path = gen_locustfile(file_path)
     else:
         # '' or other suffix
         logger.color_print("file type should be YAML/JSON/Python, exit.", "RED")
         sys.exit(1)
 
     return locustfile_path
 
 
 def gen_locustfile(testcase_file_path):
-    """ generate locustfile from template.
-    """
-    locustfile_path = 'locustfile.py'
+    """generate locustfile from template."""
+    locustfile_path = "locustfile.py"
     template_path = os.path.join(
-        os.path.dirname(os.path.realpath(__file__)),
-        "locustfile_template.py"
+        os.path.dirname(os.path.realpath(__file__)), "locustfile_template.py"
     )
 
-    with io.open(template_path, encoding='utf-8') as template:
-        with io.open(locustfile_path, 'w', encoding='utf-8') as locustfile:
+    with io.open(template_path, encoding="utf-8") as template:
+        with io.open(locustfile_path, "w", encoding="utf-8") as locustfile:
             template_content = template.read()
-            template_content = template_content.replace("$TESTCASE_FILE", testcase_file_path)
+            template_content = template_content.replace(
+                "$TESTCASE_FILE", testcase_file_path
+            )
             locustfile.write(template_content)
 
     return locustfile_path
 
 
 def start_locust_main():
+    from apimeter.utils import ga_client
+
+    ga_client.track_event("RunLoadTests", "locust")
+
     locust_main.main()
 
 
 def start_master(sys_argv):
     sys_argv.append("--master")
     sys.argv = sys_argv
     start_locust_main()
@@ -99,18 +105,17 @@
         else:
             start_master(sys_argv)
     except KeyboardInterrupt:
         manager.shutdown()
 
 
 def main():
-    """ Performance test with locust: parse command line options and run commands.
-    """
+    """Performance test with locust: parse command line options and run commands."""
     print("HttpRunner version: {}".format(__version__))
-    sys.argv[0] = 'locust'
+    sys.argv[0] = "locust"
     if len(sys.argv) == 1:
         sys.argv.extend(["-h"])
 
     if sys.argv[1] in ["-h", "--help", "-V", "--version"]:
         start_locust_main()
 
     def get_arg_index(*target_args):
@@ -140,35 +145,42 @@
         print("Testcase file is not specified, exit.")
         sys.exit(1)
 
     testcase_file_path = sys.argv[testcase_index]
     sys.argv[testcase_index] = parse_locustfile(testcase_file_path)
 
     if "--processes" in sys.argv:
-        """ locusts -f locustfile.py --processes 4
-        """
+        """locusts -f locustfile.py --processes 4"""
         if "--no-web" in sys.argv:
             logger.log_error("conflict parameter args: --processes & --no-web. \nexit.")
             sys.exit(1)
 
-        processes_index = sys.argv.index('--processes')
+        processes_index = sys.argv.index("--processes")
         processes_count_index = processes_index + 1
         if processes_count_index >= len(sys.argv):
-            """ do not specify processes count explicitly
-                locusts -f locustfile.py --processes
+            """do not specify processes count explicitly
+            locusts -f locustfile.py --processes
             """
             processes_count = multiprocessing.cpu_count()
-            logger.log_warning("processes count not specified, use {} by default.".format(processes_count))
+            logger.log_warning(
+                "processes count not specified, use {} by default.".format(
+                    processes_count
+                )
+            )
         else:
             try:
-                """ locusts -f locustfile.py --processes 4 """
+                """locusts -f locustfile.py --processes 4"""
                 processes_count = int(sys.argv[processes_count_index])
                 sys.argv.pop(processes_count_index)
             except ValueError:
-                """ locusts -f locustfile.py --processes -P 8888 """
+                """locusts -f locustfile.py --processes -P 8888"""
                 processes_count = multiprocessing.cpu_count()
-                logger.log_warning("processes count not specified, use {} by default.".format(processes_count))
+                logger.log_warning(
+                    "processes count not specified, use {} by default.".format(
+                        processes_count
+                    )
+                )
 
         sys.argv.pop(processes_index)
         run_locusts_with_processes(sys.argv, processes_count)
     else:
         start_locust_main()
```

### Comparing `apimeter-2.5.7/apimeter/ext/locusts/locustfile_template.py` & `apimeter-2.5.9/apimeter/ext/locusts/locustfile_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from locust.events import request_failure
 
 from apimeter.exceptions import MyBaseError, MyBaseFailure
 from apimeter.ext.locusts.utils import prepare_locust_tests
 from apimeter.runner import Runner
 
 logging.getLogger().setLevel(logging.CRITICAL)
-logging.getLogger('locust.main').setLevel(logging.INFO)
-logging.getLogger('locust.runners').setLevel(logging.INFO)
+logging.getLogger("locust.main").setLevel(logging.INFO)
+logging.getLogger("locust.runners").setLevel(logging.INFO)
 
 
 class WebPageTasks(TaskSet):
     def on_start(self):
         config = {}
         self.test_runner = Runner(config, self.client)
 
@@ -24,15 +24,15 @@
         try:
             self.test_runner.run_test(test_dict)
         except (AssertionError, MyBaseError, MyBaseFailure) as ex:
             request_failure.fire(
                 request_type=self.test_runner.exception_request_type,
                 name=self.test_runner.exception_name,
                 response_time=0,
-                exception=ex
+                exception=ex,
             )
 
 
 class WebPageUser(HttpLocust):
     host = ""
     task_set = WebPageTasks
     min_wait = 10
```

### Comparing `apimeter-2.5.7/apimeter/ext/locusts/utils.py` & `apimeter-2.5.9/apimeter/ext/locusts/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from apimeter import loader, parser
 
 
 def prepare_locust_tests(path):
-    """ prepare locust testcases
+    """prepare locust testcases
 
     Args:
         path (str): testcase file path.
 
     Returns:
         list: locust tests data
```

### Comparing `apimeter-2.5.7/apimeter/ext/uploader/__init__.py` & `apimeter-2.5.9/apimeter/ext/uploader/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     print(msg)
     sys.exit(0)
 
 from apimeter.exceptions import ParamsError
 
 
 def prepare_upload_test(test_dict):
-    """ preprocess for upload test
+    """preprocess for upload test
         replace `upload` info with MultipartEncoder
 
     Args:
         test_dict (dict):
 
             {
                 "variables": {},
@@ -92,22 +92,23 @@
         test_dict["variables"][key] = value
         params_list.append("{}=${}".format(key, key))
 
     params_str = ", ".join(params_list)
     test_dict["variables"]["m_encoder"] = "${multipart_encoder(" + params_str + ")}"
 
     test_dict["request"].setdefault("headers", {})
-    test_dict["request"]["headers"]["Content-Type"] = "${multipart_content_type($m_encoder)}"
+    test_dict["request"]["headers"][
+        "Content-Type"
+    ] = "${multipart_content_type($m_encoder)}"
 
     test_dict["request"]["data"] = "$m_encoder"
 
 
 def multipart_encoder(**kwargs):
-    """ initialize MultipartEncoder with uploading fields.
-    """
+    """initialize MultipartEncoder with uploading fields."""
 
     def get_filetype(file_path):
         file_type = filetype.guess(file_path)
         if file_type:
             return file_type.mime
         else:
             return "text/html"
@@ -118,27 +119,27 @@
         if os.path.isabs(value):
             # value is absolute file path
             _file_path = value
             is_exists_file = os.path.isfile(value)
         else:
             # value is not absolute file path, check if it is relative file path
             from apimeter.loader import get_pwd
+
             _file_path = os.path.join(get_pwd(), value)
             is_exists_file = os.path.isfile(_file_path)
 
         if is_exists_file:
             # value is file path to upload
             filename = os.path.basename(_file_path)
             mime_type = get_filetype(_file_path)
             # TODO: fix ResourceWarning for unclosed file
-            file_handler = open(_file_path, 'rb')
+            file_handler = open(_file_path, "rb")
             fields_dict[key] = (filename, file_handler, mime_type)
         else:
             fields_dict[key] = value
 
     return MultipartEncoder(fields=fields_dict)
 
 
 def multipart_content_type(m_encoder):
-    """ prepare Content-Type for request headers
-    """
+    """prepare Content-Type for request headers"""
     return m_encoder.content_type
```

### Comparing `apimeter-2.5.7/apimeter/loader/__init__.py` & `apimeter-2.5.9/apimeter/loader/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 - locate: locate debugtalk.py, make it's dir as project root path
 - load: load testcase files and relevant data, including debugtalk.py, .env, yaml/json api/testcases, csv, etc.
 - buildup: assemble loaded content to httprunner testcase/testsuite data structure
 
 """
 
 from apimeter.loader.check import is_test_path, is_test_content, JsonSchemaChecker
-from apimeter.loader.locate import get_project_working_directory as get_pwd, \
-    init_project_working_directory as init_pwd
+from apimeter.loader.locate import (
+    get_project_working_directory as get_pwd,
+    init_project_working_directory as init_pwd,
+)
 from apimeter.loader.load import load_csv_file, load_builtin_functions
 from apimeter.loader.buildup import load_cases, load_project_data
 
 __all__ = [
     "is_test_path",
     "is_test_content",
     "JsonSchemaChecker",
     "get_pwd",
     "init_pwd",
     "load_csv_file",
     "load_builtin_functions",
     "load_project_data",
-    "load_cases"
+    "load_cases",
 ]
```

### Comparing `apimeter-2.5.7/apimeter/loader/buildup.py` & `apimeter-2.5.9/apimeter/loader/buildup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,52 @@
 import importlib
 import os
+import sys
 
 from apimeter import exceptions, logger, utils
+from apimeter.compat import is_py3
 from apimeter.loader.check import JsonSchemaChecker
-from apimeter.loader.load import load_module_functions, load_file, load_dot_env_file, \
-    load_folder_files
-from apimeter.loader.locate import init_project_working_directory, get_project_working_directory
-
-tests_def_mapping = {
-    "api": {},
-    "testcases": {}
-}
+from apimeter.loader.load import (
+    load_dot_env_file,
+    load_file,
+    load_folder_files,
+    load_module_functions,
+)
+from apimeter.loader.locate import (
+    get_project_working_directory,
+    init_project_working_directory,
+)
+
+tests_def_mapping = {"api": {}, "testcases": {}}
 
 
 def load_debugtalk_functions():
-    """ load project debugtalk.py module functions
+    """load project debugtalk.py module functions
         debugtalk.py should be located in project working directory.
 
     Returns:
         dict: debugtalk module functions mapping
             {
                 "func1_name": func1,
                 "func2_name": func2
             }
 
     """
     # load debugtalk.py module
-    imported_module = importlib.import_module("debugtalk")
+    if is_py3 and sys.modules.get("debugtalk"):
+        # importlib.reload only works in python 3
+        imported_module = importlib.reload(sys.modules["debugtalk"])
+    else:
+        imported_module = importlib.import_module("debugtalk")
+
     return load_module_functions(imported_module)
 
 
 def __extend_with_api_ref(raw_testinfo):
-    """ extend with api reference
+    """extend with api reference
 
     Raises:
         exceptions.ApiNotFound: api not found
 
     """
     api_name = raw_testinfo["api"]
 
@@ -59,46 +70,43 @@
 
     # NOTICE: avoid project_mapping been changed during iteration.
     raw_testinfo["api_def"] = utils.deepcopy_dict(block)
     tests_def_mapping["api"][api_name] = block
 
 
 def __extend_with_testcase_ref(raw_testinfo):
-    """ extend with testcase reference
-    """
+    """extend with testcase reference"""
     testcase_path = raw_testinfo["testcase"]
 
     if testcase_path not in tests_def_mapping["testcases"]:
         # make compatible with Windows/Linux
         pwd = get_project_working_directory()
-        testcase_path = os.path.join(
-            pwd,
-            *testcase_path.split("/")
-        )
+        testcase_path = os.path.join(pwd, *testcase_path.split("/"))
         loaded_testcase = load_file(testcase_path)
 
         if isinstance(loaded_testcase, list):
             # make compatible with version < 2.2.0
             testcase_dict = load_testcase(loaded_testcase)
         elif isinstance(loaded_testcase, dict) and "teststeps" in loaded_testcase:
             # format version 2, implemented in 2.2.0
             testcase_dict = load_testcase_v2(loaded_testcase)
         else:
             raise exceptions.FileFormatError(
-                "Invalid format testcase: {}".format(testcase_path))
+                "Invalid format testcase: {}".format(testcase_path)
+            )
 
         tests_def_mapping["testcases"][testcase_path] = testcase_dict
     else:
         testcase_dict = tests_def_mapping["testcases"][testcase_path]
 
     raw_testinfo["testcase_def"] = testcase_dict
 
 
 def load_teststep(raw_testinfo):
-    """ load testcase step content.
+    """load testcase step content.
         teststep maybe defined directly, or reference api/testcase.
 
     Args:
         raw_testinfo (dict): test data, maybe in 3 formats.
             # api reference
             {
                 "name": "add product to cart",
@@ -142,15 +150,15 @@
     else:
         pass
 
     return raw_testinfo
 
 
 def load_testcase(raw_testcase):
-    """ load testcase with api/testcase references.
+    """load testcase with api/testcase references.
 
     Args:
         raw_testcase (list): raw testcase content loaded from JSON/YAML file:
             [
                 # config part
                 {
                     "config": {
@@ -183,25 +191,24 @@
         key, test_block = item.popitem()
         if key == "config":
             config.update(test_block)
         elif key == "test":
             tests.append(load_teststep(test_block))
         else:
             logger.log_warning(
-                "unexpected block key: {}. block key should only be 'config' or 'test'.".format(key)
+                "unexpected block key: {}. block key should only be 'config' or 'test'.".format(
+                    key
+                )
             )
 
-    return {
-        "config": config,
-        "teststeps": tests
-    }
+    return {"config": config, "teststeps": tests}
 
 
 def load_testcase_v2(raw_testcase):
-    """ load testcase in format version 2.
+    """load testcase in format version 2.
 
     Args:
         raw_testcase (dict): raw testcase content loaded from JSON/YAML file:
             {
                 "config": {
                     "name": "xxx",
                     "variables": {}
@@ -224,23 +231,20 @@
                 "config": {},
                 "teststeps": [test11, test12]
             }
 
     """
     JsonSchemaChecker.validate_testcase_v2_format(raw_testcase)
     raw_teststeps = raw_testcase.pop("teststeps")
-    raw_testcase["teststeps"] = [
-        load_teststep(teststep)
-        for teststep in raw_teststeps
-    ]
+    raw_testcase["teststeps"] = [load_teststep(teststep) for teststep in raw_teststeps]
     return raw_testcase
 
 
 def load_testsuite(raw_testsuite):
-    """ load testsuite with testcase references.
+    """load testsuite with testcase references.
         support two different formats.
 
     Args:
         raw_testsuite (dict): raw testsuite content loaded from JSON/YAML file:
             # version 1, compatible with version < 2.2.0
             {
                 "config": {
@@ -306,15 +310,15 @@
         # invalid format
         raise exceptions.FileFormatError("Invalid testsuite format!")
 
     return raw_testsuite
 
 
 def load_test_file(path):
-    """ load test file, file maybe testcase/testsuite/api
+    """load test file, file maybe testcase/testsuite/api
 
     Args:
         path (str): test file path
 
     Returns:
         dict: loaded test content
 
@@ -381,27 +385,29 @@
         # invalid format
         raise exceptions.FileFormatError("Invalid test file format!")
 
     return loaded_content
 
 
 def load_project_data(test_path, dot_env_path=None):
-    """ load api, testcases, .env, debugtalk.py functions.
+    """load api, testcases, .env, debugtalk.py functions.
         api/testcases folder is relative to project_working_directory
 
     Args:
         test_path (str): test file/folder path, locate pwd from this path.
         dot_env_path (str): specified .env file path
 
     Returns:
         dict: project loaded api/testcases definitions,
             environments and debugtalk.py functions.
 
     """
-    debugtalk_path, project_working_directory = init_project_working_directory(test_path)
+    debugtalk_path, project_working_directory = init_project_working_directory(
+        test_path
+    )
 
     project_mapping = {}
 
     # load .env file
     # NOTICE:
     # environment variable maybe loaded in debugtalk.py
     # thus .env file should be loaded before loading debugtalk.py
@@ -419,15 +425,15 @@
     project_mapping["functions"] = debugtalk_functions
     project_mapping["test_path"] = os.path.abspath(test_path)
 
     return project_mapping
 
 
 def load_cases(path, dot_env_path=None):
-    """ load testcases from file path, extend and merge with api/testcase definitions.
+    """load testcases from file path, extend and merge with api/testcase definitions.
 
     Args:
         path (str): testcase/testsuite file/foler path.
             path could be in 2 types:
                 - absolute/relative file path
                 - absolute/relative folder path
         dot_env_path (str): specified .env file path
@@ -472,17 +478,15 @@
                     },
                     testsuite_2_dict
                 ]
             }
 
     """
 
-    tests_mapping = {
-        "project_mapping": load_project_data(path, dot_env_path)
-    }
+    tests_mapping = {"project_mapping": load_project_data(path, dot_env_path)}
 
     def __load_file_content(path):
         loaded_content = None
         try:
             loaded_content = load_test_file(path)
         except exceptions.ApiNotFound as ex:
             logger.log_warning("Invalid api reference in {}: {}".format(path, ex))
```

### Comparing `apimeter-2.5.7/apimeter/loader/check.py` & `apimeter-2.5.9/apimeter/loader/check.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,87 +11,82 @@
 common_schema_path = os.path.join(schemas_root_dir, "common.schema.json")
 api_schema_path = os.path.join(schemas_root_dir, "api.schema.json")
 testcase_schema_v1_path = os.path.join(schemas_root_dir, "testcase.schema.v1.json")
 testcase_schema_v2_path = os.path.join(schemas_root_dir, "testcase.schema.v2.json")
 testsuite_schema_v1_path = os.path.join(schemas_root_dir, "testsuite.schema.v1.json")
 testsuite_schema_v2_path = os.path.join(schemas_root_dir, "testsuite.schema.v2.json")
 
-with io.open(api_schema_path, encoding='utf-8') as f:
+with io.open(api_schema_path, encoding="utf-8") as f:
     api_schema = json.load(f)
 
-with io.open(common_schema_path, encoding='utf-8') as f:
+with io.open(common_schema_path, encoding="utf-8") as f:
     if platform.system() == "Windows":
-        absolute_base_path = 'file:///' + os.path.abspath(schemas_root_dir).replace("\\", "/") + '/'
+        absolute_base_path = (
+            "file:///" + os.path.abspath(schemas_root_dir).replace("\\", "/") + "/"
+        )
     else:
         # Linux, Darwin
         absolute_base_path = "file://" + os.path.abspath(schemas_root_dir) + "/"
 
     common_schema = json.load(f)
     resolver = jsonschema.RefResolver(absolute_base_path, common_schema)
 
-with io.open(testcase_schema_v1_path, encoding='utf-8') as f:
+with io.open(testcase_schema_v1_path, encoding="utf-8") as f:
     testcase_schema_v1 = json.load(f)
 
-with io.open(testcase_schema_v2_path, encoding='utf-8') as f:
+with io.open(testcase_schema_v2_path, encoding="utf-8") as f:
     testcase_schema_v2 = json.load(f)
 
-with io.open(testsuite_schema_v1_path, encoding='utf-8') as f:
+with io.open(testsuite_schema_v1_path, encoding="utf-8") as f:
     testsuite_schema_v1 = json.load(f)
 
-with io.open(testsuite_schema_v2_path, encoding='utf-8') as f:
+with io.open(testsuite_schema_v2_path, encoding="utf-8") as f:
     testsuite_schema_v2 = json.load(f)
 
 
 class JsonSchemaChecker(object):
-
     @staticmethod
     def validate_format(content, scheme):
-        """ check api/testcase/testsuite format if valid
-        """
+        """check api/testcase/testsuite format if valid"""
         try:
             jsonschema.validate(content, scheme, resolver=resolver)
         except jsonschema.exceptions.ValidationError as ex:
             logger.log_error(str(ex))
             raise exceptions.FileFormatError
 
         return True
 
     @staticmethod
     def validate_api_format(content):
-        """ check api format if valid
-        """
+        """check api format if valid"""
         return JsonSchemaChecker.validate_format(content, api_schema)
 
     @staticmethod
     def validate_testcase_v1_format(content):
-        """ check testcase format v1 if valid
-        """
+        """check testcase format v1 if valid"""
         return JsonSchemaChecker.validate_format(content, testcase_schema_v1)
 
     @staticmethod
     def validate_testcase_v2_format(content):
-        """ check testcase format v2 if valid
-        """
+        """check testcase format v2 if valid"""
         return JsonSchemaChecker.validate_format(content, testcase_schema_v2)
 
     @staticmethod
     def validate_testsuite_v1_format(content):
-        """ check testsuite format v1 if valid
-        """
+        """check testsuite format v1 if valid"""
         return JsonSchemaChecker.validate_format(content, testsuite_schema_v1)
 
     @staticmethod
     def validate_testsuite_v2_format(content):
-        """ check testsuite format v2 if valid
-        """
+        """check testsuite format v2 if valid"""
         return JsonSchemaChecker.validate_format(content, testsuite_schema_v2)
 
 
 def is_test_path(path):
-    """ check if path is valid json/yaml file path or a existed directory.
+    """check if path is valid json/yaml file path or a existed directory.
 
     Args:
         path (str/list/tuple): file path/directory or file path list.
 
     Returns:
         bool: True if path is valid file path or path list, otherwise False.
 
@@ -111,29 +106,29 @@
         if not os.path.exists(path):
             return False
 
         # path exists
         if os.path.isfile(path):
             # path is a file
             file_suffix = os.path.splitext(path)[1].lower()
-            if file_suffix not in ['.json', '.yaml', '.yml']:
+            if file_suffix not in [".json", ".yaml", ".yml"]:
                 # path is not json/yaml file
                 return False
             else:
                 return True
         elif os.path.isdir(path):
             # path is a directory
             return True
         else:
             # path is neither a folder nor a file, maybe a symbol link or something else
             return False
 
 
 def is_test_content(data_structure):
-    """ check if data_structure is apis/testcases/testsuites.
+    """check if data_structure is apis/testcases/testsuites.
 
     Args:
         data_structure (dict): should include keys, apis or testcases or testsuites
 
     Returns:
         bool: True if data_structure is valid apis/testcases/testsuites, otherwise False.
```

### Comparing `apimeter-2.5.7/apimeter/loader/load.py` & `apimeter-2.5.9/apimeter/loader/load.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,48 +9,46 @@
 from apimeter import builtin
 from apimeter import exceptions, logger, utils
 from apimeter.loader.locate import get_project_working_directory
 
 try:
     # PyYAML version >= 5.1
     # ref: https://github.com/yaml/pyyaml/wiki/PyYAML-yaml.load(input)-Deprecation
-    yaml.warnings({'YAMLLoadWarning': False})
+    yaml.warnings({"YAMLLoadWarning": False})
 except AttributeError:
     pass
 
 
 def _load_yaml_file(yaml_file):
-    """ load yaml file and check file content format
-    """
-    with io.open(yaml_file, 'r', encoding='utf-8') as stream:
+    """load yaml file and check file content format"""
+    with io.open(yaml_file, "r", encoding="utf-8") as stream:
         try:
             yaml_content = yaml.load(stream)
         except yaml.YAMLError as ex:
             logger.log_error(str(ex))
             raise exceptions.FileFormatError
 
         return yaml_content
 
 
 def _load_json_file(json_file):
-    """ load json file and check file content format
-    """
-    with io.open(json_file, encoding='utf-8') as data_file:
+    """load json file and check file content format"""
+    with io.open(json_file, encoding="utf-8") as data_file:
         try:
             json_content = json.load(data_file)
         except exceptions.JSONDecodeError:
-            err_msg = u"JSONDecodeError: JSON file format error: {}".format(json_file)
+            err_msg = "JSONDecodeError: JSON file format error: {}".format(json_file)
             logger.log_error(err_msg)
             raise exceptions.FileFormatError(err_msg)
 
         return json_content
 
 
 def load_csv_file(csv_file):
-    """ load csv file and check file content format
+    """load csv file and check file content format
 
     Args:
         csv_file (str): csv file path, csv file content is like below:
 
     Returns:
         list: list of parameters, each parameter is in dict format
 
@@ -76,42 +74,42 @@
 
     if not os.path.isfile(csv_file):
         # file path not exist
         raise exceptions.CSVNotFound(csv_file)
 
     csv_content_list = []
 
-    with io.open(csv_file, encoding='utf-8') as csvfile:
+    with io.open(csv_file, encoding="utf-8") as csvfile:
         reader = csv.DictReader(csvfile)
         for row in reader:
             csv_content_list.append(row)
 
     return csv_content_list
 
 
 def load_file(file_path):
     if not os.path.isfile(file_path):
         raise exceptions.FileNotFound("{} does not exist.".format(file_path))
 
     file_suffix = os.path.splitext(file_path)[1].lower()
-    if file_suffix == '.json':
+    if file_suffix == ".json":
         return _load_json_file(file_path)
-    elif file_suffix in ['.yaml', '.yml']:
+    elif file_suffix in [".yaml", ".yml"]:
         return _load_yaml_file(file_path)
     elif file_suffix == ".csv":
         return load_csv_file(file_path)
     else:
         # '' or other suffix
-        err_msg = u"Unsupported file format: {}".format(file_path)
+        err_msg = "Unsupported file format: {}".format(file_path)
         logger.log_warning(err_msg)
         return []
 
 
 def load_folder_files(folder_path, recursive=True):
-    """ load folder path, return all files endswith yml/yaml/json in list.
+    """load folder path, return all files endswith yml/yaml/json in list.
 
     Args:
         folder_path (str): specified folder path to load
         recursive (bool): load files recursively if True
 
     Returns:
         list: files endswith yml/yaml/json
@@ -128,15 +126,15 @@
 
     file_list = []
 
     for dirpath, dirnames, filenames in os.walk(folder_path):
         filenames_list = []
 
         for filename in filenames:
-            if not filename.endswith(('.yml', '.yaml', '.json')):
+            if not filename.endswith((".yml", ".yaml", ".json")):
                 continue
 
             filenames_list.append(filename)
 
         for filename in filenames_list:
             file_path = os.path.join(dirpath, filename)
             file_list.append(file_path)
@@ -144,15 +142,15 @@
         if not recursive:
             break
 
     return file_list
 
 
 def load_dot_env_file(dot_env_path):
-    """ load .env file.
+    """load .env file.
 
     Args:
         dot_env_path (str): .env file path
 
     Returns:
         dict: environment variables mapping
 
@@ -168,15 +166,15 @@
     """
     if not os.path.isfile(dot_env_path):
         return {}
 
     logger.log_info("Loading environment variables from {}".format(dot_env_path))
     env_variables_mapping = {}
 
-    with io.open(dot_env_path, 'r', encoding='utf-8') as fp:
+    with io.open(dot_env_path, "r", encoding="utf-8") as fp:
         for line in fp:
             # maxsplit=1
             if "=" in line:
                 variable, value = line.split("=", 1)
             elif ":" in line:
                 variable, value = line.split(":", 1)
             else:
@@ -185,15 +183,15 @@
             env_variables_mapping[variable.strip()] = value.strip()
 
     utils.set_os_environ(env_variables_mapping)
     return env_variables_mapping
 
 
 def load_module_functions(module):
-    """ load python module functions.
+    """load python module functions.
 
     Args:
         module: python module
 
     Returns:
         dict: functions mapping for specified python module
 
@@ -209,11 +207,9 @@
         if isinstance(item, types.FunctionType):
             module_functions[name] = item
 
     return module_functions
 
 
 def load_builtin_functions():
-    """ load builtin module functions
-    """
+    """load builtin module functions"""
     return load_module_functions(builtin)
-
```

### Comparing `apimeter-2.5.7/apimeter/loader/locate.py` & `apimeter-2.5.9/apimeter/loader/locate.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from apimeter import exceptions, logger
 
 project_working_directory = None
 
 
 def locate_file(start_path, file_name):
-    """ locate filename and return absolute file path.
+    """locate filename and return absolute file path.
         searching will be recursive upward until current working directory or system root dir.
 
     Args:
         file_name (str): target locate file name
         start_path (str): start locating path, maybe file path or directory path
 
     Returns:
@@ -30,29 +30,33 @@
 
     file_path = os.path.join(start_dir_path, file_name)
     if os.path.isfile(file_path):
         return os.path.abspath(file_path)
 
     # current working directory
     if os.path.abspath(start_dir_path) == os.getcwd():
-        raise exceptions.FileNotFound("{} not found in {}".format(file_name, start_path))
+        raise exceptions.FileNotFound(
+            "{} not found in {}".format(file_name, start_path)
+        )
 
     # system root dir
     # Windows, e.g. 'E:\\'
     # Linux/Darwin, '/'
     parent_dir = os.path.dirname(start_dir_path)
     if parent_dir == start_dir_path:
-        raise exceptions.FileNotFound("{} not found in {}".format(file_name, start_path))
+        raise exceptions.FileNotFound(
+            "{} not found in {}".format(file_name, start_path)
+        )
 
     # locate recursive upward
     return locate_file(parent_dir, file_name)
 
 
 def locate_debugtalk_py(start_path):
-    """ locate debugtalk.py file
+    """locate debugtalk.py file
 
     Args:
         start_path (str): start locating path,
             maybe testcase file path or directory path
 
     Returns:
         str: debugtalk.py file path, None if not found
@@ -64,15 +68,15 @@
     except exceptions.FileNotFound:
         debugtalk_path = None
 
     return debugtalk_path
 
 
 def init_project_working_directory(test_path):
-    """ this should be called at startup
+    """this should be called at startup
 
         run test file:
             run_path -> load_cases -> load_project_data -> init_project_working_directory
         or run passed in data structure:
             run -> init_project_working_directory
 
     Args:
```

### Comparing `apimeter-2.5.7/apimeter/loader/schemas/api.schema.json` & `apimeter-2.5.9/apimeter/loader/schemas/api.schema.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/loader/schemas/common.schema.json` & `apimeter-2.5.9/apimeter/loader/schemas/common.schema.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/loader/schemas/testcase.schema.v1.json` & `apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v1.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/loader/schemas/testcase.schema.v2.json` & `apimeter-2.5.9/apimeter/loader/schemas/testcase.schema.v2.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/loader/schemas/testsuite.schema.v1.json` & `apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v1.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/loader/schemas/testsuite.schema.v2.json` & `apimeter-2.5.9/apimeter/loader/schemas/testsuite.schema.v2.json`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/logger.py` & `apimeter-2.5.9/apimeter/logger.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 
 init(autoreset=True)
 
 LOG_LEVEL = "INFO"
 LOG_FILE_PATH = ""
 
 log_colors_config = {
-    'DEBUG':    'cyan',
-    'INFO':     'green',
-    'WARNING':  'yellow',
-    'ERROR':    'red',
-    'CRITICAL': 'red',
+    "DEBUG": "cyan",
+    "INFO": "green",
+    "WARNING": "yellow",
+    "ERROR": "red",
+    "CRITICAL": "red",
 }
 loggers = {}
 
 
 def setup_logger(log_level, log_file=None):
     global LOG_LEVEL
     LOG_LEVEL = log_level
@@ -54,18 +54,18 @@
         if not os.path.isdir(log_dir):
             os.makedirs(log_dir)
         handler = logging.FileHandler(LOG_FILE_PATH, encoding="utf-8")
     else:
         handler = logging.StreamHandler(sys.stdout)
 
     formatter = ColoredFormatter(
-        u"%(log_color)s%(bg_white)s%(levelname)-8s%(reset)s %(message)s",
+        "%(log_color)s%(bg_white)s%(levelname)-8s%(reset)s %(message)s",
         datefmt=None,
         reset=True,
-        log_colors=log_colors_config
+        log_colors=log_colors_config,
     )
     handler.setFormatter(formatter)
     _logger.addHandler(handler)
 
     loggers[logger_key] = _logger
     return _logger
 
@@ -77,16 +77,16 @@
 
 def color_print(msg, color="WHITE"):
     fore_color = getattr(Fore, color.upper())
     print(fore_color + msg)
 
 
 def log_with_color(level):
-    """ log with color by different level
-    """
+    """log with color by different level"""
+
     def wrapper(text):
         color = log_colors_config[level.upper()]
         _logger = get_logger()
         getattr(_logger, level.lower())(coloring(text, color))
 
     return wrapper
```

### Comparing `apimeter-2.5.7/apimeter/parser.py` & `apimeter-2.5.9/apimeter/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 def get_parse_failed_testfiles():
     return parse_failed_testfiles
 
 
 def parse_string_value(str_value):
-    """ parse string to number if possible
+    """parse string to number if possible
     e.g. "123" => 123
          "12.2" => 12.3
          "abc" => "abc"
          "$var" => "$var"
     """
     try:
         return ast.literal_eval(str_value)
@@ -39,16 +39,15 @@
         return str_value
     except SyntaxError:
         # e.g. $var, ${func}
         return str_value
 
 
 def is_var_or_func_exist(content):
-    """ check if variable or function exist
-    """
+    """check if variable or function exist"""
     if not isinstance(content, basestring):
         return False
 
     try:
         match_start_position = content.index("$", 0)
     except ValueError:
         return False
@@ -67,15 +66,15 @@
         if var_match:
             return True
 
         return False
 
 
 def regex_findall_variables(content):
-    """ extract all variable names from content, which is in format $variable
+    """extract all variable names from content, which is in format $variable
 
     Args:
         content (str): string content
 
     Returns:
         list: variables list extracted from string content
 
@@ -92,24 +91,22 @@
         >>> regex_findall_variables("abc")
         []
 
     """
     try:
         vars_list = []
         for var_tuple in variable_regex_compile.findall(content):
-            vars_list.append(
-                var_tuple[0] or var_tuple[1]
-            )
+            vars_list.append(var_tuple[0] or var_tuple[1])
         return vars_list
     except TypeError:
         return []
 
 
 def regex_findall_functions(content):
-    """ extract all functions from string content, which are in format ${fun()}
+    """extract all functions from string content, which are in format ${fun()}
 
     Args:
         content (str): string content
 
     Returns:
         list: functions list extracted from string content
 
@@ -133,15 +130,15 @@
     try:
         return function_regex_compile.findall(content)
     except TypeError:
         return []
 
 
 def parse_parameters(parameters, variables_mapping=None, functions_mapping=None):
-    """ parse parameters and generate cartesian product.
+    """parse parameters and generate cartesian product.
 
     Args:
         parameters (list) parameters: parameter name and value in list
             parameter value may be in three types:
                 (1) data list, e.g. ["iOS/10.1", "iOS/10.2", "iOS/10.3"]
                 (2) call built-in parameterize function, "${parameterize(account.csv)}"
                 (3) call custom function in debugtalk.py, "${gen_app_version()}"
@@ -184,21 +181,17 @@
                 # ["app_version"], ["2.8.5"] => {"app_version": "2.8.5"}
                 # ["username", "password"], ["user1", "111111"] => {"username": "user1", "password": "111111"}
                 parameter_content_dict = dict(zip(parameter_name_list, parameter_item))
 
                 parameter_content_list.append(parameter_content_dict)
         else:
             # (2) & (3)
-            parsed_variables_mapping = parse_variables_mapping(
-                variables_mapping
-            )
+            parsed_variables_mapping = parse_variables_mapping(variables_mapping)
             parsed_parameter_content = eval_lazy_data(
-                parameter_content,
-                parsed_variables_mapping,
-                functions_mapping
+                parameter_content, parsed_variables_mapping, functions_mapping
             )
             if not isinstance(parsed_parameter_content, list):
                 raise exceptions.ParamsError("parameters syntax error!")
 
             parameter_content_list = []
             for parameter_item in parsed_parameter_content:
                 if isinstance(parameter_item, dict):
@@ -206,36 +199,35 @@
                     # {"app_version": "${gen_app_version()}"}
                     # gen_app_version() => [{'app_version': '2.8.5'}, {'app_version': '2.8.6'}]
                     # {"username-password": "${get_account()}"}
                     # get_account() => [
                     #       {"username": "user1", "password": "111111"},
                     #       {"username": "user2", "password": "222222"}
                     # ]
-                    parameter_dict = {key: parameter_item[key] for key in parameter_name_list}
+                    parameter_dict = {
+                        key: parameter_item[key] for key in parameter_name_list
+                    }
                 elif isinstance(parameter_item, (list, tuple)):
                     # {"username-password": "${get_account()}"}
                     # get_account() => [("user1", "111111"), ("user2", "222222")]
                     parameter_dict = dict(zip(parameter_name_list, parameter_item))
                 elif len(parameter_name_list) == 1:
                     # {"user_agent": "${get_user_agent()}"}
                     # get_user_agent() => ["iOS/10.1", "iOS/10.2"]
-                    parameter_dict = {
-                        parameter_name_list[0]: parameter_item
-                    }
+                    parameter_dict = {parameter_name_list[0]: parameter_item}
 
                 parameter_content_list.append(parameter_dict)
 
         parsed_parameters_list.append(parameter_content_list)
 
     return utils.gen_cartesian_product(*parsed_parameters_list)
 
 
 def get_uniform_comparator(comparator):
-    """ convert comparator alias to uniform name
-    """
+    """convert comparator alias to uniform name"""
     if comparator in ["eq", "equals", "==", "is"]:
         return "equals"
     elif comparator in ["lt", "less_than"]:
         return "less_than"
     elif comparator in ["le", "less_than_or_equals"]:
         return "less_than_or_equals"
     elif comparator in ["gt", "greater_than"]:
@@ -244,30 +236,43 @@
         return "greater_than_or_equals"
     elif comparator in ["ne", "not_equals"]:
         return "not_equals"
     elif comparator in ["str_eq", "string_equals"]:
         return "string_equals"
     elif comparator in ["len_eq", "length_equals", "count_eq"]:
         return "length_equals"
-    elif comparator in ["len_gt", "count_gt", "length_greater_than", "count_greater_than"]:
+    elif comparator in [
+        "len_gt",
+        "count_gt",
+        "length_greater_than",
+        "count_greater_than",
+    ]:
         return "length_greater_than"
-    elif comparator in ["len_ge", "count_ge", "length_greater_than_or_equals",
-                        "count_greater_than_or_equals"]:
+    elif comparator in [
+        "len_ge",
+        "count_ge",
+        "length_greater_than_or_equals",
+        "count_greater_than_or_equals",
+    ]:
         return "length_greater_than_or_equals"
     elif comparator in ["len_lt", "count_lt", "length_less_than", "count_less_than"]:
         return "length_less_than"
-    elif comparator in ["len_le", "count_le", "length_less_than_or_equals",
-                        "count_less_than_or_equals"]:
+    elif comparator in [
+        "len_le",
+        "count_le",
+        "length_less_than_or_equals",
+        "count_less_than_or_equals",
+    ]:
         return "length_less_than_or_equals"
     else:
         return comparator
 
 
 def uniform_validator(validator):
-    """ unify validator
+    """unify validator
 
     Args:
         validator (dict): validator maybe in two formats:
 
             format1: this is kept for compatiblity with the previous versions.
                 {"check": "status_code", "comparator": "eq", "expect": 201}
                 {"check": "$resp_body_success", "comparator": "eq", "expect": True}
@@ -306,23 +311,19 @@
 
     else:
         raise exceptions.ParamsError("invalid validator: {}".format(validator))
 
     # uniform comparator, e.g. lt => less_than, eq => equals
     comparator = get_uniform_comparator(comparator)
 
-    return {
-        "check": check_item,
-        "expect": expect_value,
-        "comparator": comparator
-    }
+    return {"check": check_item, "expect": expect_value, "comparator": comparator}
 
 
 def _convert_validators_to_mapping(validators):
-    """ convert validators list to mapping.
+    """convert validators list to mapping.
 
     Args:
         validators (list): validators in list
 
     Returns:
         dict: validators mapping, use (check, comparator) as key.
 
@@ -349,15 +350,15 @@
         key = (check, validator["comparator"])
         validators_mapping[key] = validator
 
     return validators_mapping
 
 
 def extend_validators(raw_validators, override_validators):
-    """ extend raw_validators with override_validators.
+    """extend raw_validators with override_validators.
         override_validators will merge and override raw_validators.
 
     Args:
         raw_validators (dict):
         override_validators (dict):
 
     Returns:
@@ -389,16 +390,17 @@
         return list(def_validators_mapping.values())
 
 
 ###############################################################################
 ##  parse content with variables and functions mapping
 ###############################################################################
 
+
 def get_mapping_variable(variable_name, variables_mapping):
-    """ get variable from variables_mapping.
+    """get variable from variables_mapping.
 
     Args:
         variable_name (str): variable name
         variables_mapping (dict): variables mapping
 
     Returns:
         mapping variable value.
@@ -410,15 +412,15 @@
     try:
         return variables_mapping[variable_name]
     except KeyError:
         raise exceptions.VariableNotFound("{} is not found.".format(variable_name))
 
 
 def get_mapping_function(function_name, functions_mapping):
-    """ get function from functions_mapping,
+    """get function from functions_mapping,
         if not found, then try to check if builtin function.
 
     Args:
         function_name (str): function name
         functions_mapping (dict): functions mapping
 
     Returns:
@@ -436,14 +438,15 @@
 
     elif function_name in ["environ", "ENV"]:
         return utils.get_os_environ
 
     elif function_name in ["multipart_encoder", "multipart_content_type"]:
         # extension for upload test
         from apimeter.ext import uploader
+
         return getattr(uploader, function_name)
 
     try:
         # check if HttpRunner builtin functions
         built_in_functions = loader.load_builtin_functions()
         return built_in_functions[function_name]
     except KeyError:
@@ -455,15 +458,15 @@
     except AttributeError:
         pass
 
     raise exceptions.FunctionNotFound("{} is not found.".format(function_name))
 
 
 def parse_function_params(params):
-    """ parse function params to args and kwargs.
+    """parse function params to args and kwargs.
 
     Args:
         params (str): function param in string
 
     Returns:
         dict: function meta dict
 
@@ -485,41 +488,37 @@
         >>> parse_function_params("a=1, b=2")
         {'args': [], 'kwargs': {'a': 1, 'b': 2}}
 
         >>> parse_function_params("1, 2, a=3, b=4")
         {'args': [1, 2], 'kwargs': {'a':3, 'b':4}}
 
     """
-    function_meta = {
-        "args": [],
-        "kwargs": {}
-    }
+    function_meta = {"args": [], "kwargs": {}}
 
     params_str = params.strip()
     if params_str == "":
         return function_meta
 
-    args_list = params_str.split(',')
+    args_list = params_str.split(",")
     for arg in args_list:
         arg = arg.strip()
-        if '=' in arg:
-            key, value = arg.split('=')
+        if "=" in arg:
+            key, value = arg.split("=")
             function_meta["kwargs"][key.strip()] = parse_string_value(value.strip())
         else:
             function_meta["args"].append(parse_string_value(arg))
 
     return function_meta
 
 
 class LazyFunction(object):
-    """ call function lazily.
-    """
+    """call function lazily."""
 
     def __init__(self, function_meta, functions_mapping=None, check_variables_set=None):
-        """ init LazyFunction object with function_meta
+        """init LazyFunction object with function_meta
 
         Args:
             function_meta (dict): function name, args and kwargs.
                 {
                     "func_name": "func",
                     "args": [1, 2]
                     "kwargs": {"a": 3, "b": 4}
@@ -528,33 +527,32 @@
         """
         self.functions_mapping = functions_mapping or {}
         self.check_variables_set = check_variables_set or set()
         self.cache_key = None
         self.__parse(function_meta)
 
     def __parse(self, function_meta):
-        """ init func as lazy functon instance
+        """init func as lazy functon instance
 
         Args:
             function_meta (dict): function meta including name, args and kwargs
         """
         self._func = get_mapping_function(
-            function_meta["func_name"],
-            self.functions_mapping
+            function_meta["func_name"], self.functions_mapping
         )
         self.func_name = self._func.__name__
         self._args = prepare_lazy_data(
             function_meta.get("args", []),
             self.functions_mapping,
-            self.check_variables_set
+            self.check_variables_set,
         )
         self._kwargs = prepare_lazy_data(
             function_meta.get("kwargs", {}),
             self.functions_mapping,
-            self.check_variables_set
+            self.check_variables_set,
         )
 
         if self.func_name == "load_csv_file":
             if len(self._args) != 1 or self._kwargs:
                 raise exceptions.ParamsError("P() should only pass in one argument!")
             self._args = [self._args[0]]
         elif self.func_name == "get_os_environ":
@@ -574,56 +572,56 @@
         if self._args:
             str_args = [str(arg) for arg in self._args]
             args_string += ", ".join(str_args)
 
         if self._kwargs:
             args_string += ", "
             str_kwargs = [
-                "{}={}".format(key, str(value))
-                for key, value in self._kwargs.items()
+                "{}={}".format(key, str(value)) for key, value in self._kwargs.items()
             ]
             args_string += ", ".join(str_kwargs)
 
         return "LazyFunction({}({}))".format(self.func_name, args_string)
 
     def __prepare_cache_key(self, args, kwargs):
         return self.func_name, repr(args), repr(kwargs)
 
     def to_value(self, variables_mapping=None):
-        """ parse lazy data with evaluated variables mapping.
-            Notice: variables_mapping should not contain any variable or function.
+        """parse lazy data with evaluated variables mapping.
+        Notice: variables_mapping should not contain any variable or function.
         """
         variables_mapping = variables_mapping or {}
         args = parse_lazy_data(self._args, variables_mapping)
         kwargs = parse_lazy_data(self._kwargs, variables_mapping)
         self.cache_key = self.__prepare_cache_key(args, kwargs)
         return self._func(*args, **kwargs)
 
 
 cached_functions_mapping = {}
 """ cached function calling results.
 """
 
 
 class LazyString(object):
-    """ evaluate string lazily.
-    """
+    """evaluate string lazily."""
 
-    def __init__(self, raw_string, functions_mapping=None, check_variables_set=None, cached=False):
-        """ make raw_string as lazy object with functions_mapping
-            check if any variable undefined in check_variables_set
+    def __init__(
+        self, raw_string, functions_mapping=None, check_variables_set=None, cached=False
+    ):
+        """make raw_string as lazy object with functions_mapping
+        check if any variable undefined in check_variables_set
         """
         self.raw_string = raw_string
         self.functions_mapping = functions_mapping or {}
         self.check_variables_set = check_variables_set or set()
         self.cached = cached
         self.__parse(raw_string)
 
     def __parse(self, raw_string):
-        """ parse raw string, replace function and variable with {}
+        """parse raw string, replace function and variable with {}
 
         Args:
             raw_string(str): string with functions or varialbes
             e.g. "ABC${func2($a, $b)}DE$c"
 
         Returns:
             string: "ABC{}DE{}"
@@ -654,22 +652,18 @@
                 match_start_position = dollar_match.end()
                 self._string += "$"
                 continue
 
             # search function like ${func($a, $b)}
             func_match = function_regex_compile.match(raw_string, match_start_position)
             if func_match:
-                function_meta = {
-                    "func_name": func_match.group(1)
-                }
+                function_meta = {"func_name": func_match.group(1)}
                 function_meta.update(parse_function_params(func_match.group(2)))
                 lazy_func = LazyFunction(
-                    function_meta,
-                    self.functions_mapping,
-                    self.check_variables_set
+                    function_meta, self.functions_mapping, self.check_variables_set
                 )
                 self._args.append(lazy_func)
                 match_start_position = func_match.end()
                 self._string += "{}"
                 continue
 
             # search variable like ${var} or $var
@@ -697,23 +691,27 @@
 
             self._string += escape_braces(remain_string)
 
     def __repr__(self):
         return "LazyString({})".format(self.raw_string)
 
     def to_value(self, variables_mapping=None):
-        """ parse lazy data with evaluated variables mapping.
-            Notice: variables_mapping should not contain any variable or function.
+        """parse lazy data with evaluated variables mapping.
+        Notice: variables_mapping should not contain any variable or function.
         """
         variables_mapping = variables_mapping or {}
 
         args = []
         for arg in self._args:
             if isinstance(arg, LazyFunction):
-                if self.cached and arg.cache_key and arg.cache_key in cached_functions_mapping:
+                if (
+                    self.cached
+                    and arg.cache_key
+                    and arg.cache_key in cached_functions_mapping
+                ):
                     value = cached_functions_mapping[arg.cache_key]
                 else:
                     value = arg.to_value(variables_mapping)
                     cached_functions_mapping[arg.cache_key] = value
                 args.append(value)
             else:
                 # variable
@@ -722,50 +720,41 @@
 
         if self._string == "{}":
             return args[0]
         else:
             return self._string.format(*args)
 
 
-def prepare_lazy_data(content, functions_mapping=None, check_variables_set=None, cached=False):
-    """ make string in content as lazy object with functions_mapping
+def prepare_lazy_data(
+    content, functions_mapping=None, check_variables_set=None, cached=False
+):
+    """make string in content as lazy object with functions_mapping
 
     Raises:
         exceptions.VariableNotFound: if any variable undefined in check_variables_set
 
     """
     # TODO: refactor type check
     if content is None or isinstance(content, (numeric_types, bool, type)):
         return content
 
     elif isinstance(content, (list, set, tuple)):
         return [
-            prepare_lazy_data(
-                item,
-                functions_mapping,
-                check_variables_set,
-                cached
-            )
+            prepare_lazy_data(item, functions_mapping, check_variables_set, cached)
             for item in content
         ]
 
     elif isinstance(content, dict):
         parsed_content = {}
         for key, value in content.items():
             parsed_key = prepare_lazy_data(
-                key,
-                functions_mapping,
-                check_variables_set,
-                cached
+                key, functions_mapping, check_variables_set, cached
             )
             parsed_value = prepare_lazy_data(
-                value,
-                functions_mapping,
-                check_variables_set,
-                cached
+                value, functions_mapping, check_variables_set, cached
             )
             parsed_content[parsed_key] = parsed_value
 
         return parsed_content
 
     elif isinstance(content, basestring):
         # content is in string format here
@@ -779,62 +768,54 @@
         check_variables_set = check_variables_set or set()
         content = LazyString(content, functions_mapping, check_variables_set, cached)
 
     return content
 
 
 def parse_lazy_data(content, variables_mapping=None):
-    """ parse lazy data with evaluated variables mapping.
-        Notice: variables_mapping should not contain any variable or function.
+    """parse lazy data with evaluated variables mapping.
+    Notice: variables_mapping should not contain any variable or function.
     """
     # TODO: refactor type check
     if content is None or isinstance(content, (numeric_types, bool, type)):
         return content
 
     elif isinstance(content, LazyString):
         variables_mapping = utils.ensure_mapping_format(variables_mapping or {})
         return content.to_value(variables_mapping)
 
     elif isinstance(content, (list, set, tuple)):
-        return [
-            parse_lazy_data(item, variables_mapping)
-            for item in content
-        ]
+        return [parse_lazy_data(item, variables_mapping) for item in content]
 
     elif isinstance(content, dict):
         parsed_content = {}
         for key, value in content.items():
             parsed_key = parse_lazy_data(key, variables_mapping)
             parsed_value = parse_lazy_data(value, variables_mapping)
             parsed_content[parsed_key] = parsed_value
 
         return parsed_content
 
     return content
 
 
 def eval_lazy_data(content, variables_mapping=None, functions_mapping=None):
-    """ evaluate data instantly.
-        Notice: variables_mapping should not contain any variable or function.
+    """evaluate data instantly.
+    Notice: variables_mapping should not contain any variable or function.
     """
     variables_mapping = variables_mapping or {}
     check_variables_set = set(variables_mapping.keys())
     return parse_lazy_data(
-        prepare_lazy_data(
-            content,
-            functions_mapping,
-            check_variables_set
-        ),
-        variables_mapping
+        prepare_lazy_data(content, functions_mapping, check_variables_set),
+        variables_mapping,
     )
 
 
 def extract_variables(content):
-    """ extract all variables in content recursively.
-    """
+    """extract all variables in content recursively."""
     if isinstance(content, (list, set, tuple)):
         variables = set()
         for item in content:
             variables = variables | extract_variables(item)
         return variables
 
     elif isinstance(content, dict):
@@ -846,15 +827,15 @@
     elif isinstance(content, LazyString):
         return set(regex_findall_variables(content.raw_string))
 
     return set()
 
 
 def parse_variables_mapping(variables_mapping):
-    """ eval each prepared variable and function in variables_mapping.
+    """eval each prepared variable and function in variables_mapping.
 
     Args:
         variables_mapping (dict):
             {
                 "varA": LazyString(123$varB),
                 "varB": LazyString(456$varC),
                 "varC": LazyString(${sum_two($a, $b)}),
@@ -907,26 +888,31 @@
                 # variables_mapping = {"key": [LazyString($key), 2]}
                 raise exceptions.VariableNotFound(var_name)
 
             if variables:
                 # reference other variable, or function call with other variable
                 # e.g. {"varA": "123$varB", "varB": "456$varC"}
                 # e.g. {"varC": "${sum_two($a, $b)}"}
-                if any([_var_name not in parsed_variables_mapping for _var_name in variables]):
+                if any(
+                    [
+                        _var_name not in parsed_variables_mapping
+                        for _var_name in variables
+                    ]
+                ):
                     # reference variable not parsed
                     continue
 
             parsed_value = parse_lazy_data(value, parsed_variables_mapping)
             parsed_variables_mapping[var_name] = parsed_value
 
     return parsed_variables_mapping
 
 
 def _extend_with_api(test_dict, api_def_dict):
-    """ extend test with api definition, test will merge and override api definition.
+    """extend test with api definition, test will merge and override api definition.
 
     Args:
         test_dict (dict): test block, this will override api_def_dict
         api_def_dict (dict): api definition
 
     Examples:
         >>> api_def_dict = {
@@ -951,35 +937,29 @@
     """
     # override api name
     test_dict.setdefault("name", api_def_dict.pop("name", "api name undefined"))
 
     # override variables
     def_variables = api_def_dict.pop("variables", [])
     test_dict["variables"] = utils.extend_variables(
-        def_variables,
-        test_dict.get("variables", {})
+        def_variables, test_dict.get("variables", {})
     )
 
     # merge & override validators TODO: relocate
     def_raw_validators = api_def_dict.pop("validate", [])
     def_validators = [
-        uniform_validator(_validator)
-        for _validator in def_raw_validators
+        uniform_validator(_validator) for _validator in def_raw_validators
     ]
     ref_validators = test_dict.pop("validate", [])
-    test_dict["validate"] = extend_validators(
-        def_validators,
-        ref_validators
-    )
+    test_dict["validate"] = extend_validators(def_validators, ref_validators)
 
     # merge & override extractors
     def_extrators = api_def_dict.pop("extract", {})
     test_dict["extract"] = utils.extend_variables(
-        def_extrators,
-        test_dict.get("extract", {})
+        def_extrators, test_dict.get("extract", {})
     )
 
     # merge & override request
     test_dict["request"] = api_def_dict.pop("request", {})
 
     # base_url & verify: priority api_def_dict > test_dict
     if api_def_dict.get("base_url"):
@@ -1006,62 +986,65 @@
         test_dict["teardown_hooks"] = extended_teardown_hooks
 
     # TODO: extend with other api definition items, e.g. times
     test_dict.update(api_def_dict)
 
 
 def _extend_with_testcase(test_dict, testcase_def_dict):
-    """ extend test with testcase definition
+    """extend test with testcase definition
         test will merge and override testcase config definition.
 
     Args:
         test_dict (dict): test block
         testcase_def_dict (dict): testcase definition
 
     Returns:
         dict: extended test dict.
 
     """
     # override testcase config variables
     testcase_def_dict["config"].setdefault("variables", {})
     testcase_def_variables = utils.ensure_mapping_format(
-        testcase_def_dict["config"].get("variables", {}))
+        testcase_def_dict["config"].get("variables", {})
+    )
     testcase_def_variables.update(test_dict.pop("variables", {}))
     testcase_def_dict["config"]["variables"] = testcase_def_variables
 
     # override base_url, verify
     # priority: testcase config > testsuite tests
     test_base_url = test_dict.pop("base_url", "")
     if not testcase_def_dict["config"].get("base_url"):
         testcase_def_dict["config"]["base_url"] = test_base_url
 
     # override name
-    test_name = test_dict.pop("name", None) \
-                or testcase_def_dict["config"].pop("name", None) \
-                or "testcase name undefined"
+    test_name = (
+        test_dict.pop("name", None)
+        or testcase_def_dict["config"].pop("name", None)
+        or "testcase name undefined"
+    )
 
     # override testcase config name, output, etc.
     testcase_def_dict["config"].update(test_dict)
     testcase_def_dict["config"]["name"] = test_name
 
     test_dict.clear()
     test_dict.update(testcase_def_dict)
 
 
 def __prepare_config(config, project_mapping, session_variables_set=None):
-    """ parse testcase/testsuite config.
-    """
+    """parse testcase/testsuite config."""
     # get config variables
     raw_config_variables = config.pop("variables", {})
 
     override_variables = utils.deepcopy_dict(project_mapping.get("variables", {}))
     functions = project_mapping.get("functions", {})
 
     if isinstance(raw_config_variables, basestring) and function_regex_compile.match(
-            raw_config_variables):
+        raw_config_variables
+    ):
         # config variables are generated by calling function
         # e.g.
         # "config": {
         #     "name": "basic test with httpbin",
         #     "variables": "${gen_variables()}"
         # }
         raw_config_variables_mapping = parse_lazy_data(
@@ -1073,21 +1056,25 @@
     # override config variables with passed in variables
     raw_config_variables_mapping.update(override_variables)
 
     if raw_config_variables_mapping:
         config["variables"] = raw_config_variables_mapping
 
     check_variables_set = set(raw_config_variables_mapping.keys())
-    check_variables_set |= (session_variables_set or set())
-    prepared_config = prepare_lazy_data(config, functions, check_variables_set, cached=True)
+    check_variables_set |= session_variables_set or set()
+    prepared_config = prepare_lazy_data(
+        config, functions, check_variables_set, cached=True
+    )
     return prepared_config
 
 
-def __prepare_testcase_tests(tests, config, project_mapping, session_variables_set=None):
-    """ override tests with testcase config variables, base_url and verify.
+def __prepare_testcase_tests(
+    tests, config, project_mapping, session_variables_set=None
+):
+    """override tests with testcase config variables, base_url and verify.
         test maybe nested testcase.
 
         variables priority:
         testcase config > testcase test > testcase_def config > testcase_def test > api
 
         base_url priority:
         testcase test > testcase config > testsuite test > testsuite config > api
@@ -1103,37 +1090,37 @@
     """
     config_variables = config.get("variables", {})
     config_base_url = config.get("base_url", "")
     config_verify = config.get("verify", True)
     functions = project_mapping.get("functions", {})
 
     prepared_testcase_tests = []
-    session_variables_set = set(config_variables.keys()) | (session_variables_set or set())
+    session_variables_set = set(config_variables.keys()) | (
+        session_variables_set or set()
+    )
     for test_dict in tests:
 
         teststep_variables_set = {"request", "response"}
 
         # 1, testcase config => testcase tests
         # override test_dict variables
         test_dict_variables = utils.extend_variables(
-            test_dict.pop("variables", {}),
-            config_variables
+            test_dict.pop("variables", {}), config_variables
         )
         test_dict["variables"] = test_dict_variables
 
         # base_url & verify: priority test_dict > config
         if (not test_dict.get("base_url")) and config_base_url:
             test_dict["base_url"] = config_base_url
 
         # unify validators' format
         if "validate" in test_dict:
             ref_raw_validators = test_dict.pop("validate", [])
             test_dict["validate"] = [
-                uniform_validator(_validator)
-                for _validator in ref_raw_validators
+                uniform_validator(_validator) for _validator in ref_raw_validators
             ]
 
         if "testcase_def" in test_dict:
             # test_dict is nested testcase
 
             # pass former teststep's (as a testcase) export value to next teststep
             # Since V2.2.2, `extract` is used to replace `output`,
@@ -1148,15 +1135,17 @@
             testcase_def = test_dict.pop("testcase_def")
             _extend_with_testcase(test_dict, testcase_def)
 
             # verify priority: nested testcase config > testcase config
             test_dict["config"].setdefault("verify", config_verify)
 
             # 3, testcase_def config => testcase_def test_dict
-            test_dict = _parse_testcase(test_dict, project_mapping, session_variables_set)
+            test_dict = _parse_testcase(
+                test_dict, project_mapping, session_variables_set
+            )
             if not test_dict:
                 continue
 
         elif "api_def" in test_dict:
             # test_dict has API reference
             # 2, test_dict => api
             api_def_dict = test_dict.pop("api_def")
@@ -1165,14 +1154,15 @@
         # verify priority: testcase teststep > testcase config
         if "request" in test_dict:
             if "verify" not in test_dict["request"]:
                 test_dict["request"]["verify"] = config_verify
 
             if "upload" in test_dict["request"]:
                 from apimeter.ext.uploader import prepare_upload_test
+
                 prepare_upload_test(test_dict)
 
         # current teststep variables
         teststep_variables_set |= set(test_dict.get("variables", {}).keys())
 
         # move extracted variable to session variables
         if "extract" in test_dict:
@@ -1183,87 +1173,75 @@
 
         # convert validators to lazy function
         validators = test_dict.pop("validate", [])
         prepared_validators = []
         for _validator in validators:
             function_meta = {
                 "func_name": _validator["comparator"],
-                "args": [
-                    _validator["check"],
-                    _validator["expect"]
-                ],
-                "kwargs": {}
+                "args": [_validator["check"], _validator["expect"]],
+                "kwargs": {},
             }
             prepared_validators.append(
-                LazyFunction(
-                    function_meta,
-                    functions,
-                    teststep_variables_set
-                )
+                LazyFunction(function_meta, functions, teststep_variables_set)
             )
         test_dict["validate"] = prepared_validators
 
         # convert variables and functions to lazy object.
         # raises VariableNotFound if undefined variable exists in test_dict
         prepared_test_dict = prepare_lazy_data(
-            test_dict,
-            functions,
-            teststep_variables_set
+            test_dict, functions, teststep_variables_set
         )
         prepared_testcase_tests.append(prepared_test_dict)
 
     return prepared_testcase_tests
 
 
 def _parse_testcase(testcase, project_mapping, session_variables_set=None):
-    """ parse testcase
+    """parse testcase
 
     Args:
         testcase (dict):
             {
                 "config": {},
                 "teststeps": []
             }
 
     """
     testcase.setdefault("config", {})
 
     try:
         prepared_config = __prepare_config(
-            testcase["config"],
-            project_mapping,
-            session_variables_set
+            testcase["config"], project_mapping, session_variables_set
         )
         prepared_testcase_tests = __prepare_testcase_tests(
             testcase["teststeps"],
             prepared_config,
             project_mapping,
-            session_variables_set
+            session_variables_set,
         )
-        return {
-            "config": prepared_config,
-            "teststeps": prepared_testcase_tests
-        }
+        return {"config": prepared_config, "teststeps": prepared_testcase_tests}
     except (exceptions.MyBaseFailure, exceptions.MyBaseError) as ex:
         testcase_type = testcase["type"]
         testcase_path = testcase.get("path")
 
-        logger.log_error("failed to parse testcase: {}, error: {}".format(testcase_path, ex))
+        logger.log_error(
+            "failed to parse testcase: {}, error: {}".format(testcase_path, ex)
+        )
 
         global parse_failed_testfiles
         if testcase_type not in parse_failed_testfiles:
             parse_failed_testfiles[testcase_type] = []
 
         parse_failed_testfiles[testcase_type].append(testcase_path)
 
         return None
 
 
 def __get_parsed_testsuite_testcases(testcases, testsuite_config, project_mapping):
-    """ override testscases with testsuite config variables, base_url and verify.
+    """override testscases with testsuite config variables, base_url and verify.
 
         variables priority:
         parameters > testsuite config > testcase config > testcase_def config > testcase_def tests > api
 
         base_url priority:
         testcase_def tests > testcase_def config > testcase config > testsuite config
 
@@ -1319,53 +1297,54 @@
 
         # base_url priority: testcase config > testsuite config
         parsed_testcase["config"].setdefault("base_url", testsuite_base_url)
 
         # 1, testsuite config => testcase config
         # override test_dict variables
         testcase_config_variables = utils.extend_variables(
-            testcase.pop("variables", {}),
-            testsuite_config_variables
+            testcase.pop("variables", {}), testsuite_config_variables
         )
 
         # 2, testcase config > testcase_def config
         # override testcase_def config variables
         overrided_testcase_config_variables = utils.extend_variables(
-            parsed_testcase["config"].pop("variables", {}),
-            testcase_config_variables
+            parsed_testcase["config"].pop("variables", {}), testcase_config_variables
         )
 
         if overrided_testcase_config_variables:
             parsed_testcase["config"]["variables"] = overrided_testcase_config_variables
 
         # parse config variables
-        parsed_config_variables = parse_variables_mapping(overrided_testcase_config_variables)
+        parsed_config_variables = parse_variables_mapping(
+            overrided_testcase_config_variables
+        )
 
         # parse parameters
         if "parameters" in testcase and testcase["parameters"]:
             cartesian_product_parameters = parse_parameters(
-                testcase["parameters"],
-                parsed_config_variables,
-                functions
+                testcase["parameters"], parsed_config_variables, functions
             )
 
             for parameter_variables in cartesian_product_parameters:
                 # deepcopy to avoid influence between parameters
                 testcase_copied = utils.deepcopy_dict(parsed_testcase)
-                parsed_config_variables_copied = utils.deepcopy_dict(parsed_config_variables)
+                parsed_config_variables_copied = utils.deepcopy_dict(
+                    parsed_config_variables
+                )
                 testcase_copied["config"]["variables"] = utils.extend_variables(
-                    parsed_config_variables_copied,
-                    parameter_variables
+                    parsed_config_variables_copied, parameter_variables
+                )
+                parsed_testcase_copied = _parse_testcase(
+                    testcase_copied, project_mapping
                 )
-                parsed_testcase_copied = _parse_testcase(testcase_copied, project_mapping)
                 if not parsed_testcase_copied:
                     continue
                 parsed_testcase_copied["config"]["name"] = parse_lazy_data(
                     parsed_testcase_copied["config"]["name"],
-                    testcase_copied["config"]["variables"]
+                    testcase_copied["config"]["variables"],
                 )
                 parsed_testcase_list.append(parsed_testcase_copied)
 
         else:
             parsed_testcase = _parse_testcase(parsed_testcase, project_mapping)
             if not parsed_testcase:
                 continue
@@ -1374,23 +1353,21 @@
     return parsed_testcase_list
 
 
 def _parse_testsuite(testsuite, project_mapping):
     testsuite.setdefault("config", {})
     prepared_config = __prepare_config(testsuite["config"], project_mapping)
     parsed_testcase_list = __get_parsed_testsuite_testcases(
-        testsuite["testcases"],
-        prepared_config,
-        project_mapping
+        testsuite["testcases"], prepared_config, project_mapping
     )
     return parsed_testcase_list
 
 
 def parse_tests(tests_mapping):
-    """ parse tests and load to parsed testcases
+    """parse tests and load to parsed testcases
         tests include api, testcases and testsuites.
 
     Args:
         tests_mapping (dict): project info and testcases list.
 
             {
                 "project_mapping": {
@@ -1471,20 +1448,18 @@
                     continue
                 testcases.append(parsed_testcase)
 
         elif test_type == "apis":
             # encapsulate api as a testcase
             for api_content in tests_mapping["apis"]:
                 testcase = {
-                    "config": {
-                        "name": api_content.get("name")
-                    },
+                    "config": {"name": api_content.get("name")},
                     "teststeps": [api_content],
                     "path": api_content.pop("path", None),
-                    "type": api_content.pop("type", "api")
+                    "type": api_content.pop("type", "api"),
                 }
                 parsed_testcase = _parse_testcase(testcase, project_mapping)
                 if not parsed_testcase:
                     continue
                 testcases.append(parsed_testcase)
 
     return testcases
```

### Comparing `apimeter-2.5.7/apimeter/report/__init__.py` & `apimeter-2.5.9/apimeter/report/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,9 +12,9 @@
 
 __all__ = [
     "get_platform",
     "aggregate_stat",
     "get_summary",
     "stringify_summary",
     "HtmlTestResult",
-    "gen_html_report"
+    "gen_html_report",
 ]
```

### Comparing `apimeter-2.5.7/apimeter/report/html/gen_report.py` & `apimeter-2.5.9/apimeter/report/html/gen_report.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,64 +4,65 @@
 
 from jinja2 import Template
 
 from apimeter import logger
 from apimeter.exceptions import SummaryEmpty
 
 
-def gen_html_report(summary, report_template=None, report_dir=None, report_file=None):
-    """ render html report with specified report name and template
+def gen_html_report(summary, report_template=None, report_dir=None, report_file=None, skip_success=False):
+    """render html report with specified report name and template
 
     Args:
         summary (dict): test result summary data
         report_template (str): specify html report template path, template should be in Jinja2 format.
         report_dir (str): specify html report save directory
         report_file (str): specify html report file path, this has higher priority than specifying report dir.
 
     """
     if not summary["time"] or summary["stat"]["testcases"]["total"] == 0:
         logger.log_error("test result summary is empty ! {}".format(summary))
         raise SummaryEmpty
 
     if not report_template:
         report_template = os.path.join(
-            os.path.abspath(os.path.dirname(__file__)),
-            "template.html"
+            os.path.abspath(os.path.dirname(__file__)), "template.html"
         )
         logger.log_debug("No html report template specified, use default.")
     else:
         logger.log_info("render with html report template: {}".format(report_template))
 
     logger.log_info("Start to render Html report ...")
 
     start_at_timestamp = summary["time"]["start_at"]
     utc_time_iso_8601_str = datetime.utcfromtimestamp(start_at_timestamp).isoformat()
     summary["time"]["start_datetime"] = utc_time_iso_8601_str
 
-    for suite in summary["details"]:
-        suite['records'] = list(filter(lambda record: record['status'] != 'success', suite['records']))
+    # skip success testcases in report
+    if skip_success:
+        for suite in summary["details"]:
+            suite['records'] = list(filter(lambda record: record['status'] != 'success', suite['records']))
 
     if report_file:
         report_dir = os.path.dirname(report_file)
         report_file_name = os.path.basename(report_file)
     else:
         report_dir = report_dir or os.path.join(os.getcwd(), "reports")
         # fix #826: Windows does not support file name include ":"
-        report_file_name = "{}.html".format(utc_time_iso_8601_str.replace(":", "").replace("-", ""))
+        report_file_name = "{}.html".format(
+            utc_time_iso_8601_str.replace(":", "").replace("-", "")
+        )
 
     if not os.path.isdir(report_dir):
         os.makedirs(report_dir)
 
     report_path = os.path.join(report_dir, report_file_name)
-    with io.open(report_template, "r", encoding='utf-8') as fp_r:
+    with io.open(report_template, "r", encoding="utf-8") as fp_r:
         template_content = fp_r.read()
-        with io.open(report_path, 'w', encoding='utf-8') as fp_w:
+        with io.open(report_path, "w", encoding="utf-8") as fp_w:
             rendered_content = Template(
-                template_content,
-                extensions=["jinja2.ext.loopcontrols"]
+                template_content, extensions=["jinja2.ext.loopcontrols"]
             ).render(summary)
             fp_w.write(rendered_content)
 
     logger.log_info("Generated Html report: {}".format(report_path))
 
     return report_path
-
```

### Comparing `apimeter-2.5.7/apimeter/report/html/result.py` & `apimeter-2.5.9/apimeter/report/html/result.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 import time
 import unittest
 
 from apimeter import logger
 
 
 class HtmlTestResult(unittest.TextTestResult):
-    """ A html result class that can generate formatted html results.
-        Used by TextTestRunner.
+    """A html result class that can generate formatted html results.
+    Used by TextTestRunner.
     """
+
     def __init__(self, stream, descriptions, verbosity):
         super(HtmlTestResult, self).__init__(stream, descriptions, verbosity)
         self.records = []
 
-    def _record_test(self, test, status, attachment=''):
+    def _record_test(self, test, status, attachment=""):
         data = {
-            'name': test.shortDescription(),
-            'status': status,
-            'attachment': attachment,
-            "meta_datas": test.meta_datas
+            "name": test.shortDescription(),
+            "status": status,
+            "attachment": attachment,
+            "meta_datas": test.meta_datas,
         }
         self.records.append(data)
 
     def startTestRun(self):
         self.start_at = time.time()
 
     def startTest(self, test):
-        """ add start test time """
+        """add start test time"""
         super(HtmlTestResult, self).startTest(test)
         logger.color_print(test.shortDescription(), "yellow")
 
     def addSuccess(self, test):
         super(HtmlTestResult, self).addSuccess(test)
-        self._record_test(test, 'success')
+        self._record_test(test, "success")
         print("")
 
     def addError(self, test, err):
         super(HtmlTestResult, self).addError(test, err)
-        self._record_test(test, 'error', self._exc_info_to_string(err, test))
+        self._record_test(test, "error", self._exc_info_to_string(err, test))
         print("")
 
     def addFailure(self, test, err):
         super(HtmlTestResult, self).addFailure(test, err)
-        self._record_test(test, 'failure', self._exc_info_to_string(err, test))
+        self._record_test(test, "failure", self._exc_info_to_string(err, test))
         print("")
 
     def addSkip(self, test, reason):
         super(HtmlTestResult, self).addSkip(test, reason)
-        self._record_test(test, 'skipped', reason)
+        self._record_test(test, "skipped", reason)
         print("")
 
     def addExpectedFailure(self, test, err):
         super(HtmlTestResult, self).addExpectedFailure(test, err)
-        self._record_test(test, 'ExpectedFailure', self._exc_info_to_string(err, test))
+        self._record_test(test, "ExpectedFailure", self._exc_info_to_string(err, test))
         print("")
 
     def addUnexpectedSuccess(self, test):
         super(HtmlTestResult, self).addUnexpectedSuccess(test)
-        self._record_test(test, 'UnexpectedSuccess')
+        self._record_test(test, "UnexpectedSuccess")
         print("")
 
     @property
     def duration(self):
         return time.time() - self.start_at
```

### Comparing `apimeter-2.5.7/apimeter/report/html/template.html` & `apimeter-2.5.9/apimeter/report/html/template.html`

 * *Files identical despite different names*

### Comparing `apimeter-2.5.7/apimeter/report/report.py` & `apimeter-2.5.9/apimeter/report/report.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,47 +5,41 @@
 
 import requests
 
 from apimeter import __version__
 
 
 def prepare_event_kwargs(event_name, params):
-    """ prepare report event kwargs"""
+    """prepare report event kwargs"""
 
     kwargs = {
-        "headers": {
-            'content-type': 'application/json'
-        },
+        "headers": {"content-type": "application/json"},
         "json": {
-            "user": {
-                "user_unique_id": str(uuid.getnode())
-            },
+            "user": {"user_unique_id": str(uuid.getnode())},
             "header": {
                 "app_id": 173519,
                 "os_name": platform.system(),
                 "os_version": platform.release(),
-                "app_version": __version__  # HttpRunner version
+                "app_version": __version__,  # HttpRunner version
             },
             "events": [
                 {
                     "event": event_name,
                     "params": json.dumps(params),
-                    "time": int(time.time())
+                    "time": int(time.time()),
                 }
             ],
-            "verbose": 1
-        }
+            "verbose": 1,
+        },
     }
     return kwargs
 
 
 def report_event(event_name, success=True):
-    params = {
-        "success": 1 if success else 0
-    }
+    params = {"success": 1 if success else 0}
     kwargs = prepare_event_kwargs(event_name, params)
     resp = requests.post("http://mcs.snssdk.com/v1/json", **kwargs)
     print("resp---", resp.json())
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     report_event("loader")
```

### Comparing `apimeter-2.5.7/apimeter/report/stringify.py` & `apimeter-2.5.9/apimeter/report/stringify.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from jinja2 import escape
 from requests.cookies import RequestsCookieJar
 
 from apimeter.compat import basestring, bytes, json, numeric_types, JSONDecodeError
 
 
 def dumps_json(value):
-    """ dumps json value to indented string
+    """dumps json value to indented string
 
     Args:
         value (dict): raw json data
 
     Returns:
         str: indented json dump string
 
@@ -24,15 +24,15 @@
     try:
         return json.detect_encoding(value)
     except AttributeError:
         return "utf-8"
 
 
 def __stringify_request(request_data):
-    """ stringfy HTTP request data
+    """stringfy HTTP request data
 
     Args:
         request_data (dict): HTTP request data in dict.
 
             {
                 "url": "http://127.0.0.1:5000/api/get-token",
                 "method": "POST",
@@ -80,15 +80,15 @@
         elif isinstance(value, RequestsCookieJar):
             value = value.get_dict()
 
         request_data[key] = value
 
 
 def __stringify_response(response_data):
-    """ stringfy HTTP response data
+    """stringfy HTTP response data
 
     Args:
         response_data (dict):
 
             {
                 "status_code": 404,
                 "headers": {
@@ -120,16 +120,15 @@
                 encoding = response_data.get("encoding")
                 if not encoding or encoding == "None":
                     encoding = detect_encoding(value)
 
                 if key == "body" and "image" in response_data["content_type"]:
                     # display image
                     value = "data:{};base64,{}".format(
-                        response_data["content_type"],
-                        b64encode(value).decode(encoding)
+                        response_data["content_type"], b64encode(value).decode(encoding)
                     )
                 else:
                     value = escape(value.decode(encoding))
             except UnicodeDecodeError:
                 pass
 
         elif not isinstance(value, (basestring, numeric_types, Iterable)):
@@ -139,15 +138,15 @@
         elif isinstance(value, RequestsCookieJar):
             value = value.get_dict()
 
         response_data[key] = value
 
 
 def __expand_meta_datas(meta_datas, meta_datas_expanded):
-    """ expand meta_datas to one level
+    """expand meta_datas to one level
 
     Args:
         meta_datas (dict/list): maybe in nested format
 
     Returns:
         list: expanded list in one level
 
@@ -169,16 +168,15 @@
         meta_datas_expanded.append(meta_datas)
     elif isinstance(meta_datas, list):
         for meta_data in meta_datas:
             __expand_meta_datas(meta_data, meta_datas_expanded)
 
 
 def __get_total_response_time(meta_datas_expanded):
-    """ caculate total response time of all meta_datas
-    """
+    """caculate total response time of all meta_datas"""
     try:
         response_time = 0
         for meta_data in meta_datas_expanded:
             response_time += meta_data["stat"]["response_time_ms"]
 
         return "{:.2f}".format(response_time)
 
@@ -196,21 +194,20 @@
         data_list = meta_datas["data"]
         for data in data_list:
             __stringify_request(data["request"])
             __stringify_response(data["response"])
 
 
 def stringify_summary(summary):
-    """ stringify summary, in order to dump json file and generate html report.
-    """
+    """stringify summary, in order to dump json file and generate html report."""
     for index, suite_summary in enumerate(summary["details"]):
 
         if not suite_summary.get("name"):
             suite_summary["name"] = "testcase {}".format(index)
 
         for record in suite_summary.get("records"):
-            meta_datas = record['meta_datas']
+            meta_datas = record["meta_datas"]
             __stringify_meta_datas(meta_datas)
             meta_datas_expanded = []
             __expand_meta_datas(meta_datas, meta_datas_expanded)
             record["meta_datas_expanded"] = meta_datas_expanded
             record["response_time"] = __get_total_response_time(meta_datas_expanded)
```

### Comparing `apimeter-2.5.7/apimeter/report/summarize.py` & `apimeter-2.5.9/apimeter/report/summarize.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,47 +3,48 @@
 from apimeter import __version__
 
 
 def get_platform():
     return {
         "httprunner_version": __version__,
         "python_version": "{} {}".format(
-            platform.python_implementation(),
-            platform.python_version()
+            platform.python_implementation(), platform.python_version()
         ),
-        "platform": platform.platform()
+        "platform": platform.platform(),
     }
 
 
 def aggregate_stat(origin_stat, new_stat):
-    """ aggregate new_stat to origin_stat.
+    """aggregate new_stat to origin_stat.
 
     Args:
         origin_stat (dict): origin stat dict, will be updated with new_stat dict.
         new_stat (dict): new stat dict.
 
     """
     for key in new_stat:
         if key not in origin_stat:
             origin_stat[key] = new_stat[key]
         elif key == "start_at":
             # start datetime
             origin_stat["start_at"] = min(origin_stat["start_at"], new_stat["start_at"])
         elif key == "duration":
             # duration = max_end_time - min_start_time
-            max_end_time = max(origin_stat["start_at"] + origin_stat["duration"],
-                               new_stat["start_at"] + new_stat["duration"])
+            max_end_time = max(
+                origin_stat["start_at"] + origin_stat["duration"],
+                new_stat["start_at"] + new_stat["duration"],
+            )
             min_start_time = min(origin_stat["start_at"], new_stat["start_at"])
             origin_stat["duration"] = max_end_time - min_start_time
         else:
             origin_stat[key] += new_stat[key]
 
 
 def get_summary(result):
-    """ get summary from test result
+    """get summary from test result
 
     Args:
         result (instance): HtmlTestResult() instance
 
     Returns:
         dict: summary extracted from result.
 
@@ -54,29 +55,28 @@
                 "records": []
             }
 
     """
     summary = {
         "success": result.wasSuccessful(),
         "stat": {
-            'total': result.testsRun,
-            'failures': len(result.failures),
-            'errors': len(result.errors),
-            'skipped': len(result.skipped),
-            'expectedFailures': len(result.expectedFailures),
-            'unexpectedSuccesses': len(result.unexpectedSuccesses)
-        }
-    }
-    summary["stat"]["successes"] = summary["stat"]["total"] \
-                                   - summary["stat"]["failures"] \
-                                   - summary["stat"]["errors"] \
-                                   - summary["stat"]["skipped"] \
-                                   - summary["stat"]["expectedFailures"] \
-                                   - summary["stat"]["unexpectedSuccesses"]
-
-    summary["time"] = {
-        'start_at': result.start_at,
-        'duration': result.duration
+            "total": result.testsRun,
+            "failures": len(result.failures),
+            "errors": len(result.errors),
+            "skipped": len(result.skipped),
+            "expectedFailures": len(result.expectedFailures),
+            "unexpectedSuccesses": len(result.unexpectedSuccesses),
+        },
     }
+    summary["stat"]["successes"] = (
+        summary["stat"]["total"]
+        - summary["stat"]["failures"]
+        - summary["stat"]["errors"]
+        - summary["stat"]["skipped"]
+        - summary["stat"]["expectedFailures"]
+        - summary["stat"]["unexpectedSuccesses"]
+    )
+
+    summary["time"] = {"start_at": result.start_at, "duration": result.duration}
     summary["records"] = result.records
 
     return summary
```

### Comparing `apimeter-2.5.7/apimeter/response.py` & `apimeter-2.5.9/apimeter/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from apimeter import exceptions, logger, utils
 from apimeter.compat import basestring, is_py2
 
 text_extractor_regexp_compile = re.compile(r".*\(.*\).*")
 
 
 class ResponseObject(object):
-
     def __init__(self, resp_obj):
-        """ initialize with a requests.Response object
+        """initialize with a requests.Response object
 
         Args:
             resp_obj (instance): requests.Response instance
 
         """
         self.resp_obj = resp_obj
 
@@ -60,17 +59,17 @@
         :return:       A list that extracted from json repsonse example.    1) [200]   2) [1, 2]
         """
         result = jsonpath.jsonpath(self.parsed_body(), field)
         if result:
             return result
         else:
             raise exceptions.ExtractFailure("\tjsonpath {} get nothing\n".format(field))
-            
+
     def _extract_field_with_regex(self, field):
-        """ extract field from response content with regex.
+        """extract field from response content with regex.
             requests.Response body could be json or html text.
 
         Args:
             field (str): regex string that matched r".*\(.*\).*"
 
         Returns:
             str: matched content.
@@ -83,23 +82,23 @@
             >>> filed = "LB[\d]*(.*)RB[\d]*"
             >>> _extract_field_with_regex(field)
             abc
 
         """
         matched = re.search(field, self.text)
         if not matched:
-            err_msg = u"Failed to extract data with regex! => {}\n".format(field)
-            err_msg += u"response body: {}\n".format(self.text)
+            err_msg = "Failed to extract data with regex! => {}\n".format(field)
+            err_msg += "response body: {}\n".format(self.text)
             logger.log_error(err_msg)
             raise exceptions.ExtractFailure(err_msg)
 
         return matched.group(1)
 
     def _extract_field_with_delimiter(self, field):
-        """ response content could be json or html text.
+        """response content could be json or html text.
 
         Args:
             field (str): string joined by delimiter.
             e.g.
                 "status_code"
                 "headers"
                 "cookies"
@@ -107,24 +106,24 @@
                 "headers.content-type"
                 "content.person.name.first_name"
 
         """
         # string.split(sep=None, maxsplit=1) -> list of strings
         # e.g. "content.person.name" => ["content", "person.name"]
         try:
-            top_query, sub_query = field.split('.', 1)
+            top_query, sub_query = field.split(".", 1)
         except ValueError:
             top_query = field
             sub_query = None
 
         # status_code
         if top_query in ["status_code", "encoding", "ok", "reason", "url"]:
             if sub_query:
                 # status_code.XX
-                err_msg = u"Failed to extract: {}\n".format(field)
+                err_msg = "Failed to extract: {}\n".format(field)
                 logger.log_error(err_msg)
                 raise exceptions.ParamsError(err_msg)
 
             return getattr(self, top_query)
 
         # cookies
         elif top_query == "cookies":
@@ -132,49 +131,53 @@
             if not sub_query:
                 # extract cookies
                 return cookies
 
             try:
                 return cookies[sub_query]
             except KeyError:
-                err_msg = u"Failed to extract cookie! => {}\n".format(field)
-                err_msg += u"response cookies: {}\n".format(cookies)
+                err_msg = "Failed to extract cookie! => {}\n".format(field)
+                err_msg += "response cookies: {}\n".format(cookies)
                 logger.log_error(err_msg)
                 raise exceptions.ExtractFailure(err_msg)
 
         # elapsed
         elif top_query == "elapsed":
-            available_attributes = u"available attributes: days, seconds, microseconds, total_seconds"
+            available_attributes = (
+                "available attributes: days, seconds, microseconds, total_seconds"
+            )
             if not sub_query:
-                err_msg = u"elapsed is datetime.timedelta instance, attribute should also be specified!\n"
+                err_msg = "elapsed is datetime.timedelta instance, attribute should also be specified!\n"
                 err_msg += available_attributes
                 logger.log_error(err_msg)
                 raise exceptions.ParamsError(err_msg)
             elif sub_query in ["days", "seconds", "microseconds"]:
                 return getattr(self.elapsed, sub_query)
             elif sub_query == "total_seconds":
                 return self.elapsed.total_seconds()
             else:
-                err_msg = "{} is not valid datetime.timedelta attribute.\n".format(sub_query)
+                err_msg = "{} is not valid datetime.timedelta attribute.\n".format(
+                    sub_query
+                )
                 err_msg += available_attributes
                 logger.log_error(err_msg)
                 raise exceptions.ParamsError(err_msg)
 
         # headers
         elif top_query == "headers":
             headers = self.headers
             if not sub_query:
                 # extract headers
                 return headers
 
             try:
                 return headers[sub_query]
             except KeyError:
-                err_msg = u"Failed to extract header! => {}\n".format(field)
-                err_msg += u"response headers: {}\n".format(headers)
+                err_msg = "Failed to extract header! => {}\n".format(field)
+                err_msg += "response headers: {}\n".format(headers)
                 logger.log_error(err_msg)
                 raise exceptions.ExtractFailure(err_msg)
 
         # response body
         elif top_query in ["body", "content", "text", "json"]:
             try:
                 body = self.json
@@ -189,16 +192,20 @@
                 # content = {"xxx": 123}, content.xxx
                 return utils.query_json(body, sub_query)
             elif sub_query.isdigit():
                 # content = "abcdefg", content.3 => d
                 return utils.query_json(body, sub_query)
             else:
                 # content = "<html>abcdefg</html>", content.xxx
-                err_msg = u"Failed to extract attribute from response body! => {}\n".format(field)
-                err_msg += u"response body: {}\n".format(body)
+                err_msg = (
+                    "Failed to extract attribute from response body! => {}\n".format(
+                        field
+                    )
+                )
+                err_msg += "response body: {}\n".format(body)
                 logger.log_error(err_msg)
                 raise exceptions.ExtractFailure(err_msg)
 
         # new set response attributes in teardown_hooks
         elif top_query in self.__dict__:
             attributes = self.__dict__[top_query]
 
@@ -210,34 +217,37 @@
                 # attributes = {"xxx": 123}, content.xxx
                 return utils.query_json(attributes, sub_query)
             elif sub_query.isdigit():
                 # attributes = "abcdefg", attributes.3 => d
                 return utils.query_json(attributes, sub_query)
             else:
                 # content = "attributes.new_attribute_not_exist"
-                err_msg = u"Failed to extract cumstom set attribute from teardown hooks! => {}\n".format(field)
-                err_msg += u"response set attributes: {}\n".format(attributes)
+                err_msg = "Failed to extract cumstom set attribute from teardown hooks! => {}\n".format(
+                    field
+                )
+                err_msg += "response set attributes: {}\n".format(attributes)
                 logger.log_error(err_msg)
                 raise exceptions.TeardownHooksFailure(err_msg)
 
         # others
         else:
-            err_msg = u"Failed to extract attribute from response! => {}\n".format(field)
-            err_msg += u"available response attributes: status_code, cookies, elapsed, headers, content, " \
-                       u"text, json, encoding, ok, reason, url.\n\n"
-            err_msg += u"If you want to set attribute in teardown_hooks, take the following example as reference:\n"
-            err_msg += u"response.new_attribute = 'new_attribute_value'\n"
+            err_msg = "Failed to extract attribute from response! => {}\n".format(field)
+            err_msg += (
+                "available response attributes: status_code, cookies, elapsed, headers, content, "
+                "text, json, encoding, ok, reason, url.\n\n"
+            )
+            err_msg += "If you want to set attribute in teardown_hooks, take the following example as reference:\n"
+            err_msg += "response.new_attribute = 'new_attribute_value'\n"
             logger.log_error(err_msg)
             raise exceptions.ParamsError(err_msg)
 
     def extract_field(self, field):
-        """ extract value from requests.Response.
-        """
+        """extract value from requests.Response."""
         if not isinstance(field, basestring):
-            err_msg = u"Invalid extractor! => {}\n".format(field)
+            err_msg = "Invalid extractor! => {}\n".format(field)
             logger.log_error(err_msg)
             raise exceptions.ParamsError(err_msg)
 
         msg = "extract: {}".format(field)
 
         if field.startswith("$"):
             value = self._extract_field_with_jsonpath(field)
@@ -251,15 +261,15 @@
 
         msg += "\t=> {}".format(value)
         logger.log_debug(msg)
 
         return value
 
     def extract_response(self, extractors):
-        """ extract value from requests.Response and store in OrderedDict.
+        """extract value from requests.Response and store in OrderedDict.
 
         Args:
             extractors (list):
 
                 [
                     {"resp_status_code": "status_code"},
                     {"resp_headers_content_type": "headers.content-type"},
```

### Comparing `apimeter-2.5.7/apimeter/runner.py` & `apimeter-2.5.9/apimeter/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 class HookTypeEnum(Enum):
     SETUP = 1
     TEARDOWN = 2
 
 
 class Runner(object):
-    """ Running testcases.
+    """Running testcases.
 
     Examples:
         >>> tests_mapping = {
                 "project_mapping": {
                     "functions": {}
                 },
                 "testcases": [
@@ -48,15 +48,15 @@
 
         >>> test_runner = runner.Runner(parsed_testcase["config"])
         >>> test_runner.run_test(parsed_testcase["teststeps"][0])
 
     """
 
     def __init__(self, config, http_client_session=None):
-        """ run testcase or testsuite.
+        """run testcase or testsuite.
 
         Args:
             config (dict): testcase/testsuite config dict
 
                 {
                     "name": "ABC",
                     "variables": {},
@@ -83,23 +83,22 @@
             self.do_hook_actions(testcase_setup_hooks, HookTypeEnum.SETUP)
 
     def __del__(self):
         if self.testcase_teardown_hooks:
             self.do_hook_actions(self.testcase_teardown_hooks, HookTypeEnum.TEARDOWN)
 
     def __clear_test_data(self):
-        """ clear request and response data
-        """
+        """clear request and response data"""
         if not isinstance(self.http_client_session, HttpSession):
             return
 
         self.http_client_session.init_meta_data()
 
     def _handle_skip_feature(self, test_dict):
-        """ handle skip feature for test
+        """handle skip feature for test
             - skip: skip current test unconditionally
             - skipIf: skip current test if condition is true
             - skipUnless: skip current test unless condition is true
 
         Args:
             test_dict (dict): test info
 
@@ -123,15 +122,15 @@
             if not self.session_context.eval_content(skip_unless_condition):
                 skip_reason = "{} evaluate to False".format(skip_unless_condition)
 
         if skip_reason:
             raise SkipTest(skip_reason)
 
     def do_hook_actions(self, actions, hook_type):
-        """ call hook actions.
+        """call hook actions.
 
         Args:
             actions (list): each action in actions list maybe in two format.
 
                 format1 (dict): assignment, the value returned by hook function will be assigned to variable.
                     {"var": "${func()}"}
                 format2 (str): only call hook functions.
@@ -149,25 +148,23 @@
                 var_name, hook_content = list(action.items())[0]
                 hook_content_eval = self.session_context.eval_content(hook_content)
                 logger.log_debug(
                     "assignment with hook: {} = {} => {}".format(
                         var_name, hook_content, hook_content_eval
                     )
                 )
-                self.session_context.update_test_variables(
-                    var_name, hook_content_eval
-                )
+                self.session_context.update_test_variables(var_name, hook_content_eval)
             else:
                 # format 2
                 logger.log_debug("call hook function: {}".format(action))
                 # TODO: check hook function if valid
                 self.session_context.eval_content(action)
 
     def _run_test(self, test_dict):
-        """ run single teststep.
+        """run single teststep.
 
         Args:
             test_dict (dict): teststep info
                 {
                     "name": "teststep description",
                     "skip": "skip this test unconditionally",
                     "times": 3,
@@ -205,45 +202,43 @@
         test_variables = test_dict.get("variables", {})
         self.session_context.init_test_variables(test_variables)
 
         # teststep name
         test_name = self.session_context.eval_content(test_dict.get("name", ""))
 
         # parse test request
-        raw_request = test_dict.get('request', {})
+        raw_request = test_dict.get("request", {})
         parsed_test_request = self.session_context.eval_content(raw_request)
         self.session_context.update_test_variables("request", parsed_test_request)
 
         # setup hooks
         setup_hooks = test_dict.get("setup_hooks", [])
         if setup_hooks:
             self.do_hook_actions(setup_hooks, HookTypeEnum.SETUP)
 
         # prepend url with base_url unless it's already an absolute URL
-        url = parsed_test_request.pop('url')
+        url = parsed_test_request.pop("url")
         base_url = self.session_context.eval_content(test_dict.get("base_url", ""))
         parsed_url = utils.build_url(base_url, url)
 
         try:
-            method = parsed_test_request.pop('method')
+            method = parsed_test_request.pop("method")
             parsed_test_request.setdefault("verify", self.verify)
             group_name = parsed_test_request.pop("group", None)
         except KeyError:
             raise exceptions.ParamsError("URL or METHOD missed!")
 
         logger.log_info("{method} {url}".format(method=method, url=parsed_url))
         logger.log_debug(
-            "request kwargs(raw): {kwargs}".format(kwargs=parsed_test_request))
+            "request kwargs(raw): {kwargs}".format(kwargs=parsed_test_request)
+        )
 
         # request
         resp = self.http_client_session.request(
-            method,
-            parsed_url,
-            name=(group_name or test_name),
-            **parsed_test_request
+            method, parsed_url, name=(group_name or test_name), **parsed_test_request
         )
         resp_obj = response.ResponseObject(resp)
 
         def log_req_resp_details():
             err_msg = "{} DETAILED REQUEST & RESPONSE {}\n".format("*" * 32, "*" * 32)
 
             # log request
@@ -280,31 +275,27 @@
             log_req_resp_details()
             raise
 
         # validate
         validators = test_dict.get("validate") or test_dict.get("validators") or []
         validate_script = test_dict.get("validate_script", [])
         if validate_script:
-            validators.append({
-                "type": "python_script",
-                "script": validate_script
-            })
+            validators.append({"type": "python_script", "script": validate_script})
 
         validator = Validator(self.session_context, resp_obj)
         try:
             validator.validate(validators)
         except exceptions.ValidationFailure:
             log_req_resp_details()
             raise
         finally:
             self.validation_results = validator.validation_results
 
     def _run_testcase(self, testcase_dict):
-        """ run single testcase.
-        """
+        """run single testcase."""
         self.meta_datas = []
         config = testcase_dict.get("config", {})
 
         # each teststeps in one testcase (YAML/JSON) share the same session.
         test_runner = Runner(config, self.http_client_session)
 
         tests = testcase_dict.get("teststeps", [])
@@ -329,15 +320,15 @@
                 self.meta_datas.append(_meta_datas)
 
         self.session_context.update_session_variables(
             test_runner.export_variables(test_runner.export)
         )
 
     def run_test(self, test_dict):
-        """ run single teststep of testcase.
+        """run single teststep of testcase.
             test_dict may be in 3 types.
 
         Args:
             test_dict (dict):
 
                 # teststep
                 {
@@ -366,15 +357,16 @@
 
         """
         self.meta_datas = None
         if "teststeps" in test_dict:
             # nested testcase
             test_dict.setdefault("config", {}).setdefault("variables", {})
             test_dict["config"]["variables"].update(
-                self.session_context.session_variables_mapping)
+                self.session_context.session_variables_mapping
+            )
             self._run_testcase(test_dict)
         else:
             # api
             self.validation_results = {}
             try:
                 self._run_test(test_dict)
             except Exception:
@@ -384,16 +376,15 @@
                 raise
             finally:
                 # get request/response data and validate results
                 self.meta_datas = getattr(self.http_client_session, "meta_data", {})
                 self.meta_datas["validators"] = self.validation_results
 
     def export_variables(self, output_variables_list):
-        """ export current testcase variables
-        """
+        """export current testcase variables"""
         variables_mapping = self.session_context.session_variables_mapping
 
         output = {}
         for variable in output_variables_list:
             if variable not in variables_mapping:
                 logger.log_warning(
                     "variable '{}' can not be found in variables mapping, "
```

### Comparing `apimeter-2.5.7/apimeter/validator.py` & `apimeter-2.5.9/apimeter/validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,93 +12,97 @@
     Attributes:
         validation_results (dict): store validation results,
             including validate_extractor and validate_script.
 
     """
 
     def __init__(self, session_context, resp_obj):
-        """ initialize a Validator for each teststep (API request)
+        """initialize a Validator for each teststep (API request)
 
         Args:
             session_context: HttpRunner session context
             resp_obj: ResponseObject instance
         """
         self.session_context = session_context
         self.resp_obj = resp_obj
         self.validation_results = {}
 
     def __eval_validator_check(self, check_item):
-        """ evaluate check item in validator.
+        """evaluate check item in validator.
 
         Args:
             check_item: check_item should only be the following 5 formats:
                 1, variable reference, e.g. $token
                 2, function reference, e.g. ${is_status_code_200($status_code)}
                 3, dict or list, maybe containing variable/function reference, e.g. {"var": "$abc"}
                 4, string joined by delimiter. e.g. "status_code", "headers.content-type"
                 5, regex string, e.g. "LB[\d]*(.*)RB[\d]*"
 
         """
-        if isinstance(check_item, (dict, list)) \
-                or isinstance(check_item, parser.LazyString):
+        if isinstance(check_item, (dict, list)) or isinstance(
+            check_item, parser.LazyString
+        ):
             # format 1/2/3
             check_value = self.session_context.eval_content(check_item)
         else:
             # format 4/5
             check_value = self.resp_obj.extract_field(check_item)
 
         return check_value
 
     def __eval_validator_expect(self, expect_item):
-        """ evaluate expect item in validator.
+        """evaluate expect item in validator.
 
         Args:
             expect_item: expect_item should only be in 2 types:
                 1, variable reference, e.g. $expect_status_code
                 2, actual value, e.g. 200
 
         """
         expect_value = self.session_context.eval_content(expect_item)
         return expect_value
 
     def validate_script(self, script):
-        """ make validation with python script
-        """
+        """make validation with python script"""
         result = {
             "validate_script": "<br/>".join(script),
             "check_result": "pass",
-            "output": ""
+            "output": "",
         }
 
         script = "\n    ".join(script)
         code = """
 # encoding: utf-8
 
 def run_validate_script():
     {}
-""".format(script)
+""".format(
+            script
+        )
 
         variables = {
             "status_code": self.resp_obj.status_code,
             "response_json": self.resp_obj.json,
-            "response": self.resp_obj
+            "response": self.resp_obj,
         }
         variables.update(self.session_context.test_variables_mapping)
         variables.update(globals())
 
         try:
             exec(code, variables)
         except SyntaxError as ex:
             logger.log_warning("SyntaxError in python validate script: {}".format(ex))
             result["check_result"] = "fail"
-            result["output"] = "<br/>".join([
-                "ErrorMessage: {}".format(ex.msg),
-                "ErrorLine: {}".format(ex.lineno),
-                "ErrorText: {}".format(ex.text)
-            ])
+            result["output"] = "<br/>".join(
+                [
+                    "ErrorMessage: {}".format(ex.msg),
+                    "ErrorLine: {}".format(ex.lineno),
+                    "ErrorText: {}".format(ex.text),
+                ]
+            )
             return result
 
         try:
             # run python validate script
             variables["run_validate_script"]()
         except Exception as ex:
             logger.log_warning("run python validate script failed: {}".format(ex))
@@ -113,24 +117,25 @@
             elif len(traceback.extract_tb(_tb)) > 0:
                 # filename, lineno, name, line
                 _, _lineno, _, _ = traceback.extract_tb(_tb)[-1]
                 line_no = _lineno - 4
             else:
                 line_no = "N/A"
 
-            result["output"] = "<br/>".join([
-                "ErrorType: {}".format(_type.__name__),
-                "ErrorLine: {}".format(line_no)
-            ])
+            result["output"] = "<br/>".join(
+                [
+                    "ErrorType: {}".format(_type.__name__),
+                    "ErrorLine: {}".format(line_no),
+                ]
+            )
 
         return result
 
     def validate(self, validators):
-        """ make validation with comparators
-        """
+        """make validation with comparators"""
         self.validation_results = {}
         if not validators:
             return
 
         logger.log_debug("start to validate.")
 
         validate_pass = True
@@ -150,36 +155,34 @@
 
             if "validate_extractor" not in self.validation_results:
                 self.validation_results["validate_extractor"] = []
 
             # validator should be LazyFunction object
             if not isinstance(validator, parser.LazyFunction):
                 raise exceptions.ValidationFailure(
-                    "validator should be parsed first: {}".format(validators))
+                    "validator should be parsed first: {}".format(validators)
+                )
 
             # evaluate validator args with context variable mapping.
             validator_args = validator.get_args()
             check_item, expect_item = validator_args
             check_value = self.__eval_validator_check(check_item)
             expect_value = self.__eval_validator_expect(expect_item)
             validator.update_args([check_value, expect_value])
 
             comparator = validator.func_name
             validator_dict = {
                 "comparator": comparator,
                 "check": check_item,
                 "check_value": check_value,
                 "expect": expect_item,
-                "expect_value": expect_value
+                "expect_value": expect_value,
             }
             validate_msg = "\nvalidate: {} {} {}({})".format(
-                check_item,
-                comparator,
-                expect_value,
-                type(expect_value).__name__
+                check_item, comparator, expect_value, type(expect_value).__name__
             )
 
             try:
                 validator.to_value(self.session_context.test_variables_mapping)
                 validator_dict["check_result"] = "pass"
                 validate_msg += "\t==> pass"
                 logger.log_debug(validate_msg)
@@ -188,15 +191,15 @@
                 validator_dict["check_result"] = "fail"
                 validate_msg += "\t==> fail"
                 validate_msg += "\n{}({}) {} {}({})".format(
                     check_value,
                     type(check_value).__name__,
                     comparator,
                     expect_value,
-                    type(expect_value).__name__
+                    type(expect_value).__name__,
                 )
                 logger.log_error(validate_msg)
                 failures.append(validate_msg)
 
             self.validation_results["validate_extractor"].append(validator_dict)
 
             # restore validator args, in case of running multiple times
```

### Comparing `apimeter-2.5.7/docs/CHANGELOG.md` & `apimeter-2.5.9/docs/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 # Release History
 
+## 2.5.9 (2022-04-30)
+
+- fix #1217: reload debugtalk.py if loaded
+- fix #1246: catch exceptions caused by GA report failure
+- refactor: format code with black
+
+## 2.5.8 (2022-03-23)
+
+- change: replace events reporter from sentry to Google Analytics
+
 ## 2.5.7 (2020-02-21)
 
 **Changed**
 
 - feat: validate with python script, display print message
 
 **Fixed**
@@ -189,15 +199,15 @@
 - docs: update installation doc for developers
 
 ## 2.4.1 (2019-12-12)
 
 **Added**
 
 - feat: add `upload` keyword for upload test, see [doc](https://docs.httprunner.org/prepare/upload-case/)
-- test: pip install package 
+- test: pip install package
 - test: hrun command
 
 **Fixed**
 
 - fix: typo testfile_paths
 - fix: check if locustio installed
 - fix: dump json file name is empty when running relative testfile
```

### Comparing `apimeter-2.5.7/pyproject.toml` & `apimeter-2.5.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apimeter"
-version = "2.5.7"
+version = "2.5.9"
 description = "One-stop solution for HTTP(S) testing."
 license = "Apache-2.0"
 readme = "README.md"
 authors = ["debugtalk <debugtalk@gmail.com>"]
 
 homepage = "https://github.com/httprunner/httprunner"
 repository = "https://github.com/httprunner/httprunner"
@@ -23,15 +23,15 @@
     "Programming Language :: Python :: 2.7",
     "Programming Language :: Python :: 3.5",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11"
+    "Programming Language :: Python :: 3.11"    
 ]
 
 include = ["docs/CHANGELOG.md"]
 
 [tool.poetry.dependencies]
 python = "~2.7 || ^3.5"
 requests = "^2.22.0"
@@ -49,14 +49,18 @@
 jsonschema = "^3.2.0"
 
 [tool.poetry.dev-dependencies]
 flask = "<1.0.0"
 coverage = "^4.5.4"
 
 [tool.poetry.scripts]
-meter = "apimeter.cli:main"
 apimeter = "apimeter.cli:main"
+meter = "apimeter.cli:main"
+hrun = "apimeter.cli:main"
+httprunner = "apimeter.cli:main"
+ate = "apimeter.cli:main"
+locusts = "apimeter.ext.locusts.cli:main"
 apilocust = "apimeter.ext.locusts.cli:main"
 
 [build-system]
 requires = ["poetry>=1.0.0"]
 build-backend = "poetry.masonry.api"
```


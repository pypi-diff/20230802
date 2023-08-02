# Comparing `tmp/pytest-retry-1.2.1.tar.gz` & `tmp/pytest-retry-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-retry-1.2.1.tar", last modified: Tue Aug 16 23:42:22 2022, max compression
+gzip compressed data, was "pytest-retry-1.3.0.tar", last modified: Mon Jul 31 08:37:06 2023, max compression
```

## Comparing `pytest-retry-1.2.1.tar` & `pytest-retry-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2022-08-16 23:42:22.162151 pytest-retry-1.2.1/
--rw-r--r--   0 silasj     (501) staff       (20)      113 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/.gitignore
--rw-r--r--   0 silasj     (501) staff       (20)     1062 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/LICENSE
--rw-r--r--   0 silasj     (501) staff       (20)       94 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/MANIFEST.in
--rw-r--r--   0 silasj     (501) staff       (20)     7427 2022-08-16 23:42:22.162205 pytest-retry-1.2.1/PKG-INFO
--rw-r--r--   0 silasj     (501) staff       (20)     5514 2022-08-11 19:26:00.000000 pytest-retry-1.2.1/README.md
--rw-r--r--   0 silasj     (501) staff       (20)       68 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/dev-requirements.txt
--rw-r--r--   0 silasj     (501) staff       (20)     1116 2022-08-16 23:42:08.000000 pytest-retry-1.2.1/pyproject.toml
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2022-08-16 23:42:22.160228 pytest-retry-1.2.1/pytest_retry/
--rw-r--r--   0 silasj     (501) staff       (20)      125 2022-08-11 19:26:00.000000 pytest-retry-1.2.1/pytest_retry/__init__.py
--rw-r--r--   0 silasj     (501) staff       (20)        0 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/pytest_retry/py.typed
--rw-r--r--   0 silasj     (501) staff       (20)    11210 2022-08-16 23:42:08.000000 pytest-retry-1.2.1/pytest_retry/retry_plugin.py
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2022-08-16 23:42:22.161822 pytest-retry-1.2.1/pytest_retry.egg-info/
--rw-r--r--   0 silasj     (501) staff       (20)     7427 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/PKG-INFO
--rw-r--r--   0 silasj     (501) staff       (20)      467 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/SOURCES.txt
--rw-r--r--   0 silasj     (501) staff       (20)        1 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/dependency_links.txt
--rw-r--r--   0 silasj     (501) staff       (20)       52 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/entry_points.txt
--rw-r--r--   0 silasj     (501) staff       (20)        1 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/not-zip-safe
--rw-r--r--   0 silasj     (501) staff       (20)       45 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/requires.txt
--rw-r--r--   0 silasj     (501) staff       (20)       13 2022-08-16 23:42:22.000000 pytest-retry-1.2.1/pytest_retry.egg-info/top_level.txt
--rw-r--r--   0 silasj     (501) staff       (20)       13 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/requirements.txt
--rw-r--r--   0 silasj     (501) staff       (20)      301 2022-08-16 23:42:22.162417 pytest-retry-1.2.1/setup.cfg
-drwxr-xr-x   0 silasj     (501) staff       (20)        0 2022-08-16 23:42:22.161924 pytest-retry-1.2.1/tests/
--rw-r--r--   0 silasj     (501) staff       (20)    12448 2022-08-16 23:42:08.000000 pytest-retry-1.2.1/tests/test_retry_plugin.py
--rw-r--r--   0 silasj     (501) staff       (20)      498 2022-08-03 08:02:36.000000 pytest-retry-1.2.1/tox.ini
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2023-07-31 08:37:06.623048 pytest-retry-1.3.0/
+-rw-r--r--   0 silasj     (501) staff       (20)      113 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/.gitignore
+-rw-r--r--   0 silasj     (501) staff       (20)     1062 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/LICENSE
+-rw-r--r--   0 silasj     (501) staff       (20)       94 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/MANIFEST.in
+-rw-r--r--   0 silasj     (501) staff       (20)     9351 2023-07-31 08:37:06.623108 pytest-retry-1.3.0/PKG-INFO
+-rw-r--r--   0 silasj     (501) staff       (20)     7438 2023-07-31 08:07:21.000000 pytest-retry-1.3.0/README.md
+-rw-r--r--   0 silasj     (501) staff       (20)       68 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/dev-requirements.txt
+-rw-r--r--   0 silasj     (501) staff       (20)     1116 2023-07-31 08:17:43.000000 pytest-retry-1.3.0/pyproject.toml
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2023-07-31 08:37:06.622098 pytest-retry-1.3.0/pytest_retry/
+-rw-r--r--   0 silasj     (501) staff       (20)      125 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/pytest_retry/__init__.py
+-rw-r--r--   0 silasj     (501) staff       (20)     1187 2023-07-31 08:07:21.000000 pytest-retry-1.3.0/pytest_retry/hooks.py
+-rw-r--r--   0 silasj     (501) staff       (20)        0 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/pytest_retry/py.typed
+-rw-r--r--   0 silasj     (501) staff       (20)    13649 2023-07-31 08:07:21.000000 pytest-retry-1.3.0/pytest_retry/retry_plugin.py
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2023-07-31 08:37:06.622827 pytest-retry-1.3.0/pytest_retry.egg-info/
+-rw-r--r--   0 silasj     (501) staff       (20)     9351 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/PKG-INFO
+-rw-r--r--   0 silasj     (501) staff       (20)      489 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/SOURCES.txt
+-rw-r--r--   0 silasj     (501) staff       (20)        1 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/dependency_links.txt
+-rw-r--r--   0 silasj     (501) staff       (20)       52 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/entry_points.txt
+-rw-r--r--   0 silasj     (501) staff       (20)        1 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/not-zip-safe
+-rw-r--r--   0 silasj     (501) staff       (20)       45 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/requires.txt
+-rw-r--r--   0 silasj     (501) staff       (20)       13 2023-07-31 08:37:06.000000 pytest-retry-1.3.0/pytest_retry.egg-info/top_level.txt
+-rw-r--r--   0 silasj     (501) staff       (20)       40 2023-07-31 08:07:21.000000 pytest-retry-1.3.0/requirements.txt
+-rw-r--r--   0 silasj     (501) staff       (20)      301 2023-07-31 08:37:06.623367 pytest-retry-1.3.0/setup.cfg
+drwxr-xr-x   0 silasj     (501) staff       (20)        0 2023-07-31 08:37:06.622928 pytest-retry-1.3.0/tests/
+-rw-r--r--   0 silasj     (501) staff       (20)    16167 2023-07-31 08:07:21.000000 pytest-retry-1.3.0/tests/test_retry_plugin.py
+-rw-r--r--   0 silasj     (501) staff       (20)      498 2023-06-07 21:09:24.000000 pytest-retry-1.3.0/tox.ini
```

### Comparing `pytest-retry-1.2.1/LICENSE` & `pytest-retry-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-retry-1.2.1/PKG-INFO` & `pytest-retry-1.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,7 @@
-Metadata-Version: 2.1
-Name: pytest-retry
-Version: 1.2.1
-Summary: Adds the ability to retry flaky tests in CI environments
-Author: str0zzapreti
-License: MIT License
-        
-        Copyright (c) 2022 Silas
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/str0zzapreti/pytest-retry
-Keywords: rerun,pytest,flaky
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Framework :: Pytest
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 ![Tests](https://github.com/str0zzapreti/pytest-retry/actions/workflows/tests.yaml/badge.svg)
 # pytest-retry
 
 pytest-retry is a plugin for Pytest which adds the ability to retry flaky tests,
 thereby improving the consistency of the test suite results. 
 
 ## Requirements
@@ -76,14 +35,43 @@
 if the test failures are due to intermittent environment issues which clear up after
 a few seconds
 
 ```
 $ python -m pytest --retries 2 --retry-delay 5
 ```
 
+#### Advanced Options:
+There are two custom hooks provided for the purpose of setting global exception
+filters for your entire Pytest suite. `pytest_set_filtered_exceptions`
+and `pytest_set_excluded_exceptions`. You can define either of them in your 
+conftest.py file and return a list of exception types. Note: these hooks are 
+mutually exclusive and cannot both be defined at the same time.
+
+Example:
+```
+def pytest_set_excluded_exceptions():
+    """
+    All tests will be retried unless they fail due to an AssertionError or CustomError
+    """
+    return [AssertionError, CustomError]
+```
+
+There is a command line option to specify the test timing method, which can either
+be `overwrite` (default) or `cumulative`. With cumulative timing, the duration of 
+each test attempt is summed for the reported overall test duration. The default
+behavior simply reports the timing of the final attempt.
+
+```
+$ python -m pytest --retries 2 --cumulative-timing 1
+```
+
+If you're not sure which to use, stick with the default `overwrite` method. This
+generally plays nicer with time-based test splitting algorithms and will result in
+more even splits. 
+
 ### 2. Pytest flaky mark
 
 Mark individual tests as 'flaky' to retry them when they fail. If no command line
 arguments are passed, only the marked tests will be retried. The default values
 are 1 retry attempt with a 0-second delay
 
 ```
@@ -94,34 +82,52 @@
 
 The number of times each test will be retried and/or the delay can be manually
 specified as well
 
 ```
 @pytest.mark.flaky(retries=3, delay=1)
 def test_unreliable_service():
+    # This test will be retried up to 3 times (4 attempts total) with a
+    # one second delay between each attempt
     ...
 ```
 
-Finally, there is both a command line option and flaky mark argument for the test
-timing method, which can either be `overwrite` (default) or `cumulative`. With 
-cumulative timing, the duration of each test attempt is summed for the overall test
-duration reported at the end. The default behavior simply uses the timing for
-the final attempt. 
+If you want to control filtered or excluded exceptions per-test, the flaky mark
+provides the `only_on` and `exclude` arguments which both take a list of exception
+types, including any custom types you may have defined for your project. Note that 
+only one of these arguments may be used at a time.
+
+A test with a list of `only_on` exceptions will only be retried if it fails with
+one of the listed exceptions. A test with a list of `exclude` exceptions will
+only be retried if it fails with an exception which does not match any of the
+listed exceptions.
+
+If the exception for a subsequent attempt changes and no longer matches the filter,
+no further attempts will be made and the test will immediately fail.
 
 ```
-@pytest.mark.flaky(timing='overwrite')
+@pytest.mark.flaky(retries=2, only_on=[ValueError, IndexError])
 def test_unreliable_service():
+    # This test will only be retried if it fails due to raising a ValueError
+    # or an IndexError. e.g., an AssertionError will fail without retrying
     ...
 ```
 
-If you're not sure which to use, stick with the default `overwrite` method. This
-generally plays nicer with time-based test splitting algorithms and will result in
-more even splits. 
+Finally, there is a flaky mark argument for the test timing method, which can either
+be `overwrite` (default) or `cumulative`. See **Command Line** > **Advanced Options** 
+for more information
+
+```
+@pytest.mark.flaky(timing='overwrite')
+def test_unreliable_service():
+    ...
+```
 
-The flaky mark will override any command line options if passed when running Pytest.
+A flaky mark will override any command line options and exception filter hooks
+specified when running Pytest.
 
 ### Things to consider
 
 - **Currently, failing test fixtures are not retried.** In the future, flaky test setup 
 may be retried, although given the undesirability of flaky tests in general, flaky setup 
 should be avoided at all costs. Any failures during teardown will immediately halt
 further attempts so that they can be addressed immediately. Make sure your teardowns
```

### Comparing `pytest-retry-1.2.1/pyproject.toml` & `pytest-retry-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pytest-retry"
-version = "1.2.1"
+version = "1.3.0"
 description = "Adds the ability to retry flaky tests in CI environments"
 readme = "README.md"
 authors = [{ name = "str0zzapreti" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
```

### Comparing `pytest-retry-1.2.1/pytest_retry/retry_plugin.py` & `pytest-retry-1.3.0/pytest_retry/retry_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,53 @@
 import pytest
 import bdb
 from time import sleep
 from io import StringIO
 from traceback import format_exception
 from typing import Generator, Optional
+from collections.abc import Iterable
 from _pytest.terminal import TerminalReporter
 from _pytest.logging import caplog_records_key
 
 
 outcome_key = pytest.StashKey[str]()
 attempts_key = pytest.StashKey[int]()
 duration_key = pytest.StashKey[float]()
 stages = ("setup", "call", "teardown")
 
 
+class ConfigurationError(Exception):
+    pass
+
+
+class ExceptionFilter:
+    """
+    Helper class which returns a bool when called based on the filter type (expected or excluded)
+    and whether the exception exists within the list
+    """
+
+    def __init__(self, expected_exceptions: Iterable, excluded_exceptions: Iterable):
+        if expected_exceptions and excluded_exceptions:
+            raise ConfigurationError(
+                "filtered_exceptions and excluded_exceptions are exclusive and cannot "
+                "be defined simultaneously."
+            )
+        self.list_type = bool(expected_exceptions)
+        self.filter = expected_exceptions or excluded_exceptions or []
+
+    def __call__(self, exception_type: Optional[type[BaseException]]) -> bool:
+        try:
+            return not self.filter or bool(self.list_type == bool(exception_type in self.filter))
+        except TypeError:
+            raise ConfigurationError(
+                "Filtered or excluded exceptions must be passed as a collection. If using the "
+                "flaky mark, this means `only_on` or `exclude` args must be a collection too."
+            )
+
+
 class RetryHandler:
     """
     Stores statistics and reports for flaky tests and fixtures which have
     failed at least once during the test session and need to be retried
     """
 
     def __init__(self) -> None:
@@ -140,14 +170,19 @@
     # Set dynamic outcome for each stage until runtest protocol has completed.
     item.stash[outcome_key] = original_report.outcome
     if not should_handle_retry(original_report):
         return
     flake_mark = item.get_closest_marker("flaky")
     if flake_mark is None:
         return
+    exception_filter = ExceptionFilter(
+        flake_mark.kwargs.get("only_on", []), flake_mark.kwargs.get("excluded", [])
+    )
+    if not exception_filter(call.excinfo.type):  # type: ignore
+        return
     delay = flake_mark.kwargs.get("delay", 0)
     retries = flake_mark.kwargs.get("retries", 1)
     timing = flake_mark.kwargs.get("timing", "overwrite")
     if timing not in ("overwrite", "cumulative"):
         raise ValueError(f"Unknown timing type: {timing}! Must be `cumulative` or `overwrite`.")
     attempts = 1
     hook = item.ihook
@@ -196,15 +231,19 @@
         retry_manager.record_node_stats(retry_report)
         # Do the exception interaction step
         # (may not bother to support this since this is designed for automated runs, not debugging)
         if has_interactive_exception(call):
             hook.pytest_exception_interact(node=item, call=call, report=retry_report)
 
         attempts += 1
-        should_keep_retrying = not retry_report.passed and attempts <= retries
+        should_keep_retrying = (
+            not retry_report.passed
+            and attempts <= retries
+            and exception_filter(call.excinfo.type)  # type: ignore
+        )
 
         if not should_keep_retrying:
             original_report.outcome = retry_report.outcome
             original_report.longrepr = retry_report.longrepr
             if timing == "overwrite":
                 original_report.duration = retry_report.duration
             else:
@@ -229,17 +268,18 @@
         return "retried", "R", ("RETRY", {"yellow": True})
     return None
 
 
 def pytest_configure(config: pytest.Config) -> None:
     config.addinivalue_line(
         "markers",
-        "flaky(retries=1, delay=0): indicate a flaky test which"
-        "will be retried the number of times specified with an"
-        "(optional) specified delay between each attempt",
+        "flaky(retries=1, delay=0, only_on=..., exclude=...): indicate a flaky test which "
+        "will be retried the number of times specified with an (optional) specified "
+        "delay between each attempt. Collections of one or more exceptions can be passed so "
+        "that the test is retried only on those exceptions, or excluding those exceptions.",
     )
     if config.getoption("verbose"):
         # if pytest config has -v enabled, then don't limit traceback length
         retry_manager.trace_limit = None
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
@@ -268,16 +308,36 @@
         dest="cumulative_timing",
         type=bool,
         default=False,
         help="if True, retry duration will be included in overall reported test duration",
     )
 
 
+def pytest_addhooks(pluginmanager: pytest.PytestPluginManager) -> None:
+    """This example assumes the hooks are grouped in the 'sample_hook' module."""
+    from pytest_retry import hooks
+
+    pluginmanager.add_hookspecs(hooks)
+
+
 def pytest_collection_modifyitems(config: pytest.Config, items: list[pytest.Item]) -> None:
     if not config.getoption("--retries"):
         return
     retry_delay = config.getoption("--retry-delay") or 0
     timing = "cumulative" if config.getoption("--cumulative-timing") else "overwrite"
-    flaky = pytest.mark.flaky(retries=config.option.retries, delay=retry_delay, timing=timing)
+    filtered_exceptions: Iterable = config.hook.pytest_set_filtered_exceptions() or []
+    excluded_exceptions: Iterable = config.hook.pytest_set_excluded_exceptions() or []
+    if filtered_exceptions and excluded_exceptions:
+        raise ConfigurationError(
+            "filtered_exceptions and excluded_exceptions should not be defined"
+            "simultaneously. Use flaky marks to override the global config"
+        )
+    flaky = pytest.mark.flaky(
+        retries=config.option.retries,
+        delay=retry_delay,
+        timing=timing,
+        only_on=filtered_exceptions,
+        exclude=excluded_exceptions,
+    )
     for item in items:
         if "flaky" not in item.keywords:
             item.add_marker(flaky)
```

### Comparing `pytest-retry-1.2.1/pytest_retry.egg-info/PKG-INFO` & `pytest-retry-1.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-retry
-Version: 1.2.1
+Version: 1.3.0
 Summary: Adds the ability to retry flaky tests in CI environments
 Author: str0zzapreti
 License: MIT License
         
         Copyright (c) 2022 Silas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -76,14 +76,43 @@
 if the test failures are due to intermittent environment issues which clear up after
 a few seconds
 
 ```
 $ python -m pytest --retries 2 --retry-delay 5
 ```
 
+#### Advanced Options:
+There are two custom hooks provided for the purpose of setting global exception
+filters for your entire Pytest suite. `pytest_set_filtered_exceptions`
+and `pytest_set_excluded_exceptions`. You can define either of them in your 
+conftest.py file and return a list of exception types. Note: these hooks are 
+mutually exclusive and cannot both be defined at the same time.
+
+Example:
+```
+def pytest_set_excluded_exceptions():
+    """
+    All tests will be retried unless they fail due to an AssertionError or CustomError
+    """
+    return [AssertionError, CustomError]
+```
+
+There is a command line option to specify the test timing method, which can either
+be `overwrite` (default) or `cumulative`. With cumulative timing, the duration of 
+each test attempt is summed for the reported overall test duration. The default
+behavior simply reports the timing of the final attempt.
+
+```
+$ python -m pytest --retries 2 --cumulative-timing 1
+```
+
+If you're not sure which to use, stick with the default `overwrite` method. This
+generally plays nicer with time-based test splitting algorithms and will result in
+more even splits. 
+
 ### 2. Pytest flaky mark
 
 Mark individual tests as 'flaky' to retry them when they fail. If no command line
 arguments are passed, only the marked tests will be retried. The default values
 are 1 retry attempt with a 0-second delay
 
 ```
@@ -94,34 +123,52 @@
 
 The number of times each test will be retried and/or the delay can be manually
 specified as well
 
 ```
 @pytest.mark.flaky(retries=3, delay=1)
 def test_unreliable_service():
+    # This test will be retried up to 3 times (4 attempts total) with a
+    # one second delay between each attempt
     ...
 ```
 
-Finally, there is both a command line option and flaky mark argument for the test
-timing method, which can either be `overwrite` (default) or `cumulative`. With 
-cumulative timing, the duration of each test attempt is summed for the overall test
-duration reported at the end. The default behavior simply uses the timing for
-the final attempt. 
+If you want to control filtered or excluded exceptions per-test, the flaky mark
+provides the `only_on` and `exclude` arguments which both take a list of exception
+types, including any custom types you may have defined for your project. Note that 
+only one of these arguments may be used at a time.
+
+A test with a list of `only_on` exceptions will only be retried if it fails with
+one of the listed exceptions. A test with a list of `exclude` exceptions will
+only be retried if it fails with an exception which does not match any of the
+listed exceptions.
+
+If the exception for a subsequent attempt changes and no longer matches the filter,
+no further attempts will be made and the test will immediately fail.
 
 ```
-@pytest.mark.flaky(timing='overwrite')
+@pytest.mark.flaky(retries=2, only_on=[ValueError, IndexError])
 def test_unreliable_service():
+    # This test will only be retried if it fails due to raising a ValueError
+    # or an IndexError. e.g., an AssertionError will fail without retrying
     ...
 ```
 
-If you're not sure which to use, stick with the default `overwrite` method. This
-generally plays nicer with time-based test splitting algorithms and will result in
-more even splits. 
+Finally, there is a flaky mark argument for the test timing method, which can either
+be `overwrite` (default) or `cumulative`. See **Command Line** > **Advanced Options** 
+for more information
+
+```
+@pytest.mark.flaky(timing='overwrite')
+def test_unreliable_service():
+    ...
+```
 
-The flaky mark will override any command line options if passed when running Pytest.
+A flaky mark will override any command line options and exception filter hooks
+specified when running Pytest.
 
 ### Things to consider
 
 - **Currently, failing test fixtures are not retried.** In the future, flaky test setup 
 may be retried, although given the undesirability of flaky tests in general, flaky setup 
 should be avoided at all costs. Any failures during teardown will immediately halt
 further attempts so that they can be addressed immediately. Make sure your teardowns
```

### Comparing `pytest-retry-1.2.1/tests/test_retry_plugin.py` & `pytest-retry-1.3.0/tests/test_retry_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -235,17 +235,15 @@
     result = testdir.runpytest("--retries", "2", "--retry-delay", "2")
 
     assert_outcomes(result, passed=1, retried=1)
     assert result.duration > 4
 
 
 def test_passing_outcome_is_available_from_item_stash(testdir):
-    testdir.makepyfile(
-        "def test_success(): assert 1 == 1"
-    )
+    testdir.makepyfile("def test_success(): assert 1 == 1")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import outcome_key
 
         @pytest.fixture(autouse=True)
         def report_check(request):
@@ -255,17 +253,15 @@
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=1)
 
 
 def test_failed_outcome_is_available_from_item_stash(testdir):
-    testdir.makepyfile(
-        "def test_success(): assert 1 == 2"
-    )
+    testdir.makepyfile("def test_success(): assert 1 == 2")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import outcome_key
 
         @pytest.fixture(autouse=True)
         def report_check(request):
@@ -301,17 +297,15 @@
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=0, skipped=1)
 
 
 def test_duration_is_available_from_item_stash(testdir):
-    testdir.makepyfile(
-        """def test_success(): assert 1 == 1"""
-    )
+    testdir.makepyfile("""def test_success(): assert 1 == 1""")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import duration_key
 
         def pytest_sessionfinish(session: pytest.Session) -> None:
             for item in session.items:
@@ -320,17 +314,15 @@
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=1)
 
 
 def test_failed_outcome_after_successful_teardown(testdir):
-    testdir.makepyfile(
-        "def test_success(): assert 1 == 2"
-    )
+    testdir.makepyfile("def test_success(): assert 1 == 2")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import outcome_key
 
         @pytest.fixture(autouse=True)
         def successful_teardown(request):
@@ -344,17 +336,15 @@
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=0, failed=1)
 
 
 def test_failed_outcome_after_unsuccessful_setup(testdir):
-    testdir.makepyfile(
-        "def test_success(): assert 1 == 1"
-    )
+    testdir.makepyfile("def test_success(): assert 1 == 1")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import outcome_key
 
         @pytest.fixture(autouse=True)
         def failed_setup(request):
@@ -367,17 +357,15 @@
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=0, errors=1)
 
 
 def test_failed_outcome_after_unsuccessful_teardown(testdir):
-    testdir.makepyfile(
-        "def test_success(): assert 1 == 1"
-    )
+    testdir.makepyfile("def test_success(): assert 1 == 1")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import outcome_key
 
         @pytest.fixture(autouse=True)
         def failed_teardown(request):
@@ -391,17 +379,15 @@
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=1, errors=1)
 
 
 def test_attempts_are_always_available_from_item_stash(testdir):
-    testdir.makepyfile(
-        "def test_success(): assert 1 == 1"
-    )
+    testdir.makepyfile("def test_success(): assert 1 == 1")
     testdir.makeconftest(
         """
         import pytest
         from pytest_retry import attempts_key
 
         def pytest_sessionfinish(session: pytest.Session) -> None:
             for item in session.items:
@@ -409,14 +395,186 @@
         """
     )
     result = testdir.runpytest()
 
     assert_outcomes(result, passed=1)
 
 
+def test_global_filtered_exception_is_retried(testdir):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 1:
+                raise AssertionError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_filtered_exceptions():
+            return [AssertionError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "1")
+
+    assert_outcomes(result, passed=1, retried=1)
+
+
+def test_temporary_filtered_exception_fails_when_attempts_exceeded(testdir):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 4:
+                raise IndexError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_filtered_exceptions():
+            return [IndexError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "3")
+
+    assert_outcomes(result, passed=0, failed=1, retried=1)
+
+
+def test_temporary_exception_is_not_retried_if_filter_not_matched(testdir):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 1:
+                raise ValueError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_filtered_exceptions():
+            return [IndexError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "1")
+
+    assert_outcomes(result, passed=0, failed=1, retried=0)
+
+
+def test_temporary_exception_is_retried_if_not_globally_excluded(testdir):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 1:
+                raise ValueError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_excluded_exceptions():
+            return [AssertionError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "1")
+
+    assert_outcomes(result, passed=1, retried=1)
+
+
+def test_temporary_exception_fails_if_not_excluded_and_attempts_exceeded(testdir):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 4:
+                raise ValueError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_excluded_exceptions():
+            return [AssertionError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "3")
+
+    assert_outcomes(result, passed=0, failed=1, retried=1)
+
+
+def test_temporary_exception_is_not_retried_if_excluded(testdir):
+    testdir.makepyfile(
+        """
+        a = []
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 1:
+                raise ValueError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_excluded_exceptions():
+            return [ValueError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "1")
+
+    assert_outcomes(result, passed=1, retried=1)
+
+
+def test_flaky_mark_exception_filter_param_overrides_global_filter(testdir):
+    testdir.makepyfile(
+        """
+        import pytest
+
+        a = []
+
+        @pytest.mark.flaky(only_on=[IndexError])
+        def test_eventually_passes():
+            a.append(1)
+            if not len(a) > 1:
+                raise ValueError
+        """
+    )
+    testdir.makeconftest(
+        """
+        import pytest
+
+        def pytest_set_excluded_exceptions():
+            return [IndexError]
+
+        """
+    )
+    result = testdir.runpytest("--retries", "1")
+
+    assert_outcomes(result, passed=0, failed=1, retried=0)
+
+
 def test_attempt_count_is_correct(testdir):
     testdir.makepyfile(
         """
         import pytest
 
         a = []
```


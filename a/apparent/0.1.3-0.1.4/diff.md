# Comparing `tmp/apparent-0.1.3.tar.gz` & `tmp/apparent-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apparent-0.1.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "apparent-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `apparent-0.1.3.tar` & `apparent-0.1.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      835 2023-07-20 21:51:33.459428 apparent-0.1.3/.github/python-publish.yml
--rwxr-xr-x   0        0        0     6413 2023-07-20 20:59:05.115769 apparent-0.1.3/.gitignore
--rw-r--r--   0        0        0    11357 2023-07-06 21:22:31.764821 apparent-0.1.3/LICENSE.txt
--rwxr-xr-x   0        0        0     5105 2023-07-20 22:12:09.800394 apparent-0.1.3/README.md
--rw-r--r--   0        0        0     6148 2023-07-13 16:08:13.480811 apparent-0.1.3/apparent/.DS_Store
--rwxr-xr-x   0        0        0        0 2023-06-22 22:19:57.000000 apparent-0.1.3/apparent/__init__.py
--rw-r--r--   0        0        0     2295 2023-08-02 21:02:15.635509 apparent-0.1.3/apparent/reports.py
--rw-r--r--   0        0        0     9459 2023-08-02 20:45:54.245193 apparent-0.1.3/apparent/timing.py
--rwxr-xr-x   0        0        0      115 2023-08-01 16:11:59.291998 apparent-0.1.3/bin/build-docs
--rwxr-xr-x   0        0        0       99 2023-08-01 16:10:10.091991 apparent-0.1.3/bin/install-dev
--rwxr-xr-x   0        0        0      224 2023-07-20 16:37:18.635949 apparent-0.1.3/bin/test
--rwxr-xr-x   0        0        0      156 2023-07-20 16:35:45.141454 apparent-0.1.3/bin/test-coverage
--rw-r--r--   0        0        0     1575 2023-07-12 17:15:11.209433 apparent-0.1.3/doc/K.svg
--rw-r--r--   0        0        0     3930 2023-07-12 17:22:30.136488 apparent-0.1.3/doc/diffs.svg
--rw-r--r--   0        0        0     1203 2023-07-12 17:27:01.825682 apparent-0.1.3/doc/variance.md
--rw-r--r--   0        0        0     6200 2023-07-12 17:13:05.887758 apparent-0.1.3/doc/variance.svg
--rw-r--r--   0        0        0     9346 2023-07-12 17:15:49.766608 apparent-0.1.3/doc/variance_calc.svg
--rw-r--r--   0        0        0     6717 2023-08-02 20:45:54.245535 apparent-0.1.3/html/apparent/index.html
--rw-r--r--   0        0        0    12625 2023-08-02 20:45:54.246145 apparent-0.1.3/html/apparent/reports.html
--rw-r--r--   0        0        0    57545 2023-08-02 20:45:54.246681 apparent-0.1.3/html/apparent/timing.html
--rwxr-xr-x   0        0        0     1046 2023-08-02 21:09:10.812796 apparent-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-06 21:32:41.925459 apparent-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0      669 2023-08-02 20:45:54.246950 apparent-0.1.3/tests/common.py
--rw-r--r--   0        0        0     3418 2023-08-02 21:01:48.115843 apparent-0.1.3/tests/timer_reports_tests.py
--rw-r--r--   0        0        0     3751 2023-07-07 22:04:36.624455 apparent-0.1.3/tests/timer_results_tests.py
--rw-r--r--   0        0        0     5519 2023-08-02 20:45:54.247469 apparent-0.1.3/tests/timer_tests.py
--rw-r--r--   0        0        0     1613 2023-07-12 17:32:41.188742 apparent-0.1.3/tests/variance_tests.py
--rw-r--r--   0        0        0     5833 1970-01-01 00:00:00.000000 apparent-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      835 2023-07-20 21:51:33.459428 apparent-0.1.4/.github/python-publish.yml
+-rwxr-xr-x   0        0        0     6413 2023-07-20 20:59:05.115769 apparent-0.1.4/.gitignore
+-rw-r--r--   0        0        0    11357 2023-07-06 21:22:31.764821 apparent-0.1.4/LICENSE.txt
+-rwxr-xr-x   0        0        0     6914 2023-08-02 21:25:54.656385 apparent-0.1.4/README.md
+-rw-r--r--   0        0        0     6148 2023-07-13 16:08:13.480811 apparent-0.1.4/apparent/.DS_Store
+-rwxr-xr-x   0        0        0        0 2023-06-22 22:19:57.000000 apparent-0.1.4/apparent/__init__.py
+-rw-r--r--   0        0        0     2295 2023-08-02 21:02:15.635509 apparent-0.1.4/apparent/reports.py
+-rw-r--r--   0        0        0     9459 2023-08-02 20:45:54.245193 apparent-0.1.4/apparent/timing.py
+-rwxr-xr-x   0        0        0      115 2023-08-01 16:11:59.291998 apparent-0.1.4/bin/build-docs
+-rwxr-xr-x   0        0        0       99 2023-08-01 16:10:10.091991 apparent-0.1.4/bin/install-dev
+-rwxr-xr-x   0        0        0      224 2023-07-20 16:37:18.635949 apparent-0.1.4/bin/test
+-rwxr-xr-x   0        0        0      156 2023-07-20 16:35:45.141454 apparent-0.1.4/bin/test-coverage
+-rw-r--r--   0        0        0     1575 2023-07-12 17:15:11.209433 apparent-0.1.4/doc/K.svg
+-rw-r--r--   0        0        0     3930 2023-07-12 17:22:30.136488 apparent-0.1.4/doc/diffs.svg
+-rw-r--r--   0        0        0     1203 2023-07-12 17:27:01.825682 apparent-0.1.4/doc/variance.md
+-rw-r--r--   0        0        0     6200 2023-07-12 17:13:05.887758 apparent-0.1.4/doc/variance.svg
+-rw-r--r--   0        0        0     9346 2023-07-12 17:15:49.766608 apparent-0.1.4/doc/variance_calc.svg
+-rw-r--r--   0        0        0     6717 2023-08-02 20:45:54.245535 apparent-0.1.4/html/apparent/index.html
+-rw-r--r--   0        0        0    12625 2023-08-02 20:45:54.246145 apparent-0.1.4/html/apparent/reports.html
+-rw-r--r--   0        0        0    57545 2023-08-02 20:45:54.246681 apparent-0.1.4/html/apparent/timing.html
+-rwxr-xr-x   0        0        0     1046 2023-08-02 21:25:54.652654 apparent-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-06 21:32:41.925459 apparent-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0      669 2023-08-02 20:45:54.246950 apparent-0.1.4/tests/common.py
+-rw-r--r--   0        0        0     3418 2023-08-02 21:01:48.115843 apparent-0.1.4/tests/timer_reports_tests.py
+-rw-r--r--   0        0        0     3751 2023-07-07 22:04:36.624455 apparent-0.1.4/tests/timer_results_tests.py
+-rw-r--r--   0        0        0     5519 2023-08-02 20:45:54.247469 apparent-0.1.4/tests/timer_tests.py
+-rw-r--r--   0        0        0     1613 2023-07-12 17:32:41.188742 apparent-0.1.4/tests/variance_tests.py
+-rw-r--r--   0        0        0     7642 1970-01-01 00:00:00.000000 apparent-0.1.4/PKG-INFO
```

### Comparing `apparent-0.1.3/.github/python-publish.yml` & `apparent-0.1.4/.github/python-publish.yml`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/.gitignore` & `apparent-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/LICENSE.txt` & `apparent-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/apparent/.DS_Store` & `apparent-0.1.4/apparent/.DS_Store`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/apparent/reports.py` & `apparent-0.1.4/apparent/reports.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/apparent/timing.py` & `apparent-0.1.4/apparent/timing.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/doc/K.svg` & `apparent-0.1.4/doc/K.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/doc/diffs.svg` & `apparent-0.1.4/doc/diffs.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/doc/variance.md` & `apparent-0.1.4/doc/variance.md`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/doc/variance.svg` & `apparent-0.1.4/doc/variance.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/doc/variance_calc.svg` & `apparent-0.1.4/doc/variance_calc.svg`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/html/apparent/index.html` & `apparent-0.1.4/html/apparent/index.html`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/html/apparent/reports.html` & `apparent-0.1.4/html/apparent/reports.html`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/html/apparent/timing.html` & `apparent-0.1.4/html/apparent/timing.html`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/pyproject.toml` & `apparent-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apparent"
-version = "0.1.3"
+version = "0.1.4"
 description = "A toolkit for code observability in-process data collection: timing, counters, and metrics."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE.txt"}
 keywords = ["apparent", "observability", "monitoring", "timers", "timing", "counters", "metrics"]
 authors = [{name = "Arnon Moscona", email = "arnon@moscona.com"}]
 maintainers = [{name = "Arnon Moscona", email = "arnon@moscona.com"}]
```

### Comparing `apparent-0.1.3/tests/common.py` & `apparent-0.1.4/tests/common.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/tests/timer_reports_tests.py` & `apparent-0.1.4/tests/timer_reports_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/tests/timer_results_tests.py` & `apparent-0.1.4/tests/timer_results_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/tests/timer_tests.py` & `apparent-0.1.4/tests/timer_tests.py`

 * *Files identical despite different names*

### Comparing `apparent-0.1.3/tests/variance_tests.py` & `apparent-0.1.4/tests/variance_tests.py`

 * *Files identical despite different names*


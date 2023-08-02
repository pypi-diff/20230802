# Comparing `tmp/caf.toolkit-0.1.2.tar.gz` & `tmp/caf.toolkit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caf.toolkit-0.1.2.tar", last modified: Thu Jul 20 09:19:22 2023, max compression
+gzip compressed data, was "caf.toolkit-0.1.3.tar", last modified: Wed Aug  2 07:34:28 2023, max compression
```

## Comparing `caf.toolkit-0.1.2.tar` & `caf.toolkit-0.1.3.tar`

### file list

```diff
@@ -1,53 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.805584 caf.toolkit-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.805584 caf.toolkit-0.1.2/src/caf/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/array_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/concurrency/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/concurrency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/config_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/cost_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/io.py
--rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/iterative_proportional_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21770 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/df_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/numpy_conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/tqdm_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    29378 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/src/caf/toolkit/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.805584 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 09:19:22.000000 caf.toolkit-0.1.2/src/caf.toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:19:22.809584 caf.toolkit-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_array_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_cost_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_iterative_proportional_fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_math_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_toolbox.py
--rw-r--r--   0 runner    (1001) docker     (123)    41120 2023-07-20 09:19:11.000000 caf.toolkit-0.1.2/tests/test_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.559051 caf.toolkit-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.559051 caf.toolkit-0.1.3/src/caf/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/src/caf/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/src/caf/toolkit/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/array_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/src/caf/toolkit/concurrency/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/concurrency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18692 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/concurrency/multiprocessing_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/config_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/src/caf/toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35909 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/iterative_proportional_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21770 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/df_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13269 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/numpy_conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/tqdm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29378 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/src/caf/toolkit/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.559051 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-02 07:34:28.000000 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-08-02 07:34:28.000000 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:34:28.000000 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 07:34:28.000000 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-08-02 07:34:28.000000 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 07:34:28.000000 caf.toolkit-0.1.3/src/caf.toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:34:28.563051 caf.toolkit-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     9836 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_array_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_cost_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29413 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_iterative_proportional_fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12273 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_math_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_toolbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41120 2023-08-02 07:34:18.000000 caf.toolkit-0.1.3/tests/test_translation.py
```

### Comparing `caf.toolkit-0.1.2/LICENSE` & `caf.toolkit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/PKG-INFO` & `caf.toolkit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit of transport planning and appraisal functionalities
 Home-page: https://github.com/Transport-for-the-North/caf.toolkit
 Author: Transport for the North
 Maintainer: Ben Taylor
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.toolkit/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.toolkit
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.2 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.3 Summary: A toolkit of
 transport planning and appraisal functionalities Home-page: https://github.com/
 Transport-for-the-North/caf.toolkit Author: Transport for the North Maintainer:
 Ben Taylor License: GPL-3.0 Project-URL: Bug Tracker, https://github.com/
 Transport-for-the-North/caf.toolkit/issues Project-URL: Source, https://
 github.com/Transport-for-the-North/caf.toolkit Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `caf.toolkit-0.1.2/README.md` & `caf.toolkit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/pyproject.toml` & `caf.toolkit-0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -48,11 +48,15 @@
 convention = "numpy"
 match = '(?!_test)(?!test_)(?!__init__).*\.py'
 add-ignore = [
     "D202",    # Temporary compatibility with black
 ]
 
 [tool.pytest.ini_options]
-addopts = "--cov=caf.toolkit --cov-report=xml"
+addopts = '--cov=caf.toolkit --cov-report=xml --doctest-modules'
+doctest_optionflags = "NORMALIZE_WHITESPACE"
+markers = [
+    "serial: marks tests to not run in parallel",
+]
 
 [tool.coverage.run]
 omit = ["*/_version.py"]
```

### Comparing `caf.toolkit-0.1.2/setup.cfg` & `caf.toolkit-0.1.3/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 python_requires = >=3.9
 install_requires = 
 	numpy>=1.19.0
 	pandas>=1.4.0
 	tqdm>=4.50.2
 	sparse>=0.13.0
 	numba>=0.56.4
-	pydantic>=1.10
-	strictyaml>=1.6
+	pydantic==1.10.*
+	strictyaml==1.6.*
+	psutil>=5.9.0
 
 [options.extras_require]
 testing = 
 	pytest~=7.1.2
 	pytest-cov~=2.12.1
 	psutil>=5.9.0
 	mypy>=0.910
@@ -39,15 +40,15 @@
 	tox~=3.24.3
 
 [options.package_data]
 caf.toolkit = py.typed
 
 [versioneer]
 VCS = git
-style = pep440-post
+style = pep440
 versionfile_source = src/caf/toolkit/_version.py
 versionfile_build = caf/toolkit/_version.py
 tag_prefix = v
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/array_utils.py` & `caf.toolkit-0.1.3/src/caf/toolkit/array_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/concurrency/multiprocessing_wrapper.py` & `caf.toolkit-0.1.3/src/caf/toolkit/concurrency/multiprocessing_wrapper.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/config_base.py` & `caf.toolkit-0.1.3/src/caf/toolkit/config_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,36 +25,57 @@
     [pydantic docs](https://pydantic-docs.helpmanual.io/):
         for more information about using pydantic's model classes.
     `pydantic.BaseModel`: which handles converting data to Python types.
     `pydantic.validator`: which allows additional custom validation methods.
 
     Examples
     --------
+    Example of creating a config class and initialising it with
+    values, values will be validated and converted to correct
+    type on initialisation.
+
     >>> from pathlib import Path
     >>> from caf.toolkit import BaseConfig
     >>> class ExampleParameters(BaseConfig):
     ...    import_folder: Path
     ...    name: str
     ...    some_option: bool = True
     >>> parameters = ExampleParameters(
     ...    import_folder="Test Folder",
     ...    name="Test",
     ...    some_option=False,
     ... )
-    >>> parameters
-    ExampleParameters(import_folder=WindowsPath('Test Folder'), name='Test', some_option=False)
-    >>> parameters.to_yaml()
-    'import_folder: Test Folder\nname: Test\nsome_option: False\n'
+
+    Example of instance of class after initialisation, the path differs
+    depending on operating system.
+
+    >>> parameters # doctest: +SKIP
+    ExampleParameters(
+        import_folder=WindowsPath('Test Folder'),
+        name='Test',
+        some_option=False,
+    )
+
+    Config class can be converted to YAML or saved with `save_yaml`.
+
+    >>> print(parameters.to_yaml())
+    import_folder: Test Folder
+    name: Test
+    some_option: no
+
+    Config class data can be loaded from a YAML config file using `load_yaml`.
+
     >>> yaml_text = '''
-    ... import_folder: Test YAML Folder
-    ... name: YAML test
-    ... some_option: True
+    ... import_folder: Test Folder
+    ... name: Test
+    ... some_option: no
     ... '''
-    >>> ExampleParameters.from_yaml(yaml_text)
-    ExampleParameters(import_folder=WindowsPath('Test YAML Folder'), name='YAML test', some_option=True)
+    >>> loaded_parameters = ExampleParameters.from_yaml(yaml_text)
+    >>> loaded_parameters == parameters
+    True
     """
 
     @classmethod
     def from_yaml(cls, text: str):
         """Parse class attributes from YAML `text`.
 
         Parameters
```

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/cost_utils.py` & `caf.toolkit-0.1.3/src/caf/toolkit/cost_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/io.py` & `caf.toolkit-0.1.3/src/caf/toolkit/io.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/iterative_proportional_fitting.py` & `caf.toolkit-0.1.3/src/caf/toolkit/iterative_proportional_fitting.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/math_utils.py` & `caf.toolkit-0.1.3/src/caf/toolkit/math_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/df_handling.py` & `caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/df_handling.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/numpy_conversions.py` & `caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/numpy_conversions.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/pandas_utils/utility.py` & `caf.toolkit-0.1.3/src/caf/toolkit/pandas_utils/utility.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 """Basic utility functions for pandas objects."""
 # Built-Ins
-from typing import Any
 from typing import TypeVar
 from typing import Protocol
 
 # Third Party
 import numpy as np
 
 # Local Imports
@@ -18,15 +17,15 @@
 _T = TypeVar("_T")
 
 
 class CastProtocol(Protocol):
     # pylint: disable=too-few-public-methods
     """Type that as the `dtype` property and `astype` method."""
 
-    dtype: np.dtype[Any]
+    dtype: np.dtype
 
     def astype(self: _T, dtype: np.dtype) -> _T:
         """Cast this object to a new type."""
 
 
 _U = TypeVar("_U", bound=CastProtocol)
 _V = TypeVar("_V", bound=CastProtocol)
```

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/timing.py` & `caf.toolkit-0.1.3/src/caf/toolkit/timing.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/toolbox.py` & `caf.toolkit-0.1.3/src/caf/toolkit/toolbox.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/tqdm_utils.py` & `caf.toolkit-0.1.3/src/caf/toolkit/tqdm_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,20 +37,28 @@
 
     Examples
     --------
     To use with tqdm, call like this:
     >>> from tqdm import tqdm
     >>> from time import sleep
     >>>
+    >>> # Removing times from tqdm output for testing only
+    >>> bar_format = "{l_bar}{bar}| {n_fmt}/{total_fmt}"
+    >>>
     >>> # Redirect stdout to tqdm.write() (don't forget the `as save_stdout`)
     >>> with std_out_err_redirect_tqdm() as orig_stdout:
-    >>> # tqdm needs the original stdout
-    >>> # and dynamic_ncols=True to autodetect console width
-    >>> for i in tqdm(range(3), file=orig_stdout, dynamic_ncols=True):
-    >>>     sleep(.5)
+    ...     # tqdm needs the original stdout
+    ...     # and dynamic_ncols=True to autodetect console width
+    ...     for i in tqdm(range(3), file=orig_stdout, bar_format=bar_format):
+    ...         sleep(.5)
+      0%|          | 0/3
+     33%|###3      | 1/3
+     67%|######6   | 2/3
+    100%|##########| 3/3
+    100%|##########| 3/3
     """
     # Init
     orig_out_err = sys.stdout, sys.stderr
     try:
         sys.stdout, sys.stderr = map(tqdm_contrib.DummyTqdmFile, orig_out_err)
         yield orig_out_err[0]
```

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/translation.py` & `caf.toolkit-0.1.3/src/caf/toolkit/translation.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf/toolkit/validators.py` & `caf.toolkit-0.1.3/src/caf/toolkit/validators.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/src/caf.toolkit.egg-info/PKG-INFO` & `caf.toolkit-0.1.3/src/caf.toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caf.toolkit
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit of transport planning and appraisal functionalities
 Home-page: https://github.com/Transport-for-the-North/caf.toolkit
 Author: Transport for the North
 Maintainer: Ben Taylor
 License: GPL-3.0
 Project-URL: Bug Tracker, https://github.com/Transport-for-the-North/caf.toolkit/issues
 Project-URL: Source, https://github.com/Transport-for-the-North/caf.toolkit
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.2 Summary: A toolkit of
+Metadata-Version: 2.1 Name: caf.toolkit Version: 0.1.3 Summary: A toolkit of
 transport planning and appraisal functionalities Home-page: https://github.com/
 Transport-for-the-North/caf.toolkit Author: Transport for the North Maintainer:
 Ben Taylor License: GPL-3.0 Project-URL: Bug Tracker, https://github.com/
 Transport-for-the-North/caf.toolkit/issues Project-URL: Source, https://
 github.com/Transport-for-the-North/caf.toolkit Classifier: Programming Language
 :: Python :: 3 :: Only Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `caf.toolkit-0.1.2/src/caf.toolkit.egg-info/SOURCES.txt` & `caf.toolkit-0.1.3/src/caf.toolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 src/caf/toolkit/__init__.py
 src/caf/toolkit/_version.py
 src/caf/toolkit/array_utils.py
 src/caf/toolkit/config_base.py
 src/caf/toolkit/cost_utils.py
 src/caf/toolkit/io.py
 src/caf/toolkit/iterative_proportional_fitting.py
+src/caf/toolkit/log_helpers.py
 src/caf/toolkit/math_utils.py
 src/caf/toolkit/py.typed
 src/caf/toolkit/timing.py
 src/caf/toolkit/toolbox.py
 src/caf/toolkit/tqdm_utils.py
 src/caf/toolkit/translation.py
 src/caf/toolkit/validators.py
@@ -33,11 +34,12 @@
 src/caf/toolkit/pandas_utils/numpy_conversions.py
 src/caf/toolkit/pandas_utils/utility.py
 tests/test_array_utils.py
 tests/test_config_base.py
 tests/test_cost_utils.py
 tests/test_io.py
 tests/test_iterative_proportional_fitting.py
+tests/test_log_helpers.py
 tests/test_math_utils.py
 tests/test_timing.py
 tests/test_toolbox.py
 tests/test_translation.py
```

### Comparing `caf.toolkit-0.1.2/tests/test_array_utils.py` & `caf.toolkit-0.1.3/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_config_base.py` & `caf.toolkit-0.1.3/tests/test_config_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     return conf
 
 
 # # # CLASSES # # #
 
 
 @dataclasses.dataclass
-class TestSubClass:
+class SubClassTest:
     """
     Subclass to be included as a parameter in ConfigTestClass
     """
 
     whole: int
     decimal: float
 
@@ -86,15 +86,15 @@
     """
 
     dictionary: dict[str, float]
     path: Path
     list: list[str]
     set: set[int]
     tuple: tuple[Path, Path]
-    sub: TestSubClass = None
+    sub: SubClassTest = None
     default: bool = True
     option: int = None
 
 
 # pylint: enable=too-few-public-methods
 
 
@@ -206,17 +206,17 @@
         basic: test config
 
         Returns
         -------
         None
         """
         conf = basic
-        conf.sub = TestSubClass(whole=3, decimal=5.7)
+        conf.sub = SubClassTest(whole=3, decimal=5.7)
         yam = conf.to_yaml()
-        assert isinstance(ConfigTestClass.from_yaml(yam).sub, TestSubClass)
+        assert isinstance(ConfigTestClass.from_yaml(yam).sub, SubClassTest)
 
     def test_save_load(self, basic, path):
         """
         Test that when a config is saved to a yaml file then read in again it
         remains identical
         Parameters
         ----------
@@ -264,15 +264,15 @@
         """Write example with descriptions."""
         example_values = dict(
             dictionary="This is a dictionary",
             path="This is a path",
             list="This is a list",
             set="This is a set",
             tuple="Two paths to files",
-            sub=TestSubClass("integer value", "decimal value"),
+            sub=SubClassTest("integer value", "decimal value"),
             default="This value defaults to true",
             option="This value is optional",
         )
         example = self.write_example(path, **example_values)
 
         expected = (
             "dictionary: {dictionary}\n"
```

### Comparing `caf.toolkit-0.1.2/tests/test_cost_utils.py` & `caf.toolkit-0.1.3/tests/test_cost_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_io.py` & `caf.toolkit-0.1.3/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_iterative_proportional_fitting.py` & `caf.toolkit-0.1.3/tests/test_iterative_proportional_fitting.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_math_utils.py` & `caf.toolkit-0.1.3/tests/test_math_utils.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_timing.py` & `caf.toolkit-0.1.3/tests/test_timing.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_toolbox.py` & `caf.toolkit-0.1.3/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `caf.toolkit-0.1.2/tests/test_translation.py` & `caf.toolkit-0.1.3/tests/test_translation.py`

 * *Files identical despite different names*


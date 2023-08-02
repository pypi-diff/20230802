# Comparing `tmp/cvxsimulator-0.7.2.tar.gz` & `tmp/cvxsimulator-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.7.2.tar", max compression
+gzip compressed data, was "cvxsimulator-0.7.3.tar", max compression
```

## Comparing `cvxsimulator-0.7.2.tar` & `cvxsimulator-0.7.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    10790 2023-07-30 18:39:04.756541 cvxsimulator-0.7.2/LICENSE
--rw-r--r--   0        0        0     5739 2023-07-30 18:39:04.756541 cvxsimulator-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/__init__.py
--rw-r--r--   0        0        0    15915 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/builder.py
--rw-r--r--   0        0        0     1924 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/grid.py
--rw-r--r--   0        0        0     1570 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/month.py
--rw-r--r--   0        0        0    24512 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      965 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      114 2023-07-30 18:39:04.820541 cvxsimulator-0.7.2/cvx/simulator/types.py
--rw-r--r--   0        0        0     1114 2023-07-30 18:39:38.584475 cvxsimulator-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     6386 1970-01-01 00:00:00.000000 cvxsimulator-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10790 2023-08-02 03:14:08.277654 cvxsimulator-0.7.3/LICENSE
+-rw-r--r--   0        0        0     5776 2023-08-02 03:14:08.277654 cvxsimulator-0.7.3/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0    15915 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/builder.py
+-rw-r--r--   0        0        0     1924 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/grid.py
+-rw-r--r--   0        0        0     1570 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/month.py
+-rw-r--r--   0        0        0    24512 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      965 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      114 2023-08-02 03:14:08.349655 cvxsimulator-0.7.3/cvx/simulator/types.py
+-rw-r--r--   0        0        0     1115 2023-08-02 03:14:45.650364 cvxsimulator-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     6395 1970-01-01 00:00:00.000000 cvxsimulator-0.7.3/PKG-INFO
```

### Comparing `cvxsimulator-0.7.2/LICENSE` & `cvxsimulator-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.2/README.md` & `cvxsimulator-0.7.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
 ```python
 portfolio.plot(kind=Plot.DRAWDOWN)
 ```
 
 supporting all plots defined in quantstats.
 
-![quantstats snapshot](portfolio.png)
+![](https://raw.githubusercontent.com/cvxgrp/simulator/main/portfolio.png)
 
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org).
 Once you have installed poetry you can perform
 
 ```bash
```

### Comparing `cvxsimulator-0.7.2/cvx/simulator/builder.py` & `cvxsimulator-0.7.3/cvx/simulator/builder.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.2/cvx/simulator/grid.py` & `cvxsimulator-0.7.3/cvx/simulator/grid.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.2/cvx/simulator/month.py` & `cvxsimulator-0.7.3/cvx/simulator/month.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.2/cvx/simulator/portfolio.py` & `cvxsimulator-0.7.3/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.2/cvx/simulator/trading_costs.py` & `cvxsimulator-0.7.3/cvx/simulator/trading_costs.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.7.2/pyproject.toml` & `cvxsimulator-0.7.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.7.2"
+version = "v0.7.3"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "*"
 pandas = "*"
 quantstats = "*"
-pandas-stubs = "*"
+#pandas-stubs = "*"
 
 [tool.poetry.group.test.dependencies]
 pytest = "7.2.0"
 pytest-cov = "4.0.0"
 mock = "*"
 
 [tool.poetry.group.jupyter.dependencies]
```

### Comparing `cvxsimulator-0.7.2/PKG-INFO` & `cvxsimulator-0.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.7.2
+Version: 0.7.3
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: pandas-stubs
 Requires-Dist: quantstats
 Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](https://www.cvxgrp.org/simulator/)
 
 [![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
@@ -171,15 +170,15 @@
 
 ```python
 portfolio.plot(kind=Plot.DRAWDOWN)
 ```
 
 supporting all plots defined in quantstats.
 
-![quantstats snapshot](portfolio.png)
+![](https://raw.githubusercontent.com/cvxgrp/simulator/main/portfolio.png)
 
 ## Poetry
 
 We assume you share already the love for [Poetry](https://python-poetry.org).
 Once you have installed poetry you can perform
 
 ```bash
```


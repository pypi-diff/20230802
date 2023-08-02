# Comparing `tmp/cvxportfolio-0.4.4.tar.gz` & `tmp/cvxportfolio-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxportfolio-0.4.4.tar", last modified: Fri Jul  7 06:00:21 2023, max compression
+gzip compressed data, was "cvxportfolio-0.4.5.tar", last modified: Wed Aug  2 20:43:48 2023, max compression
```

## Comparing `cvxportfolio-0.4.4.tar` & `cvxportfolio-0.4.5.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.937893 cvxportfolio-0.4.4/
--rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.4.4/AUTHORS
--rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.4.4/LICENSE
--rw-r--r--   0 enzo       (501) staff       (20)     6461 2023-07-07 06:00:21.937534 cvxportfolio-0.4.4/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     6091 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/README.md
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.922005 cvxportfolio-0.4.4/cvxportfolio/
--rw-r--r--   0 enzo       (501) staff       (20)     1018 2023-07-07 05:54:53.000000 cvxportfolio-0.4.4/cvxportfolio/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     2638 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/benchmark.py
--rw-r--r--   0 enzo       (501) staff       (20)    11909 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)    19207 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    20371 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/data.py
--rw-r--r--   0 enzo       (501) staff       (20)     1001 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/errors.py
--rw-r--r--   0 enzo       (501) staff       (20)    15914 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/cvxportfolio/estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)     4167 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/hyperparameters.py
--rw-r--r--   0 enzo       (501) staff       (20)    22839 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     7060 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/result.py
--rw-r--r--   0 enzo       (501) staff       (20)     8648 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/returns.py
--rw-r--r--   0 enzo       (501) staff       (20)    14416 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    33774 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/cvxportfolio/simulator.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.936930 cvxportfolio-0.4.4/cvxportfolio/tests/
--rw-r--r--   0 enzo       (501) staff       (20)        0 2023-07-07 05:54:53.000000 cvxportfolio-0.4.4/cvxportfolio/tests/__init__.py
--rw-r--r--   0 enzo       (501) staff       (20)     1680 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/base.py
--rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.4.4/cvxportfolio/tests/returns.csv
--rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.4.4/cvxportfolio/tests/sigmas.csv
--rw-r--r--   0 enzo       (501) staff       (20)    10279 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_constraints.py
--rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_costs.py
--rw-r--r--   0 enzo       (501) staff       (20)    10139 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_data.py
--rw-r--r--   0 enzo       (501) staff       (20)     7171 2023-07-07 05:51:38.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_estimator.py
--rw-r--r--   0 enzo       (501) staff       (20)     8995 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_forecast.py
--rw-r--r--   0 enzo       (501) staff       (20)     3725 2023-07-05 16:17:23.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_hyperparameters.py
--rw-r--r--   0 enzo       (501) staff       (20)    22397 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_policies.py
--rw-r--r--   0 enzo       (501) staff       (20)     5996 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_returns.py
--rw-r--r--   0 enzo       (501) staff       (20)     9361 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_risks.py
--rw-r--r--   0 enzo       (501) staff       (20)    25890 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/tests/test_simulator.py
--rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.4.4/cvxportfolio/tests/volumes.csv
--rw-r--r--   0 enzo       (501) staff       (20)     1325 2023-07-04 14:26:42.000000 cvxportfolio-0.4.4/cvxportfolio/utils.py
-drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-07-07 06:00:21.924106 cvxportfolio-0.4.4/cvxportfolio.egg-info/
--rw-r--r--   0 enzo       (501) staff       (20)     6461 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/PKG-INFO
--rw-r--r--   0 enzo       (501) staff       (20)     1094 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/SOURCES.txt
--rw-r--r--   0 enzo       (501) staff       (20)        1 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/dependency_links.txt
--rw-r--r--   0 enzo       (501) staff       (20)       65 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/requires.txt
--rw-r--r--   0 enzo       (501) staff       (20)       13 2023-07-07 06:00:21.000000 cvxportfolio-0.4.4/cvxportfolio.egg-info/top_level.txt
--rw-r--r--   0 enzo       (501) staff       (20)       38 2023-07-07 06:00:21.938017 cvxportfolio-0.4.4/setup.cfg
--rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-07-07 05:54:53.000000 cvxportfolio-0.4.4/setup.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-08-02 20:43:48.619837 cvxportfolio-0.4.5/
+-rw-r--r--   0 enzo       (501) staff       (20)      199 2023-04-08 05:48:25.000000 cvxportfolio-0.4.5/AUTHORS
+-rw-r--r--   0 enzo       (501) staff       (20)      599 2023-04-08 05:48:25.000000 cvxportfolio-0.4.5/LICENSE
+-rw-r--r--   0 enzo       (501) staff       (20)     6652 2023-08-02 20:43:48.619523 cvxportfolio-0.4.5/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     6282 2023-07-12 18:02:21.000000 cvxportfolio-0.4.5/README.md
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-08-02 20:43:48.601180 cvxportfolio-0.4.5/cvxportfolio/
+-rw-r--r--   0 enzo       (501) staff       (20)     1018 2023-08-02 20:39:52.000000 cvxportfolio-0.4.5/cvxportfolio/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2626 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/benchmark.py
+-rw-r--r--   0 enzo       (501) staff       (20)    14391 2023-07-30 10:20:36.000000 cvxportfolio-0.4.5/cvxportfolio/constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)    19760 2023-07-14 15:56:33.000000 cvxportfolio-0.4.5/cvxportfolio/costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    20371 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1001 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/errors.py
+-rw-r--r--   0 enzo       (501) staff       (20)    17316 2023-08-02 20:39:06.000000 cvxportfolio-0.4.5/cvxportfolio/estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)     4041 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/hyperparameters.py
+-rw-r--r--   0 enzo       (501) staff       (20)    23165 2023-07-14 15:56:33.000000 cvxportfolio-0.4.5/cvxportfolio/policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7060 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/result.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8648 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    16673 2023-08-02 20:39:06.000000 cvxportfolio-0.4.5/cvxportfolio/risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    34440 2023-07-15 07:14:15.000000 cvxportfolio-0.4.5/cvxportfolio/simulator.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-08-02 20:43:48.617414 cvxportfolio-0.4.5/cvxportfolio/tests/
+-rw-r--r--   0 enzo       (501) staff       (20)        0 2023-08-02 20:39:52.000000 cvxportfolio-0.4.5/cvxportfolio/tests/__init__.py
+-rw-r--r--   0 enzo       (501) staff       (20)     1680 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/tests/base.py
+-rw-r--r--   0 enzo       (501) staff       (20)   156730 2023-05-11 16:35:10.000000 cvxportfolio-0.4.5/cvxportfolio/tests/returns.csv
+-rw-r--r--   0 enzo       (501) staff       (20)   149356 2023-05-11 16:35:10.000000 cvxportfolio-0.4.5/cvxportfolio/tests/sigmas.csv
+-rw-r--r--   0 enzo       (501) staff       (20)    10280 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_constraints.py
+-rw-r--r--   0 enzo       (501) staff       (20)     9078 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_costs.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10032 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_data.py
+-rw-r--r--   0 enzo       (501) staff       (20)     7748 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_estimator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     8995 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_forecast.py
+-rw-r--r--   0 enzo       (501) staff       (20)     3635 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_hyperparameters.py
+-rw-r--r--   0 enzo       (501) staff       (20)    22397 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_policies.py
+-rw-r--r--   0 enzo       (501) staff       (20)     5996 2023-07-04 14:26:42.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_returns.py
+-rw-r--r--   0 enzo       (501) staff       (20)    10488 2023-08-02 20:39:06.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_risks.py
+-rw-r--r--   0 enzo       (501) staff       (20)    26034 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_simulator.py
+-rw-r--r--   0 enzo       (501) staff       (20)     2063 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/tests/test_utils.py
+-rw-r--r--   0 enzo       (501) staff       (20)   116620 2023-05-11 16:35:10.000000 cvxportfolio-0.4.5/cvxportfolio/tests/volumes.csv
+-rw-r--r--   0 enzo       (501) staff       (20)     2328 2023-07-10 16:35:09.000000 cvxportfolio-0.4.5/cvxportfolio/utils.py
+drwxr-xr-x   0 enzo       (501) staff       (20)        0 2023-08-02 20:43:48.603067 cvxportfolio-0.4.5/cvxportfolio.egg-info/
+-rw-r--r--   0 enzo       (501) staff       (20)     6652 2023-08-02 20:43:48.000000 cvxportfolio-0.4.5/cvxportfolio.egg-info/PKG-INFO
+-rw-r--r--   0 enzo       (501) staff       (20)     1127 2023-08-02 20:43:48.000000 cvxportfolio-0.4.5/cvxportfolio.egg-info/SOURCES.txt
+-rw-r--r--   0 enzo       (501) staff       (20)        1 2023-08-02 20:43:48.000000 cvxportfolio-0.4.5/cvxportfolio.egg-info/dependency_links.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       65 2023-08-02 20:43:48.000000 cvxportfolio-0.4.5/cvxportfolio.egg-info/requires.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       13 2023-08-02 20:43:48.000000 cvxportfolio-0.4.5/cvxportfolio.egg-info/top_level.txt
+-rw-r--r--   0 enzo       (501) staff       (20)       38 2023-08-02 20:43:48.619919 cvxportfolio-0.4.5/setup.cfg
+-rw-r--r--   0 enzo       (501) staff       (20)     1032 2023-08-02 20:39:52.000000 cvxportfolio-0.4.5/setup.py
```

### Comparing `cvxportfolio-0.4.4/LICENSE` & `cvxportfolio-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/PKG-INFO` & `cvxportfolio-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.4.4
+Version: 0.4.5
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
@@ -20,24 +20,26 @@
 
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 (also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
 
-The documentation of the package is kindly hosted by [Read the Docs](https://readthedocs.org) at [www.cvxportfolio.com](https://www.cvxportfolio.com).
+The documentation of the package is kindly hosted by [Read the Docs](https://readthedocs.org) at [www.cvxportfolio.com](https://www.cvxportfolio.com). We also show some of our tutorials and examples on our
+[youtube channel](https://www.youtube.com/@Cvxportfolio).
 
 
 Installation
 ------------
 All our source code and releases are kindly hosted by the [Python Package Index](https://pypi.org). You can install the latest one with
 
 ```
 pip install -U cvxportfolio
 ```
+You can see how this works on our [Installation and Hello World](https://youtu.be/1ThOKEu371M) youtube video.
 
 Testing locally
 ------------
 We ship our unit test suite with the pip package. After installing you can test in you local environment by
 
 ```
 python -m unittest discover cvxportfolio
@@ -55,15 +57,14 @@
 matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
 and covariances as historical covariances (both ignoring `np.nan`'s). The logic used is detailed in the `forecast` module. Many optimizations
 are applied to make sure the system works well with real data. 
 
 
 ```python
 import cvxportfolio as cvx
-import matplotlib.pyplot as plt
 
 gamma = 3       # risk aversion parameter (Chapter 4.2)
 kappa = 0.05    # covariance forecast error risk parameter (Chapter 4.3)
 objective = cvx.ReturnsForecast() - gamma * (
 	cvx.FullCovariance() + kappa * cvx.RiskForecastError()
 ) - cvx.StocksTransactionCost()
 constraints = [cvx.LeverageLimit(3)]
```

### Comparing `cvxportfolio-0.4.4/README.md` & `cvxportfolio-0.4.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,24 +7,26 @@
 
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 (also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
 
-The documentation of the package is kindly hosted by [Read the Docs](https://readthedocs.org) at [www.cvxportfolio.com](https://www.cvxportfolio.com).
+The documentation of the package is kindly hosted by [Read the Docs](https://readthedocs.org) at [www.cvxportfolio.com](https://www.cvxportfolio.com). We also show some of our tutorials and examples on our
+[youtube channel](https://www.youtube.com/@Cvxportfolio).
 
 
 Installation
 ------------
 All our source code and releases are kindly hosted by the [Python Package Index](https://pypi.org). You can install the latest one with
 
 ```
 pip install -U cvxportfolio
 ```
+You can see how this works on our [Installation and Hello World](https://youtu.be/1ThOKEu371M) youtube video.
 
 Testing locally
 ------------
 We ship our unit test suite with the pip package. After installing you can test in you local environment by
 
 ```
 python -m unittest discover cvxportfolio
@@ -42,15 +44,14 @@
 matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
 and covariances as historical covariances (both ignoring `np.nan`'s). The logic used is detailed in the `forecast` module. Many optimizations
 are applied to make sure the system works well with real data. 
 
 
 ```python
 import cvxportfolio as cvx
-import matplotlib.pyplot as plt
 
 gamma = 3       # risk aversion parameter (Chapter 4.2)
 kappa = 0.05    # covariance forecast error risk parameter (Chapter 4.3)
 objective = cvx.ReturnsForecast() - gamma * (
 	cvx.FullCovariance() + kappa * cvx.RiskForecastError()
 ) - cvx.StocksTransactionCost()
 constraints = [cvx.LeverageLimit(3)]
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/__init__.py` & `cvxportfolio-0.4.5/cvxportfolio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """Cvxportfolio __init__ module.
 
 This module only republishes the api of a selection of cvxportfolio modules.
 The __all__ attribute of each is used.
 """
 
-__version__ = "0.4.4"
+__version__ = "0.4.5"
 
 from .simulator import *
 from .policies import *
 from .constraints import *
 from .costs import *
 from .returns import *
 from .risks import *
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/benchmark.py` & `cvxportfolio-0.4.5/cvxportfolio/benchmark.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,22 +26,22 @@
 class BaseBenchmark(PolicyEstimator):
     """Base class for cvxportfolio benchmark weights."""
     pass
 
 
 class Benchmark(BaseBenchmark, DataEstimator):
     """User-provided benchmark.
-    
+
     :param benchmark_weights: benchmark weights, either constant in
         time (pd.Series indexed by assets) or varying in time
         (pd.DataFrame indexed by time and whose columns are the assets).
     :type benchmark_weights: pd.Series or pd.DataFrame
-    
+
     """
-    
+
     def __init__(self, benchmark_weights):
         DataEstimator.__init__(self, benchmark_weights)
 
 
 class CashBenchmark(BaseBenchmark):
     """Default benchmark weights for cvxportfolio risk models.
     """
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/constraints.py` & `cvxportfolio-0.4.5/cvxportfolio/constraints.py`

 * *Files 13% similar despite different names*

```diff
@@ -136,25 +136,25 @@
 
 
 class LongOnly(BaseWeightConstraint):
     """A long only constraint.
 
     Imposes that at each point in time the post-trade
     weights are non-negative.
-    
+
     :param nocash: if True requires that the cash account is zero.
     :type nocash: bool
     """
-    
+
     def __init__(self, nocash=False):
         self.nocash = nocash
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         """Return a Cvxpy constraint."""
-        return [w_plus[:-1] >= 0] + ([w_plus[-1]==0] if self.nocash else [])
+        return [w_plus[:-1] >= 0] + ([w_plus[-1] == 0] if self.nocash else [])
 
 
 class NoTrade(BaseTradeConstraint):
     """No-trade condition on name on periods(s)."""
 
     def __init__(self, asset, periods):
         self.asset = asset
@@ -301,21 +301,31 @@
         """Return a Cvxpy constraint."""
         return w_plus[:-1] <= self.limit
 
 
 class FactorMaxLimit(BaseWeightConstraint):
     """A max limit on portfolio-wide factor (e.g. beta) exposure.
 
-    :param factor_exposure: DataFrame giving the factor exposure per asset
-        per factor, where the index are the assets and the columns are
-        the factors.
-    :type factor_exposure: pd.DataFrame
-    :param limit: Factor limits, either constant (pd.Series) or varying in time
-        pd.DataFrame.
-    :type limit: pd.Series or pd.DataFrame
+    :param factor_exposure: Series or DataFrame giving the factor exposure.
+        If Series it is indexed by assets' names and represents factor
+        exposures constant in time. If DataFrame it is indexed by time 
+        and has the assets names as columns, and it represents factor 
+        exposures that change in time. In the latter case an observation
+        must be present for every point in time of a backtest.
+        If you want you can also pass multiple factor exposures at once:
+        as a dataframe indexed by assets' names and whose columns are the
+        factors (if constant in time), or a dataframe with multiindex: 
+        first level is time, second level are assets' names (if changing 
+        in time). However this latter usecase is probably better served
+        by making multiple instances of this constraint, one for each 
+        factor.
+    :type factor_exposure: pd.Series or pd.DataFrame
+    :param limit: Factor limit, either constant or varying in time. Use
+        a DataFrame if you pass multiple factors as once.
+    :type limit: float or pd.Series or pd.DataFrame
     """
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(
             factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True)
 
@@ -324,21 +334,31 @@
         return (self.factor_exposure.parameter.T @ w_plus[:-1]
                 <= self.limit.parameter)
 
 
 class FactorMinLimit(BaseWeightConstraint):
     """A min limit on portfolio-wide factor (e.g. beta) exposure.
 
-    :param factor_exposure: DataFrame giving the factor exposure per asset
-        per factor, where the index are the assets and the columns are
-        the factors.
-    :type factor_exposure: pd.DataFrame
-    :param limit: Factor limits, either constant (pd.Series) or varying in time
-        pd.DataFrame.
-    :type limit: pd.Series or pd.DataFrame
+    :param factor_exposure: Series or DataFrame giving the factor exposure.
+        If Series it is indexed by assets' names and represents factor
+        exposures constant in time. If DataFrame it is indexed by time 
+        and has the assets names as columns, and it represents factor 
+        exposures that change in time. In the latter case an observation
+        must be present for every point in time of a backtest.
+        If you want you can also pass multiple factor exposures at once:
+        as a dataframe indexed by assets' names and whose columns are the
+        factors (if constant in time), or a dataframe with multiindex: 
+        first level is time, second level are assets' names (if changing 
+        in time). However this latter usecase is probably better served
+        by making multiple instances of this constraint, one for each 
+        factor.
+    :type factor_exposure: pd.Series or pd.DataFrame
+    :param limit: Factor limit, either constant or varying in time. Use
+        a DataFrame if you pass multiple factors as once.
+    :type limit: float or pd.Series or pd.DataFrame
     """
 
     def __init__(self, factor_exposure, limit):
         self.factor_exposure = DataEstimator(
             factor_exposure, compile_parameter=True)
         self.limit = DataEstimator(limit, compile_parameter=True)
 
@@ -350,18 +370,32 @@
 
 class FixedFactorLoading(BaseWeightConstraint):
     """A constraint to fix portfolio loadings to a set of factors.
 
     This can be used to impose market neutrality, 
     a certain portfolio-wide alpha, ....
 
-    Attributes:
-        factor_exposure: An (n * r) matrix giving the factor exposure on each
-        factor
-        target: A series or number giving the targeted factor loading
+    :param factor_exposure: Series or DataFrame giving the factor exposure.
+        If Series it is indexed by assets' names and represents factor
+        exposures constant in time. If DataFrame it is indexed by time 
+        and has the assets names as columns, and it represents factor 
+        exposures that change in time. In the latter case an observation
+        must be present for every point in time of a backtest.
+        If you want you can also pass multiple factor exposures at once:
+        as a dataframe indexed by assets' names and whose columns are the
+        factors (if constant in time), or a dataframe with multiindex: 
+        first level is time, second level are assets' names (if changing 
+        in time). However this latter usecase is probably better served
+        by making multiple instances of this constraint, one for each 
+        factor.
+    :type factor_exposure: pd.Series or pd.DataFrame
+    :param target: Target portfolio factor exposures, 
+        either constant or varying in time. Use
+        a DataFrame if you pass multiple factors as once.
+    :type target: float or pd.Series or pd.DataFrame
     """
 
     def __init__(self, factor_exposure, target):
         self.factor_exposure = DataEstimator(
             factor_exposure, compile_parameter=True)
         self.target = DataEstimator(target, compile_parameter=True)
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/costs.py` & `cvxportfolio-0.4.5/cvxportfolio/costs.py`

 * *Files 5% similar despite different names*

```diff
@@ -115,15 +115,16 @@
             return CombinedCosts(self.costs + other.costs,
                                  self.multipliers + other.multipliers)
         else:
             return CombinedCosts(self.costs + [other], self.multipliers + [1.0])
 
     def __mul__(self, other):
         """Multiply by constant."""
-        return CombinedCosts(self.costs, [el * other for el in self.multipliers])
+        return CombinedCosts(self.costs,
+                             [el * other for el in self.multipliers])
 
     def _recursive_pre_evaluation(self, *args, **kwargs):
         """Iterate over constituent costs."""
         [el._recursive_pre_evaluation(*args, **kwargs) for el in self.costs]
 
     def _recursive_values_in_time(self, **kwargs):
         """Iterate over constituent costs."""
@@ -132,19 +133,33 @@
     def _compile_to_cvxpy(self, w_plus, z, portfolio_value):
         """Iterate over constituent costs."""
         self.expression = 0
         for multiplier, cost in zip(self.multipliers, self.costs):
             self.expression += multiplier * \
                 cost._compile_to_cvxpy(w_plus, z, portfolio_value)
         return self.expression
-        
+
     def _collect_hyperparameters(self):
         return sum([el._collect_hyperparameters() for el in self.costs], []) + \
             sum([el._collect_hyperparameters() for el in self.multipliers if
-                hasattr(el, '_collect_hyperparameters')], []) 
+                hasattr(el, '_collect_hyperparameters')], [])
+
+    def __repr__(self):
+        """Pretty-print."""
+        result = ''
+        for i, (mult, cost) in enumerate(zip(self.multipliers, self.costs)):
+            if mult == 0:
+                continue
+            if mult < 0:
+                result += ' - ' if i > 0 else '-'
+            else:
+                result += ' + ' if i > 0 else ''
+            result += (str(abs(mult)) + ' * ' if abs(mult) != 1 else '')
+            result += cost.__repr__()
+        return result
 
 
 class HoldingCost(BaseCost):
     """This is a generic holding cost model.
 
     Currently it is not meant to be used directly. Look at
     :class:`StocksHoldingCost` for its version specialized to
@@ -293,15 +308,16 @@
     """This is a generic model for transaction cost of financial assets.
 
     Currently it is not meant to be used directly. Look at
     :class:`StocksTransactionCost` for its version specialized
     to the stock market.
     """
 
-    def __init__(self, a=None, pershare_cost=None, b=0., window_sigma_est=None, window_volume_est=None, exponent=None):
+    def __init__(self, a=None, pershare_cost=None, b=0., window_sigma_est=None,
+                 window_volume_est=None, exponent=None):
 
         self.a = None if a is None else DataEstimator(a)
         self.pershare_cost = None if pershare_cost is None else DataEstimator(
             pershare_cost)
         self.b = None if b is None else DataEstimator(b)
         self.window_sigma_est = window_sigma_est
         self.window_volume_est = window_volume_est
@@ -311,15 +327,16 @@
         if self.a is not None or self.pershare_cost is not None:
             self.first_term_multiplier = cp.Parameter(
                 len(universe)-1, nonneg=True)
         if self.b is not None:
             self.second_term_multiplier = cp.Parameter(
                 len(universe)-1, nonneg=True)
 
-    def _values_in_time(self, t,  current_portfolio_value, past_returns, past_volumes, current_prices, **kwargs):
+    def _values_in_time(self, t,  current_portfolio_value, past_returns,
+                        past_volumes, current_prices, **kwargs):
 
         tmp = 0.
 
         if self.a is not None:
             _ = self.a.current_value
             tmp += _ * \
                 np.ones(past_returns.shape[1]-1) if np.isscalar(_) else _
@@ -330,15 +347,16 @@
             tmp += self.pershare_cost.current_value / current_prices.values
 
         if self.a is not None or self.pershare_cost is not None:
             self.first_term_multiplier.value = tmp
 
         if self.b is not None:
 
-            if (self.window_sigma_est is None) or (self.window_volume_est is None):
+            if (self.window_sigma_est is None) or \
+                    (self.window_volume_est is None):
                 ppy = periods_per_year(past_returns.index)
             windowsigma = ppy if (
                 self.window_sigma_est is None) else self.window_sigma_est
             windowvolume = ppy if (
                 self.window_volume_est is None) else self.window_volume_est
 
             # TODO refactor this with forecast.py logic
@@ -346,15 +364,16 @@
                 (past_returns.iloc[-windowsigma:, :-1]**2).mean()).values
             volume_est = past_volumes.iloc[-windowvolume:].mean().values
 
             self.second_term_multiplier.value = self.b.current_value * sigma_est * \
                 (current_portfolio_value /
                  volume_est) ** ((2 if self.exponent is None else self.exponent) - 1)
 
-    def _simulate(self, t, u, current_and_past_returns, current_and_past_volumes, current_prices, **kwargs):
+    def _simulate(self, t, u, current_and_past_returns,
+                  current_and_past_volumes, current_prices, **kwargs):
 
         if self.window_sigma_est is None:
             windowsigma = periods_per_year(current_and_past_returns.index)
         else:
             windowsigma = self.window_sigma_est
 
         exponent = (1.5 if self.exponent is None else self.exponent)
@@ -375,16 +394,17 @@
                           * np.abs(u.iloc[:-1]))
 
         if self.b is not None:
             if current_and_past_volumes is None:
                 raise SyntaxError(
                     "If you don't provide volumes you should set b to None")
             # we add 1 to the volumes to prevent 0 volumes error (trades are cancelled on 0 volumes)
-            result += (np.abs(u.iloc[:-1])**exponent) @ (self.b._recursive_values_in_time(t) *
-                                                         sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (exponent - 1)))
+            result += (np.abs(u.iloc[:-1])**exponent) @ (
+                self.b._recursive_values_in_time(t) *
+                sigma / ((current_and_past_volumes.iloc[-1] + 1) ** (exponent - 1)))
 
         assert not np.isnan(result)
         assert not np.isinf(result)
 
         return -result
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/data.py` & `cvxportfolio-0.4.5/cvxportfolio/data.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/errors.py` & `cvxportfolio-0.4.5/cvxportfolio/errors.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/estimator.py` & `cvxportfolio-0.4.5/cvxportfolio/estimator.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 """
 This module implements Estimator base classes. Policies, costs, and constraints inherit
 from this.
 """
 
 import numpy as np
 import pandas as pd
+import cvxpy as cp
+
+
 from .errors import MissingValuesError, DataError
 from .hyperparameters import HyperParameter
-import cvxpy as cp
+from .utils import repr_numpy_pandas
 
 
 class Estimator:
     """Estimator base class.
 
     Policies, costs, and constraints inherit from this. When overloading
     methods defined here one should be careful on deciding whether to call
@@ -51,28 +54,50 @@
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "_recursive_values_in_time"):
                 subestimator._recursive_values_in_time(**kwargs)
         if hasattr(self, "_values_in_time"):
             self.current_value = self._values_in_time(**kwargs)
             return self.current_value
 
+    def __repr__(self):
+        """Pretty-print the cvxportfolio object in question.
+
+        We make sure that every object the user interacts with can be
+        pretty-printed to the interpreter, ideally in a way such that
+        copy-pasting the output to the prompt results in an identical object.
+        We can't do that all the times but we do our best. This is used 
+        throughout the library, for example it is included in backtest results 
+        so the user knows which policy generated that backtest, .... We prefer
+        to define the logic of this directly insted of relying, e.g., on
+        dataclasses logic, because we want to customize it to our usecase.
+        """
+        lhs = self.__class__.__name__ + '('
+        core = ''
+        for name, attr in self.__dict__.items():
+            if attr is None:
+                continue
+            if hasattr(attr, "_recursive_values_in_time") or \
+                    hasattr(attr, "_values_in_time") or (name[0] != '_'):
+                core += name + '=' + attr.__repr__() + ', '
+        core = core[:-2]  # remove trailing comma and space if present
+        rhs = ')'
+        return lhs + core + rhs
+
 
 class PolicyEstimator(Estimator):
     """Base class for (most) estimators that are part of policy objects."""
-    
-    
+
     def _collect_hyperparameters(self):
         """This method finds all hyperparameters defined as part of a policy.
         """
         result = []
         for _, subestimator in self.__dict__.items():
             if hasattr(subestimator, "_collect_hyperparameters"):
                 result += subestimator._collect_hyperparameters()
         return result
-            
 
     def _recursive_pre_evaluation(self, universe, backtest_times):
         """Recursively initialize estimator tree for backtest.
 
         :param universe: names of assets to be traded 
         :type universe: pandas.Index
         :param backtest_times: times at which the estimator will be evaluated
@@ -180,38 +205,38 @@
             if np.any(np.isnan(result)) and not self.allow_nans:
                 message = f"{self.__class__.__name__}._recursive_values_in_time result is an array with np.nan's."
                 if hasattr(self.data, 'columns') and len(self.data.columns) == len(result):
                     message += "Specifically, the problem is with symbol(s): " + str(
                         self.data.columns[np.isnan(result)])
                 raise MissingValuesError(message)
             else:
-                return result
+                # we pass a copy because it can be accidentally overwritten
+                return np.array(result)
 
         raise DataError(
             f"{self.__class__.__name__}._recursive_values_in_time result is not a scalar or array."
         )
 
     def internal__recursive_values_in_time(self, t, *args, **kwargs):
         """Internal method called by `self._recursive_values_in_time`."""
 
         if hasattr(self.data, "values_in_time"):
             _ = self.data.values_in_time(t=t, *args, **kwargs)
             if hasattr(_, 'values'):
                 return self.value_checker(_.values)
             else:
                 return self.value_checker(_)
-                                
 
         if (hasattr(self.data, "loc") and hasattr(self.data, "index")
             and (isinstance(self.data.index, pd.DatetimeIndex)
-                or (
+                 or (
                 isinstance(self.data.index, pd.MultiIndex)
                 and isinstance(self.data.index.levels[0], pd.DatetimeIndex)
-                )
             )
+        )
         ):
             try:
                 if self.use_last_available_time:
                     if isinstance(self.data.index, pd.MultiIndex):
                         newt = self.data.index.levels[0][
                             self.data.index.levels[0] <= t
                         ][-1]
@@ -245,19 +270,24 @@
             result (float, numpy.array): if you use a callable object make
                 sure that it returns a float or numpy array (and not,
                 for example, a pandas object)
 
         """
         self.current_value = self.internal__recursive_values_in_time(
             t, *args, **kwargs)
-        # we do this because in some cases they never get compiled
         if hasattr(self, 'parameter'):
             self.parameter.value = self.current_value
         return self.current_value
 
+    def __repr__(self):
+        if np.isscalar(self.data):
+            return str(self.data)
+        if hasattr(self.data, 'values_in_time'):
+            return self.data.__repr__()
+        return repr_numpy_pandas(self.data)
 
 # class ConstantEstimator(cvxpy.Constant, DataEstimator):
 #     """Cvxpy constant that uses the pre_evalution method to be initialized."""
 #
 #     def _recursive_pre_evaluation(self, returns, volumes, start_time, end_time, **kwargs):
 #         """You should call super().__init__ it here."""
 #         raise NotImplementedError
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/forecast.py` & `cvxportfolio-0.4.5/cvxportfolio/forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/hyperparameters.py` & `cvxportfolio-0.4.5/cvxportfolio/hyperparameters.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,90 +13,89 @@
 # limitations under the License.
 """This module defines hyperparameter objects.
 These are used currently as symbolic multipliers
 of cost terms in Single and Multi Period Optimization policies
 and can be iterated (and optimized over) automatically.
 """
 
+import numpy as np
+import copy
 GAMMA_RISK_RANGE = [.5, 1., 2., 5., 10.]
 GAMMA_COST_RANGE = [0., .1, .2, .5, 1., 2., 5., 10.]
 
-import copy
-
-import numpy as np
 
 __all__ = ['GammaRisk', 'GammaTrade', 'GammaHold']
 
 
 class HyperParameter:
     """Base Hyper Parameter class.
-    
+
     Implements arithmetic operations between hyper parameters.
-    
+
     You can sum and multiply HPs between themselves and with scalars,
     and divide by a scalar. Arbitrary algebraic combination of these
     operations are supported.
     """
-    
+
     def __mul__(self, other):
         if np.isscalar(other) or isinstance(other, HyperParameter):
             return CombinedHyperParameter([self], [other])
         return NotImplemented
-        
+
     def __rmul__(self, other):
         return self.__mul__(other)
-        
+
     def __div__(self, other):
         if np.isscalar(other):
             return CombinedHyperParameter([self], [1./other])
         return NotImplemented
-        
+
     def __truediv__(self, other):
         return self.__div__(other)
-        
+
     def __add__(self, other):
         if isinstance(other, HyperParameter):
             return CombinedHyperParameter([self, other], [1., 1.])
         return NotImplemented
-        
+
     def __radd__(self, other):
         return self.__add__(other)
-        
+
     def __sub__(self, other):
         return self + (-other)
-        
+
     def __neg__(self):
         return self * (-1)
-        
+
     def _collect_hyperparameters(self):
         return [self]
 
-      
+
 class CombinedHyperParameter(HyperParameter):
     """Algebraic combination of HyperParameters."""
-    
+
     def __init__(self, left, right):
         self.left = left
         self.right = right
-        
+
     @property
     def current_value(self):
         return sum([
             (le.current_value if hasattr(le, 'current_value') else le)
             * (ri.current_value if hasattr(ri, 'current_value') else ri)
-            for le,ri in zip(self.left, self.right)])
-            
+            for le, ri in zip(self.left, self.right)])
+
     def _collect_hyperparameters(self):
         """Collect (not combined) hyperparameters."""
         result = []
         for el in self.left + self.right:
             if hasattr(el, '_collect_hyperparameters'):
                 result += el._collect_hyperparameters()
         return result
-        
+
 
 class RangeHyperParameter(HyperParameter):
     """Range Hyper Parameter.
 
     This is not meant to be used directly, look at
     its subclasses for ones that you can use.
     """
@@ -107,23 +106,23 @@
         self.values_range = values_range
         self.current_value = initial_value
 
 
 class GammaRisk(RangeHyperParameter):
     """Multiplier of a risk term."""
 
-    def __init__(self, values_range = GAMMA_RISK_RANGE, initial_value = 1.):
+    def __init__(self, values_range=GAMMA_RISK_RANGE, initial_value=1.):
         super().__init__(values_range, initial_value)
 
 
 class GammaTrade(RangeHyperParameter):
     """Multiplier of a transaction cost term."""
 
-    def __init__(self, values_range = GAMMA_COST_RANGE, initial_value = 1.):
+    def __init__(self, values_range=GAMMA_COST_RANGE, initial_value=1.):
         super().__init__(values_range, initial_value)
 
 
 class GammaHold(RangeHyperParameter):
     """Multiplier of a holding cost term."""
 
-    def __init__(self, values_range = GAMMA_COST_RANGE, initial_value = 1.):
+    def __init__(self, values_range=GAMMA_COST_RANGE, initial_value=1.):
         super().__init__(values_range, initial_value)
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/policies.py` & `cvxportfolio-0.4.5/cvxportfolio/policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -467,15 +467,15 @@
             )
         if self.problem.status in ["infeasible", 'infeasible_inaccurate']:
             raise PortfolioOptimizationError(
                 f"Policy {self.__class__.__name__} at time {t} resulted in an infeasible problem."
             )
 
         return pd.Series(self.z_at_lags[0].value, current_weights.index)
-        
+
     def _collect_hyperparameters(self):
         result = []
         for el in self.objective:
             result += el._collect_hyperparameters()
         for el in self.constraints:
             for constr in el:
                 result += el._collect_hyperparameters()
@@ -505,7 +505,14 @@
     :param \**kwargs: these will be passed to cvxpy.Problem.solve, so you can choose your own solver and pass
         parameters to it.
     """
 
     def __init__(self, objective, constraints=[], include_cash_return=True, benchmark=CashBenchmark, **kwargs):
         super().__init__([objective], [constraints], include_cash_return=include_cash_return,
                          benchmark=benchmark, **kwargs)
+                         
+    # def __repr__(self):
+    #     return self.__class__.__name__ + '(' \
+    #         + 'objective=' + str(self.objective[0]) \
+    #         + ', constraints=' + str(self.constraints[0])
+    #         + ', benchmark=' + str(self.constraints[0])
+    #         + ', cvxpy_kwargs=' + str(self.cvxpy_kwargs)
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/result.py` & `cvxportfolio-0.4.5/cvxportfolio/result.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/returns.py` & `cvxportfolio-0.4.5/cvxportfolio/returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/risks.py` & `cvxportfolio-0.4.5/cvxportfolio/risks.py`

 * *Files 17% similar despite different names*

```diff
@@ -108,26 +108,26 @@
     # :type kelly: bool
     # """
 
     def __init__(self, Sigma=None, kelly=True):
 
         if not Sigma is None:
             self.Sigma = DataEstimator(Sigma)
-            self.alreadyfactorized = False
+            self._alreadyfactorized = False
         else:
             self.Sigma = HistoricalFactorizedCovariance(kelly=kelly)
-            self.alreadyfactorized = True
+            self._alreadyfactorized = True
 
     def _pre_evaluation(self, universe, backtest_times):
         self.Sigma_sqrt = cp.Parameter((len(universe)-1, len(universe)-1))
 
     def _values_in_time(self, t, past_returns, **kwargs):
         """Update forecast error risk here, and take square root of Sigma."""
 
-        if self.alreadyfactorized:
+        if self._alreadyfactorized:
             self.Sigma_sqrt.value = self.Sigma.current_value
         else:
             Sigma = self.Sigma.current_value
             eigval, eigvec = np.linalg.eigh(Sigma)
             eigval = np.maximum(eigval, 0.)
             self.Sigma_sqrt.value = eigvec @ np.diag(np.sqrt(eigval))
 
@@ -229,71 +229,93 @@
 
 
 class FactorModelCovariance(BaseRiskModel):
     """Factor model covariance, either user-provided or fitted from the data.
 
     It has the structure
 
-    :math:`F F^T + \mathbf{diag}(d)`
+    :math:`F \Sigma_{F} F^T + \mathbf{diag}(d)`
 
-    where :math:`F` is a *tall* matrix (many more rows than columns) and the vector
-    :math:`d` is all non-negative. 
-
-    :param F: exposure matrices either constant or varying in time; if so, use a pandas multiindexed
-         dataframe. If None it will be fitted.
+    where the factors exposure :math:`F` has as many rows as the number of assets and as many
+    columns as the number of factors,
+    the factors covariance matrix :math:`Sigma_{F}` is positive semi-definite,
+    and the idyosyncratic variances vector :math:`d` is non-negative. 
+    
+    The advantage of this risk model over the standard :class:`FullCovariance` is mostly
+    computational. When well-specified (as we do here) it costs much less to solve an 
+    optimization problem with this model than with a full covariance. It is a standard 
+    model that has been used for many decades in the portfolio optimization community
+    and multiple vendors exist for covariance matrices in this form. We also provide
+    the functionality to compute this automatically (which happens if you only specify
+    the number of factors to the constructor) with a standard PCA of the historical 
+    covariance at each point in time of the backtest (only looking at past returns).
+
+    :param F: factors exposure matrix either constant or varying in time. If constant
+        use a dataframe where the index are the factors and the columns are the asset names.
+        If varying in time use a pandas multiindexed dataframe where the first index level
+        is time and the second level are the factors. The columns
+        should always be the asset names. If None the constructor will default to fit the model from
+        past returns at each point of the backtest.
     :type F: pd.DataFrame or None
-    :param d: idyosyncratic variances either constant or varying in time; If None it will be fitted.
+    :param Sigma_F: factors covariance matrix either constant or varying in time. If varying in time
+        use a multiindexed dataframe where the first index level is time, and the second are the
+        factors (like the columns). If None it is assumed that :math:`Sigma_F` is the identity matrix: Leaving
+        this to None will not trigger automatic fit of the model. You can also have a factors
+        exposure matrix that is fixed in time and a factors covariance that instead changes in time,
+        or the opposite.
+    :type Sigma_F: pd.DataFrame or None
+    :param d: idyosyncratic variances either constant or varying in time. If constant use a pandas series,
+        if varying in time use a pandas dataframe where the index is time and the columns are the asset
+        names. You can have this varying in time and the exposures or the factors covariance fixed, or the
+        opposite. If you leave this to None you will trigger automatic fit of the model. If you wish
+        to have no idyosyncratic variances you can for example just pass 0.
     :type d: pd.Series or pd.DataFrame or None
-    :param num_factors: number of factors (columns of F), used if fitting the model
+    :param num_factors: number of factors (columns of F) that are obtained when fitting the model automatically
     :type num_factors: int    
+    :param kelly: when fitting the model you can perform a PCA on the covariance defined in the standard way
+        with this equal to False, or use the the quadratic term of the Taylor approximation of the Kelly
+        gambling objective with this equal to True. The difference is very small and it's better both
+        computationally and in terms of portfolio performance to leave this to True.
+    :type kelly: bool
     """
 
-    # Args:
-    #     exposures (pd.DataFrame): constant factor exposure matrix or a dataframe
-    #         where the first index is time.
-    #     idyosync (pd.DataFrame or pd.Series): idyosyncratic variances for the symbol,
-    #         either fixed (pd.Series) or through time (pd.DataFrame).
-    #     factor_Sigma (pd.DataFrame or None): a constant factor covariance matrix
-    #         or a DataFrame with multiindex where the first index is time. If None,
-    #         the default, it is understood that the factor covariance is the identity.
-    #         (Otherwise we compute its matrix square root at each step internally and
-    #          apply it to the exposures).
-    #     forecast_error_kappa (float or pd.Series): uncertainty on the
-    #         assets' correlations. See the paper, pages 32-33.
-
-    # """
-
-    factor_Sigma = None
-
-    # , normalize=False):
-    def __init__(self, F=None, d=None, num_factors=1, kelly=True):
+    def __init__(self, F=None, d=None, Sigma_F=None, num_factors=1, kelly=True):
         self.F = F if F is None else DataEstimator(F, compile_parameter=True)
         self.d = d if d is None else DataEstimator(d)
+        self.Sigma_F = Sigma_F if Sigma_F is None else DataEstimator(Sigma_F)
         if (self.F is None) or (self.d is None):
-            self.fit = True
-            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly)  # Sigma
+            self._fit = True
+            self.Sigma = HistoricalFactorizedCovariance(kelly=kelly)
         else:
-            self.fit = False
+            self._fit = False
         self.num_factors = num_factors
 
     def _pre_evaluation(self, universe, backtest_times):
         self.idyosync_sqrt_parameter = cp.Parameter(len(universe)-1)
         effective_num_factors = min(self.num_factors, len(universe)-1)
-        self.F_parameter = cp.Parameter((effective_num_factors, len(
-            universe)-1)) if self.F is None else self.F.parameter
+        if self._fit:
+            self.F_parameter = cp.Parameter((effective_num_factors, len(universe)-1)) 
+        else:
+            if self.Sigma_F is None:
+                self.F_parameter = self.F.parameter
+            else:
+                # we could refactor the code here so we don't create duplicate parameters
+                self.F_parameter = cp.Parameter(self.F.parameter.shape)        
 
     def _values_in_time(self, t, past_returns, **kwargs):
-
-        if self.fit:
+        if self._fit:
             Sigmasqrt = self.Sigma.current_value
             # numpy eigendecomposition has largest eigenvalues last
             self.F_parameter.value = Sigmasqrt[:, -self.num_factors:].T
             d = np.sum(Sigmasqrt[:, :-self.num_factors]**2, axis=1)
         else:
             d = self.d.current_value
+            if not (self.Sigma_F is None):
+                self.F_parameter.value = (self.F.parameter.value.T @ np.linalg.cholesky(self.Sigma_F.current_value)).T
+
         self.idyosync_sqrt_parameter.value = np.sqrt(d)
 
     def _compile_to_cvxpy(self, w_plus, z, w_plus_minus_w_bm):
         self.expression = cp.sum_squares(cp.multiply(
             self.idyosync_sqrt_parameter, w_plus_minus_w_bm[:-1]))
         assert self.expression.is_dcp(dpp=True)
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/simulator.py` & `cvxportfolio-0.4.5/cvxportfolio/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,15 @@
                  volumes=None,
                  prices=None,
                  datasource='YFinance',
                  cash_key='USDOLLAR',
                  base_location=BASE_LOCATION,
                  min_history=pd.Timedelta('365.24d'),
                  # TODO change logic for this (it's now this to not drop quarterly data)
-                 max_contiguous_missing='365d',
+                 max_contiguous_missing='370d',
                  trading_frequency=None,
                  copy_dataframes=True,
                  **kwargs,
                  ):
 
         # drop duplicates and ensure ordering
         universe = sorted(set(universe))
@@ -170,22 +170,33 @@
 
     def _downsample(self, interval):
         """_downsample market data."""
         if not interval in self.sampling_intervals:
             raise SyntaxError(
                 'Unsopported trading interval for down-sampling.')
         interval = self.sampling_intervals[interval]
+        new_returns_index = pd.Series(self.returns.index, self.returns.index
+            ).resample(interval, closed='left', label='left').first().values
+        # print(new_returns_index)
         self.returns = np.exp(np.log(
-            1+self.returns).resample(interval, closed='left', label='left').sum(False, 1))-1
+            1+self.returns).resample(interval, closed='left', label='left'
+                ).sum(False, 1))-1
+        self.returns.index = new_returns_index
         if self.volumes is not None:
+            new_volumes_index = pd.Series(self.volumes.index, self.volumes.index
+                ).resample(interval, closed='left', label='left').first().values
             self.volumes = self.volumes.resample(
                 interval, closed='left', label='left').sum(False, 1)
+            self.volumes.index = new_volumes_index
         if self.prices is not None:
+            new_prices_index = pd.Series(self.prices.index, self.prices.index
+                ).resample(interval, closed='left', label='left').first().values
             self.prices = self.prices.resample(
                 interval, closed='left', label='left').first()
+            self.prices.index = new_prices_index
 
     @property
     def PPY(self):
         "Periods per year, assumes returns are about equally spaced."
         return periods_per_year(self.returns.index)
 
     def _check_sizes(self):
@@ -421,15 +432,15 @@
                  prices=None, costs=[], round_trades=False,
                  min_history=pd.Timedelta('365d'),
                  datasource='YFinance',
                  cash_key="USDOLLAR", base_location=BASE_LOCATION,
                  trading_frequency=None, **kwargs):
         """Initialize the Simulator and download data if necessary."""
         self.base_location = Path(base_location)
-        
+
         self.enable_caching = len(universe) > 0
 
         self.market_data = MarketData(
             universe=universe, returns=returns,
             volumes=volumes, prices=prices,
             cash_key=cash_key, base_location=base_location,
             trading_frequency=trading_frequency,
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/base.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/base.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/returns.csv` & `cvxportfolio-0.4.5/cvxportfolio/tests/returns.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/sigmas.csv` & `cvxportfolio-0.4.5/cvxportfolio/tests/sigmas.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_constraints.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import cvxpy as cp
 import cvxportfolio as cvx
 
+
 def listvalue(li):
     return all([el.value() for el in li])
 
 
 class TestConstraints(unittest.TestCase):
 
     @classmethod
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_costs.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_data.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,26 +228,16 @@
         store = storeclass(*args, **kwargs)
 
         # second level is object
         timeindex = pd.date_range("2022-01-01", "2022-01-30")
         second_level = ["hello", "ciao", "hola"]
         index = pd.MultiIndex.from_product([timeindex, second_level])
         data = pd.DataFrame(np.random.randn(len(index), 10), index=index)
-        data.columns = [
-            "one",
-            "two",
-            "tre",
-            "quattro",
-            "cinque",
-            "sei",
-            "sette",
-            "otto",
-            "nove",
-            "dieci",
-        ]
+        data.columns = ["one", "two", "tre", "quattro",
+                        "cinque", "sei", "sette", "otto", "nove", "dieci"]
 
         print(data.index)
         print(data)
         print(data.index.dtype)
         print(data.dtypes)
 
         store.store("example", data)
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_estimator.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_estimator.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 import numpy as np
 import pandas as pd
 import unittest
 
 from cvxportfolio.estimator import DataEstimator  # , ParameterEstimator
 from cvxportfolio.errors import MissingValuesError, DataError
+import cvxportfolio as cvx
 
 
 class PlaceholderCallable:
     def __init__(self, value):
         self.value = value
 
     def values_in_time(self, t, **kwargs):
@@ -170,10 +171,23 @@
             universe=None, backtest_times=timeindex)
         # assert hasattr(estimator, 'parameter')
         self.assertTrue(hasattr(estimator, "parameter"))
         estimator._recursive_values_in_time("2022-01-05")
         self.assertTrue(
             np.all(estimator.parameter.value == data.loc["2022-01-05"]))
 
+    def test_repr_dataestimator(self):
+        print(DataEstimator(3))
+        print(DataEstimator(np.array([1, 2, 3])))
+        print(DataEstimator(pd.Series([1, 2, 3])))
+        print(DataEstimator(pd.DataFrame([1, 2, 3])))
+
+    def test_repr(self):
+        print(cvx.FactorModelCovariance(num_factors=10))
+        print(cvx.ReturnsForecast() - .5 * cvx.FullCovariance())
+        print(cvx.SinglePeriodOptimization(cvx.ReturnsForecast(),
+                                           [cvx.LongOnly(nocash=True)]))
+        print(cvx.LeverageLimit(3))
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_forecast.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_hyperparameters.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_hyperparameters.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,77 +22,77 @@
 import numpy as np
 import pandas as pd
 
 
 import cvxportfolio as cvx
 from cvxportfolio.hyperparameters import *
 
+
 class TestHyperparameters(unittest.TestCase):
 
     @classmethod
     def setUpClass(cls):
         """Load the data and initialize cvxpy vars."""
         # cls.sigma = pd.read_csv(Path(__file__).parent / "sigmas.csv", index_col=0, parse_dates=[0])
         cls.returns = pd.read_csv(
             Path(__file__).parent / "returns.csv", index_col=0, parse_dates=[0])
         # cls.volumes = pd.read_csv(Path(__file__).parent / "volumes.csv", index_col=0, parse_dates=[0])
         cls.w_plus = cp.Variable(cls.returns.shape[1])
         cls.w_plus_minus_w_bm = cp.Variable(cls.returns.shape[1])
         cls.z = cp.Variable(cls.returns.shape[1])
         cls.N = cls.returns.shape[1]
-        
-    
+
     def test_basic_HP(self):
-        
-        gamma = GammaRisk(initial_value = 1)
-        
+
+        gamma = GammaRisk(initial_value=1)
+
         self.assertTrue((-gamma).current_value == -1)
         self.assertTrue((gamma * .5).current_value == .5)
         self.assertTrue((.5 * gamma).current_value == .5)
         self.assertTrue((gamma).current_value == 1)
-        
+
         cvx.SinglePeriodOptimization(GammaRisk() * cvx.FullCovariance())
-        
+
         with self.assertRaises(SyntaxError):
             cvx.SinglePeriodOptimization(GammaRisk * cvx.FullCovariance())
-            
+
         cvx.SinglePeriodOptimization(-GammaRisk() * cvx.FullCovariance())
-        
+
     def test_HP_algebra(self):
-        grisk = GammaRisk(initial_value = 1)
-        gtrade = GammaRisk(initial_value = .5)
-        
+        grisk = GammaRisk(initial_value=1)
+        gtrade = GammaRisk(initial_value=.5)
+
         self.assertTrue((grisk + gtrade).current_value == 1.5)
         self.assertTrue((grisk * gtrade).current_value == .5)
         self.assertTrue((2 * grisk * gtrade).current_value == 1)
         self.assertTrue((2 * grisk * gtrade + grisk).current_value == 2)
         self.assertTrue((1.9 * grisk * gtrade + grisk).current_value == 1.95)
         self.assertTrue((grisk + 2*gtrade).current_value == 2)
         self.assertTrue((grisk/2 + 2*gtrade).current_value == 1.5)
         self.assertTrue((grisk/2 + 2 * (gtrade + gtrade/2)).current_value == 2)
-        
+
     def test_collect_HPs(self):
         """Collect hyperparameters."""
-        
+
         pol = cvx.SinglePeriodOptimization(GammaRisk() * cvx.FullCovariance())
-        
+
         res = pol._collect_hyperparameters()
         print(res)
         self.assertTrue(len(res) == 1)
-        
-        pol = cvx.SinglePeriodOptimization(-GammaRisk() * cvx.FullCovariance()\
-             - GammaTrade() * cvx.TransactionCost())
-        
+
+        pol = cvx.SinglePeriodOptimization(-GammaRisk() * cvx.FullCovariance()
+                                           - GammaTrade() * cvx.TransactionCost())
+
         res = pol._collect_hyperparameters()
         print(res)
         self.assertTrue(len(res) == 2)
-        
-        pol = cvx.SinglePeriodOptimization(-(GammaRisk()+ .5 * GammaRisk()) 
-            * cvx.FullCovariance() - GammaTrade() * cvx.TransactionCost())
-        
+
+        pol = cvx.SinglePeriodOptimization(-(GammaRisk() + .5 * GammaRisk())
+                                           * cvx.FullCovariance() - GammaTrade() * cvx.TransactionCost())
+
         res = pol._collect_hyperparameters()
         print(res)
         self.assertTrue(len(res) == 3)
-        
-        
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_policies.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_policies.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_returns.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_returns.py`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_risks.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_risks.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,14 +188,39 @@
         risk_model._recursive_values_in_time(
             t=self.returns.index[12], past_returns='hello')
         self.w_plus_minus_w_bm.value = np.random.randn(self.N)
 
         self.assertTrue(np.isclose(cvxpy_expression.value,
                                    self.w_plus_minus_w_bm.value[:-1] @ np.diag(d) @ self.w_plus_minus_w_bm.value[:-1] +
                                    ((F @ self.w_plus_minus_w_bm.value[:-1])**2).sum()))
+                                   
+
+
+    def test_low_rank_covariance_with_SigmaF(self):
+
+        F = pd.DataFrame(np.random.randn(2, self.N-1),
+                         columns=self.returns.columns[:-1])
+        d = pd.Series(np.random.uniform(size=(self.N-1)),
+                      self.returns.columns[:-1])
+        SigmaF = np.random.randn(2,2)
+        SigmaF = SigmaF.T @ SigmaF
+        risk_model = FactorModelCovariance(F=F, d=d, Sigma_F = SigmaF)
+
+        cvxpy_expression = self.boilerplate(risk_model)
+        self.assertTrue(cvxpy_expression.is_convex())
+
+        risk_model._recursive_values_in_time(
+            t=self.returns.index[12], past_returns='hello')
+        self.w_plus_minus_w_bm.value = np.random.randn(self.N)
+
+        self.assertTrue(np.isclose(cvxpy_expression.value,
+                                   self.w_plus_minus_w_bm.value[:-1] @ np.diag(d) @ self.w_plus_minus_w_bm.value[:-1] +
+                                   self.w_plus_minus_w_bm.value[:-1].T @ F.T @ SigmaF @ F @ self.w_plus_minus_w_bm.value[:-1])
+                                   )
+                                            
 
     def test_estimated_low_rank_covariance(self):
 
         risk_model = FactorModelCovariance()  # normalize=False)
 
         cvxpy_expression = self.boilerplate(risk_model)
         self.assertTrue(cvxpy_expression.is_convex())
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/test_simulator.py` & `cvxportfolio-0.4.5/cvxportfolio/tests/test_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,20 @@
             new_md._downsample(freqs[i])
             print(new_md.returns)
             self.assertTrue(np.isnan(new_md.returns.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.volumes.GOOG.iloc[0]))
             self.assertTrue(np.isnan(new_md.prices.GOOG.iloc[0]))
 
             if freqs[i] == 'weekly':
-                self.assertTrue(all(new_md.returns.index.weekday == 0))
+                print((new_md.returns.index.weekday < 2).mean())
+                self.assertTrue((new_md.returns.index.weekday < 2).mean() > .95)
 
             if freqs[i] == 'monthly':
-                self.assertTrue(all(new_md.returns.index.day == 1))
+                print((new_md.returns.index.day < 5).mean())
+                self.assertTrue((new_md.returns.index.day < 5).mean() > .95)
 
             self.assertTrue(
                 all(md.prices.loc[testdays[i]] == new_md.prices.loc[testdays[i]]))
             self.assertTrue(np.allclose(
                 md.volumes.loc[periods[i]].sum(), new_md.volumes.loc[testdays[i]]))
             self.assertTrue(np.allclose(
                 (1 + md.returns.loc[periods[i]]).prod(), 1 + new_md.returns.loc[testdays[i]]))
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio/tests/volumes.csv` & `cvxportfolio-0.4.5/cvxportfolio/tests/volumes.csv`

 * *Files identical despite different names*

### Comparing `cvxportfolio-0.4.4/cvxportfolio.egg-info/PKG-INFO` & `cvxportfolio-0.4.5/cvxportfolio.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxportfolio
-Version: 0.4.4
+Version: 0.4.5
 Summary: Portfolio optimization.
 Home-page: https://cvxportfolio.readthedocs.io
 Author: Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.
 Author-email: enzo.busseti@gmail.com
 Maintainer: Enzo Busseti
 License: Apache 2.0
 Description-Content-Type: text/markdown
@@ -20,24 +20,26 @@
 
 
 
 `cvxportfolio` is a python library for portfolio optimization and simulation
 based on the book [Multi-Period Trading via Convex Optimization](https://web.stanford.edu/~boyd/papers/pdf/cvx_portfolio.pdf)
 (also [available in print](https://www.amazon.com/Multi-Period-Trading-Convex-Optimization-Foundations/dp/1680833286/)).
 
-The documentation of the package is kindly hosted by [Read the Docs](https://readthedocs.org) at [www.cvxportfolio.com](https://www.cvxportfolio.com).
+The documentation of the package is kindly hosted by [Read the Docs](https://readthedocs.org) at [www.cvxportfolio.com](https://www.cvxportfolio.com). We also show some of our tutorials and examples on our
+[youtube channel](https://www.youtube.com/@Cvxportfolio).
 
 
 Installation
 ------------
 All our source code and releases are kindly hosted by the [Python Package Index](https://pypi.org). You can install the latest one with
 
 ```
 pip install -U cvxportfolio
 ```
+You can see how this works on our [Installation and Hello World](https://youtu.be/1ThOKEu371M) youtube video.
 
 Testing locally
 ------------
 We ship our unit test suite with the pip package. After installing you can test in you local environment by
 
 ```
 python -m unittest discover cvxportfolio
@@ -55,15 +57,14 @@
 matches what is described in Chapter 7 of the book. For example, returns are forecasted as the historical mean returns 
 and covariances as historical covariances (both ignoring `np.nan`'s). The logic used is detailed in the `forecast` module. Many optimizations
 are applied to make sure the system works well with real data. 
 
 
 ```python
 import cvxportfolio as cvx
-import matplotlib.pyplot as plt
 
 gamma = 3       # risk aversion parameter (Chapter 4.2)
 kappa = 0.05    # covariance forecast error risk parameter (Chapter 4.3)
 objective = cvx.ReturnsForecast() - gamma * (
 	cvx.FullCovariance() + kappa * cvx.RiskForecastError()
 ) - cvx.StocksTransactionCost()
 constraints = [cvx.LeverageLimit(3)]
```

### Comparing `cvxportfolio-0.4.4/cvxportfolio.egg-info/SOURCES.txt` & `cvxportfolio-0.4.5/cvxportfolio.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 cvxportfolio/tests/test_estimator.py
 cvxportfolio/tests/test_forecast.py
 cvxportfolio/tests/test_hyperparameters.py
 cvxportfolio/tests/test_policies.py
 cvxportfolio/tests/test_returns.py
 cvxportfolio/tests/test_risks.py
 cvxportfolio/tests/test_simulator.py
+cvxportfolio/tests/test_utils.py
 cvxportfolio/tests/volumes.csv
```

### Comparing `cvxportfolio-0.4.4/setup.py` & `cvxportfolio-0.4.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_descr = ''.join(f.readlines())
 
 setup(
     name='cvxportfolio',
-    version='0.4.4',
+    version='0.4.5',
     author='Enzo Busseti, Stephen Boyd, Steven Diamond, BlackRock Inc.',
     maintainer='Enzo Busseti',
     author_email='enzo.busseti@gmail.com',
     packages=['cvxportfolio',
               'cvxportfolio.tests'],
     package_dir={'cvxportfolio': 'cvxportfolio'},
     package_data={'cvxportfolio': [
```


# Comparing `tmp/quantile-forest-1.1.3.tar.gz` & `tmp/quantile-forest-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantile-forest-1.1.3.tar", last modified: Sat Jul  8 11:46:41 2023, max compression
+gzip compressed data, was "quantile-forest-1.2.0.tar", last modified: Wed Aug  2 07:11:10 2023, max compression
```

## Comparing `quantile-forest-1.1.3.tar` & `quantile-forest-1.2.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2633 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.454120 quantile-forest-1.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.450119 quantile-forest-1.1.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.454120 quantile-forest-1.1.3/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_static/css/quantile-forest.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.454120 quantile-forest-1.1.3/docs/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_static/js/copybutton.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.458120 quantile-forest-1.1.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/numpydoc_docstring.rst
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/_templates/sidebar-search-bs.html
--rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/api.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     7000 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/conf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/make.bat
--rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/sphinx_requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    12126 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/docs/user_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.458120 quantile-forest-1.1.3/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/README.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_extrapolation_problem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_interpolation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_regression_intervals.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_toy_example.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1578 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_vs_standard_forest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/examples/plot_quantile_weighted_vs_unweighted.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.458120 quantile-forest-1.1.3/quantile_forest/
--rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_min_dependencies.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    51906 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_quantile_forest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pxd
--rwxr-xr-x   0 runner    (1001) docker     (123)    37885 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/quantile_forest/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/tests/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43958 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/tests/test_quantile_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/quantile_forest/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/quantile_forest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-08 11:46:41.000000 quantile-forest-1.1.3/quantile_forest.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-08 11:46:41.462120 quantile-forest-1.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-07-08 11:46:11.000000 quantile-forest-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.650361 quantile-forest-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-02 07:11:10.650361 quantile-forest-1.2.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2813 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.646361 quantile-forest-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.642361 quantile-forest-1.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.646361 quantile-forest-1.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_static/css/quantile-forest.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.646361 quantile-forest-1.2.0/docs/_static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_static/js/copybutton.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.646361 quantile-forest-1.2.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_templates/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_templates/numpydoc_docstring.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/_templates/sidebar-search-bs.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)      314 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/api.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7000 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/conf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      922 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      912 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/make.bat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      268 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/sphinx_requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12713 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/docs/user_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.646361 quantile-forest-1.2.0/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      101 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/README.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2878 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/plot_quantile_extrapolation_problem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1865 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/plot_quantile_interpolation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3961 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/plot_quantile_regression_intervals.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1784 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/plot_quantile_toy_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1578 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/plot_quantile_vs_standard_forest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3270 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/examples/plot_quantile_weighted_vs_unweighted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.650361 quantile-forest-1.2.0/quantile_forest/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      956 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/_min_dependencies.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    52621 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/_quantile_forest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1347 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/_quantile_forest_fast.pxd
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37885 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/_quantile_forest_fast.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.650361 quantile-forest-1.2.0/quantile_forest/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/tests/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44878 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/tests/test_quantile_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/quantile_forest/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 07:11:10.650361 quantile-forest-1.2.0/quantile_forest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 07:11:10.000000 quantile-forest-1.2.0/quantile_forest.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-02 07:11:10.650361 quantile-forest-1.2.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-08-02 07:10:40.000000 quantile-forest-1.2.0/setup.py
```

### Comparing `quantile-forest-1.1.3/LICENSE` & `quantile-forest-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/PKG-INFO` & `quantile-forest-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-forest
-Version: 1.1.3
+Version: 1.2.0
 Summary: scikit-learn compatible quantile forests.
 Maintainer: Zillow Group AI Team
 License: Apache License 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
@@ -29,15 +29,15 @@
 [![GitHub Actions](https://github.com/zillow/quantile-forest/actions/workflows/build.yml/badge.svg)](https://github.com/zillow/quantile-forest/actions/workflows/build.yml)
 [![Codecov](https://codecov.io/gh/zillow/quantile-forest/branch/main/graph/badge.svg?token=STRT8T67YP)](https://codecov.io/gh/zillow/quantile-forest)
 [![Code Style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/quantile-forest)](https://pypi.org/project/quantile-forest)
 
 **quantile-forest** offers a Python implementation of quantile regression forests compatible with scikit-learn.
 
-Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles; they can estimate arbitrary quantiles at prediction time without retraining. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
+Quantile regression forests (QRF) are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package are performant, Cython-optimized QRF implementations that extend the forest estimators available in scikit-learn to estimate conditional quantiles. The estimators can estimate arbitrary quantiles at prediction time without retraining and provide methods for out-of-bag estimation, calculating quantile ranks, and computing proximity counts. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
 
 #### Example of fitted model predictions and prediction intervals on California housing data ([code](https://zillow.github.io/quantile-forest/auto_examples/plot_quantile_regression_intervals.html#sphx-glr-auto-examples-plot-quantile-regression-intervals-py))
 <img src="https://zillow.github.io/quantile-forest/_images/sphx_glr_plot_quantile_regression_intervals_001.png" height="300" />
 
 Quick Start
 -----------
```

### Comparing `quantile-forest-1.1.3/README.md` & `quantile-forest-1.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![GitHub Actions](https://github.com/zillow/quantile-forest/actions/workflows/build.yml/badge.svg)](https://github.com/zillow/quantile-forest/actions/workflows/build.yml)
 [![Codecov](https://codecov.io/gh/zillow/quantile-forest/branch/main/graph/badge.svg?token=STRT8T67YP)](https://codecov.io/gh/zillow/quantile-forest)
 [![Code Style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/quantile-forest)](https://pypi.org/project/quantile-forest)
 
 **quantile-forest** offers a Python implementation of quantile regression forests compatible with scikit-learn.
 
-Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles; they can estimate arbitrary quantiles at prediction time without retraining. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
+Quantile regression forests (QRF) are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package are performant, Cython-optimized QRF implementations that extend the forest estimators available in scikit-learn to estimate conditional quantiles. The estimators can estimate arbitrary quantiles at prediction time without retraining and provide methods for out-of-bag estimation, calculating quantile ranks, and computing proximity counts. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
 
 #### Example of fitted model predictions and prediction intervals on California housing data ([code](https://zillow.github.io/quantile-forest/auto_examples/plot_quantile_regression_intervals.html#sphx-glr-auto-examples-plot-quantile-regression-intervals-py))
 <img src="https://zillow.github.io/quantile-forest/_images/sphx_glr_plot_quantile_regression_intervals_001.png" height="300" />
 
 Quick Start
 -----------
```

### Comparing `quantile-forest-1.1.3/docs/Makefile` & `quantile-forest-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/_static/css/quantile-forest.css` & `quantile-forest-1.2.0/docs/_static/css/quantile-forest.css`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/_static/js/copybutton.js` & `quantile-forest-1.2.0/docs/_static/js/copybutton.js`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/conf.py` & `quantile-forest-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/index.rst` & `quantile-forest-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/install.rst` & `quantile-forest-1.2.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/make.bat` & `quantile-forest-1.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/docs/user_guide.rst` & `quantile-forest-1.2.0/docs/user_guide.rst`

 * *Files 6% similar despite different names*

```diff
@@ -55,17 +55,27 @@
 
     >>> y_pred = reg.predict(X_test, quantiles=[0.25, 0.5, 0.75])  # returns three columns per row
 
 If the `predict` method is called without quantiles, the prediction defaults to the empirical median (`quantiles = 0.5`)::
 
     >>> y_pred = reg.predict(X_test)  # returns empirical median prediction for each test sample
 
-If the `predict` method is explicitly called with `quantiles = None`, the prediction returns the empirical mean::
+If the `predict` method is explicitly called with `quantiles = "mean"`, the prediction returns the empirical mean::
 
-    >>> y_pred = reg.predict(X_test, quantiles=None)  # returns empirical mean prediction for each test sample
+    >>> y_pred = reg.predict(X_test, quantiles="mean")  # returns empirical mean prediction for each test sample
+
+Default quantiles can be specified at model initialization using the `default_quantiles` parameter:
+
+    >>> reg = RandomForestQuantileRegressor(default_quantiles=[0.25, 0.5, 0.75]).fit(X_train, y_train)
+    >>> y_pred = reg.predict(X_test)  # predicts using the default quantiles
+
+The default quantiles can be overwritten at prediction time by specifying a value for `quantiles`:
+
+    >>> reg = RandomForestQuantileRegressor(default_quantiles=[0.25, 0.5, 0.75]).fit(X_train, y_train)
+    >>> y_pred = reg.predict(X_test, quantiles=0.5)  # predicts using the override quantiles
 
 The output of the `predict` method is an array with one column for each specified quantile or a single column if no quantiles are specified. The order of the output columns corresponds to the order of the quantiles, which can be specified in any order (i.e., they do not need to be monotonically ordered)::
 
     >>> y_pred = reg.predict(X_test, quantiles=[0.5, 0.25, 0.75])  # first column corresponds to quantile 0.5
 
 By default, the predict method calculates quantiles by weighting each sample inversely according to the size of its leaf node (`weighted_leaves = True`). If `weighted_leaves = False`, each sample in a leaf (including repeated bootstrap samples) will be given equal weight. Note that this leaf-based weighting can only be used with weighted quantiles.
 
@@ -88,29 +98,29 @@
     >>> indices = np.concatenate([np.arange(len(X_train)), np.full(len(X_test), -1, dtype=int)])
     >>> y_pred_mix = reg.predict(X_mixed, quantiles=[0.25, 0.5, 0.75], oob_score=True, indices=indices)
     >>> y_pred_train_oob = y_pred_mix[:len(X_train)]  # predictions on the training data are OOB
     >>> y_pred_test = y_pred_mix[-len(X_test):]  # predictions on the new test data are IB
 
 This allows all samples, both from the training and test sets, to be scored with a single call to `predict`, whereby OOB predictions are returned for the training samples and IB (i.e., non-OOB) predictions are returned for the test samples.
 
-The predictions of a standard random forest can also be recovered from a quantile forest without retraining by passing `quantiles = None` and `aggregate_leaves_first = False`, the latter which specifies a Boolean flag to average the leaf values before aggregating the leaves across trees. This configuration essentially replicates the prediction process used by a standard random forest regressor, which is an averaging of mean leaf values across trees::
+The predictions of a standard random forest can also be recovered from a quantile forest without retraining by passing `quantiles = "mean"` and `aggregate_leaves_first = False`, the latter which specifies a Boolean flag to average the leaf values before aggregating the leaves across trees. This configuration essentially replicates the prediction process used by a standard random forest regressor, which is an averaging of mean leaf values across trees::
 
     >>> import numpy as np
     >>> from sklearn import datasets
     >>> from sklearn.ensemble import RandomForestRegressor
     >>> from sklearn.model_selection import train_test_split
     >>> from quantile_forest import RandomForestQuantileRegressor
     >>> X, y = datasets.load_diabetes(return_X_y=True)
     >>> X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.25)
     >>> rf = RandomForestRegressor(random_state=0)
     >>> qrf = RandomForestQuantileRegressor(max_samples_leaf=None, random_state=0)
     >>> rf.fit(X_train, y_train), qrf.fit(X_train, y_train)
     (RandomForestRegressor(random_state=0), RandomForestQuantileRegressor(max_samples_leaf=None, random_state=0))
     >>> y_pred_rf = rf.predict(X_test)
-    >>> y_pred_qrf = qrf.predict(X_test, quantiles=None, aggregate_leaves_first=False)
+    >>> y_pred_qrf = qrf.predict(X_test, quantiles="mean", aggregate_leaves_first=False)
     >>> np.allclose(y_pred_rf, y_pred_qrf)
     True
 
 Quantile Ranks
 ----------------
 
 The quantile rank of a score is the quantile of scores in its frequency distribution that are equal to or lower than it. The output quantile rank will be a value in the range [0, 1] for each test sample. The quantile rank of each sample is calculated by aggregating all of the training samples that share the same leaf node across all of the trees::
```

### Comparing `quantile-forest-1.1.3/examples/plot_quantile_extrapolation_problem.py` & `quantile-forest-1.2.0/examples/plot_quantile_extrapolation_problem.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/examples/plot_quantile_interpolation.py` & `quantile-forest-1.2.0/examples/plot_quantile_interpolation.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/examples/plot_quantile_regression_intervals.py` & `quantile-forest-1.2.0/examples/plot_quantile_regression_intervals.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/examples/plot_quantile_toy_example.py` & `quantile-forest-1.2.0/examples/plot_quantile_toy_example.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/examples/plot_quantile_vs_standard_forest.py` & `quantile-forest-1.2.0/examples/plot_quantile_vs_standard_forest.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/examples/plot_quantile_weighted_vs_unweighted.py` & `quantile-forest-1.2.0/examples/plot_quantile_weighted_vs_unweighted.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/pyproject.toml` & `quantile-forest-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/quantile_forest/__init__.py` & `quantile-forest-1.2.0/quantile_forest/__init__.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/quantile_forest/_min_dependencies.py` & `quantile-forest-1.2.0/quantile_forest/_min_dependencies.py`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/quantile_forest/_quantile_forest.py` & `quantile-forest-1.2.0/quantile_forest/_quantile_forest.py`

 * *Files 2% similar despite different names*

```diff
@@ -363,15 +363,15 @@
         )
         unsampled_indices = _generate_unsampled_indices(sample_indices, duplicates=duplicates)
         return np.asarray(unsampled_indices)
 
     def predict(
         self,
         X,
-        quantiles=0.5,
+        quantiles=None,
         interpolation="linear",
         weighted_quantile=True,
         weighted_leaves=True,
         aggregate_leaves_first=True,
         oob_score=False,
         indices=None,
         duplicates=None,
@@ -381,18 +381,19 @@
         Parameters
         ----------
         X : {array-like, sparse matrix} of shape (n_samples, n_features)
             The input samples. Internally, its dtype will be converted to
             ``dtype=np.float32``. If a sparse matrix is provided, it will be
             converted into a sparse ``csr_matrix``.
 
-        quantiles : float or list, default=0.5
+        quantiles : float, list, or "mean", default=None
             The quantile or list of quantiles that the model tries to predict.
-            Each quantile must be strictly between 0 and 1. If None, the model
-            predicts the mean. By default, the model predicts the median.
+            Each quantile must be strictly between 0 and 1. If "mean", the
+            model predicts the mean. If None, the model uses the value of
+            `default_quantiles`.
 
         interpolation : {"linear", "lower", "higher", "midpoint", "nearest"}, \
                 default="linear"
             Specifies the interpolation method to use when the desired
             quantile lies between two data points ``i < j``:
 
             - If "linear", then ``i + (j - i) * fraction``, where ``fraction``
@@ -442,14 +443,20 @@
             where ``q`` is the quantile.
         """
         check_is_fitted(self)
         # Check data.
         X = self._validate_X_predict(X)
 
         if quantiles is None:
+            if self.default_quantiles is None:
+                quantiles = [-1]
+            else:
+                quantiles = self.default_quantiles
+
+        if quantiles == "mean":
             quantiles = [-1]
 
         if not isinstance(quantiles, list):
             quantiles = [quantiles]
 
         if not isinstance(interpolation, (bytes, bytearray)):
             interpolation = interpolation.encode()
@@ -738,14 +745,19 @@
     each tree.
 
     Parameters
     ----------
     n_estimators : int, default=100
         The number of trees in the forest.
 
+    default_quantiles : float, list, or "mean", default=0.5
+        The default quantile or list of quantiles that the model tries to
+        predict. Each quantile must be strictly between 0 and 1. If "mean",
+        the model predicts the mean.
+
     criterion : {"squared_error", "absolute_error", "poisson"}, \
             default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
         variance reduction as feature selection criterion, "absolute_error"
         for the mean absolute error, and "poisson" which uses reduction in
         Poisson deviance to find splits.
@@ -921,28 +933,28 @@
     .. [1] N. Meinshausen, "Quantile Regression Forests", Journal of Machine
            Learning Research, 7(Jun), 983-999, 2006.
            http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
 
     Examples
     --------
     >>> from quantile_forest import RandomForestQuantileRegressor
-    >>> from sklearn.datasets import make_regression
-    >>> X, y = make_regression(
-    ...     n_features=4, n_informative=2, random_state=0, shuffle=False)
-    >>> regr = RandomForestQuantileRegressor(max_depth=2, random_state=0)
-    >>> regr.fit(X, y)
-    RandomForestQuantileRegressor(...)
-    >>> print(regr.predict([[0, 0, 0, 0]], quantiles=0.5))
-    [-3.04264873]
+    >>> from sklearn.datasets import fetch_california_housing
+    >>> X, y = fetch_california_housing(return_X_y=True)
+    >>> qrf = RandomForestQuantileRegressor(random_state=0)
+    >>> qrf.fit(X[:1000], y[:1000])
+    RandomForestQuantileRegressor(random_state=0)
+    >>> qrf.score(X, y, quantiles=0.5)
+    0.3592...
     """
 
     def __init__(
         self,
         n_estimators=100,
         *,
+        default_quantiles=0.5,
         criterion="squared_error",
         max_depth=None,
         min_samples_split=2,
         min_samples_leaf=1,
         max_samples_leaf=1,
         min_weight_fraction_leaf=0.0,
         max_features=1.0,
@@ -980,14 +992,15 @@
             "random_state": random_state,
             "verbose": verbose,
             "warm_start": warm_start,
             "max_samples": max_samples,
         }
         super(RandomForestQuantileRegressor, self).__init__(**init_dict)
 
+        self.default_quantiles = default_quantiles
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_samples_leaf = max_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
@@ -1014,14 +1027,19 @@
     over-fitting.
 
     Parameters
     ----------
     n_estimators : int, default=100
         The number of trees in the forest.
 
+    default_quantiles : float, list, or "mean", default=0.5
+        The default quantile or list of quantiles that the model tries to
+        predict. Each quantile must be strictly between 0 and 1. If "mean",
+        the model predicts the mean.
+
     criterion : {"squared_error", "absolute_error"}, default="squared_error"
         The function to measure the quality of a split. Supported criteria
         are "squared_error" for the mean squared error, which is equal to
         variance reduction as feature selection criterion, and "absolute_error"
         for the mean absolute error.
 
     max_depth : int, default=None
@@ -1195,30 +1213,29 @@
     ----------
     .. [1] N. Meinshausen, "Quantile Regression Forests", Journal of Machine
            Learning Research, 7(Jun), 983-999, 2006.
            http://www.jmlr.org/papers/volume7/meinshausen06a/meinshausen06a.pdf
 
     Examples
     --------
-    >>> from sklearn.datasets import load_diabetes
-    >>> from sklearn.model_selection import train_test_split
     >>> from quantile_forest import ExtraTreesQuantileRegressor
-    >>> X, y = load_diabetes(return_X_y=True)
-    >>> X_train, X_test, y_train, y_test = train_test_split(
-    ...     X, y, random_state=0)
-    >>> reg = ExtraTreesQuantileRegressor(
-    ...     n_estimators=100, random_state=0).fit(X_train, y_train)
-    >>> reg.score(X_test, y_test, quantiles=0.5)
-    0.2152...
+    >>> from sklearn.datasets import fetch_california_housing
+    >>> X, y = fetch_california_housing(return_X_y=True)
+    >>> qrf = ExtraTreesQuantileRegressor(random_state=0)
+    >>> qrf.fit(X[:1000], y[:1000])
+    ExtraTreesQuantileRegressor(random_state=0)
+    >>> qrf.score(X, y, quantiles=0.5)
+    0.3352...
     """
 
     def __init__(
         self,
         n_estimators=100,
         *,
+        default_quantiles=0.5,
         criterion="squared_error",
         max_depth=None,
         min_samples_split=2,
         min_samples_leaf=1,
         max_samples_leaf=1,
         min_weight_fraction_leaf=0.0,
         max_features=1.0,
@@ -1256,14 +1273,15 @@
             "random_state": random_state,
             "verbose": verbose,
             "warm_start": warm_start,
             "max_samples": max_samples,
         }
         super(ExtraTreesQuantileRegressor, self).__init__(**init_dict)
 
+        self.default_quantiles = default_quantiles
         self.criterion = criterion
         self.max_depth = max_depth
         self.min_samples_split = min_samples_split
         self.min_samples_leaf = min_samples_leaf
         self.max_samples_leaf = max_samples_leaf
         self.min_weight_fraction_leaf = min_weight_fraction_leaf
         self.max_features = max_features
```

### Comparing `quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pxd` & `quantile-forest-1.2.0/quantile_forest/_quantile_forest_fast.pxd`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/quantile_forest/_quantile_forest_fast.pyx` & `quantile-forest-1.2.0/quantile_forest/_quantile_forest_fast.pyx`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/quantile_forest/tests/test_quantile_forest.py` & `quantile-forest-1.2.0/quantile_forest/tests/test_quantile_forest.py`

 * *Files 1% similar despite different names*

```diff
@@ -358,20 +358,22 @@
 
     # Check that unaggregated predicted means match non-quantile regressor.
     if not aggregate_leaves_first:
         if name == "ExtraTreesQuantileRegressor":
             est1 = ExtraTreesRegressor(n_estimators=10, random_state=0)
             est2 = ExtraTreesQuantileRegressor(
                 n_estimators=10,
+                default_quantiles=None,
                 random_state=0,
             )
         else:
             est1 = RandomForestRegressor(n_estimators=10, random_state=0)
             est2 = RandomForestQuantileRegressor(
                 n_estimators=10,
+                default_quantiles=None,
                 random_state=0,
             )
         y_pred_1 = est1.fit(X_train, y_train).predict(X_test)
         y_pred_2 = est2.fit(X_train, y_train).predict(
             X_test,
             quantiles=None,
             weighted_quantile=weighted_quantile,
@@ -379,14 +381,27 @@
             aggregate_leaves_first=False,
         )
         assert_allclose(y_pred_1, y_pred_2)
 
     est = ForestRegressor(n_estimators=1, random_state=0)
     est.fit(X_train, y_train)
 
+    # Check that specifying `quantiles` overwrites `default_quantiles`.
+    est1 = ForestRegressor(n_estimators=1, random_state=0)
+    est1.fit(X_train, y_train)
+    y_pred_1 = est1.predict(X_test, quantiles=0.5)
+    est2 = ForestRegressor(
+        n_estimators=1,
+        default_quantiles=[0.25, 0.5, 0.75],
+        random_state=0,
+    )
+    est2.fit(X_train, y_train)
+    y_pred_2 = est2.predict(X_test, quantiles=0.5)
+    assert_allclose(y_pred_1, y_pred_2)
+
     # Check error if invalid quantiles.
     assert_raises(ValueError, est.predict, X_test, -0.01)
     assert_raises(ValueError, est.predict, X_test, 1.01)
 
 
 @pytest.mark.parametrize("name", FOREST_REGRESSORS)
 @pytest.mark.parametrize("weighted_quantile", [True, False])
@@ -814,14 +829,23 @@
         weighted_quantile=weighted_quantile,
         aggregate_leaves_first=aggregate_leaves_first,
         oob_score=True,
         indices=-np.ones(len(X)),
     )
     assert np.all(y_pred_ib == y_pred_oob)
 
+    # Check OOB predictions with `default_quantiles`.
+    est1 = ForestRegressor(n_estimators=1, random_state=0)
+    est1.fit(X, y)
+    est2 = ForestRegressor(n_estimators=1, default_quantiles=quantiles, random_state=0)
+    est2.fit(X, y)
+    y_pred_oob1 = est1.predict(X, quantiles=quantiles)
+    y_pred_oob2 = est2.predict(X)
+    assert_allclose(y_pred_oob1, y_pred_oob2)
+
     # Check error if OOB score without `indices` do not match training count.
     assert_raises(ValueError, est.predict, X[:1], oob_score=True)
 
     # Check error if OOB score with `indices` do not match samples count.
     assert_raises(
         ValueError,
         est.predict,
@@ -880,15 +904,15 @@
             weighted_quantile=weighted_quantile,
             aggregate_leaves_first=aggregate_leaves_first,
             oob_score=True,
         )
 
 
 @pytest.mark.parametrize("name", FOREST_REGRESSORS)
-@pytest.mark.parametrize("quantiles", [None, 0.5, [0.2, 0.5, 0.8]])
+@pytest.mark.parametrize("quantiles", ["mean", 0.5, [0.2, 0.5, 0.8]])
 @pytest.mark.parametrize("weighted_quantile", [True, False])
 @pytest.mark.parametrize("aggregate_leaves_first", [True, False])
 def test_predict_oob(
     name,
     quantiles,
     weighted_quantile,
     aggregate_leaves_first,
```

### Comparing `quantile-forest-1.1.3/quantile_forest.egg-info/PKG-INFO` & `quantile-forest-1.2.0/quantile_forest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantile-forest
-Version: 1.1.3
+Version: 1.2.0
 Summary: scikit-learn compatible quantile forests.
 Maintainer: Zillow Group AI Team
 License: Apache License 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python
@@ -29,15 +29,15 @@
 [![GitHub Actions](https://github.com/zillow/quantile-forest/actions/workflows/build.yml/badge.svg)](https://github.com/zillow/quantile-forest/actions/workflows/build.yml)
 [![Codecov](https://codecov.io/gh/zillow/quantile-forest/branch/main/graph/badge.svg?token=STRT8T67YP)](https://codecov.io/gh/zillow/quantile-forest)
 [![Code Style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/quantile-forest)](https://pypi.org/project/quantile-forest)
 
 **quantile-forest** offers a Python implementation of quantile regression forests compatible with scikit-learn.
 
-Quantile regression forests are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package extend the forest estimators available in scikit-learn to estimate conditional quantiles; they can estimate arbitrary quantiles at prediction time without retraining. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
+Quantile regression forests (QRF) are a non-parametric, tree-based ensemble method for estimating conditional quantiles, with application to high-dimensional data and uncertainty estimation [[1]](#1). The estimators in this package are performant, Cython-optimized QRF implementations that extend the forest estimators available in scikit-learn to estimate conditional quantiles. The estimators can estimate arbitrary quantiles at prediction time without retraining and provide methods for out-of-bag estimation, calculating quantile ranks, and computing proximity counts. They are compatible with and can serve as drop-in replacements for the scikit-learn variants.
 
 #### Example of fitted model predictions and prediction intervals on California housing data ([code](https://zillow.github.io/quantile-forest/auto_examples/plot_quantile_regression_intervals.html#sphx-glr-auto-examples-plot-quantile-regression-intervals-py))
 <img src="https://zillow.github.io/quantile-forest/_images/sphx_glr_plot_quantile_regression_intervals_001.png" height="300" />
 
 Quick Start
 -----------
```

### Comparing `quantile-forest-1.1.3/quantile_forest.egg-info/SOURCES.txt` & `quantile-forest-1.2.0/quantile_forest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/setup.cfg` & `quantile-forest-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `quantile-forest-1.1.3/setup.py` & `quantile-forest-1.2.0/setup.py`

 * *Files identical despite different names*


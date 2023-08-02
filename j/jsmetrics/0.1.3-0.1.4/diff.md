# Comparing `tmp/jsmetrics-0.1.3.tar.gz` & `tmp/jsmetrics-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsmetrics-0.1.3.tar", last modified: Fri Jul  7 08:35:47 2023, max compression
+gzip compressed data, was "jsmetrics-0.1.4.tar", last modified: Wed Aug  2 16:34:15 2023, max compression
```

## Comparing `jsmetrics-0.1.3.tar` & `jsmetrics-0.1.4.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    20782 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12891 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.353314 jsmetrics-0.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.349313 jsmetrics-0.1.3/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
--rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
--rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
--rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/_static/images/jet_shift_violin.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/statement.rst
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/core/check_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/details_for_all_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    26464 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms_components.py
--rw-r--r--   0 runner    (1001) docker     (123)    22927 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)    42237 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics_components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.361315 jsmetrics-0.1.3/jsmetrics/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/jsmetrics/utils/windspeed_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.357314 jsmetrics-0.1.3/jsmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20782 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-07 08:35:47.000000 jsmetrics-0.1.3/jsmetrics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.361315 jsmetrics-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.361315 jsmetrics-0.1.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
--rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/tests/metric_verification/
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/metric_verification/metric_verification.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 08:35:47.365315 jsmetrics-0.1.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_jet_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_jet_statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_spatial_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_waviness_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-07 08:35:44.000000 jsmetrics-0.1.3/tests/unit/test_windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.142871 jsmetrics-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7146 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-08-02 16:34:15.146872 jsmetrics-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13215 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.130871 jsmetrics-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.130871 jsmetrics-0.1.4/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.134871 jsmetrics-0.1.4/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)  1083764 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png
+-rw-r--r--   0 runner    (1001) docker     (123)   279496 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1519071 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png
+-rw-r--r--   0 runner    (1001) docker     (123)   788211 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/_static/images/jet_shift_violin.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     5634 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/statement.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.138871 jsmetrics-0.1.4/jsmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.138871 jsmetrics-0.1.4/jsmetrics/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/core/check_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12176 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/details_for_all_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.138871 jsmetrics-0.1.4/jsmetrics/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/jet_core_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26464 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/jet_core_algorithms_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27005 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42351 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/jet_statistics_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/metrics/waviness_metrics_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.138871 jsmetrics-0.1.4/jsmetrics/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9731 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/utils/spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/jsmetrics/utils/windspeed_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.138871 jsmetrics-0.1.4/jsmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21434 2023-08-02 16:34:15.000000 jsmetrics-0.1.4/jsmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-02 16:34:15.000000 jsmetrics-0.1.4/jsmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:34:15.000000 jsmetrics-0.1.4/jsmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:34:15.000000 jsmetrics-0.1.4/jsmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-02 16:34:15.000000 jsmetrics-0.1.4/jsmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-08-02 16:34:15.000000 jsmetrics-0.1.4/jsmetrics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-02 16:34:15.146872 jsmetrics-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.138871 jsmetrics-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.142871 jsmetrics-0.1.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1262096 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1260860 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+-rw-r--r--   0 runner    (1001) docker     (123)  1104721 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.142871 jsmetrics-0.1.4/tests/metric_verification/
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/metric_verification/metric_verification.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:34:15.142871 jsmetrics-0.1.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/test_jet_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14671 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/test_jet_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/test_spatial_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/test_waviness_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-08-02 16:34:12.000000 jsmetrics-0.1.4/tests/unit/test_windspeed_utils.py
```

### Comparing `jsmetrics-0.1.3/CONTRIBUTING.rst` & `jsmetrics-0.1.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/HISTORY.rst` & `jsmetrics-0.1.4/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 =======
 History
 =======
 
+0.1.4 (2023-08-02)
+-------------------------
+* Add new metric to package: Zappa et al. 2018 (This method builds on Ceppi et al. 2018)
+* Raise KeyError if no time coordinate is passed to a given metrics
+
+0.1.4-alpha (2023-07-21)
+-------------------------
+* add KeyError raise if no time coordinate is passed to various metrics
+
+
 0.1.3 (2023-07-07)
 -------------------------
 * Add "method='nearest'" to jet statistics and core algorithms for cases when coords cannot be represented within float precision range.
 
 0.1.2 (2023-06-06)
 -------------------------
 * Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data
```

### Comparing `jsmetrics-0.1.3/LICENSE` & `jsmetrics-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/PKG-INFO` & `jsmetrics-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -28,14 +28,15 @@
 ============================================
 jsmetrics: Jet-stream metrics and algorithms
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
 **preprint now available here: https://egusphere.copernicus.org/preprints/2023/egusphere-2023-661/**   
+**example notebooks: https://github.com/Thomasjkeel/jsmetrics-examples**
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
@@ -65,15 +66,15 @@
 
 Let me know if you have any problems installing this package, as I have not extensively tested for Mac-OS and Windows versions. 
     
 Documentation
 -------------
 The official documentation is at https://jsmetrics.readthedocs.io/en/latest/  
 
-My email is: thomas.keel.18@ucl.ac.uk
+My email is: thomas.keel.18@ucl.ac.uk. Please feel free to email me if you would like some help working with this package.
 
 Usage
 -------------
 .. code-block:: python
 
  import xarray as xr
  import jsmetrics
@@ -87,16 +88,18 @@
  print(w10['jet_lat'])
  print(w10['jet_speed'])
 
  # run Kuang et al. 2014 metric. NOTE: may take a long time after you have more than 50 time steps.
  k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
  print(k14['jet_center'].sel(time=0))
 
-Gallery
+Examples
 -------------
+Some example notebooks are available here: https://github.com/Thomasjkeel/jsmetrics-examples
+
 .. image:: docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
   :width: 560
   :align: center
   :alt: Jet latitude circbars with errorbars
 
 *Estimation of North Pacific mean jet latitude by month with 1-stdev errorbars. Data is monthly ERA5 700-850 hPa u-wind between 1980-2020.*
 
@@ -154,20 +157,20 @@
    `Manney et al. 2011 <https://acp.copernicus.org/articles/11/6115/2011/>`_       In progess*         `Allen et al. 2012 <http://www.nature.com/articles/nature11097>`_               To start
    `Barnes & Polvani 2013 <https://doi.org/10.1175/JCLI-D-12-00536.1>`_            To verify           `Pena-Ortiz et al. 2013 <http://doi.wiley.com/10.1002/jgrd.50305>`_             To verify      
    `Screen & Simmonds 2013 <http://doi.wiley.com/10.1002/grl.50174>`_              In progress*        `Kuang et al. 2014 <http://link.springer.com/10.1007/s00704-013-0994-x>`_       To verify            
    `Barnes & Polvani 2015 <https://doi.org/10.1175/JCLI-D-14-00589.1>`_            To verify           `Francis & Vavrus 2015 <https://doi.org/10.1088/1748-9326/10/1/014005>`_        Complete            
    `Cattiaux et al. 2016 <https://doi.wiley.com/10.1002/2016GL070309>`_            To verify           `Barnes & Simpson 2017 <https://doi.org/10.1175/JCLI-D-17-0299.1>`_             Complete            
    `Chenoli et al. 2017 <http://link.springer.com/10.1007/s00382-016-3102-y>`_     In progress         `Grise & Polvani 2017 <https://doi.org/10.1175/JCLI-D-16-0849.1>`_              Complete                        
    `Molnos et al. 2017  <https://doi.org/10.5194/esd-8-75-2017>`_                  In progress*        `Adam et al. 2018 <https://doi.org/10.5194/gmd-11-4339-2018>`_                  To start            
-   `Bracegirdle et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0320.1>`_           Complete            `Ceppi et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0323.1>`_                 To verify            
+   `Bracegirdle et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0320.1>`_           Complete            `Ceppi et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0323.1>`_                 Complete            
    `Kern et al. 2018 <http://ieeexplore.ieee.org/document/8017585/>`_              To start*           `Rikus 2018 <http://dx.doi.org/10.1007/s00382-015-2560-y>`_                     In progress            
-   `Kern & Westermann 2019 <https://doi.org/10.2312/vmv.20191321>`_                To start            `Kerr et al. 2020 <https://doi.org/10.1029/2020JD032735>`_                      To verify            
-   `Maher et al. 2020 <https://doi.org/10.1007/s00382-019-05084-6>`_               To start            `Winters et al. 2020 <https://doi.org/10.1175/MWR-D-19-0353.1>`_                To start            
-   `Martin 2021 <https://onlinelibrary.wiley.com/doi/10.1029/2020JD033668>`_       To start*           `Bosiger et al. 2022 <https://doi.org/10.5194/gmd-15-1079-2022>`_               To start            
-   `Local Wave Activity <https://doi.org/10.1175/JAS-D-15-0194.1>`_                In progress*                        
+   `Zappa et al. 2018 <https://doi.org/10.1029/2019GL083653>`_                     Complete            `Kern & Westermann 2019 <https://doi.org/10.2312/vmv.20191321>`_                To start
+   `Kerr et al. 2020 <https://doi.org/10.1029/2020JD032735>`_                      To verify           `Maher et al. 2020 <https://doi.org/10.1007/s00382-019-05084-6>`_               To start
+   `Winters et al. 2020 <https://doi.org/10.1175/MWR-D-19-0353.1>`_                To start            `Martin 2021 <https://onlinelibrary.wiley.com/doi/10.1029/2020JD033668>`_       To start*        
+   `Bosiger et al. 2022 <https://doi.org/10.5194/gmd-15-1079-2022>`_               To start            `Local Wave Activity <https://doi.org/10.1175/JAS-D-15-0194.1>`_                In progress*                        
    =============================================================================== ==============  ==  =============================================================================== ==============
 
 * == help needed
 
 .. _all metrics: https://github.com/Thomasjkeel/jsmetrics/blob/main/details_for_all_metrics.py
 .. _Status: https://github.com/Thomasjkeel/jsmetrics/projects/1
 
@@ -228,16 +231,16 @@
 .. |codefactor| image:: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics/badge
    :target: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics
    :alt: CodeFactor
    
 .. |coveralls| image:: https://coveralls.io/repos/github/Thomasjkeel/jsmetrics/badge.svg?branch=main
    :target: https://coveralls.io/github/Thomasjkeel/jsmetrics?branch=main
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7974550.svg
-        :target:  https://doi.org/10.5281/zenodo.7974550
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8123560.svg
+        :target:  https://doi.org/10.5281/zenodo.8123560
         :alt: DOI
 .. |docs| image:: https://readthedocs.org/projects/jsmetrics/badge/?version=latest
        :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status
 .. |pypi| image:: https://img.shields.io/pypi/v/jsmetrics.svg
         :target: https://pypi.org/project/jsmetrics/
         :alt: Python Package Index Build
@@ -247,14 +250,24 @@
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+0.1.4 (2023-08-02)
+-------------------------
+* Add new metric to package: Zappa et al. 2018 (This method builds on Ceppi et al. 2018)
+* Raise KeyError if no time coordinate is passed to a given metrics
+
+0.1.4-alpha (2023-07-21)
+-------------------------
+* add KeyError raise if no time coordinate is passed to various metrics
+
+
 0.1.3 (2023-07-07)
 -------------------------
 * Add "method='nearest'" to jet statistics and core algorithms for cases when coords cannot be represented within float precision range.
 
 0.1.2 (2023-06-06)
 -------------------------
 * Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data
```

### Comparing `jsmetrics-0.1.3/README.rst` & `jsmetrics-0.1.4/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ============================================
 jsmetrics: Jet-stream metrics and algorithms
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
 **preprint now available here: https://egusphere.copernicus.org/preprints/2023/egusphere-2023-661/**   
+**example notebooks: https://github.com/Thomasjkeel/jsmetrics-examples**
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
@@ -38,15 +39,15 @@
 
 Let me know if you have any problems installing this package, as I have not extensively tested for Mac-OS and Windows versions. 
     
 Documentation
 -------------
 The official documentation is at https://jsmetrics.readthedocs.io/en/latest/  
 
-My email is: thomas.keel.18@ucl.ac.uk
+My email is: thomas.keel.18@ucl.ac.uk. Please feel free to email me if you would like some help working with this package.
 
 Usage
 -------------
 .. code-block:: python
 
  import xarray as xr
  import jsmetrics
@@ -60,16 +61,18 @@
  print(w10['jet_lat'])
  print(w10['jet_speed'])
 
  # run Kuang et al. 2014 metric. NOTE: may take a long time after you have more than 50 time steps.
  k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
  print(k14['jet_center'].sel(time=0))
 
-Gallery
+Examples
 -------------
+Some example notebooks are available here: https://github.com/Thomasjkeel/jsmetrics-examples
+
 .. image:: docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
   :width: 560
   :align: center
   :alt: Jet latitude circbars with errorbars
 
 *Estimation of North Pacific mean jet latitude by month with 1-stdev errorbars. Data is monthly ERA5 700-850 hPa u-wind between 1980-2020.*
 
@@ -127,20 +130,20 @@
    `Manney et al. 2011 <https://acp.copernicus.org/articles/11/6115/2011/>`_       In progess*         `Allen et al. 2012 <http://www.nature.com/articles/nature11097>`_               To start
    `Barnes & Polvani 2013 <https://doi.org/10.1175/JCLI-D-12-00536.1>`_            To verify           `Pena-Ortiz et al. 2013 <http://doi.wiley.com/10.1002/jgrd.50305>`_             To verify      
    `Screen & Simmonds 2013 <http://doi.wiley.com/10.1002/grl.50174>`_              In progress*        `Kuang et al. 2014 <http://link.springer.com/10.1007/s00704-013-0994-x>`_       To verify            
    `Barnes & Polvani 2015 <https://doi.org/10.1175/JCLI-D-14-00589.1>`_            To verify           `Francis & Vavrus 2015 <https://doi.org/10.1088/1748-9326/10/1/014005>`_        Complete            
    `Cattiaux et al. 2016 <https://doi.wiley.com/10.1002/2016GL070309>`_            To verify           `Barnes & Simpson 2017 <https://doi.org/10.1175/JCLI-D-17-0299.1>`_             Complete            
    `Chenoli et al. 2017 <http://link.springer.com/10.1007/s00382-016-3102-y>`_     In progress         `Grise & Polvani 2017 <https://doi.org/10.1175/JCLI-D-16-0849.1>`_              Complete                        
    `Molnos et al. 2017  <https://doi.org/10.5194/esd-8-75-2017>`_                  In progress*        `Adam et al. 2018 <https://doi.org/10.5194/gmd-11-4339-2018>`_                  To start            
-   `Bracegirdle et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0320.1>`_           Complete            `Ceppi et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0323.1>`_                 To verify            
+   `Bracegirdle et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0320.1>`_           Complete            `Ceppi et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0323.1>`_                 Complete            
    `Kern et al. 2018 <http://ieeexplore.ieee.org/document/8017585/>`_              To start*           `Rikus 2018 <http://dx.doi.org/10.1007/s00382-015-2560-y>`_                     In progress            
-   `Kern & Westermann 2019 <https://doi.org/10.2312/vmv.20191321>`_                To start            `Kerr et al. 2020 <https://doi.org/10.1029/2020JD032735>`_                      To verify            
-   `Maher et al. 2020 <https://doi.org/10.1007/s00382-019-05084-6>`_               To start            `Winters et al. 2020 <https://doi.org/10.1175/MWR-D-19-0353.1>`_                To start            
-   `Martin 2021 <https://onlinelibrary.wiley.com/doi/10.1029/2020JD033668>`_       To start*           `Bosiger et al. 2022 <https://doi.org/10.5194/gmd-15-1079-2022>`_               To start            
-   `Local Wave Activity <https://doi.org/10.1175/JAS-D-15-0194.1>`_                In progress*                        
+   `Zappa et al. 2018 <https://doi.org/10.1029/2019GL083653>`_                     Complete            `Kern & Westermann 2019 <https://doi.org/10.2312/vmv.20191321>`_                To start
+   `Kerr et al. 2020 <https://doi.org/10.1029/2020JD032735>`_                      To verify           `Maher et al. 2020 <https://doi.org/10.1007/s00382-019-05084-6>`_               To start
+   `Winters et al. 2020 <https://doi.org/10.1175/MWR-D-19-0353.1>`_                To start            `Martin 2021 <https://onlinelibrary.wiley.com/doi/10.1029/2020JD033668>`_       To start*        
+   `Bosiger et al. 2022 <https://doi.org/10.5194/gmd-15-1079-2022>`_               To start            `Local Wave Activity <https://doi.org/10.1175/JAS-D-15-0194.1>`_                In progress*                        
    =============================================================================== ==============  ==  =============================================================================== ==============
 
 * == help needed
 
 .. _all metrics: https://github.com/Thomasjkeel/jsmetrics/blob/main/details_for_all_metrics.py
 .. _Status: https://github.com/Thomasjkeel/jsmetrics/projects/1
 
@@ -201,16 +204,16 @@
 .. |codefactor| image:: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics/badge
    :target: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics
    :alt: CodeFactor
    
 .. |coveralls| image:: https://coveralls.io/repos/github/Thomasjkeel/jsmetrics/badge.svg?branch=main
    :target: https://coveralls.io/github/Thomasjkeel/jsmetrics?branch=main
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7974550.svg
-        :target:  https://doi.org/10.5281/zenodo.7974550
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8123560.svg
+        :target:  https://doi.org/10.5281/zenodo.8123560
         :alt: DOI
 .. |docs| image:: https://readthedocs.org/projects/jsmetrics/badge/?version=latest
        :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status
 .. |pypi| image:: https://img.shields.io/pypi/v/jsmetrics.svg
         :target: https://pypi.org/project/jsmetrics/
         :alt: Python Package Index Build
```

### Comparing `jsmetrics-0.1.3/docs/Makefile` & `jsmetrics-0.1.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png` & `jsmetrics-0.1.4/docs/_static/images/all_jet_lats_stj_pfj_npac_maps_more_metrics.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png` & `jsmetrics-0.1.4/docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png` & `jsmetrics-0.1.4/docs/_static/images/jet_core_algorithm_comparions_NA_5_texas2021.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/_static/images/jet_shift_violin.png` & `jsmetrics-0.1.4/docs/_static/images/jet_shift_violin.png`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/conf.py` & `jsmetrics-0.1.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/index.rst` & `jsmetrics-0.1.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/installation.rst` & `jsmetrics-0.1.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/make.bat` & `jsmetrics-0.1.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/docs/metrics.rst` & `jsmetrics-0.1.4/docs/metrics.rst`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics/core/check_data.py` & `jsmetrics-0.1.4/jsmetrics/core/check_data.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics/details_for_all_metrics.py` & `jsmetrics-0.1.4/jsmetrics/details_for_all_metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -253,14 +253,32 @@
     #     {"variables": ["ua", "va"], "coords":{"plev": [0, 100000]}, "plev_units": "Pa",
     #      "metric": jetstream_metrics.kern_et_al_2018,
     #      "description": "Kern 2018"},
     # "Rikus2018":
     #     {"variables": ["ua"], "coords":{"plev": [0, 100000]}, "plev_units": "Pa",
     #      "metric": jetstream_metrics.rikus_2018,
     #      "description": "Rikus 2018"},
+    "Zappa2018_NorthAtlantic": {
+        "variables": ["ua"],
+        "coords": {"plev": [85000, 85000], "lat": [20, 70], "lon": [300, 360]},
+        "plev_units": "Pa",
+        "metric": jet_statistics.zappa_et_al_2018,
+        "name": "Zappa et al. 2018 North Atlantic",
+        "description": "",
+        "doi": "10.1002/2017GL076096",
+    },
+    "Zappa2018_NorthPacific": {
+        "variables": ["ua"],
+        "coords": {"plev": [85000, 85000], "lat": [20, 70], "lon": [140, 240]},
+        "plev_units": "Pa",
+        "metric": jet_statistics.zappa_et_al_2018,
+        "name": "Zappa et al. 2018 North Pacific",
+        "description": "",
+        "doi": "10.1002/2017GL076096",
+    },
     "Kerr2020_NorthernHemisphere": {
         "variables": ["ua"],
         "coords": {"plev": [50000, 50000], "lat": [20, 70]},
         "plev_units": "Pa",
         "metric": jet_statistics.kerr_et_al_2020,
         "name": "Kerr et al. 2020",
         "description": "",
```

### Comparing `jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms.py` & `jsmetrics-0.1.4/jsmetrics/metrics/jet_core_algorithms.py`

 * *Files 6% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     output : xr.Dataset
         Data with local jet maximas
     """
     #  Step 1. Calculate wind vector
     data["ws"] = windspeed_utils.get_resultant_wind(data["ua"], data["va"])
 
     #  Step 2. Calculate jet maximas
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         output = jet_core_algorithms_components.get_local_jet_maximas_by_oneday_by_plev(
             data
         )
     else:
         output = data.groupby("time").map(
             jet_core_algorithms_components.get_local_jet_maximas_by_oneday_by_plev
@@ -129,14 +131,16 @@
     output : xarray.Dataset
         Data containing jet-cores (ID number relates to each unique core)
     """
     if "plev" not in data.dims:
         data = data.expand_dims("plev")
 
     # Step 1. Run Jet-stream Core Idenfication Algorithm
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         if "time" in data.dims:
             data = data.isel(time=0)
         output = jet_core_algorithms_components.run_jet_core_algorithm_on_one_day(
             data, ws_core_threshold, ws_boundary_threshold
         )
     else:
@@ -169,14 +173,16 @@
     output : xarray.Dataset
         Data containing number of days per month with local wind maxima
     """
     #  Step 1. Calculate wind vector
     data["ws"] = windspeed_utils.get_resultant_wind(data["ua"], data["va"])
 
     #  Step 2. Make array of zeros for local wind maxima location algorithm
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1 and "time" not in data.dims:
         data = data.expand_dims("time")
     output = jet_core_algorithms_components.get_empty_local_wind_maxima_data(data)
 
     #  Step 3. Find local wind maxima locations by day
     output = output.groupby("time").map(
         jet_core_algorithms_components.get_local_wind_maxima_by_timeunit
```

### Comparing `jsmetrics-0.1.3/jsmetrics/metrics/jet_core_algorithms_components.py` & `jsmetrics-0.1.4/jsmetrics/metrics/jet_core_algorithms_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics.py` & `jsmetrics-0.1.4/jsmetrics/metrics/jet_statistics.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
     Returns
     ----------
     output : xarray.Dataset
         Data containing mass weighted average ws, mass flux weighted pressure and latitude
     """
     #  Step 1. Get monthly means
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         print(
             "Warning: only found one time step, and the time coord is being renamed month."
         )
         mon_mean = data.assign_coords(month=data["time"].dt.month)
         mon_mean = mon_mean.expand_dims("month")
     else:
@@ -308,14 +310,16 @@
             data = data.isel(plev=0)
         else:
             print(
                 "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
             )
             data = data.mean("plev")
     data = data.mean("lon")
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1 and "time" not in data.dims:
         data = data.expand_dims("time")
     if not data.indexes["time"].is_monotonic_increasing:
         raise IndexError("Data needs to have a montonic increasing index")
     # Check that data can be resampled into 10 days
     if not data["time"].size == 1:
         time_step_in_data = int((data["time"][1] - data["time"][0]).dt.days)
@@ -352,14 +356,16 @@
     output : xarray.Dataset
         Data containing max latitudes per time unit scaled to 0.01 resolution
     """
     if isinstance(data, xarray.DataArray):
         data = data.to_dataset()
 
     # Step 0: Expand time dimensions so we can map a function to the dataset properly
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         data = data.expand_dims("time")
 
     # Step 1. Calculate zonal-mean
     zonal_mean = windspeed_utils.get_zonal_mean(data)
 
     # Step 2. Get the 3 latitudes and speeds around max zonal wind-speed (e.g. lat-1, lat, lat+1)
@@ -435,14 +441,16 @@
             print(
                 "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
             )
             data = data.mean("plev")
             # raise ValueError("Please subset to one plev value for this metric")
 
     # Step 0: Expand time dimensions so we can map a function to the dataset properly
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         data = data.expand_dims("time")
 
     #  Step 1. Make seasonal & annual climatologies
     seasonal_climatology = jet_statistics_components.get_climatology(data, "season")
     annual_climatology = jet_statistics_components.get_climatology(data, "year")
 
@@ -479,15 +487,15 @@
 @sort_xarray_data_coords(coords=["lat", "lon"])
 def ceppi_et_al_2018(data, lon_resolution=None):
     """
     Calculates the jet latitude per time unit where jet-lat is defined as a centroid of a zonal wind distribution.
     This method has been slightly adapted to include a jet speed extraction (after Screen et al. 2022 and refs therein).
     Method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1
 
-    Also used in Zappa et al. 2018, Ayres & Screen, 2019 and Screen et al. 2022. Similar methods used in: Chen et al. 2008; Ceppi et al. 2014.
+    Also see Zappa et al. 2018 method which includes exclusion of <0 m/s u-wind
 
     Parameters
     ----------
     data : xarray.Dataset
         Data containing u-component windspeed
     lon_resolution : numeric
         Resolution to use for longitude coord if size 1
@@ -519,14 +527,100 @@
 
     # Step 3: Assign laitude of jet-stream centroids to main data
     data["jet_lat"] = jet_statistics_components.calc_centroid_jet_lat_from_zonal_mean(
         zonal_mean, area_by_lat=zonal_mean["total_area_m2"]
     )
 
     # Expand time dimension
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
+    if data["time"].size == 1:
+        data = data.expand_dims("time")
+        zonal_mean = zonal_mean.expand_dims("time")
+
+    # Step 4 (adapted from original methodology): Get nearest latitude actually in data to the one determined by metric
+    nearest_latitudes_to_jet_lat_estimates = np.array(
+        list(
+            map(
+                lambda row: data_utils.find_nearest_value_to_array(
+                    data["lat"], float(row)
+                ),
+                data["jet_lat"],
+            )
+        )
+    )
+
+    # Step 5 (adapted from original methodology): Get speed of associated nearest latitude
+    data["jet_speed"] = (
+        ("time",),
+        np.array(
+            list(
+                map(
+                    lambda data_row, lat_val: jet_statistics_components.get_latitude_value_in_data_row(
+                        data_row, lat_val
+                    ),
+                    zonal_mean["ua"],
+                    nearest_latitudes_to_jet_lat_estimates,
+                )
+            )
+        ),
+    )
+    return data
+
+
+def zappa_et_al_2018(data, lon_resolution=None):
+    """
+    Calculates the jet latitude per time unit where jet-lat is defined as a centroid of a zonal wind distribution.
+    This method has been slightly adapted to include a jet speed extraction (after Screen et al. 2022 and refs therein).
+    Method from Zappa et al. 2018 https://doi.org/10.1029/2019GL083653
+    Adapted from and very similar to Ceppi et al (2018).
+
+    Also used in Ayres & Screen, 2019 and Screen et al. 2022. Similar methods used in: Chen et al. 2008; Ceppi et al. 2014, Ceppi et al. 2018.
+
+    Parameters
+    ----------
+    data : xarray.Dataset
+        Data containing u-component windspeed
+    lon_resolution : numeric
+        Resolution to use for longitude coord if size 1
+
+    Returns
+    ----------
+    output : xarray.Dataset
+        Data containing centroid latitude of u-wind for each time unit (e.g. each day)
+    """
+    #  Step 1. Get area in m2 by latitude/longitude grid cells
+    if not data["lon"].size == 1 and not data["lat"].size == 1:
+        total_area_m2 = spatial_utils.grid_cell_areas(data["lon"], data["lat"])
+    elif lon_resolution and not data["lat"].size == 1 and data["lon"].size == 1:
+        lons_to_use = [float(data["lon"]), float(data["lon"]) + lon_resolution]
+        total_area_m2 = spatial_utils.grid_cell_areas(lons_to_use, data["lat"])
+        total_area_m2 = total_area_m2.mean(axis=1)
+        total_area_m2 = total_area_m2.reshape(-1, 1)
+        if data["lon"].shape == ():
+            data = data.expand_dims("lon")
+    else:
+        raise ValueError(
+            "For this method, your data needs to have at least 2 'lat' values and 'lon' values needs to be more than one unless you set the 'lon_resolution' parameter"
+        )
+
+    data["total_area_m2"] = (("lat", "lon"), total_area_m2)
+
+    #  Step 2. calculate zonal mean and floor ua values to 0
+    zonal_mean = windspeed_utils.get_zonal_mean(data)
+    zonal_mean["ua"] = zonal_mean["ua"].where(lambda x: x > 0, 0)
+
+    # Step 3: Assign laitude of jet-stream centroids to main data
+    data["jet_lat"] = jet_statistics_components.calc_centroid_jet_lat_from_zonal_mean(
+        zonal_mean, area_by_lat=zonal_mean["total_area_m2"]
+    )
+
+    # Expand time dimension
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         data = data.expand_dims("time")
         zonal_mean = zonal_mean.expand_dims("time")
 
     # Step 4 (adapted from original methodology): Get nearest latitude actually in data to the one determined by metric
     nearest_latitudes_to_jet_lat_estimates = np.array(
         list(
@@ -580,16 +674,17 @@
             data = data.isel(plev=0)
         else:
             print(
                 "this metric was meant to only work on one plev, please subset plev to one value. For now taking the mean..."
             )
             data = data.mean("plev")
             # raise ValueError("Please subset to one plev value for this metric")
-
-    if data["time"].size == 1:
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
+    elif data["time"].size == 1:
         output = (
             jet_statistics_components.get_moving_averaged_smoothed_jet_lats_for_one_day(
                 data, width_of_pulse
             )
         )
     else:
         output = data.groupby("time").map(
```

### Comparing `jsmetrics-0.1.3/jsmetrics/metrics/jet_statistics_components.py` & `jsmetrics-0.1.4/jsmetrics/metrics/jet_statistics_components.py`

 * *Files 0% similar despite different names*

```diff
@@ -1166,15 +1166,15 @@
 
 
 def calc_centroid_jet_lat_from_zonal_mean(zonal_mean, area_by_lat):
     """
     Will get the centroid latitude of the u-component wind using:
     jet_lat = integral(60deg, 30deg)(zonal_u**2*lat) dlat / integral(60deg, 30deg)(zonal_u**2) dlat
 
-    Component of method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1
+    Component of method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1 & Zappa et al. 2018 https://doi.org/10.1029/2019GL083653
 
     Parameters
     ----------
     zonal_mean : xarray.Dataset
         zonally-average data containing u-component wind data
     area_by_lat : xarray.DataArray
         Information on area in each latitude (i.e. m2 per latitude)
@@ -1184,15 +1184,15 @@
     return u_hat_by_lat.sum("lat") / u_hat.sum("lat")
 
 
 def get_latitude_value_in_data_row(data_row, lat_val):
     """
     Will return the latitude value of a given data row. Needed to loop through data and external array
 
-    Component of method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1
+    Component of method from Ceppi et al (2018) https://doi.org/10.1175/JCLI-D-17-0323.1 & Zappa et al. 2018 https://doi.org/10.1029/2019GL083653
 
     Parameters
     ----------
     data_row : xarray.DataArray
         Data row to extract variable from using given latitude
     lat_val : float or int
         latitude value to extract from data row
```

### Comparing `jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics.py` & `jsmetrics-0.1.4/jsmetrics/metrics/waviness_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,14 +100,16 @@
     data : xarray.Dataset
         Data containing sinuosity of zonal mean by each time unit
     """
     if isinstance(data, xarray.DataArray):
         data = data.to_dataset()
 
     #  Step 1. get zonal average for each timestep
+    if "time" not in data.coords:
+        raise KeyError("Please provide a time coordinate for data to run this metric")
     if data["time"].size == 1:
         data = data.expand_dims("time")
     data["zonal_mean_zg_30Nto70N"] = (
         data["zg"].sel(lat=slice(30, 70)).groupby("time").mean(...)
     )
 
     #  Step 2. Get latitude circle of 50 N
```

### Comparing `jsmetrics-0.1.3/jsmetrics/metrics/waviness_metrics_components.py` & `jsmetrics-0.1.4/jsmetrics/metrics/waviness_metrics_components.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics/utils/data_utils.py` & `jsmetrics-0.1.4/jsmetrics/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics/utils/spatial_utils.py` & `jsmetrics-0.1.4/jsmetrics/utils/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics/utils/windspeed_utils.py` & `jsmetrics-0.1.4/jsmetrics/utils/windspeed_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/jsmetrics.egg-info/PKG-INFO` & `jsmetrics-0.1.4/jsmetrics.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsmetrics
-Version: 0.1.3
+Version: 0.1.4
 Summary: Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray.
 Home-page: https://github.com/Thomasjkeel/jsmetrics
 Author: Thomas Keel
 Author-email: thomas.keel.18@ucl.ac.uk
 License: MIT License
 Keywords: jet-stream climate metrics algorithms xarray
 Platform: UNKNOWN
@@ -28,14 +28,15 @@
 ============================================
 jsmetrics: Jet-stream metrics and algorithms
 ============================================
 
 |pypi| |pre-commit| |codefactor| |coveralls| |docs| |license| |black| |zenodo|  
 ------------------------------------------------------------------------------
 **preprint now available here: https://egusphere.copernicus.org/preprints/2023/egusphere-2023-661/**   
+**example notebooks: https://github.com/Thomasjkeel/jsmetrics-examples**
 
 This is jsmetrics, a package containing implementations of various metrics and algorithms for identifying or characterising jet-streams
 written in Python and built from xarray.
 
 .. WRITE WHY JET-STREAM (maybe in blog, maybe in readme) -> heatwaves, beast from the east, climate proxy (put it all down)
 .. At the foundation of studies that look at jet-streams is the metric used to describe or characterise it.
 
@@ -65,15 +66,15 @@
 
 Let me know if you have any problems installing this package, as I have not extensively tested for Mac-OS and Windows versions. 
     
 Documentation
 -------------
 The official documentation is at https://jsmetrics.readthedocs.io/en/latest/  
 
-My email is: thomas.keel.18@ucl.ac.uk
+My email is: thomas.keel.18@ucl.ac.uk. Please feel free to email me if you would like some help working with this package.
 
 Usage
 -------------
 .. code-block:: python
 
  import xarray as xr
  import jsmetrics
@@ -87,16 +88,18 @@
  print(w10['jet_lat'])
  print(w10['jet_speed'])
 
  # run Kuang et al. 2014 metric. NOTE: may take a long time after you have more than 50 time steps.
  k14 = jsmetrics.jet_core_algorithms.kuang_et_al_2014(uv_data)
  print(k14['jet_center'].sel(time=0))
 
-Gallery
+Examples
 -------------
+Some example notebooks are available here: https://github.com/Thomasjkeel/jsmetrics-examples
+
 .. image:: docs/_static/images/all_metrics_jetlat_circbar_w_errorbars.png
   :width: 560
   :align: center
   :alt: Jet latitude circbars with errorbars
 
 *Estimation of North Pacific mean jet latitude by month with 1-stdev errorbars. Data is monthly ERA5 700-850 hPa u-wind between 1980-2020.*
 
@@ -154,20 +157,20 @@
    `Manney et al. 2011 <https://acp.copernicus.org/articles/11/6115/2011/>`_       In progess*         `Allen et al. 2012 <http://www.nature.com/articles/nature11097>`_               To start
    `Barnes & Polvani 2013 <https://doi.org/10.1175/JCLI-D-12-00536.1>`_            To verify           `Pena-Ortiz et al. 2013 <http://doi.wiley.com/10.1002/jgrd.50305>`_             To verify      
    `Screen & Simmonds 2013 <http://doi.wiley.com/10.1002/grl.50174>`_              In progress*        `Kuang et al. 2014 <http://link.springer.com/10.1007/s00704-013-0994-x>`_       To verify            
    `Barnes & Polvani 2015 <https://doi.org/10.1175/JCLI-D-14-00589.1>`_            To verify           `Francis & Vavrus 2015 <https://doi.org/10.1088/1748-9326/10/1/014005>`_        Complete            
    `Cattiaux et al. 2016 <https://doi.wiley.com/10.1002/2016GL070309>`_            To verify           `Barnes & Simpson 2017 <https://doi.org/10.1175/JCLI-D-17-0299.1>`_             Complete            
    `Chenoli et al. 2017 <http://link.springer.com/10.1007/s00382-016-3102-y>`_     In progress         `Grise & Polvani 2017 <https://doi.org/10.1175/JCLI-D-16-0849.1>`_              Complete                        
    `Molnos et al. 2017  <https://doi.org/10.5194/esd-8-75-2017>`_                  In progress*        `Adam et al. 2018 <https://doi.org/10.5194/gmd-11-4339-2018>`_                  To start            
-   `Bracegirdle et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0320.1>`_           Complete            `Ceppi et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0323.1>`_                 To verify            
+   `Bracegirdle et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0320.1>`_           Complete            `Ceppi et al. 2018 <https://doi.org/10.1175/JCLI-D-17-0323.1>`_                 Complete            
    `Kern et al. 2018 <http://ieeexplore.ieee.org/document/8017585/>`_              To start*           `Rikus 2018 <http://dx.doi.org/10.1007/s00382-015-2560-y>`_                     In progress            
-   `Kern & Westermann 2019 <https://doi.org/10.2312/vmv.20191321>`_                To start            `Kerr et al. 2020 <https://doi.org/10.1029/2020JD032735>`_                      To verify            
-   `Maher et al. 2020 <https://doi.org/10.1007/s00382-019-05084-6>`_               To start            `Winters et al. 2020 <https://doi.org/10.1175/MWR-D-19-0353.1>`_                To start            
-   `Martin 2021 <https://onlinelibrary.wiley.com/doi/10.1029/2020JD033668>`_       To start*           `Bosiger et al. 2022 <https://doi.org/10.5194/gmd-15-1079-2022>`_               To start            
-   `Local Wave Activity <https://doi.org/10.1175/JAS-D-15-0194.1>`_                In progress*                        
+   `Zappa et al. 2018 <https://doi.org/10.1029/2019GL083653>`_                     Complete            `Kern & Westermann 2019 <https://doi.org/10.2312/vmv.20191321>`_                To start
+   `Kerr et al. 2020 <https://doi.org/10.1029/2020JD032735>`_                      To verify           `Maher et al. 2020 <https://doi.org/10.1007/s00382-019-05084-6>`_               To start
+   `Winters et al. 2020 <https://doi.org/10.1175/MWR-D-19-0353.1>`_                To start            `Martin 2021 <https://onlinelibrary.wiley.com/doi/10.1029/2020JD033668>`_       To start*        
+   `Bosiger et al. 2022 <https://doi.org/10.5194/gmd-15-1079-2022>`_               To start            `Local Wave Activity <https://doi.org/10.1175/JAS-D-15-0194.1>`_                In progress*                        
    =============================================================================== ==============  ==  =============================================================================== ==============
 
 * == help needed
 
 .. _all metrics: https://github.com/Thomasjkeel/jsmetrics/blob/main/details_for_all_metrics.py
 .. _Status: https://github.com/Thomasjkeel/jsmetrics/projects/1
 
@@ -228,16 +231,16 @@
 .. |codefactor| image:: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics/badge
    :target: https://www.codefactor.io/repository/github/thomasjkeel/jsmetrics
    :alt: CodeFactor
    
 .. |coveralls| image:: https://coveralls.io/repos/github/Thomasjkeel/jsmetrics/badge.svg?branch=main
    :target: https://coveralls.io/github/Thomasjkeel/jsmetrics?branch=main
 
-.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7974550.svg
-        :target:  https://doi.org/10.5281/zenodo.7974550
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.8123560.svg
+        :target:  https://doi.org/10.5281/zenodo.8123560
         :alt: DOI
 .. |docs| image:: https://readthedocs.org/projects/jsmetrics/badge/?version=latest
        :target: https://jsmetrics.readthedocs.io/en/latest/?badge=latest
        :alt: Documentation Status
 .. |pypi| image:: https://img.shields.io/pypi/v/jsmetrics.svg
         :target: https://pypi.org/project/jsmetrics/
         :alt: Python Package Index Build
@@ -247,14 +250,24 @@
 ..         :alt: Conda-forge Build Version
 
 
 =======
 History
 =======
 
+0.1.4 (2023-08-02)
+-------------------------
+* Add new metric to package: Zappa et al. 2018 (This method builds on Ceppi et al. 2018)
+* Raise KeyError if no time coordinate is passed to a given metrics
+
+0.1.4-alpha (2023-07-21)
+-------------------------
+* add KeyError raise if no time coordinate is passed to various metrics
+
+
 0.1.3 (2023-07-07)
 -------------------------
 * Add "method='nearest'" to jet statistics and core algorithms for cases when coords cannot be represented within float precision range.
 
 0.1.2 (2023-06-06)
 -------------------------
 * Fix  Barnes & Polvani 2013 to better deal when min max jet lat is at edge data
```

### Comparing `jsmetrics-0.1.3/jsmetrics.egg-info/SOURCES.txt` & `jsmetrics-0.1.4/jsmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/setup.cfg` & `jsmetrics-0.1.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.1.3
+current_version = 0.1.4
 commit = True
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+).(?P<patch>\d+)(\-(?P<release>[a-z]+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}
 	{major}.{minor}.{patch}
```

### Comparing `jsmetrics-0.1.3/setup.py` & `jsmetrics-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 NAME = "jsmetrics"
 DESCRIPTION = "Library of algorithms and metrics used to characterise and/or identify jet-streams, based on xarray."
 URL = "https://github.com/Thomasjkeel/jsmetrics"
 AUTHOR = "Thomas Keel"
 AUTHOR_EMAIL = "thomas.keel.18@ucl.ac.uk"
 REQUIRES_PYTHON = ">=3.7.0"
-VERSION = "0.1.3"
+VERSION = "0.1.4"
 LICENSE = "MIT License"
 
 KEYWORDS = "jet-stream climate metrics algorithms xarray"
 
 with open("README.rst") as file:
     readme = file.read()
```

### Comparing `jsmetrics-0.1.3/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.4/tests/data/ua_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.4/tests/data/va_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc` & `jsmetrics-0.1.4/tests/data/zg_day_UKESM1-0-LL_ssp585_r2i1p1f2_gn_20150101-20150105.nc`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/metric_verification/metric_verification.ipynb` & `jsmetrics-0.1.4/tests/metric_verification/metric_verification.ipynb`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/unit/__init__.py` & `jsmetrics-0.1.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/unit/test_data_utils.py` & `jsmetrics-0.1.4/tests/unit/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/unit/test_jet_algorithms.py` & `jsmetrics-0.1.4/tests/unit/test_jet_algorithms.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/unit/test_jet_statistics.py` & `jsmetrics-0.1.4/tests/unit/test_jet_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -290,14 +290,30 @@
         result = jet_statistics.grise_polvani_2017(self.data)
         jet_statistics.grise_polvani_2017(self.data["ua"])
         self.assertEqual(float(result["jet_lat"].min()), 35.38)
         self.assertEqual(float(result["jet_lat"].max()), 36.41)
         self.assertEqual(round(float(result["jet_speed"].max()), 5), 22.92644)
 
 
+class TestBracegirdle2018(unittest.TestCase):
+    def setUp(self):
+        self.data = set_up_test_u_data()
+
+    def test_metric(self):
+        tested_func = jet_statistics.bracegirdle_et_al_2018
+        test_data = self.data.sel(plev=slice(85000, 85000))
+        result = tested_func(test_data)
+        tested_func(test_data["ua"])
+        # self.assertRaises(ValueError, lambda: tested_func(self.data))
+        self.assertEqual(float(result["seasonal_JPOS"].max()), 37.725)
+        self.assertEqual(float(result["annual_JPOS"].max()), 37.725)
+        self.assertEqual(round(float(result["seasonal_JSTR"].max()), 3), 8.589)
+        self.assertEqual(round(float(result["annual_JSTR"].max()), 3), 8.589)
+
+
 class TestCeppi2018(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
         tested_func = jet_statistics.ceppi_et_al_2018
         result = tested_func(self.data)
@@ -320,28 +336,42 @@
             ValueError,
             lambda: tested_func(
                 self.data.sel(lon=slice(0, 0), lat=slice(0, 0)), lon_resolution=1.875
             ),
         )
 
 
-class TestBracegirdle2018(unittest.TestCase):
+class TestZappa2018(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_u_data()
 
     def test_metric(self):
-        tested_func = jet_statistics.bracegirdle_et_al_2018
-        test_data = self.data.sel(plev=slice(85000, 85000))
-        result = tested_func(test_data)
-        tested_func(test_data["ua"])
-        # self.assertRaises(ValueError, lambda: tested_func(self.data))
-        self.assertEqual(float(result["seasonal_JPOS"].max()), 37.725)
-        self.assertEqual(float(result["annual_JPOS"].max()), 37.725)
-        self.assertEqual(round(float(result["seasonal_JSTR"].max()), 3), 8.589)
-        self.assertEqual(round(float(result["annual_JSTR"].max()), 3), 8.589)
+        tested_func = jet_statistics.zappa_et_al_2018
+        result = tested_func(self.data)
+        self.assertEqual(round(float(result["jet_lat"][0].data), 3), 37.943)
+        self.assertEqual(round(float(result["jet_speed"][0].data), 3), 22.341)
+
+    def test_one_latlon_coord(self):
+        tested_func = jet_statistics.zappa_et_al_2018
+        self.assertRaises(ValueError, lambda: tested_func(self.data.isel(lon=0)))
+        self.assertRaises(ValueError, lambda: tested_func(self.data.isel(lat=0)))
+        self.assertRaises(
+            ValueError, lambda: tested_func(self.data.sel(lat=slice(0, 0)))
+        )
+        self.assertRaises(
+            ValueError, lambda: tested_func(self.data.sel(lon=slice(0, 0)))
+        )
+        tested_func(self.data.sel(lon=slice(0, 0)), lon_resolution=1.875)
+        tested_func(self.data.sel(lon=0), lon_resolution=1.875)
+        self.assertRaises(
+            ValueError,
+            lambda: tested_func(
+                self.data.sel(lon=slice(0, 0), lat=slice(0, 0)), lon_resolution=1.875
+            ),
+        )
 
 
 class TestKerr2020(unittest.TestCase):
     def setUp(self):
         self.data = set_up_test_uv_data()
 
     def test_metric(self):
```

### Comparing `jsmetrics-0.1.3/tests/unit/test_spatial_utils.py` & `jsmetrics-0.1.4/tests/unit/test_spatial_utils.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/unit/test_waviness_metrics.py` & `jsmetrics-0.1.4/tests/unit/test_waviness_metrics.py`

 * *Files identical despite different names*

### Comparing `jsmetrics-0.1.3/tests/unit/test_windspeed_utils.py` & `jsmetrics-0.1.4/tests/unit/test_windspeed_utils.py`

 * *Files identical despite different names*


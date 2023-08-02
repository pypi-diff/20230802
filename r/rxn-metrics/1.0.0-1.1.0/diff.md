# Comparing `tmp/rxn-metrics-1.0.0.tar.gz` & `tmp/rxn-metrics-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rxn-metrics-1.0.0.tar", last modified: Fri Feb 24 09:25:26 2023, max compression
+gzip compressed data, was "rxn-metrics-1.1.0.tar", last modified: Wed Aug  2 13:00:20 2023, max compression
```

## Comparing `rxn-metrics-1.0.0.tar` & `rxn-metrics-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.676730 rxn-metrics-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-24 09:25:26.676730 rxn-metrics-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-24 09:25:26.676730 rxn-metrics-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.672729 rxn-metrics-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.668729 rxn-metrics-1.0.0/src/rxn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.672729 rxn-metrics-1.0.0/src/rxn/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/classification_translation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/context_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/forward_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/metrics_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3057 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/metrics_files.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/retro_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/run_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.672729 rxn-metrics-1.0.0/src/rxn/metrics/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/ensure_data_dimension.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/join_data_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/parse_metrics_into_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/prepare_context_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/prepare_forward_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/prepare_retro_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/reorder_retro_predictions_class_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/scripts/rxn_evaluate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/tokenize_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/src/rxn/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.672729 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-24 09:25:26.000000 rxn-metrics-1.0.0/src/rxn_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 09:25:26.676730 rxn-metrics-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/tests/test_context_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-02-24 09:25:15.000000 rxn-metrics-1.0.0/tests/test_tokenize_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.037457 rxn-metrics-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-02 13:00:20.037457 rxn-metrics-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-08-02 13:00:20.041457 rxn-metrics-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.025457 rxn-metrics-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.025457 rxn-metrics-1.1.0/src/rxn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.033456 rxn-metrics-1.1.0/src/rxn/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/class_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/classification_translation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/context_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/forward_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/metrics_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/metrics_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5650 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/retro_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/run_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.037457 rxn-metrics-1.1.0/src/rxn/metrics/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/ensure_data_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/join_data_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/parse_metrics_into_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/prepare_context_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/prepare_forward_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/prepare_retro_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/reorder_retro_predictions_class_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/scripts/rxn_evaluate_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/tokenize_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/true_reactant_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/src/rxn/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.037457 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-08-02 13:00:20.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-08-02 13:00:20.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:00:20.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-08-02 13:00:20.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:00:19.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-02 13:00:20.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-02 13:00:20.000000 rxn-metrics-1.1.0/src/rxn_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:00:20.037457 rxn-metrics-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/tests/test_context_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/tests/test_tokenize_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3206 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/tests/test_true_reactant_accuracy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-08-02 13:00:11.000000 rxn-metrics-1.1.0/tests/test_utils.py
```

### Comparing `rxn-metrics-1.0.0/LICENSE` & `rxn-metrics-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/PKG-INFO` & `rxn-metrics-1.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,44 @@
-Metadata-Version: 2.1
-Name: rxn-metrics
-Version: 1.0.0
-Summary: Metrics for RXN models
-Home-page: https://github.com/rxn4chemistry/rxn-metrics
-Author: IBM RXN team
-License: MIT
-Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-metrics/
-Project-URL: Repository, https://github.com/rxn4chemistry/rxn-metrics
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: rdkit
-License-File: LICENSE
-
 # RXN package for the calculation of metrics for OpenNMT-based models
 
 [![Actions tests](https://github.com/rxn4chemistry/rxn-metrics/actions/workflows/tests.yaml/badge.svg)](https://github.com/rxn4chemistry/rxn-metrics/actions)
 
 This repository contains a Python package and associated scripts for training reaction models based on the OpenNMT library.
 This repository is closely related to [`rxn-onmt-models`](https://github.com/rxn4chemistry/rxn-onmt-models), which handles the training pipelines for these models.
 The repository also relies on other RXN packages; see [`rxn-utilities`](https://github.com/rxn4chemistry/rxn-utilities), [`rxn-chemutils`](https://github.com/rxn4chemistry/rxn-chemutils), and [`rxn-onmt-utils`](https://github.com/rxn4chemistry/rxn-onmt-utils).
 
-The documentation can be found [here](https://rxn4chemistry.github.io/rxn-metrics/).
+Links:
+* [GitHub repository](https://github.com/rxn4chemistry/rxn-metrics)
+* [Documentation](https://rxn4chemistry.github.io/rxn-metrics/)
+* [PyPI package](https://pypi.org/project/rxn-metrics/)
 
 This repository was produced through a collaborative project involving IBM Research Europe and Syngenta.
 
 ## System Requirements
 
 This package is supported on all operating systems.
 It has been tested on the following systems:
 + macOS: Big Sur (11.1)
 + Linux: Ubuntu 18.04.4
 
 A Python version of 3.6, 3.7, or 3.8 is recommended.
-Python versions 3.9 and above are not expected to work due to compatibility with the selected version of OpenNMT.
+Python versions 3.9 and above are not expe`cted to work due to compatibility with the selected version of OpenNMT.
 
 ## Installation guide
 
 The package can be installed from Pypi:
 ```bash
-pip install rxn-metrics[rdkit]
+pip install rxn-metrics[rdkit,rxnmapper]
 ```
-You can leave out `[rdkit]` if RDKit is already available in your environment.
+You can leave out the extra dependency `rdkit` if RDKit is already available in your environment.
+Also, you can leave out the extra dependency `rxnmapper` if you don't plan on calculating the "true reactant" accuracy.
 
 For local development, the package can be installed with:
 ```bash
-pip install -e ".[dev,rdkit]"
+pip install -e ".[dev,rdkit,rxnmapper]"
 ```
 
 ## Calculation of metrics
 
 The metrics are best calculated by launching one of the following scripts:
 * `rxn-prepare-context-metrics`
 * `rxn-prepare-forward-metrics`
```

### Comparing `rxn-metrics-1.0.0/README.md` & `rxn-metrics-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,65 @@
+Metadata-Version: 2.1
+Name: rxn-metrics
+Version: 1.1.0
+Summary: Metrics for RXN models
+Home-page: https://github.com/rxn4chemistry/rxn-metrics
+Author: IBM RXN team
+License: MIT
+Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-metrics/
+Project-URL: Repository, https://github.com/rxn4chemistry/rxn-metrics
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: rdkit
+Provides-Extra: rxnmapper
+License-File: LICENSE
+
 # RXN package for the calculation of metrics for OpenNMT-based models
 
 [![Actions tests](https://github.com/rxn4chemistry/rxn-metrics/actions/workflows/tests.yaml/badge.svg)](https://github.com/rxn4chemistry/rxn-metrics/actions)
 
 This repository contains a Python package and associated scripts for training reaction models based on the OpenNMT library.
 This repository is closely related to [`rxn-onmt-models`](https://github.com/rxn4chemistry/rxn-onmt-models), which handles the training pipelines for these models.
 The repository also relies on other RXN packages; see [`rxn-utilities`](https://github.com/rxn4chemistry/rxn-utilities), [`rxn-chemutils`](https://github.com/rxn4chemistry/rxn-chemutils), and [`rxn-onmt-utils`](https://github.com/rxn4chemistry/rxn-onmt-utils).
 
-The documentation can be found [here](https://rxn4chemistry.github.io/rxn-metrics/).
+Links:
+* [GitHub repository](https://github.com/rxn4chemistry/rxn-metrics)
+* [Documentation](https://rxn4chemistry.github.io/rxn-metrics/)
+* [PyPI package](https://pypi.org/project/rxn-metrics/)
 
 This repository was produced through a collaborative project involving IBM Research Europe and Syngenta.
 
 ## System Requirements
 
 This package is supported on all operating systems.
 It has been tested on the following systems:
 + macOS: Big Sur (11.1)
 + Linux: Ubuntu 18.04.4
 
 A Python version of 3.6, 3.7, or 3.8 is recommended.
-Python versions 3.9 and above are not expected to work due to compatibility with the selected version of OpenNMT.
+Python versions 3.9 and above are not expe`cted to work due to compatibility with the selected version of OpenNMT.
 
 ## Installation guide
 
 The package can be installed from Pypi:
 ```bash
-pip install rxn-metrics[rdkit]
+pip install rxn-metrics[rdkit,rxnmapper]
 ```
-You can leave out `[rdkit]` if RDKit is already available in your environment.
+You can leave out the extra dependency `rdkit` if RDKit is already available in your environment.
+Also, you can leave out the extra dependency `rxnmapper` if you don't plan on calculating the "true reactant" accuracy.
 
 For local development, the package can be installed with:
 ```bash
-pip install -e ".[dev,rdkit]"
+pip install -e ".[dev,rdkit,rxnmapper]"
 ```
 
 ## Calculation of metrics
 
 The metrics are best calculated by launching one of the following scripts:
 * `rxn-prepare-context-metrics`
 * `rxn-prepare-forward-metrics`
```

### Comparing `rxn-metrics-1.0.0/setup.cfg` & `rxn-metrics-1.1.0/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -10,26 +10,28 @@
 project_urls = 
 	Documentation = https://rxn4chemistry.github.io/rxn-metrics/
 	Repository = https://github.com/rxn4chemistry/rxn-metrics
 classifiers = 
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
 
 [options]
 package_dir = 
 	= src
 packages = find_namespace:
 python_requires = >= 3.6
 zip_safe = False
 include_package_data = True
 install_requires = 
 	click>=8.0
 	pandas>=1.1.0
-	rxn-chem-utils>=1.1.4
+	rxn-chem-utils>=1.3.0
 	rxn-onmt-models>=1.0.0
 	rxn-onmt-utils>=1.0.0
 	rxn-utils>=1.1.9
 
 [options.packages.find]
 where = src
 
@@ -45,14 +47,17 @@
 	isort>=5.10.1
 	mypy>=0.910
 	pytest>=5.3.4
 	types-setuptools>=57.4.14
 rdkit = 
 	rdkit-pypi>=2021.3.2 ; python_version<"3.7"
 	rdkit>=2022.3.4 ; python_version>="3.7"
+rxnmapper = 
+	rxnmapper>=0.3.0
+	transformers<4.23.0  # Versions >=4.23.0 are not compatible with torch 1.5.1
 
 [options.entry_points]
 console_scripts = 
 	rxn-evaluate-metrics = rxn.metrics.scripts.rxn_evaluate_metrics:main
 	rxn-parse-metrics-into-csv = rxn.metrics.scripts.parse_metrics_into_csv:main
 	rxn-prepare-context-metrics = rxn.metrics.scripts.prepare_context_metrics:main
 	rxn-prepare-forward-metrics = rxn.metrics.scripts.prepare_forward_metrics:main
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/classification_translation.py` & `rxn-metrics-1.1.0/src/rxn/metrics/classification_translation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,75 @@
 import logging
 from pathlib import Path
 from typing import Optional, Union
 
 from rxn.chemutils.tokenization import file_is_tokenized, tokenize_file
 from rxn.onmt_utils import translate
-from rxn.utilities.files import is_path_exists_or_creatable
+from rxn.utilities.files import dump_list_to_file, is_path_exists_or_creatable
 
+from .metrics_files import RetroFiles
 from .tokenize_file import (
     classification_file_is_tokenized,
     detokenize_classification_file,
     tokenize_classification_file,
 )
+from .utils import combine_precursors_and_products_from_files
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
+def maybe_classify_predictions(
+    classification_model: Optional[Path],
+    retro_files: RetroFiles,
+    batch_size: int,
+    gpu: bool,
+) -> None:
+    """Classify the reactions for determining the diversity metric.
+
+    Only executed if a classification model is available."""
+
+    if classification_model is None:
+        return
+
+    create_rxn_from_files(
+        retro_files.predicted_canonical,
+        retro_files.predicted_products_canonical,
+        retro_files.predicted_rxn_canonical,
+    )
+
+    classification_translation(
+        src_file=retro_files.predicted_rxn_canonical,
+        tgt_file=None,
+        pred_file=retro_files.predicted_classes,
+        model=classification_model,
+        n_best=1,
+        beam_size=5,
+        batch_size=batch_size,
+        gpu=gpu,
+    )
+
+
+def create_rxn_from_files(
+    input_file_precursors: Union[str, Path],
+    input_file_products: Union[str, Path],
+    output_file: Union[str, Path],
+) -> None:
+    logger.info(
+        f'Combining files "{input_file_precursors}" and "{input_file_products}" -> "{output_file}".'
+    )
+    dump_list_to_file(
+        combine_precursors_and_products_from_files(
+            precursors_file=input_file_precursors,
+            products_file=input_file_products,
+        ),
+        output_file,
+    )
+
+
 def classification_translation(
     src_file: Union[str, Path],
     tgt_file: Optional[Union[str, Path]],
     pred_file: Union[str, Path],
     model: Union[str, Path],
     n_best: int,
     beam_size: int,
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/context_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/context_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from typing import Any, Dict, Iterable, List, Sequence
 
 import numpy as np
 from rxn.chemutils.reaction_smiles import parse_any_reaction_smiles
 from rxn.utilities.containers import chunker
 from rxn.utilities.files import PathLike, iterate_lines_from_file
 
-from .metrics import get_sequence_multiplier, top_n_accuracy
+from .metrics import top_n_accuracy
 from .metrics_calculator import MetricsCalculator
 from .metrics_files import ContextFiles, MetricsFiles
+from .utils import get_sequence_multiplier
 
 
 class ContextMetrics(MetricsCalculator):
     """
     Class to compute common metrics for context prediction models, starting from
     files containing the ground truth and predictions.
 
@@ -105,9 +106,9 @@
     # We will process sample by sample - for that, we need to chunk the predictions
     prediction_chunks = chunker(predictions, chunk_size=multiplier)
     for gt, predictions in zip(ground_truth, prediction_chunks):
         for i, prediction in enumerate(predictions):
             overlap = identical_fraction(gt, prediction)
             overlap_for_n[i].append(overlap)
 
-    accuracy = {i + 1: np.mean(overlap_for_n[i]) for i in range(multiplier)}
+    accuracy = {i + 1: float(np.mean(overlap_for_n[i])) for i in range(multiplier)}
     return accuracy
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/forward_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/forward_metrics.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 Definition of the different metrics.
 """
 
 from typing import Dict, List, Sequence, Tuple, TypeVar
 
 import numpy as np
 from rxn.utilities.containers import chunker
-from rxn.utilities.misc import get_multiplier
+
+from .utils import get_sequence_multiplier
 
 T = TypeVar("T")
 
 
 def top_n_accuracy(
     ground_truth: Sequence[T], predictions: Sequence[T]
 ) -> Dict[int, float]:
@@ -68,16 +69,20 @@
         correct_values = 0
         for i, prediction in enumerate(predictions):
             correct = gt == prediction
             correct_values += int(correct)
             correct_for_n[i].append(correct_values)
 
     # Note: for the "n"-th value, we must divide by "n=i+1" because the list elements were not averaged.
-    accuracy = {i + 1: np.mean(correct_for_n[i]) / (i + 1) for i in range(multiplier)}
-    std_dev = {i + 1: np.std(correct_for_n[i]) / (i + 1) for i in range(multiplier)}
+    accuracy = {
+        i + 1: float(np.mean(correct_for_n[i])) / (i + 1) for i in range(multiplier)
+    }
+    std_dev = {
+        i + 1: float(np.std(correct_for_n[i])) / (i + 1) for i in range(multiplier)
+    }
     return accuracy, std_dev
 
 
 def coverage(ground_truth: Sequence[T], predictions: Sequence[T]) -> Dict[int, float]:
     """
     Compute the coverage values, split by n-th predictions.
 
@@ -148,24 +153,12 @@
         for i, (pred, pred_class) in enumerate(preds_and_classes):
             if gt == pred and pred_class != "":
                 classes.add(pred_class)
             classes_for_n[i].append(len(classes))
 
     # Note: the total number of predictions to take into account for the "n"-th (= "i+1"th)
     # value is "len(ground_truth)". A value < 1 is the consequence of having incorrect predictions
-    classdiversity = {i + 1: np.mean(classes_for_n[i]) for i in range(multiplier)}
-    std_dev = {i + 1: np.std(classes_for_n[i]) for i in range(multiplier)}
+    classdiversity = {
+        i + 1: float(np.mean(classes_for_n[i])) for i in range(multiplier)
+    }
+    std_dev = {i + 1: float(np.std(classes_for_n[i])) for i in range(multiplier)}
     return classdiversity, std_dev
-
-
-def get_sequence_multiplier(ground_truth: Sequence[T], predictions: Sequence[T]) -> int:
-    """
-    Get the multiplier for the number of predictions by ground truth sample.
-
-    Raises:
-        ValueError: if the lists have inadequate sizes (possibly forwarded
-            from get_multiplier).
-    """
-    n_gt = len(ground_truth)
-    n_pred = len(predictions)
-
-    return get_multiplier(n_gt, n_pred)
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/metrics_calculator.py` & `rxn-metrics-1.1.0/src/rxn/metrics/metrics_calculator.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/metrics_files.py` & `rxn-metrics-1.1.0/src/rxn/metrics/metrics_files.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,16 @@
             self.directory / "predicted_products_canonical.txt"
         )
         self.predicted_products_log_probs = (
             self.directory / "predicted_products.txt.tokenized_log_probs"
         )
         self.predicted_rxn_canonical = self.directory / "predicted_rxn_canonical.txt"
         self.predicted_classes = self.directory / "predicted_classes.txt"
+        self.gt_mapped = self.directory / "gt_mapped.txt"
+        self.predicted_mapped = self.directory / "predicted_mapped.txt"
 
     @staticmethod
     def reordered(path: PathLike) -> Path:
         """Add the reordered path extension."""
         return Path(str(path) + RetroFiles._REORDERED_FILE_EXTENSION)
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/retro_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/retro_metrics.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-import os
-from typing import Any, Dict, Iterable, Optional
+from typing import Any, Dict, Iterable, List, Optional
 
-from rxn.utilities.files import PathLike, iterate_lines_from_file
+from rxn.utilities.files import PathLike, iterate_lines_from_file, load_list_from_file
 
 from .metrics import class_diversity, coverage, round_trip_accuracy, top_n_accuracy
 from .metrics_calculator import MetricsCalculator
 from .metrics_files import MetricsFiles, RetroFiles
+from .true_reactant_accuracy import true_reactant_accuracy
 
 
 class RetroMetrics(MetricsCalculator):
     """
     Class to compute common metrics for retro models, starting from files
     containing the ground truth and predictions.
 
@@ -18,60 +18,73 @@
 
     def __init__(
         self,
         gt_precursors: Iterable[str],
         gt_products: Iterable[str],
         predicted_precursors: Iterable[str],
         predicted_products: Iterable[str],
-        predicted_classes: Optional[Iterable[str]] = None,
+        predicted_classes: Optional[List[str]] = None,
+        gt_mapped_rxns: Optional[List[str]] = None,
+        predicted_mapped_rxns: Optional[List[str]] = None,
     ):
         self.gt_products = list(gt_products)
         self.gt_precursors = list(gt_precursors)
         self.predicted_products = list(predicted_products)
         self.predicted_precursors = list(predicted_precursors)
-        self.predicted_classes = (
-            list(predicted_classes) if predicted_classes is not None else None
-        )
+
+        self.predicted_classes = predicted_classes
+        self.gt_mapped_rxns = gt_mapped_rxns
+        self.predicted_mapped_rxns = predicted_mapped_rxns
 
     def get_metrics(self) -> Dict[str, Any]:
         topn = top_n_accuracy(
             ground_truth=self.gt_precursors, predictions=self.predicted_precursors
         )
         roundtrip, roundtrip_std = round_trip_accuracy(
             ground_truth=self.gt_products, predictions=self.predicted_products
         )
         cov = coverage(
             ground_truth=self.gt_products, predictions=self.predicted_products
         )
-        if self.predicted_classes:
+        if self.predicted_classes is not None:
             classdiversity, classdiversity_std = class_diversity(
                 ground_truth=self.gt_products,
                 predictions=self.predicted_products,
                 predicted_classes=self.predicted_classes,
             )
         else:
             classdiversity, classdiversity_std = {}, {}
+        if self.gt_mapped_rxns is not None and self.predicted_mapped_rxns is not None:
+            reactant_accuracy = true_reactant_accuracy(
+                self.gt_mapped_rxns, self.predicted_mapped_rxns
+            )
+        else:
+            reactant_accuracy = {}
 
         return {
             "accuracy": topn,
             "round-trip": roundtrip,
             "round-trip-std": roundtrip_std,
             "coverage": cov,
             "class-diversity": classdiversity,
             "class-diversity-std": classdiversity_std,
+            "true-reactant-accuracy": reactant_accuracy,
         }
 
     @classmethod
     def from_metrics_files(cls, metrics_files: MetricsFiles) -> "RetroMetrics":
         if not isinstance(metrics_files, RetroFiles):
             raise ValueError("Invalid type provided")
 
         # Whether to use the reordered files - for class token
         # To determine whether True or False, we check if the reordered files exist
         reordered = RetroFiles.reordered(metrics_files.predicted_canonical).exists()
+        mapped = (
+            metrics_files.gt_mapped.exists() and metrics_files.predicted_mapped.exists()
+        )
 
         return cls.from_raw_files(
             gt_precursors_file=metrics_files.gt_tgt,
             gt_products_file=metrics_files.gt_src,
             predicted_precursors_file=(
                 metrics_files.predicted_canonical
                 if not reordered
@@ -80,32 +93,44 @@
             predicted_products_file=(
                 metrics_files.predicted_products_canonical
                 if not reordered
                 else RetroFiles.reordered(metrics_files.predicted_products_canonical)
             ),
             predicted_classes_file=(
                 None
-                if not os.path.exists(metrics_files.predicted_classes)
+                if not metrics_files.predicted_classes.exists()
                 else metrics_files.predicted_classes
                 if not reordered
                 else RetroFiles.reordered(metrics_files.predicted_classes)
             ),
+            gt_mapped_rxns_file=metrics_files.gt_mapped if mapped else None,
+            predicted_mapped_rxns_file=(
+                metrics_files.predicted_mapped if mapped else None
+            ),
         )
 
     @classmethod
     def from_raw_files(
         cls,
         gt_precursors_file: PathLike,
         gt_products_file: PathLike,
         predicted_precursors_file: PathLike,
         predicted_products_file: PathLike,
         predicted_classes_file: Optional[PathLike] = None,
+        gt_mapped_rxns_file: Optional[PathLike] = None,
+        predicted_mapped_rxns_file: Optional[PathLike] = None,
     ) -> "RetroMetrics":
+        # to simplify because it is called multiple times.
+        def maybe_load_lines(filename: Optional[PathLike]) -> Optional[List[str]]:
+            if filename is None:
+                return None
+            return load_list_from_file(filename)
+
         return cls(
             gt_precursors=iterate_lines_from_file(gt_precursors_file),
             gt_products=iterate_lines_from_file(gt_products_file),
             predicted_precursors=iterate_lines_from_file(predicted_precursors_file),
             predicted_products=iterate_lines_from_file(predicted_products_file),
-            predicted_classes=None
-            if predicted_classes_file is None
-            else iterate_lines_from_file(predicted_classes_file),
+            predicted_classes=maybe_load_lines(predicted_classes_file),
+            gt_mapped_rxns=maybe_load_lines(gt_mapped_rxns_file),
+            predicted_mapped_rxns=maybe_load_lines(predicted_mapped_rxns_file),
         )
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/run_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/run_metrics.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/ensure_data_dimension.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/ensure_data_dimension.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/join_data_files.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/join_data_files.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/parse_metrics_into_csv.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/parse_metrics_into_csv.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/prepare_context_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/prepare_context_metrics.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/prepare_forward_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/prepare_forward_metrics.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/reorder_retro_predictions_class_token.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/reorder_retro_predictions_class_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from pathlib import Path
 from typing import List, Tuple, Union
 
 import click
 from rxn.utilities.containers import chunker
 from rxn.utilities.files import dump_list_to_file, load_list_from_file
 
-from rxn.metrics.metrics import get_sequence_multiplier
 from rxn.metrics.metrics_files import RetroFiles
+from rxn.metrics.utils import get_sequence_multiplier
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 def reorder_retro_predictions_class_token(
     ground_truth_file: Union[str, Path],
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/scripts/rxn_evaluate_metrics.py` & `rxn-metrics-1.1.0/src/rxn/metrics/scripts/rxn_evaluate_metrics.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @click.option(
     "--task", required=True, type=click.Choice(["forward", "retro", "context"])
 )
 @click.option(
     "--results_dir", required=True, help="Where the retro predictions are stored"
 )
 def main(task: str, results_dir: str) -> None:
-    """Evaluate the metrics (the metrics must have been generated already!)"""
+    """Evaluate the metrics (the predictions must have been generated already!)"""
 
     setup_console_logger()
 
     evaluate_metrics(task, results_dir)
 
 
 if __name__ == "__main__":
```

### Comparing `rxn-metrics-1.0.0/src/rxn/metrics/tokenize_file.py` & `rxn-metrics-1.1.0/src/rxn/metrics/tokenize_file.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/src/rxn_metrics.egg-info/PKG-INFO` & `rxn-metrics-1.1.0/src/rxn_metrics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,65 @@
 Metadata-Version: 2.1
 Name: rxn-metrics
-Version: 1.0.0
+Version: 1.1.0
 Summary: Metrics for RXN models
 Home-page: https://github.com/rxn4chemistry/rxn-metrics
 Author: IBM RXN team
 License: MIT
 Project-URL: Documentation, https://rxn4chemistry.github.io/rxn-metrics/
 Project-URL: Repository, https://github.com/rxn4chemistry/rxn-metrics
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: rdkit
+Provides-Extra: rxnmapper
 License-File: LICENSE
 
 # RXN package for the calculation of metrics for OpenNMT-based models
 
 [![Actions tests](https://github.com/rxn4chemistry/rxn-metrics/actions/workflows/tests.yaml/badge.svg)](https://github.com/rxn4chemistry/rxn-metrics/actions)
 
 This repository contains a Python package and associated scripts for training reaction models based on the OpenNMT library.
 This repository is closely related to [`rxn-onmt-models`](https://github.com/rxn4chemistry/rxn-onmt-models), which handles the training pipelines for these models.
 The repository also relies on other RXN packages; see [`rxn-utilities`](https://github.com/rxn4chemistry/rxn-utilities), [`rxn-chemutils`](https://github.com/rxn4chemistry/rxn-chemutils), and [`rxn-onmt-utils`](https://github.com/rxn4chemistry/rxn-onmt-utils).
 
-The documentation can be found [here](https://rxn4chemistry.github.io/rxn-metrics/).
+Links:
+* [GitHub repository](https://github.com/rxn4chemistry/rxn-metrics)
+* [Documentation](https://rxn4chemistry.github.io/rxn-metrics/)
+* [PyPI package](https://pypi.org/project/rxn-metrics/)
 
 This repository was produced through a collaborative project involving IBM Research Europe and Syngenta.
 
 ## System Requirements
 
 This package is supported on all operating systems.
 It has been tested on the following systems:
 + macOS: Big Sur (11.1)
 + Linux: Ubuntu 18.04.4
 
 A Python version of 3.6, 3.7, or 3.8 is recommended.
-Python versions 3.9 and above are not expected to work due to compatibility with the selected version of OpenNMT.
+Python versions 3.9 and above are not expe`cted to work due to compatibility with the selected version of OpenNMT.
 
 ## Installation guide
 
 The package can be installed from Pypi:
 ```bash
-pip install rxn-metrics[rdkit]
+pip install rxn-metrics[rdkit,rxnmapper]
 ```
-You can leave out `[rdkit]` if RDKit is already available in your environment.
+You can leave out the extra dependency `rdkit` if RDKit is already available in your environment.
+Also, you can leave out the extra dependency `rxnmapper` if you don't plan on calculating the "true reactant" accuracy.
 
 For local development, the package can be installed with:
 ```bash
-pip install -e ".[dev,rdkit]"
+pip install -e ".[dev,rdkit,rxnmapper]"
 ```
 
 ## Calculation of metrics
 
 The metrics are best calculated by launching one of the following scripts:
 * `rxn-prepare-context-metrics`
 * `rxn-prepare-forward-metrics`
```

### Comparing `rxn-metrics-1.0.0/src/rxn_metrics.egg-info/SOURCES.txt` & `rxn-metrics-1.1.0/src/rxn_metrics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 src/rxn/metrics/__init__.py
+src/rxn/metrics/class_tokens.py
 src/rxn/metrics/classification_translation.py
 src/rxn/metrics/context_metrics.py
 src/rxn/metrics/forward_metrics.py
 src/rxn/metrics/metrics.py
 src/rxn/metrics/metrics_calculator.py
 src/rxn/metrics/metrics_files.py
 src/rxn/metrics/py.typed
 src/rxn/metrics/retro_metrics.py
 src/rxn/metrics/run_metrics.py
 src/rxn/metrics/tokenize_file.py
+src/rxn/metrics/true_reactant_accuracy.py
 src/rxn/metrics/utils.py
 src/rxn/metrics/scripts/__init__.py
 src/rxn/metrics/scripts/ensure_data_dimension.py
 src/rxn/metrics/scripts/join_data_files.py
 src/rxn/metrics/scripts/parse_metrics_into_csv.py
 src/rxn/metrics/scripts/prepare_context_metrics.py
 src/rxn/metrics/scripts/prepare_forward_metrics.py
@@ -29,8 +31,10 @@
 src/rxn_metrics.egg-info/dependency_links.txt
 src/rxn_metrics.egg-info/entry_points.txt
 src/rxn_metrics.egg-info/not-zip-safe
 src/rxn_metrics.egg-info/requires.txt
 src/rxn_metrics.egg-info/top_level.txt
 tests/test_context_metrics.py
 tests/test_metrics.py
-tests/test_tokenize_file.py
+tests/test_tokenize_file.py
+tests/test_true_reactant_accuracy.py
+tests/test_utils.py
```

### Comparing `rxn-metrics-1.0.0/tests/test_context_metrics.py` & `rxn-metrics-1.1.0/tests/test_context_metrics.py`

 * *Files identical despite different names*

### Comparing `rxn-metrics-1.0.0/tests/test_tokenize_file.py` & `rxn-metrics-1.1.0/tests/test_tokenize_file.py`

 * *Files identical despite different names*


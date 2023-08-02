# Comparing `tmp/pymilo-0.1.tar.gz` & `tmp/pymilo-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymilo-0.1.tar", last modified: Thu Jun 29 07:11:01 2023, max compression
+gzip compressed data, was "pymilo-0.2.tar", last modified: Wed Aug  2 13:43:38 2023, max compression
```

## Comparing `pymilo-0.1.tar` & `pymilo-0.2.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.419667 pymilo-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-29 07:10:51.000000 pymilo-0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-29 07:10:51.000000 pymilo-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-06-29 07:11:01.419667 pymilo-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-06-29 07:10:51.000000 pymilo-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.415667 pymilo-0.1/pymilo/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.415667 pymilo-0.1/pymilo/chains/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/chains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/chains/linear_model_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.415667 pymilo-0.1/pymilo/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/exceptions/deserialize_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/exceptions/pymilo_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/exceptions/serialize_exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/pymilo_func.py
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/pymilo_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     4808 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/pymilo_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.415667 pymilo-0.1/pymilo/transporters/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/transporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/transporters/baseloss_transporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9549 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/transporters/general_data_structure_transporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/transporters/labelbinarizer_transporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/transporters/lossfunction_transporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/transporters/transporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.419667 pymilo-0.1/pymilo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/utils/data_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/utils/test_pymilo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-29 07:10:51.000000 pymilo-0.1/pymilo/utils/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 07:11:01.415667 pymilo-0.1/pymilo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-06-29 07:11:01.000000 pymilo-0.1/pymilo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-29 07:11:01.000000 pymilo-0.1/pymilo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 07:11:01.000000 pymilo-0.1/pymilo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-29 07:11:01.000000 pymilo-0.1/pymilo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-29 07:11:01.000000 pymilo-0.1/pymilo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-29 07:11:01.419667 pymilo-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-06-29 07:10:51.000000 pymilo-0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.366870 pymilo-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-08-02 13:43:22.000000 pymilo-0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 13:43:22.000000 pymilo-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-08-02 13:43:38.366870 pymilo-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-08-02 13:43:22.000000 pymilo-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.362871 pymilo-0.2/pymilo/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.362871 pymilo-0.2/pymilo/chains/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/chains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/chains/linear_model_chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/chains/neural_network_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.366870 pymilo-0.2/pymilo/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/exceptions/deserialize_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/exceptions/pymilo_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3634 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/exceptions/serialize_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/pymilo_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/pymilo_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5217 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/pymilo_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.366870 pymilo-0.2/pymilo/transporters/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/adamoptimizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/baseloss_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12130 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/general_data_structure_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/labelbinarizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/lossfunction_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3074 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/randomstate_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/sgdoptimizer_transporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/transporters/transporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.366870 pymilo-0.2/pymilo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/utils/data_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/utils/test_pymilo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-08-02 13:43:22.000000 pymilo-0.2/pymilo/utils/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:43:38.362871 pymilo-0.2/pymilo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-08-02 13:43:38.000000 pymilo-0.2/pymilo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-02 13:43:38.000000 pymilo-0.2/pymilo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:43:38.000000 pymilo-0.2/pymilo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 13:43:38.000000 pymilo-0.2/pymilo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 13:43:38.000000 pymilo-0.2/pymilo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:43:38.366870 pymilo-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-08-02 13:43:22.000000 pymilo-0.2/setup.py
```

### Comparing `pymilo-0.1/AUTHORS.md` & `pymilo-0.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/LICENSE` & `pymilo-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/PKG-INFO` & `pymilo-0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pymilo
-Version: 0.1
+Version: 0.2
 Summary: Transportation of ML models
 Home-page: https://github.com/openscilab/pymilo
-Download-URL: https://github.com/openscilab/pymilo/tarball/v0.1
+Download-URL: https://github.com/openscilab/pymilo/tarball/v0.2
 Author: PyMilo Development Team
 Author-email: info@pycm.io
 License: MIT
 Project-URL: Source, https://github.com/openscilab/pymilo
 Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
@@ -29,15 +28,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
 <div align="center">
     <img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png" width="500" height="300">
@@ -115,17 +114,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.1`
+- Run `pip install pymilo==0.2`
 ### Source code
-- Download [Version 0.1](https://github.com/openscilab/pymilo/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.2](https://github.com/openscilab/pymilo/archive/v0.2.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Simple Linear Model Preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -157,18 +156,19 @@
 ```
 #### Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
 
 ## Supported ML Models
 | scikit-learn | PyTorch | 
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
-| Neural networks &#x274C; | -  | 
+| Neural networks &#x2705; | -  | 
 | Clustering &#x274C; | -  | 
 | Trees &#x274C; | -  | 
 | Ensemble Models &#x274C; | - | 
+Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com "info@openscilab.com"). 
 
 - Please complete the issue template
  
@@ -194,16 +194,40 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.2] - 2023-08-02
+### Added
+- scikit-learn neural network models 
+- `MLP Regressor` model 
+- `MLP Classifier` model
+- `BernoulliRBN` model
+- `SGDOptimizer` transporter
+- `RandomState(MT19937)` transporter
+- `Adamoptimizer` transporter
+- Neural Network chain
+- Neural Network exceptions 
+- `ndarray_to_list` method in `GeneralDataStructureTransporter`
+- `list_to_ndarray` method in `GeneralDataStructureTransporter` 
+- `neural_network_chain.py` chain
+### Changed
+- `GeneralDataStructure` Transporter updated
+- `LabelBinerizer` Transporter updated
+- `linear model` chain updated
+- GeneralDataStructure transporter enhanced
+- LabelBinerizer transporter updated
+- transporters' chain router added to `pymilo func`
+- NeuralNetwork params initialized in `pymilo_param`
+- `pymilo_test` updated to support multiple models
+- `linear_model_chain` refactored
 ## [0.1] - 2023-06-29
 ### Added
 - scikit-learn linear models support
 - `Export` class
 - `Import` class
 
-
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.1...dev
+[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: pymilo Version: 0.1 Summary: Transportation of ML
+Metadata-Version: 2.1 Name: pymilo Version: 0.2 Summary: Transportation of ML
 models Home-page: https://github.com/openscilab/pymilo Download-URL: https://
-github.com/openscilab/pymilo/tarball/v0.1 Author: PyMilo Development Team
+github.com/openscilab/pymilo/tarball/v0.2 Author: PyMilo Development Team
 Author-email: info@pycm.io License: MIT Project-URL: Source, https://
 github.com/openscilab/pymilo Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
-Manufacturing Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering :: Information Analysis Classifier: Topic ::
-Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Human Machine Interfaces Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
-Engineering :: Physics Requires-Python: >=3.5 Description-Content-Type: text/
-markdown License-File: LICENSE License-File: AUTHORS.md
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: End Users/Desktop Classifier:
+Intended Audience :: Manufacturing Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Education Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
+Scientific/Engineering :: Physics Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
      [https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png]
 
         [Codecov] [PyPI_version] [built_with_Python3] [Discord_Channel]
 ---------- ## Table of contents * [Overview](https://github.com/openscilab/
 pymilo#overview) * [Installation](https://github.com/openscilab/
 pymilo#installation) * [Usage](https://github.com/openscilab/pymilo#usage) *
 [Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-
@@ -49,17 +48,17 @@
 Github Stars [https://img.shields.io/github/stars/openscilab/
                    pymilo.svg?style=social&label=Stars]
 Branch                     main                                  dev
        [https://github.com/openscilab/ [https://github.com/openscilab/pymilo/
    CI       pymilo/workflows/CI/         workflows/CI/badge.svg?branch=dev]
            badge.svg?branch=main]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.1` ### Source
-code - Download [Version 0.1](https://github.com/openscilab/pymilo/archive/
-v0.1.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.2` ### Source
+code - Download [Version 0.2](https://github.com/openscilab/pymilo/archive/
+v0.2.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Simple Linear Model Preparation
 ```pycon >>> from sklearn import datasets >>> from pymilo import Export, Import
 >>> from sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save Model ```pycon >>>
@@ -68,23 +67,37 @@
 exported_model.save(PATH_TO_JSON_FILE) ``` ### Load Model ```pycon >>> ####
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated Scikit model ```pycon
 >>> imported_sklearn_model = imported_model.to_model() ``` #### Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML Models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models &#x2705; | - | | Neural networks
-&#x274C; | - | | Clustering &#x274C; | - | | Trees &#x274C; | - | | Ensemble
-Models &#x274C; | - | ## Issues & bug reports Just fill an issue and describe
-it. We'll check it ASAP! or send an email to [info@openscilab.com](mailto:
-info@openscilab.com "info@openscilab.com"). - Please complete the issue
-template You can also join our discord server [Discord_Channel] ## Show Your
-Support ### Star this repo Give a â­ï¸ if this project helped you! ### Donate
-to our project If you do like our project and we hope that you do, can you
-please support us? Our project is not and is never going to be working for
-profit. We need the money just so we can continue doing what we do ;-) .
-[PyMilo_Donation] # Changelog All notable changes to this project will be
-documented in this file. The format is based on [Keep a Changelog](http://
-keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
-(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [0.1] - 2023-06-29 ###
-Added - scikit-learn linear models support - `Export` class - `Import` class
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.1...dev [0.1]:
-https://github.com/openscilab/pymilo/compare/e887108...v0.1
+&#x2705; | - | | Clustering &#x274C; | - | | Trees &#x274C; | - | | Ensemble
+Models &#x274C; | - | Details are available in [Supported Models](https://
+github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug
+reports Just fill an issue and describe it. We'll check it ASAP! or send an
+email to [info@openscilab.com](mailto:info@openscilab.com
+"info@openscilab.com"). - Please complete the issue template You can also join
+our discord server [Discord_Channel] ## Show Your Support ### Star this repo
+Give a â­ï¸ if this project helped you! ### Donate to our project If you do
+like our project and we hope that you do, can you please support us? Our
+project is not and is never going to be working for profit. We need the money
+just so we can continue doing what we do ;-) . [PyMilo_Donation] # Changelog
+All notable changes to this project will be documented in this file. The format
+is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
+project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
+## [Unreleased] ## [0.2] - 2023-08-02 ### Added - scikit-learn neural network
+models - `MLP Regressor` model - `MLP Classifier` model - `BernoulliRBN` model
+- `SGDOptimizer` transporter - `RandomState(MT19937)` transporter -
+`Adamoptimizer` transporter - Neural Network chain - Neural Network exceptions
+- `ndarray_to_list` method in `GeneralDataStructureTransporter` -
+`list_to_ndarray` method in `GeneralDataStructureTransporter` -
+`neural_network_chain.py` chain ### Changed - `GeneralDataStructure`
+Transporter updated - `LabelBinerizer` Transporter updated - `linear model`
+chain updated - GeneralDataStructure transporter enhanced - LabelBinerizer
+transporter updated - transporters' chain router added to `pymilo func` -
+NeuralNetwork params initialized in `pymilo_param` - `pymilo_test` updated to
+support multiple models - `linear_model_chain` refactored ## [0.1] - 2023-06-29
+### Added - scikit-learn linear models support - `Export` class - `Import`
+class [Unreleased]: https://github.com/openscilab/pymilo/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2 [0.1]: https://
+github.com/openscilab/pymilo/compare/e887108...v0.1
```

### Comparing `pymilo-0.1/README.md` & `pymilo-0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -74,17 +74,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.1`
+- Run `pip install pymilo==0.2`
 ### Source code
-- Download [Version 0.1](https://github.com/openscilab/pymilo/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.2](https://github.com/openscilab/pymilo/archive/v0.2.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Simple Linear Model Preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -116,18 +116,19 @@
 ```
 #### Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
 
 ## Supported ML Models
 | scikit-learn | PyTorch | 
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
-| Neural networks &#x274C; | -  | 
+| Neural networks &#x2705; | -  | 
 | Clustering &#x274C; | -  | 
 | Trees &#x274C; | -  | 
 | Ensemble Models &#x274C; | - | 
+Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com "info@openscilab.com"). 
 
 - Please complete the issue template
```

#### html2text {}

```diff
@@ -26,17 +26,17 @@
 Github Stars [https://img.shields.io/github/stars/openscilab/
                    pymilo.svg?style=social&label=Stars]
 Branch                     main                                  dev
        [https://github.com/openscilab/ [https://github.com/openscilab/pymilo/
    CI       pymilo/workflows/CI/         workflows/CI/badge.svg?branch=dev]
            badge.svg?branch=main]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.1` ### Source
-code - Download [Version 0.1](https://github.com/openscilab/pymilo/archive/
-v0.1.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.2` ### Source
+code - Download [Version 0.2](https://github.com/openscilab/pymilo/archive/
+v0.2.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Simple Linear Model Preparation
 ```pycon >>> from sklearn import datasets >>> from pymilo import Export, Import
 >>> from sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save Model ```pycon >>>
@@ -45,17 +45,18 @@
 exported_model.save(PATH_TO_JSON_FILE) ``` ### Load Model ```pycon >>> ####
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated Scikit model ```pycon
 >>> imported_sklearn_model = imported_model.to_model() ``` #### Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML Models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models &#x2705; | - | | Neural networks
-&#x274C; | - | | Clustering &#x274C; | - | | Trees &#x274C; | - | | Ensemble
-Models &#x274C; | - | ## Issues & bug reports Just fill an issue and describe
-it. We'll check it ASAP! or send an email to [info@openscilab.com](mailto:
-info@openscilab.com "info@openscilab.com"). - Please complete the issue
-template You can also join our discord server [Discord_Channel] ## Show Your
-Support ### Star this repo Give a â­ï¸ if this project helped you! ### Donate
-to our project If you do like our project and we hope that you do, can you
-please support us? Our project is not and is never going to be working for
-profit. We need the money just so we can continue doing what we do ;-) .
-[PyMilo_Donation]
+&#x2705; | - | | Clustering &#x274C; | - | | Trees &#x274C; | - | | Ensemble
+Models &#x274C; | - | Details are available in [Supported Models](https://
+github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug
+reports Just fill an issue and describe it. We'll check it ASAP! or send an
+email to [info@openscilab.com](mailto:info@openscilab.com
+"info@openscilab.com"). - Please complete the issue template You can also join
+our discord server [Discord_Channel] ## Show Your Support ### Star this repo
+Give a â­ï¸ if this project helped you! ### Donate to our project If you do
+like our project and we hope that you do, can you please support us? Our
+project is not and is never going to be working for profit. We need the money
+just so we can continue doing what we do ;-) . [PyMilo_Donation]
```

### Comparing `pymilo-0.1/pymilo/chains/linear_model_chain.py` & `pymilo-0.2/pymilo/chains/linear_model_chain.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,22 @@
     "LabelBinarizerTransporter": LabelBinarizerTransporter()}
 
 
 def is_linear_model(model):
     """
     Check if the input model is a sklearn's linear model.
 
-    :param model: given model
+    :param model: name of a linear model or a sklearn object of it
     :type model: any object
     :return: check result as bool
     """
-    return type(model) in SKLEARN_LINEAR_MODEL_TABLE.values()
+    if isinstance(model, str):
+        return model in SKLEARN_LINEAR_MODEL_TABLE.keys()
+    else:
+        return type(model) in SKLEARN_LINEAR_MODEL_TABLE.values()
 
 
 def is_deserialized_linear_model(content):
     """
     Check if the given content is a previously serialized model by Pymilo's Export or not.
 
     :param content: given object to be authorized as a valid pymilo exported serialized model
@@ -154,26 +157,26 @@
     :param command: command to specify whether the request should be serialized or deserialized
     :type command: transporter.Command
     :param is_inner_model: determines whether the request is an inner linear model, as a single field of a wrapper linear model
     :type is_inner_model: boolean
     :return: None
     """
     if command == Command.SERIALIZE:
-        if get_sklearn_type(model) in SKLEARN_LINEAR_MODEL_TABLE.keys():
+        if is_linear_model(model):
             return
         else:
             raise PymiloSerializationException(
                 {
                     'error_type': SerilaizatoinErrorTypes.INVALID_MODEL,
                     'object': model
                 }
             )
     elif command == Command.DESERIALZIE:
         model_type = model["type"] if is_inner_model else model.type
-        if model_type in SKLEARN_LINEAR_MODEL_TABLE.keys():
+        if is_linear_model(model_type):
             return
         else:
             raise PymiloDeserializationException(
                 {
                     'error_type': DeSerilaizatoinErrorTypes.INVALID_MODEL,
                     'object': model
                 }
```

### Comparing `pymilo-0.1/pymilo/exceptions/deserialize_exception.py` & `pymilo-0.2/pymilo/exceptions/deserialize_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/exceptions/pymilo_exception.py` & `pymilo-0.2/pymilo/exceptions/pymilo_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/exceptions/serialize_exception.py` & `pymilo-0.2/pymilo/exceptions/serialize_exception.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/pymilo_func.py` & `pymilo-0.2/pymilo/pymilo_func.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 """Functions."""
 import numpy as np
 import sklearn
-from .chains.linear_model_chain import transport_linear_model
+
+from .chains.linear_model_chain import transport_linear_model, is_linear_model
+from .chains.neural_network_chain import transport_neural_network, is_neural_network
+
 from .transporters.transporter import Command
 
 
 def get_sklearn_version():
     """
     Return sklearn version.
 
@@ -19,26 +22,36 @@
     """
     Return sklearn data by serializing given model.
 
     :param model: given model
     :type model: any sklearn's model class
     :return: sklearn data
     """
-    return transport_linear_model(model, Command.SERIALIZE)
+    if is_linear_model(model):
+        return transport_linear_model(model, Command.SERIALIZE)
+    elif is_neural_network(model):
+        return transport_neural_network(model, Command.SERIALIZE)
+    else:
+        return None
 
 
 def to_sklearn_model(import_obj):
     """
     Deserialize the imported object as a sklearn model.
 
     :param import_obj: given object
     :type import_obj: pymilo.Import
     :return: sklearn model
     """
-    return transport_linear_model(import_obj, Command.DESERIALZIE)
+    if is_linear_model(import_obj.type):
+        return transport_linear_model(import_obj, Command.DESERIALZIE)
+    elif is_neural_network(import_obj.type):
+        return transport_neural_network(import_obj, Command.DESERIALZIE)
+    else:
+        return None
 
 
 def compare_model_outputs(exported_output,
                           imported_output,
                           epsilon_error=10**(-8)):
     """
     Check if the given models outputs are the same.
```

### Comparing `pymilo-0.1/pymilo/pymilo_obj.py` & `pymilo-0.2/pymilo/pymilo_obj.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/pymilo_param.py` & `pymilo-0.2/pymilo/pymilo_param.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,20 +26,25 @@
 from sklearn.linear_model import LassoCV
 from sklearn.linear_model import Lasso
 from sklearn.linear_model import RidgeClassifierCV
 from sklearn.linear_model import RidgeClassifier
 from sklearn.linear_model import RidgeCV
 from sklearn.linear_model import Ridge
 from sklearn.linear_model import LinearRegression
+
+from sklearn.neural_network import MLPRegressor
+from sklearn.neural_network import MLPClassifier
+from sklearn.neural_network import BernoulliRBM
+
 from numpy import int64
 from numpy import int32
 from sklearn.preprocessing import LabelBinarizer
 import numpy as np
 
-PYMILO_VERSION = "0.1"
+PYMILO_VERSION = "0.2"
 NOT_SUPPORTED = "NOT_SUPPORTED"
 
 # Handle python 3.5.4 issues.
 glm_support = {
     'GammaRegressor': False,
     'PoissonRegressor': False,
     'TweedieRegressor': False
@@ -105,14 +110,19 @@
     "PassiveAggressiveClassifier": PassiveAggressiveClassifier,
     "RANSACRegressor": RANSACRegressor,
     "TheilSenRegressor": TheilSenRegressor,
     "HuberRegressor": HuberRegressor,
     "QuantileRegressor": NOT_SUPPORTED if not quantile_regressor_support else QuantileRegressor,
 }
 
+SKLEARN_NEURAL_NETWORK_TABLE = {
+    "MLPRegressor": MLPRegressor,
+    "MLPClassifier": MLPClassifier,
+    "BernoulliRBM": BernoulliRBM,
+}
 KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION = {
     "_label_binarizer": LabelBinarizer,  # in Ridge Classifier
     "active_": int32,  # in Lasso Lars
     "n_nonzero_coefs_": int64,  # in OMP-CV
     "scores_": dict,  # in Logistic Regression CV,
     "_base_loss": {},  # BaseLoss in Logistic Regression,
     "loss_function_": {},  # LossFunction in SGD Classifier,
@@ -120,7 +130,12 @@
 }
 
 NUMPY_TYPE_DICT = {
     "numpy.int32": int32,
     "numpy.int64": int64,
     "numpy.infinity": lambda _: np.inf
 }
+
+EXPORTED_MODELS_PATH = {
+    "LINEAR_MODEL": "exported_linear_models",
+    "NEURAL_NETWORK": "exported_neural_networks"
+}
```

### Comparing `pymilo-0.1/pymilo/transporters/baseloss_transporter.py` & `pymilo-0.2/pymilo/transporters/baseloss_transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/transporters/general_data_structure_transporter.py` & `pymilo-0.2/pymilo/transporters/general_data_structure_transporter.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 """PyMilo GeneralDataStructure transporter."""
 import numpy as np
 from ..pymilo_param import NUMPY_TYPE_DICT
+from ..utils.util import get_homogeneous_type, all_same
 from ..utils.util import is_primitive, is_iterable, check_str_in_iterable
 from .transporter import AbstractTransporter
 
 
 class GeneralDataStructureTransporter(AbstractTransporter):
     """Customized PyMilo Transporter developed to handle fields with general datastructures."""
 
@@ -21,15 +22,15 @@
         :type dictionary: dict
         :return: fully serializable dictionary
         """
         black_list_key_values = []
         for key in dictionary.keys():
             # check inner field as a np.ndarray
             if isinstance(dictionary[key], np.ndarray):
-                dictionary[key] = dictionary[key].tolist()
+                dictionary[key] = self.ndarray_to_list(dictionary[key])
             # check inner field as np.int32
             if isinstance(key, np.int32):
                 new_value = {
                     "np-type": "numpy.int32",
                     "key-value": dictionary[key]
                 }
                 black_list_key_values.append([key, new_value])
@@ -88,32 +89,34 @@
             for item in data[key]:
                 if isinstance(item, np.int32):
                     new_list.append(
                         {"value": int(item), "np-type": "numpy.int32"})
                 elif isinstance(item, np.int64):
                     new_list.append(
                         {"value": int(item), "np-type": "numpy.int64"})
+                elif isinstance(item, np.ndarray):
+                    new_list.append(self.ndarray_to_list(item))
                 else:
                     new_list.append(item)
             data[key] = new_list
 
         elif isinstance(data[key], np.ndarray):
-            data[key] = data[key].tolist()
+            data[key] = self.ndarray_to_list(data[key])
 
         elif isinstance(data[key], dict):
             data[key] = self.serialize_dict(data[key])
 
         return data[key]
 
     def deserialize(self, data, key, model_type):
         """
         Deserialize the general datastructures.
 
             1. Dictionary deserialization
-            2. Convert lists to numpy.ndarray class
+            2. Deep Convertion of lists to numpy.ndarray class
             3. Convert custom serializable object of np.int32|int64 to the main np.int32|int64 type
 
         deserialize the special loss_function_ of the SGDClassifier, SGDOneClassSVM, Perceptron and PassiveAggressiveClassifier.
         the associated loss_function_ field of the pymilo serialized model, is extracted through the SGDClassifier's _get_loss_function function
         with enough feeding of the needed inputs.
 
         deserialize the data[key] of the given model which its type is model_type.
@@ -128,40 +131,40 @@
         :param model_type: the model type of the ML model, which its internal serialized data dictionary is given as the data param.
         :type model_type: str
         :return: pymilo deserialized output of data[key]
         """
         if isinstance(data[key], dict):
             return self.get_deserialized_dict(data[key])
         elif isinstance(data[key], list):
-            return self.get_deserialized_list(data[key])
+            return self.list_to_ndarray(data[key])
         elif self.is_numpy_primary_type(data[key]):
             return self.get_deserialized_regular_primary_types(data[key])
         else:
             # TODO
             return data[key]
 
     def get_deserialized_dict(self, content):
         """
         Deserialize the given previously made serializable dictionary.
 
             1. convert numpy types values which previously made serializable to its origianl form
-            2. convert list values to nd arrays
+            2. deep convertion of list values to nd arrays
 
         It is mainly used in serializing/deserialzing the "scores_" field in Logistic regression([+CV]).
 
         :param content: given dictionary
         :type content: dict
         :return: the original dictionary
         """
         black_list_key_values = []
         if not isinstance(content, dict):
             return content
         for key in content:
             if isinstance(content[key], list):
-                content[key] = self.get_deserialized_list(content[key])
+                content[key] = self.list_to_ndarray(content[key])
             if check_str_in_iterable(
                     "np-type", content[key]):
                 new_key = NUMPY_TYPE_DICT[content[key]["np-type"]](key)
                 new_value = content[key]["key-value"]
                 black_list_key_values.append([key, new_key, new_value])
         for black_key_value in black_list_key_values:
             prev_key, new_key, new_value = black_key_value
@@ -222,7 +225,69 @@
         current_supported_primary_types = NUMPY_TYPE_DICT.values()
         if not is_iterable(content):
             return False
         if "np-type" in content and content["np-type"] in current_supported_primary_types:
             return True
         else:
             return False
+
+    def ndarray_to_list(self, ndarray_item):
+        """
+        Serialize deeply the given ndarray to its fully listed format.
+
+            1. convert itself to a list
+            2. iterate over it's elements and apply nd2list serialization if it's eligible
+
+        :param ndarray_item: given ndarray needed to get serialized to it's fully listed form
+        :type ndarray_item: numpy.ndarray
+        :return: list
+        """
+        if isinstance(ndarray_item, np.ndarray):
+            listed_ndarray = ndarray_item.tolist()
+            new_list = []
+            for item in listed_ndarray:
+                new_list.append(self.ndarray_to_list(item))
+            return new_list
+        else:
+            return ndarray_item
+
+    def list_to_ndarray(self, list_item):
+        """
+        Deserialize deeply the given list to its fully ndarray format.
+
+            1. iterate over it's elements and apply list2nd deserialization if it's eligible
+            2. convert the coarse-grained list to ndarray
+
+        :param list_item: given list needed to get deserialized to it's np.ndarray form
+        :type list_item: list
+        :return: numpy.ndarray
+        """
+        if isinstance(list_item, list):
+
+            if len(list_item) == 0:
+                return np.asarray(list_item)
+
+            new_list = []
+            for item in list_item:
+                new_list.append(self.list_to_ndarray(item))
+
+            is_homogeneous_type, the_homogeneous_type = get_homogeneous_type(
+                new_list)
+            if is_homogeneous_type:
+                if the_homogeneous_type in [int, float, str, bool]:
+                    return np.asarray(new_list)
+                elif the_homogeneous_type == np.ndarray:
+                    is_homogeneous_type, _ = get_homogeneous_type(
+                        [x.dtype for x in new_list])
+                    if (is_homogeneous_type):
+                        if all_same([len(x) for x in new_list]):
+                            return np.asarray(new_list)
+
+            return np.asarray(new_list, dtype=object)
+        else:
+            if is_primitive(list_item):
+                return list_item
+            elif "np-type" in item.keys():
+                return NUMPY_TYPE_DICT[list_item["np-type"]
+                                       ](list_item['value'])
+            else:
+                return list_item
```

### Comparing `pymilo-0.1/pymilo/transporters/labelbinarizer_transporter.py` & `pymilo-0.2/pymilo/transporters/labelbinarizer_transporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 # -*- coding: utf-8 -*-
 """PyMilo LabelBinarizer transporter."""
 from ..pymilo_param import KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION
 from sklearn import preprocessing
 import numpy as np
 from .transporter import AbstractTransporter
 
-# TODO exception handling
-# Handling Label Binarizer for Ridge Classifier(+[CV])
-
 
 class LabelBinarizerTransporter(AbstractTransporter):
-    """Customized PyMilo Transporter developed to handle LabelBinarizer field."""
+    """Customized PyMilo Transporter developed to handle LabelBinarizer field(for Ridge Classifier(+[CV]))."""
 
     def serialize(self, data, key, model_type):
         """
         Serialize the LabelBinarizer field(if there is).
 
         serialize the data[key] of the given model which type is model_type.
         basically in order to fully serialize a model, we should traverse over all the keys of its data dictionary and
@@ -75,13 +72,10 @@
         :param content: a label_binarizer object
         :type content: sklearn.preprocessing.LabelBinarizer
         :return: a sklearn.preprocessing.LabelBinarizer instance derived from the
         pymilo deserialized output of the previously pymilo serialized label_binarizer field.
         """
         raw_lb = KEYS_NEED_PREPROCESSING_BEFORE_DESERIALIZATION["_label_binarizer"](
         )
-        for key in content.keys():
-            if isinstance(content[key], list):
-                content[key] = np.array(content[key])
         for item in content.keys():
             setattr(raw_lb, item, content[item])
         return raw_lb
```

### Comparing `pymilo-0.1/pymilo/transporters/lossfunction_transporter.py` & `pymilo-0.2/pymilo/transporters/lossfunction_transporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # -*- coding: utf-8 -*-
 """PyMilo Loss function transporter."""
 from sklearn.linear_model._stochastic_gradient import SGDClassifier
 from ..utils.util import is_primitive, check_str_in_iterable
 from .transporter import AbstractTransporter
 
-# Handling LossFunction for SGD-Classifier
-
 
 class LossFunctionTransporter(AbstractTransporter):
     """Customized PyMilo Transporter developed to handle Loss function field."""
 
     def serialize(self, data, key, model_type):
         """
         Serialize the special loss_function_ of the SGDClassifier, SGDOneClassSVM, Perceptron and PassiveAggressiveClassifier.
```

### Comparing `pymilo-0.1/pymilo/transporters/transporter.py` & `pymilo-0.2/pymilo/transporters/transporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/utils/data_exporter.py` & `pymilo-0.2/pymilo/utils/data_exporter.py`

 * *Files identical despite different names*

### Comparing `pymilo-0.1/pymilo/utils/test_pymilo.py` & `pymilo-0.2/pymilo/utils/test_pymilo.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,14 +6,37 @@
 from ..pymilo_obj import Import
 
 from sklearn.metrics import mean_squared_error, r2_score
 from sklearn.metrics import accuracy_score, hinge_loss
 
 from ..pymilo_func import compare_model_outputs
 
+from ..chains.linear_model_chain import is_linear_model
+from ..chains.neural_network_chain import is_neural_network
+
+from ..pymilo_param import EXPORTED_MODELS_PATH
+
+
+def pymilo_export_path(model):
+    """
+    Return the associated folder name to save the json file generated by pymilo Export(applied to the given model).
+
+    :param model: given model
+    :type model: any sklearn's model class
+    :return: folder name
+    """
+    model_type = None
+    if is_linear_model(model):
+        model_type = "LINEAR_MODEL"
+    elif is_neural_network(model):
+        model_type = "NEURAL_NETWORK"
+    else:
+        model_type = None
+    return EXPORTED_MODELS_PATH[model_type]
+
 
 def pymilo_test(model, model_name, test_data):
     """
     Return the pymilo imported model's outputs for given test_data.
 
     :param model: given model
     :type model: any sklearn's model class
@@ -21,17 +44,18 @@
     :type model_name: str
     :param test_data: data for testing
     :type test_data: np.ndarray or list
     :return: imported model's output
     """
     x_test, _ = test_data
 
+    export_model_path = pymilo_export_path(model)
     exported_model = Export(model)
     exported_model_serialized_path = os.path.join(
-        os.getcwd(), "tests", "exported_models", model_name + '.json')
+        os.getcwd(), "tests", export_model_path, model_name + '.json')
     exported_model.save(exported_model_serialized_path)
 
     imported_model = Import(exported_model_serialized_path)
     imported_sklearn_model = imported_model.to_model()
     return imported_sklearn_model.predict(x_test)
```

### Comparing `pymilo-0.1/pymilo/utils/util.py` & `pymilo-0.2/pymilo/utils/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -54,7 +54,38 @@
     if not is_iterable(content):
         return False
     if isinstance(content, ndarray):
         # https://stackoverflow.com/questions/40659212/futurewarning-elementwise-comparison-failed-returning-scalar-but-in-the-futur.
         return False
     else:
         return field in content
+
+
+def get_homogeneous_type(seq):
+    """
+    Check if the given sequence's inner items have the same type or not and if they do, return the associated type.
+
+    :param seq: given sequence
+    :type seq: sequence
+
+    :return: Tuple of (True, inner_type) or (False, None)
+    """
+    iseq = iter(seq)
+    first_type = type(next(iseq))
+    return (
+        True,
+        first_type) if all(
+        (type(x) is first_type) for x in iseq) else (
+            False,
+        None)
+
+
+def all_same(arr):
+    """
+    Check if the given array's items are the same or not.
+
+    :param arr: given array
+    :type arr: array
+
+    :return: bool
+    """
+    return all(x == arr[0] for x in arr)
```

### Comparing `pymilo-0.1/pymilo.egg-info/PKG-INFO` & `pymilo-0.2/pymilo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: pymilo
-Version: 0.1
+Version: 0.2
 Summary: Transportation of ML models
 Home-page: https://github.com/openscilab/pymilo
-Download-URL: https://github.com/openscilab/pymilo/tarball/v0.1
+Download-URL: https://github.com/openscilab/pymilo/tarball/v0.2
 Author: PyMilo Development Team
 Author-email: info@pycm.io
 License: MIT
 Project-URL: Source, https://github.com/openscilab/pymilo
 Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Developers
@@ -29,15 +28,15 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Education
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 
 
 <div align="center">
     <img src="https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png" width="500" height="300">
@@ -115,17 +114,17 @@
 
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)
-- Run `pip install pymilo==0.1`
+- Run `pip install pymilo==0.2`
 ### Source code
-- Download [Version 0.1](https://github.com/openscilab/pymilo/archive/v0.1.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
+- Download [Version 0.2](https://github.com/openscilab/pymilo/archive/v0.2.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/dev.zip)
 - Run `pip install .`
 
 ## Usage
 ### Simple Linear Model Preparation 
 ```pycon
 >>> from sklearn import datasets
 >>> from pymilo import Export, Import
@@ -157,18 +156,19 @@
 ```
 #### Note: `imported_sklearn_model` has the **exact same** functionality as the `model` object earlier.
 
 ## Supported ML Models
 | scikit-learn | PyTorch | 
 | ---------------- | ---------------- | 
 | Linear Models &#x2705; | - | 
-| Neural networks &#x274C; | -  | 
+| Neural networks &#x2705; | -  | 
 | Clustering &#x274C; | -  | 
 | Trees &#x274C; | -  | 
 | Ensemble Models &#x274C; | - | 
+Details are available in [Supported Models](https://github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md).
 
 ## Issues & bug reports
 
 Just fill an issue and describe it. We'll check it ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com "info@openscilab.com"). 
 
 - Please complete the issue template
  
@@ -194,16 +194,40 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.2] - 2023-08-02
+### Added
+- scikit-learn neural network models 
+- `MLP Regressor` model 
+- `MLP Classifier` model
+- `BernoulliRBN` model
+- `SGDOptimizer` transporter
+- `RandomState(MT19937)` transporter
+- `Adamoptimizer` transporter
+- Neural Network chain
+- Neural Network exceptions 
+- `ndarray_to_list` method in `GeneralDataStructureTransporter`
+- `list_to_ndarray` method in `GeneralDataStructureTransporter` 
+- `neural_network_chain.py` chain
+### Changed
+- `GeneralDataStructure` Transporter updated
+- `LabelBinerizer` Transporter updated
+- `linear model` chain updated
+- GeneralDataStructure transporter enhanced
+- LabelBinerizer transporter updated
+- transporters' chain router added to `pymilo func`
+- NeuralNetwork params initialized in `pymilo_param`
+- `pymilo_test` updated to support multiple models
+- `linear_model_chain` refactored
 ## [0.1] - 2023-06-29
 ### Added
 - scikit-learn linear models support
 - `Export` class
 - `Import` class
 
-
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.1...dev
+[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/pymilo/compare/e887108...v0.1
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: pymilo Version: 0.1 Summary: Transportation of ML
+Metadata-Version: 2.1 Name: pymilo Version: 0.2 Summary: Transportation of ML
 models Home-page: https://github.com/openscilab/pymilo Download-URL: https://
-github.com/openscilab/pymilo/tarball/v0.1 Author: PyMilo Development Team
+github.com/openscilab/pymilo/tarball/v0.2 Author: PyMilo Development Team
 Author-email: info@pycm.io License: MIT Project-URL: Source, https://
 github.com/openscilab/pymilo Keywords: python3 python machine_learning ML
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Classifier: Intended
-Audience :: Developers Classifier: Intended Audience :: Education Classifier:
-Intended Audience :: End Users/Desktop Classifier: Intended Audience ::
-Manufacturing Classifier: Intended Audience :: Science/Research Classifier:
-Topic :: Scientific/Engineering :: Information Analysis Classifier: Topic ::
-Education Classifier: Topic :: Scientific/Engineering Classifier: Topic ::
-Scientific/Engineering :: Artificial Intelligence Classifier: Topic ::
-Scientific/Engineering :: Human Machine Interfaces Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Topic :: Scientific/
-Engineering :: Physics Requires-Python: >=3.5 Description-Content-Type: text/
-markdown License-File: LICENSE License-File: AUTHORS.md
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
+Education Classifier: Intended Audience :: End Users/Desktop Classifier:
+Intended Audience :: Manufacturing Classifier: Intended Audience :: Science/
+Research Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Education Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
+Classifier: Topic :: Scientific/Engineering :: Mathematics Classifier: Topic ::
+Scientific/Engineering :: Physics Requires-Python: >=3.6 Description-Content-
+Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
      [https://github.com/openscilab/pymilo/raw/main/otherfiles/logo.png]
 
         [Codecov] [PyPI_version] [built_with_Python3] [Discord_Channel]
 ---------- ## Table of contents * [Overview](https://github.com/openscilab/
 pymilo#overview) * [Installation](https://github.com/openscilab/
 pymilo#installation) * [Usage](https://github.com/openscilab/pymilo#usage) *
 [Issues & Bug Reports](https://github.com/openscilab/pymilo#issues--bug-
@@ -49,17 +48,17 @@
 Github Stars [https://img.shields.io/github/stars/openscilab/
                    pymilo.svg?style=social&label=Stars]
 Branch                     main                                  dev
        [https://github.com/openscilab/ [https://github.com/openscilab/pymilo/
    CI       pymilo/workflows/CI/         workflows/CI/badge.svg?branch=dev]
            badge.svg?branch=main]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install pymilo==0.1` ### Source
-code - Download [Version 0.1](https://github.com/openscilab/pymilo/archive/
-v0.1.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
+packaging.python.org/installing/) - Run `pip install pymilo==0.2` ### Source
+code - Download [Version 0.2](https://github.com/openscilab/pymilo/archive/
+v0.2.zip) or [Latest Source](https://github.com/openscilab/pymilo/archive/
 dev.zip) - Run `pip install .` ## Usage ### Simple Linear Model Preparation
 ```pycon >>> from sklearn import datasets >>> from pymilo import Export, Import
 >>> from sklearn.linear_model import LinearRegression >>> import os >>> X, Y =
 datasets.load_diabetes(return_X_y=True) >>> threshold = 20 >>> X_train, X_test
 = X[:-threshold], X[-threshold:] >>> Y_train, Y_test = Y[:-threshold], Y[-
 threshold:] >>> model = LinearRegression() >>> #### Train the model using the
 training sets >>> model.fit(X_train, Y_train) ``` ### Save Model ```pycon >>>
@@ -68,23 +67,37 @@
 exported_model.save(PATH_TO_JSON_FILE) ``` ### Load Model ```pycon >>> ####
 Import the pymilo-exported model and get a real scikit model >>> imported_model
 = Import(PATH_TO_JSON_FILE) ``` ### Get the associated Scikit model ```pycon
 >>> imported_sklearn_model = imported_model.to_model() ``` #### Note:
 `imported_sklearn_model` has the **exact same** functionality as the `model`
 object earlier. ## Supported ML Models | scikit-learn | PyTorch | | -----------
 ----- | ---------------- | | Linear Models &#x2705; | - | | Neural networks
-&#x274C; | - | | Clustering &#x274C; | - | | Trees &#x274C; | - | | Ensemble
-Models &#x274C; | - | ## Issues & bug reports Just fill an issue and describe
-it. We'll check it ASAP! or send an email to [info@openscilab.com](mailto:
-info@openscilab.com "info@openscilab.com"). - Please complete the issue
-template You can also join our discord server [Discord_Channel] ## Show Your
-Support ### Star this repo Give a â­ï¸ if this project helped you! ### Donate
-to our project If you do like our project and we hope that you do, can you
-please support us? Our project is not and is never going to be working for
-profit. We need the money just so we can continue doing what we do ;-) .
-[PyMilo_Donation] # Changelog All notable changes to this project will be
-documented in this file. The format is based on [Keep a Changelog](http://
-keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning]
-(http://semver.org/spec/v2.0.0.html). ## [Unreleased] ## [0.1] - 2023-06-29 ###
-Added - scikit-learn linear models support - `Export` class - `Import` class
-[Unreleased]: https://github.com/openscilab/pymilo/compare/v0.1...dev [0.1]:
-https://github.com/openscilab/pymilo/compare/e887108...v0.1
+&#x2705; | - | | Clustering &#x274C; | - | | Trees &#x274C; | - | | Ensemble
+Models &#x274C; | - | Details are available in [Supported Models](https://
+github.com/openscilab/pymilo/blob/main/SUPPORTED_MODELS.md). ## Issues & bug
+reports Just fill an issue and describe it. We'll check it ASAP! or send an
+email to [info@openscilab.com](mailto:info@openscilab.com
+"info@openscilab.com"). - Please complete the issue template You can also join
+our discord server [Discord_Channel] ## Show Your Support ### Star this repo
+Give a â­ï¸ if this project helped you! ### Donate to our project If you do
+like our project and we hope that you do, can you please support us? Our
+project is not and is never going to be working for profit. We need the money
+just so we can continue doing what we do ;-) . [PyMilo_Donation] # Changelog
+All notable changes to this project will be documented in this file. The format
+is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
+project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
+## [Unreleased] ## [0.2] - 2023-08-02 ### Added - scikit-learn neural network
+models - `MLP Regressor` model - `MLP Classifier` model - `BernoulliRBN` model
+- `SGDOptimizer` transporter - `RandomState(MT19937)` transporter -
+`Adamoptimizer` transporter - Neural Network chain - Neural Network exceptions
+- `ndarray_to_list` method in `GeneralDataStructureTransporter` -
+`list_to_ndarray` method in `GeneralDataStructureTransporter` -
+`neural_network_chain.py` chain ### Changed - `GeneralDataStructure`
+Transporter updated - `LabelBinerizer` Transporter updated - `linear model`
+chain updated - GeneralDataStructure transporter enhanced - LabelBinerizer
+transporter updated - transporters' chain router added to `pymilo func` -
+NeuralNetwork params initialized in `pymilo_param` - `pymilo_test` updated to
+support multiple models - `linear_model_chain` refactored ## [0.1] - 2023-06-29
+### Added - scikit-learn linear models support - `Export` class - `Import`
+class [Unreleased]: https://github.com/openscilab/pymilo/compare/v0.2...dev
+[0.2]: https://github.com/openscilab/pymilo/compare/v0.1...v0.2 [0.1]: https://
+github.com/openscilab/pymilo/compare/e887108...v0.1
```

### Comparing `pymilo-0.1/setup.py` & `pymilo-0.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,35 +30,34 @@
     name='pymilo',
     packages=[
         'pymilo',
         'pymilo.utils',
         'pymilo.chains',
         'pymilo.transporters',
         'pymilo.exceptions'],
-    version='0.1',
+    version='0.2',
     description='Transportation of ML models',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='PyMilo Development Team',
     author_email='info@pycm.io',
     url='https://github.com/openscilab/pymilo',
-    download_url='https://github.com/openscilab/pymilo/tarball/v0.1',
+    download_url='https://github.com/openscilab/pymilo/tarball/v0.2',
     keywords="python3 python machine_learning ML",
     project_urls={
             'Source': 'https://github.com/openscilab/pymilo',
     },
     install_requires=get_requires(),
-    python_requires='>=3.5',
+    python_requires='>=3.6',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Intended Audience :: Developers',
```


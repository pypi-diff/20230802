# Comparing `tmp/types-aiobotocore-machinelearning-2.5.2.tar.gz` & `tmp/types-aiobotocore-machinelearning-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-machinelearning-2.5.2.tar", last modified: Sat Jul  8 01:43:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-machinelearning-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:36 2023, max compression
```

## Comparing `types-aiobotocore-machinelearning-2.5.2.tar` & `types-aiobotocore-machinelearning-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.874475 types-aiobotocore-machinelearning-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-07-08 01:43:55.870475 types-aiobotocore-machinelearning-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17162 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:55.874475 types-aiobotocore-machinelearning-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.866475 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27994 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6991 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    31719 2023-07-08 01:34:30.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31694 2023-07-08 01:34:30.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-08 01:34:29.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.870475 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18759 2023-07-08 01:43:55.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-08 01:43:55.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:55.000000 types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18695 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17145 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28039 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27994 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10287 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10285 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    31653 2023-08-02 14:42:41.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 2023-08-02 14:42:41.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6335 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-08-02 14:42:40.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.217532 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18695 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:36.000000 types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/LICENSE` & `types-aiobotocore-machinelearning-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/PKG-INFO` & `types-aiobotocore-machinelearning-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore machinelearning type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore machinelearning type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -34,29 +33,29 @@
 <a id="types-aiobotocore-machinelearning"></a>
 
 # types-aiobotocore-machinelearning
 
 [![PyPI - types-aiobotocore-machinelearning](https://img.shields.io/pypi/v/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-machinelearning?color=blue)](https://pypistats.org/packages/types-aiobotocore-machinelearning)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MachineLearning 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -377,93 +376,93 @@
 )
 
 
 def check_value(value: AlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_machinelearning.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_machinelearning.type_defs import (
     TagTypeDef,
-    AddTagsOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
-    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
-    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
-    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
-    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
-    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
-    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
-    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
-    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
-    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
-    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
-    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    AddTagsOutputTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
+    CreateEvaluationOutputTypeDef,
+    CreateMLModelOutputTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
+    DeleteDataSourceOutputTypeDef,
+    DeleteEvaluationOutputTypeDef,
+    DeleteMLModelOutputTypeDef,
+    DeleteTagsOutputTypeDef,
     DescribeTagsOutputTypeDef,
+    GetBatchPredictionOutputTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
+    UpdateDataSourceOutputTypeDef,
+    UpdateEvaluationOutputTypeDef,
+    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
@@ -473,15 +472,15 @@
     CreateDataSourceFromRedshiftInputRequestTypeDef,
     DataSourceTypeDef,
     GetDataSourceOutputTypeDef,
     DescribeDataSourcesOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/README.md` & `types-aiobotocore-machinelearning-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-machinelearning"></a>
 
 # types-aiobotocore-machinelearning
 
 [![PyPI - types-aiobotocore-machinelearning](https://img.shields.io/pypi/v/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-machinelearning?color=blue)](https://pypistats.org/packages/types-aiobotocore-machinelearning)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MachineLearning 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -344,93 +344,93 @@
 )
 
 
 def check_value(value: AlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_machinelearning.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_machinelearning.type_defs import (
     TagTypeDef,
-    AddTagsOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
-    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
-    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
-    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
-    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
-    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
-    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
-    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
-    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
-    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
-    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
-    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    AddTagsOutputTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
+    CreateEvaluationOutputTypeDef,
+    CreateMLModelOutputTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
+    DeleteDataSourceOutputTypeDef,
+    DeleteEvaluationOutputTypeDef,
+    DeleteMLModelOutputTypeDef,
+    DeleteTagsOutputTypeDef,
     DescribeTagsOutputTypeDef,
+    GetBatchPredictionOutputTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
+    UpdateDataSourceOutputTypeDef,
+    UpdateEvaluationOutputTypeDef,
+    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
@@ -440,15 +440,15 @@
     CreateDataSourceFromRedshiftInputRequestTypeDef,
     DataSourceTypeDef,
     GetDataSourceOutputTypeDef,
     DescribeDataSourcesOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/setup.py` & `types-aiobotocore-machinelearning-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-machinelearning",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_machinelearning"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        " mypy-boto3-builder 7.17.1"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
-    keywords="aiobotocore machinelearning type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore machinelearning type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_machinelearning": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/"
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/__init__.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/__init__.pyi` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/__main__.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MachineLearning 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.MachineLearning 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("2.5.2")
+    print("2.5.2.post1")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/client.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/client.pyi` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/literals.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/literals.pyi` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/paginator.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 
@@ -104,15 +104,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 
@@ -130,15 +130,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 
@@ -156,13 +156,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/paginator.pyi` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBatchPredictionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeBatchPredictions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describebatchpredictionspaginator)
         """
 
 class DescribeDataSourcesPaginator(AioPaginator):
@@ -100,15 +100,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDataSourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describedatasourcespaginator)
         """
 
 class DescribeEvaluationsPaginator(AioPaginator):
@@ -125,15 +125,15 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEvaluationsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describeevaluationspaginator)
         """
 
 class DescribeMLModelsPaginator(AioPaginator):
@@ -150,13 +150,13 @@
         GT: str = ...,
         LT: str = ...,
         GE: str = ...,
         LE: str = ...,
         NE: str = ...,
         Prefix: str = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMLModelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning.Paginator.DescribeMLModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/paginators/#describemlmodelspaginator)
         """
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/type_defs.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_machinelearning.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -33,86 +33,85 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "AddTagsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
-    "CreateBatchPredictionOutputTypeDef",
-    "CreateDataSourceFromRDSOutputTypeDef",
-    "CreateDataSourceFromRedshiftOutputTypeDef",
     "S3DataSpecTypeDef",
-    "CreateDataSourceFromS3OutputTypeDef",
     "CreateEvaluationInputRequestTypeDef",
-    "CreateEvaluationOutputTypeDef",
     "CreateMLModelInputRequestTypeDef",
-    "CreateMLModelOutputTypeDef",
     "CreateRealtimeEndpointInputRequestTypeDef",
     "RealtimeEndpointInfoTypeDef",
     "DeleteBatchPredictionInputRequestTypeDef",
-    "DeleteBatchPredictionOutputTypeDef",
     "DeleteDataSourceInputRequestTypeDef",
-    "DeleteDataSourceOutputTypeDef",
     "DeleteEvaluationInputRequestTypeDef",
-    "DeleteEvaluationOutputTypeDef",
     "DeleteMLModelInputRequestTypeDef",
-    "DeleteMLModelOutputTypeDef",
     "DeleteRealtimeEndpointInputRequestTypeDef",
     "DeleteTagsInputRequestTypeDef",
-    "DeleteTagsOutputTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBatchPredictionsInputRequestTypeDef",
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
-    "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
-    "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
-    "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
-    "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
-    "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "AddTagsOutputTypeDef",
+    "CreateBatchPredictionOutputTypeDef",
+    "CreateDataSourceFromRDSOutputTypeDef",
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    "CreateDataSourceFromS3OutputTypeDef",
+    "CreateEvaluationOutputTypeDef",
+    "CreateMLModelOutputTypeDef",
+    "DeleteBatchPredictionOutputTypeDef",
+    "DeleteDataSourceOutputTypeDef",
+    "DeleteEvaluationOutputTypeDef",
+    "DeleteMLModelOutputTypeDef",
+    "DeleteTagsOutputTypeDef",
     "DescribeTagsOutputTypeDef",
+    "GetBatchPredictionOutputTypeDef",
+    "UpdateBatchPredictionOutputTypeDef",
+    "UpdateDataSourceOutputTypeDef",
+    "UpdateEvaluationOutputTypeDef",
+    "UpdateMLModelOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -130,20 +129,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AddTagsOutputTypeDef = TypedDict(
-    "AddTagsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchPredictionTypeDef = TypedDict(
     "BatchPredictionTypeDef",
     {
         "BatchPredictionId": str,
@@ -179,46 +180,20 @@
     "_OptionalCreateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionName": str,
     },
     total=False,
 )
 
-
 class CreateBatchPredictionInputRequestTypeDef(
     _RequiredCreateBatchPredictionInputRequestTypeDef,
     _OptionalCreateBatchPredictionInputRequestTypeDef,
 ):
     pass
 
-
-CreateBatchPredictionOutputTypeDef = TypedDict(
-    "CreateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRDSOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRDSOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3DataSpecTypeDef = TypedDict(
     "_RequiredS3DataSpecTypeDef",
     {
         "DataLocationS3": str,
     },
 )
 _OptionalS3DataSpecTypeDef = TypedDict(
@@ -227,27 +202,17 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaLocationS3": str,
     },
     total=False,
 )
 
-
 class S3DataSpecTypeDef(_RequiredS3DataSpecTypeDef, _OptionalS3DataSpecTypeDef):
     pass
 
-
-CreateDataSourceFromS3OutputTypeDef = TypedDict(
-    "CreateDataSourceFromS3OutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateEvaluationInputRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
     },
@@ -256,29 +221,19 @@
     "_OptionalCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationName": str,
     },
     total=False,
 )
 
-
 class CreateEvaluationInputRequestTypeDef(
     _RequiredCreateEvaluationInputRequestTypeDef, _OptionalCreateEvaluationInputRequestTypeDef
 ):
     pass
 
-
-CreateEvaluationOutputTypeDef = TypedDict(
-    "CreateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredCreateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
         "MLModelType": MLModelTypeType,
         "TrainingDataSourceId": str,
     },
@@ -290,29 +245,19 @@
         "Parameters": Mapping[str, str],
         "Recipe": str,
         "RecipeUri": str,
     },
     total=False,
 )
 
-
 class CreateMLModelInputRequestTypeDef(
     _RequiredCreateMLModelInputRequestTypeDef, _OptionalCreateMLModelInputRequestTypeDef
 ):
     pass
 
-
-CreateMLModelOutputTypeDef = TypedDict(
-    "CreateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateRealtimeEndpointInputRequestTypeDef = TypedDict(
     "CreateRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -330,67 +275,35 @@
 DeleteBatchPredictionInputRequestTypeDef = TypedDict(
     "DeleteBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-DeleteBatchPredictionOutputTypeDef = TypedDict(
-    "DeleteBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDataSourceInputRequestTypeDef = TypedDict(
     "DeleteDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 
-DeleteDataSourceOutputTypeDef = TypedDict(
-    "DeleteDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEvaluationInputRequestTypeDef = TypedDict(
     "DeleteEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
-DeleteEvaluationOutputTypeDef = TypedDict(
-    "DeleteEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMLModelInputRequestTypeDef = TypedDict(
     "DeleteMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
-DeleteMLModelOutputTypeDef = TypedDict(
-    "DeleteMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRealtimeEndpointInputRequestTypeDef = TypedDict(
     "DeleteRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -399,45 +312,29 @@
     {
         "TagKeys": Sequence[str],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-DeleteTagsOutputTypeDef = TypedDict(
-    "DeleteTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FilterVariable": BatchPredictionFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBatchPredictionsInputRequestTypeDef = TypedDict(
     "DescribeBatchPredictionsInputRequestTypeDef",
     {
@@ -452,31 +349,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    {
-        "FilterVariable": DataSourceFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSourcesInputRequestTypeDef = TypedDict(
     "DescribeDataSourcesInputRequestTypeDef",
     {
         "FilterVariable": DataSourceFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -487,31 +367,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    {
-        "FilterVariable": EvaluationFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEvaluationsInputRequestTypeDef = TypedDict(
     "DescribeEvaluationsInputRequestTypeDef",
     {
         "FilterVariable": EvaluationFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -522,31 +385,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
-    {
-        "FilterVariable": MLModelFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMLModelsInputRequestTypeDef = TypedDict(
     "DescribeMLModelsInputRequestTypeDef",
     {
         "FilterVariable": MLModelFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -580,59 +426,33 @@
 GetBatchPredictionInputRequestTypeDef = TypedDict(
     "GetBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-GetBatchPredictionOutputTypeDef = TypedDict(
-    "GetBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "MLModelId": str,
-        "BatchPredictionDataSourceId": str,
-        "InputDataLocationS3": str,
-        "CreatedByIamUser": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Name": str,
-        "Status": EntityStatusType,
-        "OutputUri": str,
-        "LogUri": str,
-        "Message": str,
-        "ComputeTime": int,
-        "FinishedAt": datetime,
-        "StartedAt": datetime,
-        "TotalRecordCount": int,
-        "InvalidRecordCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDataSourceInputRequestTypeDef = TypedDict(
     "_RequiredGetDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalGetDataSourceInputRequestTypeDef = TypedDict(
     "_OptionalGetDataSourceInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
-
 class GetDataSourceInputRequestTypeDef(
     _RequiredGetDataSourceInputRequestTypeDef, _OptionalGetDataSourceInputRequestTypeDef
 ):
     pass
 
-
 GetEvaluationInputRequestTypeDef = TypedDict(
     "GetEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
@@ -646,31 +466,19 @@
     "_OptionalGetMLModelInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
-
 class GetMLModelInputRequestTypeDef(
     _RequiredGetMLModelInputRequestTypeDef, _OptionalGetMLModelInputRequestTypeDef
 ):
     pass
 
-
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PredictInputRequestTypeDef = TypedDict(
     "PredictInputRequestTypeDef",
     {
         "MLModelId": str,
         "Record": Mapping[str, str],
         "PredictEndpoint": str,
     },
@@ -715,73 +523,38 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 UpdateBatchPredictionInputRequestTypeDef = TypedDict(
     "UpdateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
         "BatchPredictionName": str,
     },
 )
 
-UpdateBatchPredictionOutputTypeDef = TypedDict(
-    "UpdateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDataSourceInputRequestTypeDef = TypedDict(
     "UpdateDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSourceName": str,
     },
 )
 
-UpdateDataSourceOutputTypeDef = TypedDict(
-    "UpdateDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEvaluationInputRequestTypeDef = TypedDict(
     "UpdateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "EvaluationName": str,
     },
 )
 
-UpdateEvaluationOutputTypeDef = TypedDict(
-    "UpdateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 _OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
@@ -789,54 +562,198 @@
     {
         "MLModelName": str,
         "ScoreThreshold": float,
     },
     total=False,
 )
 
-
 class UpdateMLModelInputRequestTypeDef(
     _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
 ):
     pass
 
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+    },
+)
 
-UpdateMLModelOutputTypeDef = TypedDict(
-    "UpdateMLModelOutputTypeDef",
+AddTagsOutputTypeDef = TypedDict(
+    "AddTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBatchPredictionOutputTypeDef = TypedDict(
+    "CreateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSourceFromRDSOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRDSOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSourceFromS3OutputTypeDef = TypedDict(
+    "CreateDataSourceFromS3OutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEvaluationOutputTypeDef = TypedDict(
+    "CreateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMLModelOutputTypeDef = TypedDict(
+    "CreateMLModelOutputTypeDef",
     {
         "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
+DeleteBatchPredictionOutputTypeDef = TypedDict(
+    "DeleteBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDataSourceOutputTypeDef = TypedDict(
+    "DeleteDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEvaluationOutputTypeDef = TypedDict(
+    "DeleteEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteMLModelOutputTypeDef = TypedDict(
+    "DeleteMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTagsOutputTypeDef = TypedDict(
+    "DeleteTagsOutputTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBatchPredictionOutputTypeDef = TypedDict(
+    "GetBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "MLModelId": str,
+        "BatchPredictionDataSourceId": str,
+        "InputDataLocationS3": str,
+        "CreatedByIamUser": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Name": str,
+        "Status": EntityStatusType,
+        "OutputUri": str,
+        "LogUri": str,
+        "Message": str,
+        "ComputeTime": int,
+        "FinishedAt": datetime,
+        "StartedAt": datetime,
+        "TotalRecordCount": int,
+        "InvalidRecordCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBatchPredictionOutputTypeDef = TypedDict(
+    "UpdateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDataSourceOutputTypeDef = TypedDict(
+    "UpdateDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEvaluationOutputTypeDef = TypedDict(
+    "UpdateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMLModelOutputTypeDef = TypedDict(
+    "UpdateMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromS3InputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromS3InputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -848,37 +765,35 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
-
 class CreateDataSourceFromS3InputRequestTypeDef(
     _RequiredCreateDataSourceFromS3InputRequestTypeDef,
     _OptionalCreateDataSourceFromS3InputRequestTypeDef,
 ):
     pass
 
-
 CreateRealtimeEndpointOutputTypeDef = TypedDict(
     "CreateRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRealtimeEndpointOutputTypeDef = TypedDict(
     "DeleteRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMLModelOutputTypeDef = TypedDict(
     "GetMLModelOutputTypeDef",
     {
         "MLModelId": str,
@@ -898,15 +813,15 @@
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "Recipe": str,
         "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MLModelTypeDef = TypedDict(
     "MLModelTypeDef",
     {
         "MLModelId": str,
@@ -1004,14 +919,82 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    {
+        "FilterVariable": BatchPredictionFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    {
+        "FilterVariable": DataSourceFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    {
+        "FilterVariable": EvaluationFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
+    {
+        "FilterVariable": MLModelFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
         "InputDataLocationS3": str,
@@ -1043,23 +1026,23 @@
         "Status": EntityStatusType,
         "PerformanceMetrics": PerformanceMetricsTypeDef,
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictOutputTypeDef = TypedDict(
     "PredictOutputTypeDef",
     {
         "Prediction": PredictionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRDSDataSpecTypeDef = TypedDict(
     "_RequiredRDSDataSpecTypeDef",
     {
         "DatabaseInformation": RDSDatabaseTypeDef,
@@ -1078,19 +1061,17 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
-
 class RDSDataSpecTypeDef(_RequiredRDSDataSpecTypeDef, _OptionalRDSDataSpecTypeDef):
     pass
 
-
 RDSMetadataTypeDef = TypedDict(
     "RDSMetadataTypeDef",
     {
         "Database": RDSDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
         "ResourceRole": str,
@@ -1115,19 +1096,17 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
-
 class RedshiftDataSpecTypeDef(_RequiredRedshiftDataSpecTypeDef, _OptionalRedshiftDataSpecTypeDef):
     pass
 
-
 RedshiftMetadataTypeDef = TypedDict(
     "RedshiftMetadataTypeDef",
     {
         "RedshiftDatabase": RedshiftDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
     },
@@ -1135,24 +1114,24 @@
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
     "DescribeMLModelsOutputTypeDef",
     {
         "Results": List[MLModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEvaluationsOutputTypeDef = TypedDict(
     "DescribeEvaluationsOutputTypeDef",
     {
         "Results": List[EvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromRDSInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRDSInputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -1165,22 +1144,20 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
-
 class CreateDataSourceFromRDSInputRequestTypeDef(
     _RequiredCreateDataSourceFromRDSInputRequestTypeDef,
     _OptionalCreateDataSourceFromRDSInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRedshiftInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSpec": RedshiftDataSpecTypeDef,
         "RoleARN": str,
     },
@@ -1190,22 +1167,20 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
-
 class CreateDataSourceFromRedshiftInputRequestTypeDef(
     _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef,
     _OptionalCreateDataSourceFromRedshiftInputRequestTypeDef,
 ):
     pass
 
-
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "DataSourceId": str,
         "DataLocationS3": str,
         "DataRearrangement": str,
         "CreatedByIamUser": str,
@@ -1246,19 +1221,19 @@
         "RDSMetadata": RDSMetadataTypeDef,
         "RoleARN": str,
         "ComputeStatistics": bool,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "DataSourceSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSourcesOutputTypeDef = TypedDict(
     "DescribeDataSourcesOutputTypeDef",
     {
         "Results": List[DataSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/type_defs.pyi` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_machinelearning.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -33,85 +33,86 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "AddTagsOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchPredictionTypeDef",
     "CreateBatchPredictionInputRequestTypeDef",
-    "CreateBatchPredictionOutputTypeDef",
-    "CreateDataSourceFromRDSOutputTypeDef",
-    "CreateDataSourceFromRedshiftOutputTypeDef",
     "S3DataSpecTypeDef",
-    "CreateDataSourceFromS3OutputTypeDef",
     "CreateEvaluationInputRequestTypeDef",
-    "CreateEvaluationOutputTypeDef",
     "CreateMLModelInputRequestTypeDef",
-    "CreateMLModelOutputTypeDef",
     "CreateRealtimeEndpointInputRequestTypeDef",
     "RealtimeEndpointInfoTypeDef",
     "DeleteBatchPredictionInputRequestTypeDef",
-    "DeleteBatchPredictionOutputTypeDef",
     "DeleteDataSourceInputRequestTypeDef",
-    "DeleteDataSourceOutputTypeDef",
     "DeleteEvaluationInputRequestTypeDef",
-    "DeleteEvaluationOutputTypeDef",
     "DeleteMLModelInputRequestTypeDef",
-    "DeleteMLModelOutputTypeDef",
     "DeleteRealtimeEndpointInputRequestTypeDef",
     "DeleteTagsInputRequestTypeDef",
-    "DeleteTagsOutputTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBatchPredictionsInputRequestTypeDef",
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
     "DescribeDataSourcesInputRequestTypeDef",
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
     "DescribeEvaluationsInputRequestTypeDef",
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "DescribeMLModelsInputRequestTypeDef",
     "DescribeTagsInputRequestTypeDef",
     "PerformanceMetricsTypeDef",
     "GetBatchPredictionInputRequestTypeDef",
-    "GetBatchPredictionOutputTypeDef",
     "GetDataSourceInputRequestTypeDef",
     "GetEvaluationInputRequestTypeDef",
     "GetMLModelInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictInputRequestTypeDef",
     "PredictionTypeDef",
     "RDSDatabaseCredentialsTypeDef",
     "RDSDatabaseTypeDef",
     "RedshiftDatabaseCredentialsTypeDef",
     "RedshiftDatabaseTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateBatchPredictionInputRequestTypeDef",
-    "UpdateBatchPredictionOutputTypeDef",
     "UpdateDataSourceInputRequestTypeDef",
-    "UpdateDataSourceOutputTypeDef",
     "UpdateEvaluationInputRequestTypeDef",
-    "UpdateEvaluationOutputTypeDef",
     "UpdateMLModelInputRequestTypeDef",
-    "UpdateMLModelOutputTypeDef",
     "AddTagsInputRequestTypeDef",
+    "AddTagsOutputTypeDef",
+    "CreateBatchPredictionOutputTypeDef",
+    "CreateDataSourceFromRDSOutputTypeDef",
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    "CreateDataSourceFromS3OutputTypeDef",
+    "CreateEvaluationOutputTypeDef",
+    "CreateMLModelOutputTypeDef",
+    "DeleteBatchPredictionOutputTypeDef",
+    "DeleteDataSourceOutputTypeDef",
+    "DeleteEvaluationOutputTypeDef",
+    "DeleteMLModelOutputTypeDef",
+    "DeleteTagsOutputTypeDef",
     "DescribeTagsOutputTypeDef",
+    "GetBatchPredictionOutputTypeDef",
+    "UpdateBatchPredictionOutputTypeDef",
+    "UpdateDataSourceOutputTypeDef",
+    "UpdateEvaluationOutputTypeDef",
+    "UpdateMLModelOutputTypeDef",
     "DescribeBatchPredictionsOutputTypeDef",
     "CreateDataSourceFromS3InputRequestTypeDef",
     "CreateRealtimeEndpointOutputTypeDef",
     "DeleteRealtimeEndpointOutputTypeDef",
     "GetMLModelOutputTypeDef",
     "MLModelTypeDef",
     "DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef",
     "DescribeDataSourcesInputDataSourceAvailableWaitTypeDef",
     "DescribeEvaluationsInputEvaluationAvailableWaitTypeDef",
     "DescribeMLModelsInputMLModelAvailableWaitTypeDef",
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
     "EvaluationTypeDef",
     "GetEvaluationOutputTypeDef",
     "PredictOutputTypeDef",
     "RDSDataSpecTypeDef",
     "RDSMetadataTypeDef",
     "RedshiftDataSpecTypeDef",
     "RedshiftMetadataTypeDef",
@@ -129,20 +130,22 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
-AddTagsOutputTypeDef = TypedDict(
-    "AddTagsOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchPredictionTypeDef = TypedDict(
     "BatchPredictionTypeDef",
     {
         "BatchPredictionId": str,
@@ -178,43 +181,21 @@
     "_OptionalCreateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionName": str,
     },
     total=False,
 )
 
+
 class CreateBatchPredictionInputRequestTypeDef(
     _RequiredCreateBatchPredictionInputRequestTypeDef,
     _OptionalCreateBatchPredictionInputRequestTypeDef,
 ):
     pass
 
-CreateBatchPredictionOutputTypeDef = TypedDict(
-    "CreateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRDSOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRDSOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
-    "CreateDataSourceFromRedshiftOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredS3DataSpecTypeDef = TypedDict(
     "_RequiredS3DataSpecTypeDef",
     {
         "DataLocationS3": str,
     },
 )
@@ -224,24 +205,18 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaLocationS3": str,
     },
     total=False,
 )
 
+
 class S3DataSpecTypeDef(_RequiredS3DataSpecTypeDef, _OptionalS3DataSpecTypeDef):
     pass
 
-CreateDataSourceFromS3OutputTypeDef = TypedDict(
-    "CreateDataSourceFromS3OutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateEvaluationInputRequestTypeDef = TypedDict(
     "_RequiredCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
@@ -251,26 +226,20 @@
     "_OptionalCreateEvaluationInputRequestTypeDef",
     {
         "EvaluationName": str,
     },
     total=False,
 )
 
+
 class CreateEvaluationInputRequestTypeDef(
     _RequiredCreateEvaluationInputRequestTypeDef, _OptionalCreateEvaluationInputRequestTypeDef
 ):
     pass
 
-CreateEvaluationOutputTypeDef = TypedDict(
-    "CreateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredCreateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
         "MLModelType": MLModelTypeType,
         "TrainingDataSourceId": str,
@@ -283,26 +252,20 @@
         "Parameters": Mapping[str, str],
         "Recipe": str,
         "RecipeUri": str,
     },
     total=False,
 )
 
+
 class CreateMLModelInputRequestTypeDef(
     _RequiredCreateMLModelInputRequestTypeDef, _OptionalCreateMLModelInputRequestTypeDef
 ):
     pass
 
-CreateMLModelOutputTypeDef = TypedDict(
-    "CreateMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 CreateRealtimeEndpointInputRequestTypeDef = TypedDict(
     "CreateRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
@@ -321,67 +284,35 @@
 DeleteBatchPredictionInputRequestTypeDef = TypedDict(
     "DeleteBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-DeleteBatchPredictionOutputTypeDef = TypedDict(
-    "DeleteBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDataSourceInputRequestTypeDef = TypedDict(
     "DeleteDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 
-DeleteDataSourceOutputTypeDef = TypedDict(
-    "DeleteDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteEvaluationInputRequestTypeDef = TypedDict(
     "DeleteEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
-DeleteEvaluationOutputTypeDef = TypedDict(
-    "DeleteEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteMLModelInputRequestTypeDef = TypedDict(
     "DeleteMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
-DeleteMLModelOutputTypeDef = TypedDict(
-    "DeleteMLModelOutputTypeDef",
-    {
-        "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteRealtimeEndpointInputRequestTypeDef = TypedDict(
     "DeleteRealtimeEndpointInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 
@@ -390,45 +321,29 @@
     {
         "TagKeys": Sequence[str],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
     },
 )
 
-DeleteTagsOutputTypeDef = TypedDict(
-    "DeleteTagsOutputTypeDef",
-    {
-        "ResourceId": str,
-        "ResourceType": TaggableResourceTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
-    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "FilterVariable": BatchPredictionFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBatchPredictionsInputRequestTypeDef = TypedDict(
     "DescribeBatchPredictionsInputRequestTypeDef",
     {
@@ -443,31 +358,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
-    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
-    {
-        "FilterVariable": DataSourceFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDataSourcesInputRequestTypeDef = TypedDict(
     "DescribeDataSourcesInputRequestTypeDef",
     {
         "FilterVariable": DataSourceFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -478,31 +376,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
-    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
-    {
-        "FilterVariable": EvaluationFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeEvaluationsInputRequestTypeDef = TypedDict(
     "DescribeEvaluationsInputRequestTypeDef",
     {
         "FilterVariable": EvaluationFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -513,31 +394,14 @@
         "SortOrder": SortOrderType,
         "NextToken": str,
         "Limit": int,
     },
     total=False,
 )
 
-DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
-    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
-    {
-        "FilterVariable": MLModelFilterVariableType,
-        "EQ": str,
-        "GT": str,
-        "LT": str,
-        "GE": str,
-        "LE": str,
-        "NE": str,
-        "Prefix": str,
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMLModelsInputRequestTypeDef = TypedDict(
     "DescribeMLModelsInputRequestTypeDef",
     {
         "FilterVariable": MLModelFilterVariableType,
         "EQ": str,
         "GT": str,
         "LT": str,
@@ -571,57 +435,35 @@
 GetBatchPredictionInputRequestTypeDef = TypedDict(
     "GetBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
     },
 )
 
-GetBatchPredictionOutputTypeDef = TypedDict(
-    "GetBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "MLModelId": str,
-        "BatchPredictionDataSourceId": str,
-        "InputDataLocationS3": str,
-        "CreatedByIamUser": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "Name": str,
-        "Status": EntityStatusType,
-        "OutputUri": str,
-        "LogUri": str,
-        "Message": str,
-        "ComputeTime": int,
-        "FinishedAt": datetime,
-        "StartedAt": datetime,
-        "TotalRecordCount": int,
-        "InvalidRecordCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDataSourceInputRequestTypeDef = TypedDict(
     "_RequiredGetDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
     },
 )
 _OptionalGetDataSourceInputRequestTypeDef = TypedDict(
     "_OptionalGetDataSourceInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
+
 class GetDataSourceInputRequestTypeDef(
     _RequiredGetDataSourceInputRequestTypeDef, _OptionalGetDataSourceInputRequestTypeDef
 ):
     pass
 
+
 GetEvaluationInputRequestTypeDef = TypedDict(
     "GetEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
     },
 )
 
@@ -635,28 +477,20 @@
     "_OptionalGetMLModelInputRequestTypeDef",
     {
         "Verbose": bool,
     },
     total=False,
 )
 
+
 class GetMLModelInputRequestTypeDef(
     _RequiredGetMLModelInputRequestTypeDef, _OptionalGetMLModelInputRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
 
 PredictInputRequestTypeDef = TypedDict(
     "PredictInputRequestTypeDef",
     {
         "MLModelId": str,
         "Record": Mapping[str, str],
         "PredictEndpoint": str,
@@ -702,73 +536,38 @@
     "RedshiftDatabaseTypeDef",
     {
         "DatabaseName": str,
         "ClusterIdentifier": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 UpdateBatchPredictionInputRequestTypeDef = TypedDict(
     "UpdateBatchPredictionInputRequestTypeDef",
     {
         "BatchPredictionId": str,
         "BatchPredictionName": str,
     },
 )
 
-UpdateBatchPredictionOutputTypeDef = TypedDict(
-    "UpdateBatchPredictionOutputTypeDef",
-    {
-        "BatchPredictionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateDataSourceInputRequestTypeDef = TypedDict(
     "UpdateDataSourceInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSourceName": str,
     },
 )
 
-UpdateDataSourceOutputTypeDef = TypedDict(
-    "UpdateDataSourceOutputTypeDef",
-    {
-        "DataSourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEvaluationInputRequestTypeDef = TypedDict(
     "UpdateEvaluationInputRequestTypeDef",
     {
         "EvaluationId": str,
         "EvaluationName": str,
     },
 )
 
-UpdateEvaluationOutputTypeDef = TypedDict(
-    "UpdateEvaluationOutputTypeDef",
-    {
-        "EvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateMLModelInputRequestTypeDef = TypedDict(
     "_RequiredUpdateMLModelInputRequestTypeDef",
     {
         "MLModelId": str,
     },
 )
 _OptionalUpdateMLModelInputRequestTypeDef = TypedDict(
@@ -776,52 +575,200 @@
     {
         "MLModelName": str,
         "ScoreThreshold": float,
     },
     total=False,
 )
 
+
 class UpdateMLModelInputRequestTypeDef(
     _RequiredUpdateMLModelInputRequestTypeDef, _OptionalUpdateMLModelInputRequestTypeDef
 ):
     pass
 
-UpdateMLModelOutputTypeDef = TypedDict(
-    "UpdateMLModelOutputTypeDef",
+
+AddTagsInputRequestTypeDef = TypedDict(
+    "AddTagsInputRequestTypeDef",
+    {
+        "Tags": Sequence[TagTypeDef],
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+    },
+)
+
+AddTagsOutputTypeDef = TypedDict(
+    "AddTagsOutputTypeDef",
+    {
+        "ResourceId": str,
+        "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateBatchPredictionOutputTypeDef = TypedDict(
+    "CreateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSourceFromRDSOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRDSOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSourceFromRedshiftOutputTypeDef = TypedDict(
+    "CreateDataSourceFromRedshiftOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDataSourceFromS3OutputTypeDef = TypedDict(
+    "CreateDataSourceFromS3OutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateEvaluationOutputTypeDef = TypedDict(
+    "CreateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMLModelOutputTypeDef = TypedDict(
+    "CreateMLModelOutputTypeDef",
     {
         "MLModelId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddTagsInputRequestTypeDef = TypedDict(
-    "AddTagsInputRequestTypeDef",
+DeleteBatchPredictionOutputTypeDef = TypedDict(
+    "DeleteBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteDataSourceOutputTypeDef = TypedDict(
+    "DeleteDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteEvaluationOutputTypeDef = TypedDict(
+    "DeleteEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteMLModelOutputTypeDef = TypedDict(
+    "DeleteMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteTagsOutputTypeDef = TypedDict(
+    "DeleteTagsOutputTypeDef",
     {
-        "Tags": Sequence[TagTypeDef],
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTagsOutputTypeDef = TypedDict(
     "DescribeTagsOutputTypeDef",
     {
         "ResourceId": str,
         "ResourceType": TaggableResourceTypeType,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetBatchPredictionOutputTypeDef = TypedDict(
+    "GetBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "MLModelId": str,
+        "BatchPredictionDataSourceId": str,
+        "InputDataLocationS3": str,
+        "CreatedByIamUser": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "Name": str,
+        "Status": EntityStatusType,
+        "OutputUri": str,
+        "LogUri": str,
+        "Message": str,
+        "ComputeTime": int,
+        "FinishedAt": datetime,
+        "StartedAt": datetime,
+        "TotalRecordCount": int,
+        "InvalidRecordCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateBatchPredictionOutputTypeDef = TypedDict(
+    "UpdateBatchPredictionOutputTypeDef",
+    {
+        "BatchPredictionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDataSourceOutputTypeDef = TypedDict(
+    "UpdateDataSourceOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEvaluationOutputTypeDef = TypedDict(
+    "UpdateEvaluationOutputTypeDef",
+    {
+        "EvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMLModelOutputTypeDef = TypedDict(
+    "UpdateMLModelOutputTypeDef",
+    {
+        "MLModelId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBatchPredictionsOutputTypeDef = TypedDict(
     "DescribeBatchPredictionsOutputTypeDef",
     {
         "Results": List[BatchPredictionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromS3InputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromS3InputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -833,35 +780,37 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
+
 class CreateDataSourceFromS3InputRequestTypeDef(
     _RequiredCreateDataSourceFromS3InputRequestTypeDef,
     _OptionalCreateDataSourceFromS3InputRequestTypeDef,
 ):
     pass
 
+
 CreateRealtimeEndpointOutputTypeDef = TypedDict(
     "CreateRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRealtimeEndpointOutputTypeDef = TypedDict(
     "DeleteRealtimeEndpointOutputTypeDef",
     {
         "MLModelId": str,
         "RealtimeEndpointInfo": RealtimeEndpointInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMLModelOutputTypeDef = TypedDict(
     "GetMLModelOutputTypeDef",
     {
         "MLModelId": str,
@@ -881,15 +830,15 @@
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "Recipe": str,
         "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MLModelTypeDef = TypedDict(
     "MLModelTypeDef",
     {
         "MLModelId": str,
@@ -987,14 +936,82 @@
         "NextToken": str,
         "Limit": int,
         "WaiterConfig": WaiterConfigTypeDef,
     },
     total=False,
 )
 
+DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef = TypedDict(
+    "DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef",
+    {
+        "FilterVariable": BatchPredictionFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef = TypedDict(
+    "DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef",
+    {
+        "FilterVariable": DataSourceFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef = TypedDict(
+    "DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef",
+    {
+        "FilterVariable": EvaluationFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMLModelsInputDescribeMLModelsPaginateTypeDef = TypedDict(
+    "DescribeMLModelsInputDescribeMLModelsPaginateTypeDef",
+    {
+        "FilterVariable": MLModelFilterVariableType,
+        "EQ": str,
+        "GT": str,
+        "LT": str,
+        "GE": str,
+        "LE": str,
+        "NE": str,
+        "Prefix": str,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 EvaluationTypeDef = TypedDict(
     "EvaluationTypeDef",
     {
         "EvaluationId": str,
         "MLModelId": str,
         "EvaluationDataSourceId": str,
         "InputDataLocationS3": str,
@@ -1026,23 +1043,23 @@
         "Status": EntityStatusType,
         "PerformanceMetrics": PerformanceMetricsTypeDef,
         "LogUri": str,
         "Message": str,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictOutputTypeDef = TypedDict(
     "PredictOutputTypeDef",
     {
         "Prediction": PredictionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRDSDataSpecTypeDef = TypedDict(
     "_RequiredRDSDataSpecTypeDef",
     {
         "DatabaseInformation": RDSDatabaseTypeDef,
@@ -1061,17 +1078,19 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
+
 class RDSDataSpecTypeDef(_RequiredRDSDataSpecTypeDef, _OptionalRDSDataSpecTypeDef):
     pass
 
+
 RDSMetadataTypeDef = TypedDict(
     "RDSMetadataTypeDef",
     {
         "Database": RDSDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
         "ResourceRole": str,
@@ -1096,17 +1115,19 @@
         "DataRearrangement": str,
         "DataSchema": str,
         "DataSchemaUri": str,
     },
     total=False,
 )
 
+
 class RedshiftDataSpecTypeDef(_RequiredRedshiftDataSpecTypeDef, _OptionalRedshiftDataSpecTypeDef):
     pass
 
+
 RedshiftMetadataTypeDef = TypedDict(
     "RedshiftMetadataTypeDef",
     {
         "RedshiftDatabase": RedshiftDatabaseTypeDef,
         "DatabaseUserName": str,
         "SelectSqlQuery": str,
     },
@@ -1114,24 +1135,24 @@
 )
 
 DescribeMLModelsOutputTypeDef = TypedDict(
     "DescribeMLModelsOutputTypeDef",
     {
         "Results": List[MLModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEvaluationsOutputTypeDef = TypedDict(
     "DescribeEvaluationsOutputTypeDef",
     {
         "Results": List[EvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceFromRDSInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRDSInputRequestTypeDef",
     {
         "DataSourceId": str,
@@ -1144,20 +1165,22 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
+
 class CreateDataSourceFromRDSInputRequestTypeDef(
     _RequiredCreateDataSourceFromRDSInputRequestTypeDef,
     _OptionalCreateDataSourceFromRDSInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceFromRedshiftInputRequestTypeDef",
     {
         "DataSourceId": str,
         "DataSpec": RedshiftDataSpecTypeDef,
         "RoleARN": str,
     },
@@ -1167,20 +1190,22 @@
     {
         "DataSourceName": str,
         "ComputeStatistics": bool,
     },
     total=False,
 )
 
+
 class CreateDataSourceFromRedshiftInputRequestTypeDef(
     _RequiredCreateDataSourceFromRedshiftInputRequestTypeDef,
     _OptionalCreateDataSourceFromRedshiftInputRequestTypeDef,
 ):
     pass
 
+
 DataSourceTypeDef = TypedDict(
     "DataSourceTypeDef",
     {
         "DataSourceId": str,
         "DataLocationS3": str,
         "DataRearrangement": str,
         "CreatedByIamUser": str,
@@ -1221,19 +1246,19 @@
         "RDSMetadata": RDSMetadataTypeDef,
         "RoleARN": str,
         "ComputeStatistics": bool,
         "ComputeTime": int,
         "FinishedAt": datetime,
         "StartedAt": datetime,
         "DataSourceSchema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDataSourcesOutputTypeDef = TypedDict(
     "DescribeDataSourcesOutputTypeDef",
     {
         "Results": List[DataSourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/waiter.py` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning/waiter.pyi` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/PKG-INFO` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-machinelearning
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MachineLearning 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore machinelearning type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore machinelearning type-annotations botocore mypy typeshed autocomplete
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
@@ -34,29 +33,29 @@
 <a id="types-aiobotocore-machinelearning"></a>
 
 # types-aiobotocore-machinelearning
 
 [![PyPI - types-aiobotocore-machinelearning](https://img.shields.io/pypi/v/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-machinelearning.svg?color=blue)](https://pypi.org/project/types-aiobotocore-machinelearning)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-machinelearning?color=blue)](https://pypistats.org/packages/types-aiobotocore-machinelearning)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-machinelearning)](https://pepy.tech/project/types-aiobotocore-machinelearning)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MachineLearning 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/machinelearning.html#MachineLearning)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.17.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [types-aiobotocore](https://pypi.org/project/types-aiobotocore/) page and in
 [types-aiobotocore-machinelearning docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_machinelearning/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +74,15 @@
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Literals](#literals)
-    - [Typed dictionaries](#typed-dictionaries)
+    - [Type definitions](#type-definitions)
   - [How it works](#how-it-works)
   - [What's new](#what's-new)
     - [Implemented features](#implemented-features)
     - [Latest changes](#latest-changes)
   - [Versioning](#versioning)
   - [Thank you](#thank-you)
   - [Documentation](#documentation)
@@ -377,93 +376,93 @@
 )
 
 
 def check_value(value: AlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_machinelearning.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_machinelearning.type_defs import (
     TagTypeDef,
-    AddTagsOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchPredictionTypeDef,
     CreateBatchPredictionInputRequestTypeDef,
-    CreateBatchPredictionOutputTypeDef,
-    CreateDataSourceFromRDSOutputTypeDef,
-    CreateDataSourceFromRedshiftOutputTypeDef,
     S3DataSpecTypeDef,
-    CreateDataSourceFromS3OutputTypeDef,
     CreateEvaluationInputRequestTypeDef,
-    CreateEvaluationOutputTypeDef,
     CreateMLModelInputRequestTypeDef,
-    CreateMLModelOutputTypeDef,
     CreateRealtimeEndpointInputRequestTypeDef,
     RealtimeEndpointInfoTypeDef,
     DeleteBatchPredictionInputRequestTypeDef,
-    DeleteBatchPredictionOutputTypeDef,
     DeleteDataSourceInputRequestTypeDef,
-    DeleteDataSourceOutputTypeDef,
     DeleteEvaluationInputRequestTypeDef,
-    DeleteEvaluationOutputTypeDef,
     DeleteMLModelInputRequestTypeDef,
-    DeleteMLModelOutputTypeDef,
     DeleteRealtimeEndpointInputRequestTypeDef,
     DeleteTagsInputRequestTypeDef,
-    DeleteTagsOutputTypeDef,
     WaiterConfigTypeDef,
-    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBatchPredictionsInputRequestTypeDef,
-    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
     DescribeDataSourcesInputRequestTypeDef,
-    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
     DescribeEvaluationsInputRequestTypeDef,
-    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     DescribeMLModelsInputRequestTypeDef,
     DescribeTagsInputRequestTypeDef,
     PerformanceMetricsTypeDef,
     GetBatchPredictionInputRequestTypeDef,
-    GetBatchPredictionOutputTypeDef,
     GetDataSourceInputRequestTypeDef,
     GetEvaluationInputRequestTypeDef,
     GetMLModelInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PredictInputRequestTypeDef,
     PredictionTypeDef,
     RDSDatabaseCredentialsTypeDef,
     RDSDatabaseTypeDef,
     RedshiftDatabaseCredentialsTypeDef,
     RedshiftDatabaseTypeDef,
-    ResponseMetadataTypeDef,
     UpdateBatchPredictionInputRequestTypeDef,
-    UpdateBatchPredictionOutputTypeDef,
     UpdateDataSourceInputRequestTypeDef,
-    UpdateDataSourceOutputTypeDef,
     UpdateEvaluationInputRequestTypeDef,
-    UpdateEvaluationOutputTypeDef,
     UpdateMLModelInputRequestTypeDef,
-    UpdateMLModelOutputTypeDef,
     AddTagsInputRequestTypeDef,
+    AddTagsOutputTypeDef,
+    CreateBatchPredictionOutputTypeDef,
+    CreateDataSourceFromRDSOutputTypeDef,
+    CreateDataSourceFromRedshiftOutputTypeDef,
+    CreateDataSourceFromS3OutputTypeDef,
+    CreateEvaluationOutputTypeDef,
+    CreateMLModelOutputTypeDef,
+    DeleteBatchPredictionOutputTypeDef,
+    DeleteDataSourceOutputTypeDef,
+    DeleteEvaluationOutputTypeDef,
+    DeleteMLModelOutputTypeDef,
+    DeleteTagsOutputTypeDef,
     DescribeTagsOutputTypeDef,
+    GetBatchPredictionOutputTypeDef,
+    UpdateBatchPredictionOutputTypeDef,
+    UpdateDataSourceOutputTypeDef,
+    UpdateEvaluationOutputTypeDef,
+    UpdateMLModelOutputTypeDef,
     DescribeBatchPredictionsOutputTypeDef,
     CreateDataSourceFromS3InputRequestTypeDef,
     CreateRealtimeEndpointOutputTypeDef,
     DeleteRealtimeEndpointOutputTypeDef,
     GetMLModelOutputTypeDef,
     MLModelTypeDef,
     DescribeBatchPredictionsInputBatchPredictionAvailableWaitTypeDef,
     DescribeDataSourcesInputDataSourceAvailableWaitTypeDef,
     DescribeEvaluationsInputEvaluationAvailableWaitTypeDef,
     DescribeMLModelsInputMLModelAvailableWaitTypeDef,
+    DescribeBatchPredictionsInputDescribeBatchPredictionsPaginateTypeDef,
+    DescribeDataSourcesInputDescribeDataSourcesPaginateTypeDef,
+    DescribeEvaluationsInputDescribeEvaluationsPaginateTypeDef,
+    DescribeMLModelsInputDescribeMLModelsPaginateTypeDef,
     EvaluationTypeDef,
     GetEvaluationOutputTypeDef,
     PredictOutputTypeDef,
     RDSDataSpecTypeDef,
     RDSMetadataTypeDef,
     RedshiftDataSpecTypeDef,
     RedshiftMetadataTypeDef,
@@ -473,15 +472,15 @@
     CreateDataSourceFromRedshiftInputRequestTypeDef,
     DataSourceTypeDef,
     GetDataSourceOutputTypeDef,
     DescribeDataSourcesOutputTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-machinelearning-2.5.2/types_aiobotocore_machinelearning.egg-info/SOURCES.txt` & `types-aiobotocore-machinelearning-2.5.2.post1/types_aiobotocore_machinelearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*


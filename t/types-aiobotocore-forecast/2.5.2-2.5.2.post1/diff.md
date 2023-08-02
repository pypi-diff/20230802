# Comparing `tmp/types-aiobotocore-forecast-2.5.2.tar.gz` & `tmp/types-aiobotocore-forecast-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-forecast-2.5.2.tar", last modified: Sat Jul  8 01:43:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-forecast-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
```

## Comparing `types-aiobotocore-forecast-2.5.2.tar` & `types-aiobotocore-forecast-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:39.734171 types-aiobotocore-forecast-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23624 2023-07-08 01:43:39.734171 types-aiobotocore-forecast-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:39.734171 types-aiobotocore-forecast-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:39.734171 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54437 2023-07-08 01:31:02.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54351 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-07-08 01:31:02.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-07-08 01:31:02.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17837 2023-07-08 01:31:02.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    17821 2023-07-08 01:31:02.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    65478 2023-07-08 01:31:04.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    65425 2023-07-08 01:31:04.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:01.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:39.734171 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23624 2023-07-08 01:43:39.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:43:39.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:39.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:39.000000 types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.241582 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3667 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54527 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54441 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11543 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17809 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17793 2023-08-02 14:38:54.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    72389 2023-08-02 14:38:57.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72322 2023-08-02 14:38:56.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:53.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.249582 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24420 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:52:19.000000 types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-forecast-2.5.2/LICENSE` & `types-aiobotocore-forecast-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2/PKG-INFO` & `types-aiobotocore-forecast-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecast
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ForecastService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ForecastService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore forecast type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore forecast type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-forecast"></a>
 
 # types-aiobotocore-forecast
 
 [![PyPI - types-aiobotocore-forecast](https://img.shields.io/pypi/v/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-forecast?color=blue)](https://pypistats.org/packages/types-aiobotocore-forecast)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecast)](https://pepy.tech/project/types-aiobotocore-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ForecastService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [types-aiobotocore-forecast docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +73,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -383,49 +382,39 @@
 )
 
 
 def check_value(value: AttributeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_forecast.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_forecast.type_defs import (
     ActionTypeDef,
+    AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
+    AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
+    CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
+    ResponseMetadataTypeDef,
     ExplainabilityConfigTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -440,107 +429,128 @@
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
+    FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
     SupplementaryFeatureTypeDef,
     IntegerParameterRangeTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
-    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
-    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
+    FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
-    CreateAutoPredictorRequestRequestTypeDef,
     DescribeAutoPredictorResponseTypeDef,
+    CreateAutoPredictorRequestRequestTypeDef,
+    DataConfigUnionTypeDef,
     BaselineTypeDef,
     ListExplainabilitiesResponseTypeDef,
     CreateExplainabilityExportRequestRequestTypeDef,
     CreateForecastExportJobRequestRequestTypeDef,
     CreatePredictorBacktestExportJobRequestRequestTypeDef,
     CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -551,46 +561,58 @@
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     ListPredictorsResponseTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    InputDataConfigUnionTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    CreateExplainabilityRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
+    TimeSeriesIdentifiersOutputTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    CreateExplainabilityRequestRequestTypeDef,
+    SchemaUnionTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
+    FeaturizationConfigUnionTypeDef,
     CreatePredictorRequestRequestTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
+    DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
-    DescribeWhatIfForecastResponseTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    CreateForecastRequestRequestTypeDef,
-    CreateWhatIfAnalysisRequestRequestTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
+    CreateForecastRequestRequestTypeDef,
+    CreateWhatIfAnalysisRequestRequestTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_value() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-forecast-2.5.2/README.md` & `types-aiobotocore-forecast-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-forecast"></a>
 
 # types-aiobotocore-forecast
 
 [![PyPI - types-aiobotocore-forecast](https://img.shields.io/pypi/v/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-forecast?color=blue)](https://pypistats.org/packages/types-aiobotocore-forecast)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecast)](https://pepy.tech/project/types-aiobotocore-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ForecastService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [types-aiobotocore-forecast docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +41,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -350,49 +350,39 @@
 )
 
 
 def check_value(value: AttributeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_forecast.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_forecast.type_defs import (
     ActionTypeDef,
+    AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
+    AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
+    CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
+    ResponseMetadataTypeDef,
     ExplainabilityConfigTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -407,107 +397,128 @@
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
+    FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
     SupplementaryFeatureTypeDef,
     IntegerParameterRangeTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
-    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
-    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
+    FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
-    CreateAutoPredictorRequestRequestTypeDef,
     DescribeAutoPredictorResponseTypeDef,
+    CreateAutoPredictorRequestRequestTypeDef,
+    DataConfigUnionTypeDef,
     BaselineTypeDef,
     ListExplainabilitiesResponseTypeDef,
     CreateExplainabilityExportRequestRequestTypeDef,
     CreateForecastExportJobRequestRequestTypeDef,
     CreatePredictorBacktestExportJobRequestRequestTypeDef,
     CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -518,46 +529,58 @@
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     ListPredictorsResponseTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    InputDataConfigUnionTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    CreateExplainabilityRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
+    TimeSeriesIdentifiersOutputTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    CreateExplainabilityRequestRequestTypeDef,
+    SchemaUnionTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
+    FeaturizationConfigUnionTypeDef,
     CreatePredictorRequestRequestTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
+    DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
-    DescribeWhatIfForecastResponseTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    CreateForecastRequestRequestTypeDef,
-    CreateWhatIfAnalysisRequestRequestTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
+    CreateForecastRequestRequestTypeDef,
+    CreateWhatIfAnalysisRequestRequestTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_value() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-forecast-2.5.2/setup.py` & `types-aiobotocore-forecast-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-forecast",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_forecast"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ForecastService 2.5.2 service generated with"
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
-    keywords="aiobotocore forecast type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore forecast type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_forecast": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/"
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/__init__.py` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/__init__.pyi` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/__main__.py` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ForecastService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ForecastService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService\nOther"
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

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/client.py` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
-    DataConfigTypeDef,
+    DataConfigUnionTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -75,19 +75,19 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
-    FeaturizationConfigTypeDef,
+    FeaturizationConfigUnionTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    HyperParameterTuningJobConfigTypeDef,
-    InputDataConfigTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
+    InputDataConfigUnionTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListForecastsResponseTypeDef,
@@ -96,20 +96,20 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    TimeSeriesReplacementsDataSourceTypeDef,
-    TimeSeriesSelectorTypeDef,
-    TimeSeriesTransformationTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -172,15 +172,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: DataConfigTypeDef = ...,
+        DataConfig: DataConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -194,15 +194,15 @@
 
     async def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: SchemaTypeDef,
+        Schema: SchemaUnionTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -249,15 +249,15 @@
     async def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: SchemaTypeDef = ...,
+        Schema: SchemaUnionTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -286,15 +286,15 @@
     async def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_forecast)
@@ -328,24 +328,24 @@
         """
 
     async def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: InputDataConfigTypeDef,
-        FeaturizationConfig: FeaturizationConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
+        FeaturizationConfig: FeaturizationConfigUnionTypeDef,
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
+        HPOConfig: HyperParameterTuningJobConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -371,15 +371,15 @@
         """
 
     async def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -388,16 +388,16 @@
         """
 
     async def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
-        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
+        TimeSeriesTransformations: Sequence[TimeSeriesTransformationUnionTypeDef] = ...,
+        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/client.pyi` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     CreateForecastResponseTypeDef,
     CreateMonitorResponseTypeDef,
     CreatePredictorBacktestExportJobResponseTypeDef,
     CreatePredictorResponseTypeDef,
     CreateWhatIfAnalysisResponseTypeDef,
     CreateWhatIfForecastExportResponseTypeDef,
     CreateWhatIfForecastResponseTypeDef,
-    DataConfigTypeDef,
+    DataConfigUnionTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     DescribeAutoPredictorResponseTypeDef,
     DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -75,19 +75,19 @@
     DescribeWhatIfAnalysisResponseTypeDef,
     DescribeWhatIfForecastExportResponseTypeDef,
     DescribeWhatIfForecastResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EncryptionConfigTypeDef,
     EvaluationParametersTypeDef,
     ExplainabilityConfigTypeDef,
-    FeaturizationConfigTypeDef,
+    FeaturizationConfigUnionTypeDef,
     FilterTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    HyperParameterTuningJobConfigTypeDef,
-    InputDataConfigTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
+    InputDataConfigUnionTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     ListExplainabilitiesResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListForecastsResponseTypeDef,
@@ -96,20 +96,20 @@
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListPredictorsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MonitorConfigTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    TimeSeriesReplacementsDataSourceTypeDef,
-    TimeSeriesSelectorTypeDef,
-    TimeSeriesTransformationTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -165,15 +165,15 @@
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int = ...,
         ForecastTypes: Sequence[str] = ...,
         ForecastDimensions: Sequence[str] = ...,
         ForecastFrequency: str = ...,
-        DataConfig: DataConfigTypeDef = ...,
+        DataConfig: DataConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         ReferencePredictorArn: str = ...,
         OptimizationMetric: OptimizationMetricType = ...,
         ExplainPredictor: bool = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MonitorConfig: MonitorConfigTypeDef = ...,
         TimeAlignmentBoundary: TimeAlignmentBoundaryTypeDef = ...
@@ -186,15 +186,15 @@
         """
     async def create_dataset(
         self,
         *,
         DatasetName: str,
         Domain: DomainType,
         DatasetType: DatasetTypeType,
-        Schema: SchemaTypeDef,
+        Schema: SchemaUnionTypeDef,
         DataFrequency: str = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateDatasetResponseTypeDef:
         """
         Creates an Amazon Forecast dataset.
 
@@ -238,15 +238,15 @@
     async def create_explainability(
         self,
         *,
         ExplainabilityName: str,
         ResourceArn: str,
         ExplainabilityConfig: ExplainabilityConfigTypeDef,
         DataSource: DataSourceTypeDef = ...,
-        Schema: SchemaTypeDef = ...,
+        Schema: SchemaUnionTypeDef = ...,
         EnableVisualization: bool = ...,
         StartDateTime: str = ...,
         EndDateTime: str = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateExplainabilityResponseTypeDef:
         """
         .
@@ -273,15 +273,15 @@
     async def create_forecast(
         self,
         *,
         ForecastName: str,
         PredictorArn: str,
         ForecastTypes: Sequence[str] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...
     ) -> CreateForecastResponseTypeDef:
         """
         Creates a forecast for each item in the `TARGET_TIME_SERIES` dataset that was
         used to train the predictor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_forecast)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_forecast)
@@ -312,24 +312,24 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_monitor)
         """
     async def create_predictor(
         self,
         *,
         PredictorName: str,
         ForecastHorizon: int,
-        InputDataConfig: InputDataConfigTypeDef,
-        FeaturizationConfig: FeaturizationConfigTypeDef,
+        InputDataConfig: InputDataConfigUnionTypeDef,
+        FeaturizationConfig: FeaturizationConfigUnionTypeDef,
         AlgorithmArn: str = ...,
         ForecastTypes: Sequence[str] = ...,
         PerformAutoML: bool = ...,
         AutoMLOverrideStrategy: AutoMLOverrideStrategyType = ...,
         PerformHPO: bool = ...,
         TrainingParameters: Mapping[str, str] = ...,
         EvaluationParameters: EvaluationParametersTypeDef = ...,
-        HPOConfig: HyperParameterTuningJobConfigTypeDef = ...,
+        HPOConfig: HyperParameterTuningJobConfigUnionTypeDef = ...,
         EncryptionConfig: EncryptionConfigTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         OptimizationMetric: OptimizationMetricType = ...
     ) -> CreatePredictorResponseTypeDef:
         """
         .
 
@@ -353,15 +353,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_predictor_backtest_export_job)
         """
     async def create_what_if_analysis(
         self,
         *,
         WhatIfAnalysisName: str,
         ForecastArn: str,
-        TimeSeriesSelector: TimeSeriesSelectorTypeDef = ...,
+        TimeSeriesSelector: TimeSeriesSelectorUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfAnalysisResponseTypeDef:
         """
         What-if analysis is a scenario modeling technique where you make a hypothetical
         change to a time series and compare the forecasts generated by these changes
         against the baseline, unchanged time series.
 
@@ -369,16 +369,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/client/#create_what_if_analysis)
         """
     async def create_what_if_forecast(
         self,
         *,
         WhatIfForecastName: str,
         WhatIfAnalysisArn: str,
-        TimeSeriesTransformations: Sequence[TimeSeriesTransformationTypeDef] = ...,
-        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceTypeDef = ...,
+        TimeSeriesTransformations: Sequence[TimeSeriesTransformationUnionTypeDef] = ...,
+        TimeSeriesReplacementsDataSource: TimeSeriesReplacementsDataSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> CreateWhatIfForecastResponseTypeDef:
         """
         A what-if forecast is a forecast that is created from a modified version of the
         baseline forecast.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Client.create_what_if_forecast)
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/literals.py` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/literals.pyi` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/paginator.py` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -83,263 +83,247 @@
     "ListPredictorBacktestExportJobsPaginator",
     "ListPredictorsPaginator",
     "ListWhatIfAnalysesPaginator",
     "ListWhatIfForecastExportsPaginator",
     "ListWhatIfForecastsPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListDatasetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetgroupspaginator)
         """
 
-
 class ListDatasetImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
-
 class ListDatasetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetspaginator)
         """
 
-
 class ListExplainabilitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
         """
 
-
 class ListExplainabilityExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
-
 class ListForecastExportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
         """
 
-
 class ListForecastsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
         """
 
-
 class ListMonitorEvaluationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
-
 class ListMonitorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
         """
 
-
 class ListPredictorBacktestExportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
-
 class ListPredictorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
         """
 
-
 class ListWhatIfAnalysesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
         """
 
-
 class ListWhatIfForecastExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
-
 class ListWhatIfForecastsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/paginator.pyi` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,247 +83,263 @@
     "ListPredictorBacktestExportJobsPaginator",
     "ListPredictorsPaginator",
     "ListWhatIfAnalysesPaginator",
     "ListWhatIfForecastExportsPaginator",
     "ListWhatIfForecastsPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListDatasetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetgroupspaginator)
         """
 
+
 class ListDatasetImportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetImportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasetImportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetimportjobspaginator)
         """
 
+
 class ListDatasetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatasetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListDatasets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listdatasetspaginator)
         """
 
+
 class ListExplainabilitiesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExplainabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilitiespaginator)
         """
 
+
 class ListExplainabilityExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListExplainabilityExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListExplainabilityExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listexplainabilityexportspaginator)
         """
 
+
 class ListForecastExportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListForecastExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecastExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastexportjobspaginator)
         """
 
+
 class ListForecastsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listforecastspaginator)
         """
 
+
 class ListMonitorEvaluationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         MonitorArn: str,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitorEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitorEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorevaluationspaginator)
         """
 
+
 class ListMonitorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListMonitors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listmonitorspaginator)
         """
 
+
 class ListPredictorBacktestExportJobsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPredictorBacktestExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictorBacktestExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorbacktestexportjobspaginator)
         """
 
+
 class ListPredictorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPredictorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListPredictors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listpredictorspaginator)
         """
 
+
 class ListWhatIfAnalysesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWhatIfAnalysesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfAnalyses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifanalysespaginator)
         """
 
+
 class ListWhatIfForecastExportsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWhatIfForecastExportsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecastExports.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastexportspaginator)
         """
 
+
 class ListWhatIfForecastsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Sequence[FilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListWhatIfForecastsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService.Paginator.ListWhatIfForecasts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/paginators/#listwhatifforecastspaginator)
         """
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/type_defs.py` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_forecast.type_defs import ActionTypeDef
 
-    data: ActionTypeDef = {...}
+    data: ActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttributeTypeType,
     AutoMLOverrideStrategyType,
     ConditionType,
     DatasetTypeType,
     DayOfWeekType,
@@ -42,39 +42,29 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ActionTypeDef",
+    "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
+    "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
+    "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
-    "CreateAutoPredictorResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateExplainabilityExportResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ExplainabilityConfigTypeDef",
-    "CreateExplainabilityResponseTypeDef",
-    "CreateForecastExportJobResponseTypeDef",
-    "CreateForecastResponseTypeDef",
-    "CreateMonitorResponseTypeDef",
-    "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
-    "CreatePredictorResponseTypeDef",
-    "CreateWhatIfAnalysisResponseTypeDef",
-    "CreateWhatIfForecastExportResponseTypeDef",
-    "CreateWhatIfForecastResponseTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -89,107 +79,128 @@
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
+    "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
     "SupplementaryFeatureTypeDef",
     "IntegerParameterRangeTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
+    "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateAutoPredictorResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateExplainabilityExportResponseTypeDef",
+    "CreateExplainabilityResponseTypeDef",
+    "CreateForecastExportJobResponseTypeDef",
+    "CreateForecastResponseTypeDef",
+    "CreateMonitorResponseTypeDef",
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    "CreatePredictorResponseTypeDef",
+    "CreateWhatIfAnalysisResponseTypeDef",
+    "CreateWhatIfForecastExportResponseTypeDef",
+    "CreateWhatIfForecastResponseTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
+    "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
-    "ListForecastsRequestListForecastsPaginateTypeDef",
     "ListForecastsRequestRequestTypeDef",
-    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     "ListMonitorsRequestRequestTypeDef",
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     "ListPredictorsRequestRequestTypeDef",
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
+    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+    "ListForecastsRequestListForecastsPaginateTypeDef",
+    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
+    "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
-    "CreateAutoPredictorRequestRequestTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
+    "CreateAutoPredictorRequestRequestTypeDef",
+    "DataConfigUnionTypeDef",
     "BaselineTypeDef",
     "ListExplainabilitiesResponseTypeDef",
     "CreateExplainabilityExportRequestRequestTypeDef",
     "CreateForecastExportJobRequestRequestTypeDef",
     "CreatePredictorBacktestExportJobRequestRequestTypeDef",
     "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
@@ -200,53 +211,86 @@
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "ListPredictorsResponseTypeDef",
+    "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
+    "InputDataConfigUnionTypeDef",
+    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "CreateExplainabilityRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DescribeExplainabilityResponseTypeDef",
+    "TimeSeriesIdentifiersOutputTypeDef",
+    "TimeSeriesReplacementsDataSourceOutputTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "CreateExplainabilityRequestRequestTypeDef",
+    "SchemaUnionTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
+    "TimeSeriesTransformationUnionTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
+    "FeaturizationConfigUnionTypeDef",
     "CreatePredictorRequestRequestTypeDef",
+    "HyperParameterTuningJobConfigUnionTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
+    "TimeSeriesSelectorOutputTypeDef",
+    "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
+    "TimeSeriesReplacementsDataSourceUnionTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
-    "DescribeWhatIfForecastResponseTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
-    "CreateForecastRequestRequestTypeDef",
-    "CreateWhatIfAnalysisRequestRequestTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
+    "CreateForecastRequestRequestTypeDef",
+    "CreateWhatIfAnalysisRequestRequestTypeDef",
+    "TimeSeriesSelectorUnionTypeDef",
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
 )
 
+_RequiredAdditionalDatasetOutputTypeDef = TypedDict(
+    "_RequiredAdditionalDatasetOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAdditionalDatasetOutputTypeDef = TypedDict(
+    "_OptionalAdditionalDatasetOutputTypeDef",
+    {
+        "Configuration": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+
+class AdditionalDatasetOutputTypeDef(
+    _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
+):
+    pass
+
+
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
@@ -260,14 +304,22 @@
 
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
 
+AttributeConfigOutputTypeDef = TypedDict(
+    "AttributeConfigOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Transformations": Dict[str, str],
+    },
+)
+
 AttributeConfigTypeDef = TypedDict(
     "AttributeConfigTypeDef",
     {
         "AttributeName": str,
         "Transformations": Mapping[str, str],
     },
 )
@@ -277,14 +329,22 @@
     {
         "Name": str,
         "Value": float,
     },
     total=False,
 )
 
+CategoricalParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
+
 CategoricalParameterRangeTypeDef = TypedDict(
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -342,143 +402,42 @@
         "DayOfMonth": int,
         "DayOfWeek": DayOfWeekType,
         "Hour": int,
     },
     total=False,
 )
 
-CreateAutoPredictorResponseTypeDef = TypedDict(
-    "CreateAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "DatasetImportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateExplainabilityExportResponseTypeDef = TypedDict(
-    "CreateExplainabilityExportResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ExplainabilityExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ExplainabilityConfigTypeDef = TypedDict(
     "ExplainabilityConfigTypeDef",
     {
         "TimeSeriesGranularity": TimeSeriesGranularityType,
         "TimePointGranularity": TimePointGranularityType,
     },
 )
 
-CreateExplainabilityResponseTypeDef = TypedDict(
-    "CreateExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastExportJobResponseTypeDef = TypedDict(
-    "CreateForecastExportJobResponseTypeDef",
-    {
-        "ForecastExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastResponseTypeDef = TypedDict(
-    "CreateForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMonitorResponseTypeDef = TypedDict(
-    "CreateMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    {
-        "PredictorBacktestExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluationParametersTypeDef = TypedDict(
     "EvaluationParametersTypeDef",
     {
         "NumberOfBacktestWindows": int,
         "BackTestWindowOffset": int,
     },
     total=False,
 )
 
-CreatePredictorResponseTypeDef = TypedDict(
-    "CreatePredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfAnalysisResponseTypeDef = TypedDict(
-    "CreateWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastExportResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastExportResponseTypeDef",
-    {
-        "WhatIfForecastExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -654,28 +613,14 @@
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupName": str,
-        "DatasetGroupArn": str,
-        "DatasetArns": List[str],
-        "Domain": DomainType,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetImportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetImportJobRequestRequestTypeDef",
     {
         "DatasetImportJobArn": str,
     },
 )
 
@@ -771,33 +716,47 @@
 DescribeWhatIfForecastRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorMetricTypeDef = TypedDict(
     "ErrorMetricTypeDef",
     {
         "ForecastType": str,
         "WAPE": float,
         "RMSE": float,
         "MASE": float,
         "MAPE": float,
     },
     total=False,
 )
 
+_RequiredFeaturizationMethodOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodName": Literal["filling"],
+    },
+)
+_OptionalFeaturizationMethodOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodParameters": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class FeaturizationMethodOutputTypeDef(
+    _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
+):
+    pass
+
+
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
@@ -874,39 +833,33 @@
 
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
 
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -984,24 +937,14 @@
         "DatasetImportJobArn": str,
         "ForecastArn": str,
         "PredictorArn": str,
     },
     total=False,
 )
 
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
 PredictorEventTypeDef = TypedDict(
     "PredictorEventTypeDef",
     {
         "Detail": str,
         "Datetime": datetime,
     },
     total=False,
@@ -1014,25 +957,14 @@
         "TestWindowEnd": datetime,
         "Status": str,
         "Message": str,
     },
     total=False,
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
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -1073,14 +1005,34 @@
     "UpdateDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetArns": Sequence[str],
     },
 )
 
+_RequiredDataConfigOutputTypeDef = TypedDict(
+    "_RequiredDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalDataConfigOutputTypeDef = TypedDict(
+    "_OptionalDataConfigOutputTypeDef",
+    {
+        "AttributeConfigs": List[AttributeConfigOutputTypeDef],
+        "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
+    pass
+
+
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1147,30 +1099,163 @@
 
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateAutoPredictorResponseTypeDef = TypedDict(
+    "CreateAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "DatasetImportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityExportResponseTypeDef = TypedDict(
+    "CreateExplainabilityExportResponseTypeDef",
+    {
+        "ExplainabilityExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityResponseTypeDef = TypedDict(
+    "CreateExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastExportJobResponseTypeDef = TypedDict(
+    "CreateForecastExportJobResponseTypeDef",
+    {
+        "ForecastExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastResponseTypeDef = TypedDict(
+    "CreateForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMonitorResponseTypeDef = TypedDict(
+    "CreateMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    {
+        "PredictorBacktestExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorResponseTypeDef = TypedDict(
+    "CreatePredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfAnalysisResponseTypeDef = TypedDict(
+    "CreateWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastExportResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastExportResponseTypeDef",
+    {
+        "WhatIfForecastExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupName": str,
+        "DatasetGroupArn": str,
+        "DatasetArns": List[str],
+        "Domain": DomainType,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ExplainabilitySummaryTypeDef = TypedDict(
     "ExplainabilitySummaryTypeDef",
     {
         "ExplainabilityArn": str,
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
@@ -1197,24 +1282,24 @@
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "DatasetGroups": List[DatasetGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorSummaryTypeDef = TypedDict(
     "PredictorSummaryTypeDef",
     {
         "PredictorArn": str,
@@ -1226,14 +1311,35 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
+_RequiredFeaturizationOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationOutputTypeDef",
+    {
+        "AttributeName": str,
+    },
+)
+_OptionalFeaturizationOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationOutputTypeDef",
+    {
+        "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class FeaturizationOutputTypeDef(
+    _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
+):
+    pass
+
+
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
@@ -1245,332 +1351,379 @@
 )
 
 
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
 
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestRequestTypeDef",
+ListExplainabilitiesRequestRequestTypeDef = TypedDict(
+    "ListExplainabilitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilitiesRequestRequestTypeDef = TypedDict(
-    "ListExplainabilitiesRequestRequestTypeDef",
+ListForecastExportJobsRequestRequestTypeDef = TypedDict(
+    "ListForecastExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+ListForecastsRequestRequestTypeDef = TypedDict(
+    "ListForecastsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestRequestTypeDef",
+_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
+    {
+        "MonitorArn": str,
+    },
+)
+_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+
+class ListMonitorEvaluationsRequestRequestTypeDef(
+    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
+    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
+):
+    pass
+
+
+ListMonitorsRequestRequestTypeDef = TypedDict(
+    "ListMonitorsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastExportJobsRequestRequestTypeDef = TypedDict(
-    "ListForecastExportJobsRequestRequestTypeDef",
+ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
-    "ListForecastsRequestListForecastsPaginateTypeDef",
+ListPredictorsRequestRequestTypeDef = TypedDict(
+    "ListPredictorsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastsRequestRequestTypeDef = TypedDict(
-    "ListForecastsRequestRequestTypeDef",
+ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestRequestTypeDef",
     {
-        "MonitorArn": str,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
+    total=False,
 )
-_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+
+ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
+ListForecastsResponseTypeDef = TypedDict(
+    "ListForecastsResponseTypeDef",
+    {
+        "Forecasts": List[ForecastSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
-    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
+    },
+    total=False,
+)
+
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
     pass
 
 
-_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
     {
-        "MonitorArn": str,
+        "DatasetGroupArn": str,
     },
 )
-_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filters": Sequence[FilterTypeDef],
+        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
 
-class ListMonitorEvaluationsRequestRequestTypeDef(
-    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
-    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
-):
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
 
-ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+ParameterRangesOutputTypeDef = TypedDict(
+    "ParameterRangesOutputTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
+        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMonitorsRequestRequestTypeDef = TypedDict(
-    "ListMonitorsRequestRequestTypeDef",
+ParameterRangesTypeDef = TypedDict(
+    "ParameterRangesTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filters": Sequence[FilterTypeDef],
+        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
+        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorsRequestRequestTypeDef = TypedDict(
-    "ListPredictorsRequestRequestTypeDef",
+ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestRequestTypeDef",
+ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
+    "ListForecastsRequestListForecastsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestRequestTypeDef",
+_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    {
+        "MonitorArn": str,
+    },
+)
+_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
+
+class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
+    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+):
+    pass
+
+
+ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestRequestTypeDef",
+ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListForecastsResponseTypeDef = TypedDict(
-    "ListForecastsResponseTypeDef",
+ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     {
-        "Forecasts": List[ForecastSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
+ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     {
-        "DatasetGroupArn": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
+
+ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     {
-        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
-    pass
-
-
-ParameterRangesTypeDef = TypedDict(
-    "ParameterRangesTypeDef",
+ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     {
-        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
-        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
-        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitorsResponseTypeDef = TypedDict(
     "ListMonitorsResponseTypeDef",
     {
         "Monitors": List[MonitorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastsResponseTypeDef = TypedDict(
     "ListWhatIfForecastsResponseTypeDef",
     {
         "WhatIfForecasts": List[WhatIfForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsTypeDef = TypedDict(
     "MetricsTypeDef",
     {
         "RMSE": float,
@@ -1604,31 +1757,74 @@
     {
         "AlgorithmArn": str,
         "TestWindows": List[TestWindowSummaryTypeDef],
     },
     total=False,
 )
 
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
+    {
+        "Attributes": List[SchemaAttributeTypeDef],
+    },
+    total=False,
+)
+
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "Attributes": Sequence[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
+TimeSeriesTransformationOutputTypeDef = TypedDict(
+    "TimeSeriesTransformationOutputTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "TimeSeriesConditions": List[TimeSeriesConditionTypeDef],
+    },
+    total=False,
+)
+
 TimeSeriesTransformationTypeDef = TypedDict(
     "TimeSeriesTransformationTypeDef",
     {
         "Action": ActionTypeDef,
         "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
+DescribeAutoPredictorResponseTypeDef = TypedDict(
+    "DescribeAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "PredictorName": str,
+        "ForecastHorizon": int,
+        "ForecastTypes": List[str],
+        "ForecastFrequency": str,
+        "ForecastDimensions": List[str],
+        "DatasetImportJobArns": List[str],
+        "DataConfig": DataConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "OptimizationMetric": OptimizationMetricType,
+        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
+        "MonitorInfo": MonitorInfoTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
     },
 )
 _OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
@@ -1654,54 +1850,29 @@
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeAutoPredictorResponseTypeDef = TypedDict(
-    "DescribeAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "PredictorName": str,
-        "ForecastHorizon": int,
-        "ForecastTypes": List[str],
-        "ForecastFrequency": str,
-        "ForecastDimensions": List[str],
-        "DatasetImportJobArns": List[str],
-        "DataConfig": DataConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "OptimizationMetric": OptimizationMetricType,
-        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
-        "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+DataConfigUnionTypeDef = Union[DataConfigTypeDef, DataConfigOutputTypeDef]
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
 
 ListExplainabilitiesResponseTypeDef = TypedDict(
     "ListExplainabilitiesResponseTypeDef",
     {
         "Explainabilities": List[ExplainabilitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
     {
         "ExplainabilityExportName": str,
@@ -1809,15 +1980,15 @@
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
@@ -1825,15 +1996,15 @@
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
@@ -1841,15 +2012,15 @@
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
@@ -1858,15 +2029,15 @@
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
@@ -1984,27 +2155,49 @@
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredFeaturizationConfigOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastFrequency": str,
+    },
+)
+_OptionalFeaturizationConfigOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastDimensions": List[str],
+        "Featurizations": List[FeaturizationOutputTypeDef],
     },
+    total=False,
 )
 
+
+class FeaturizationConfigOutputTypeDef(
+    _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -2019,14 +2212,23 @@
 
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
 
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
+HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigOutputTypeDef",
+    {
+        "ParameterRanges": ParameterRangesOutputTypeDef,
+    },
+    total=False,
+)
+
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
     {
         "ParameterRanges": ParameterRangesTypeDef,
     },
     total=False,
 )
@@ -2044,26 +2246,98 @@
 )
 
 ListMonitorEvaluationsResponseTypeDef = TypedDict(
     "ListMonitorEvaluationsResponseTypeDef",
     {
         "NextToken": str,
         "PredictorMonitorEvaluations": List[PredictorMonitorEvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorExecutionDetailsTypeDef = TypedDict(
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
     },
     total=False,
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": str,
+        "Domain": DomainType,
+        "DatasetType": DatasetTypeType,
+        "DataFrequency": str,
+        "Schema": SchemaOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExplainabilityResponseTypeDef = TypedDict(
+    "DescribeExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
+        "EnableVisualization": bool,
+        "DataSource": DataSourceTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "StartDateTime": str,
+        "EndDateTime": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Message": str,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TimeSeriesIdentifiersOutputTypeDef = TypedDict(
+    "TimeSeriesIdentifiersOutputTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "Format": str,
+    },
+    total=False,
+)
+
+_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "S3Config": S3ConfigTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+)
+_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "Format": str,
+        "TimestampFormat": str,
+    },
+    total=False,
+)
+
+
+class TimeSeriesReplacementsDataSourceOutputTypeDef(
+    _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
+    _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
+):
+    pass
+
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2111,52 +2385,15 @@
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "DatasetName": str,
-        "Domain": DomainType,
-        "DatasetType": DatasetTypeType,
-        "DataFrequency": str,
-        "Schema": SchemaTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExplainabilityResponseTypeDef = TypedDict(
-    "DescribeExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "EnableVisualization": bool,
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaTypeDef,
-        "StartDateTime": str,
-        "EndDateTime": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Message": str,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2183,77 +2420,83 @@
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
 
+TimeSeriesTransformationUnionTypeDef = Union[
+    TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef
+]
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
         "LastEvaluationTime": datetime,
         "LastEvaluationState": str,
         "Baseline": BaselineTypeDef,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "EstimatedEvaluationTimeRemainingInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExplainabilityExportsResponseTypeDef = TypedDict(
     "ListExplainabilityExportsResponseTypeDef",
     {
         "ExplainabilityExports": List[ExplainabilityExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListForecastExportJobsResponseTypeDef = TypedDict(
     "ListForecastExportJobsResponseTypeDef",
     {
         "ForecastExportJobs": List[ForecastExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPredictorBacktestExportJobsResponseTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsResponseTypeDef",
     {
         "PredictorBacktestExportJobs": List[PredictorBacktestExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastExportsResponseTypeDef = TypedDict(
     "ListWhatIfForecastExportsResponseTypeDef",
     {
         "WhatIfForecastExports": List[WhatIfForecastExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FeaturizationConfigUnionTypeDef = Union[
+    FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef
+]
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
         "ForecastHorizon": int,
         "InputDataConfig": InputDataConfigTypeDef,
         "FeaturizationConfig": FeaturizationConfigTypeDef,
@@ -2280,14 +2523,17 @@
 
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
 
+HyperParameterTuningJobConfigUnionTypeDef = Union[
+    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
+]
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2303,90 +2549,135 @@
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
         "EvaluationParameters": EvaluationParametersTypeDef,
-        "HPOConfig": HyperParameterTuningJobConfigTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "FeaturizationConfig": FeaturizationConfigTypeDef,
+        "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TimeSeriesSelectorOutputTypeDef = TypedDict(
+    "TimeSeriesSelectorOutputTypeDef",
+    {
+        "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
+    },
+    total=False,
+)
+
+DescribeWhatIfForecastResponseTypeDef = TypedDict(
+    "DescribeWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastName": str,
+        "WhatIfForecastArn": str,
+        "WhatIfAnalysisArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
+        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
+        "ForecastTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
 
+TimeSeriesReplacementsDataSourceUnionTypeDef = Union[
+    TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
+]
 _RequiredCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
+        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationUnionTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeWhatIfForecastResponseTypeDef = TypedDict(
-    "DescribeWhatIfForecastResponseTypeDef",
+GetAccuracyMetricsResponseTypeDef = TypedDict(
+    "GetAccuracyMetricsResponseTypeDef",
     {
-        "WhatIfForecastName": str,
-        "WhatIfForecastArn": str,
-        "WhatIfAnalysisArn": str,
+        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
+        "IsAutoPredictor": bool,
+        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
+        "OptimizationMetric": OptimizationMetricType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeForecastResponseTypeDef = TypedDict(
+    "DescribeForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ForecastName": str,
+        "ForecastTypes": List[str],
+        "PredictorArn": str,
+        "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
-        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
-        "ForecastTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAccuracyMetricsResponseTypeDef = TypedDict(
-    "GetAccuracyMetricsResponseTypeDef",
+DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
+    "DescribeWhatIfAnalysisResponseTypeDef",
     {
-        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
-        "IsAutoPredictor": bool,
-        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
-        "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WhatIfAnalysisName": str,
+        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
         "ForecastName": str,
@@ -2430,40 +2721,8 @@
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeForecastResponseTypeDef = TypedDict(
-    "DescribeForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ForecastName": str,
-        "ForecastTypes": List[str],
-        "PredictorArn": str,
-        "DatasetGroupArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
-    "DescribeWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisName": str,
-        "WhatIfAnalysisArn": str,
-        "ForecastArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+TimeSeriesSelectorUnionTypeDef = Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef]
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast/type_defs.pyi` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_forecast.type_defs import ActionTypeDef
 
-    data: ActionTypeDef = {...}
+    data: ActionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AttributeTypeType,
     AutoMLOverrideStrategyType,
     ConditionType,
     DatasetTypeType,
     DayOfWeekType,
@@ -41,39 +41,29 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ActionTypeDef",
+    "AdditionalDatasetOutputTypeDef",
     "AdditionalDatasetTypeDef",
+    "AttributeConfigOutputTypeDef",
     "AttributeConfigTypeDef",
     "BaselineMetricTypeDef",
+    "CategoricalParameterRangeOutputTypeDef",
     "CategoricalParameterRangeTypeDef",
     "ContinuousParameterRangeTypeDef",
     "EncryptionConfigTypeDef",
     "MonitorConfigTypeDef",
     "TagTypeDef",
     "TimeAlignmentBoundaryTypeDef",
-    "CreateAutoPredictorResponseTypeDef",
-    "CreateDatasetGroupResponseTypeDef",
-    "CreateDatasetImportJobResponseTypeDef",
-    "CreateDatasetResponseTypeDef",
-    "CreateExplainabilityExportResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ExplainabilityConfigTypeDef",
-    "CreateExplainabilityResponseTypeDef",
-    "CreateForecastExportJobResponseTypeDef",
-    "CreateForecastResponseTypeDef",
-    "CreateMonitorResponseTypeDef",
-    "CreatePredictorBacktestExportJobResponseTypeDef",
     "EvaluationParametersTypeDef",
-    "CreatePredictorResponseTypeDef",
-    "CreateWhatIfAnalysisResponseTypeDef",
-    "CreateWhatIfForecastExportResponseTypeDef",
-    "CreateWhatIfForecastResponseTypeDef",
     "S3ConfigTypeDef",
     "DatasetGroupSummaryTypeDef",
     "DatasetSummaryTypeDef",
     "DeleteDatasetGroupRequestRequestTypeDef",
     "DeleteDatasetImportJobRequestRequestTypeDef",
     "DeleteDatasetRequestRequestTypeDef",
     "DeleteExplainabilityExportRequestRequestTypeDef",
@@ -88,107 +78,128 @@
     "DeleteWhatIfForecastExportRequestRequestTypeDef",
     "DeleteWhatIfForecastRequestRequestTypeDef",
     "DescribeAutoPredictorRequestRequestTypeDef",
     "ExplainabilityInfoTypeDef",
     "MonitorInfoTypeDef",
     "ReferencePredictorSummaryTypeDef",
     "DescribeDatasetGroupRequestRequestTypeDef",
-    "DescribeDatasetGroupResponseTypeDef",
     "DescribeDatasetImportJobRequestRequestTypeDef",
     "StatisticsTypeDef",
     "DescribeDatasetRequestRequestTypeDef",
     "DescribeExplainabilityExportRequestRequestTypeDef",
     "DescribeExplainabilityRequestRequestTypeDef",
     "DescribeForecastExportJobRequestRequestTypeDef",
     "DescribeForecastRequestRequestTypeDef",
     "DescribeMonitorRequestRequestTypeDef",
     "DescribePredictorBacktestExportJobRequestRequestTypeDef",
     "DescribePredictorRequestRequestTypeDef",
     "DescribeWhatIfAnalysisRequestRequestTypeDef",
     "DescribeWhatIfForecastExportRequestRequestTypeDef",
     "DescribeWhatIfForecastRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ErrorMetricTypeDef",
+    "FeaturizationMethodOutputTypeDef",
     "FeaturizationMethodTypeDef",
     "FilterTypeDef",
     "ForecastSummaryTypeDef",
     "GetAccuracyMetricsRequestRequestTypeDef",
     "SupplementaryFeatureTypeDef",
     "IntegerParameterRangeTypeDef",
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDatasetGroupsRequestRequestTypeDef",
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     "ListDatasetsRequestRequestTypeDef",
     "MonitorSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "WhatIfAnalysisSummaryTypeDef",
     "WhatIfForecastSummaryTypeDef",
     "MetricResultTypeDef",
     "WeightedQuantileLossTypeDef",
     "MonitorDataSourceTypeDef",
-    "PaginatorConfigTypeDef",
     "PredictorEventTypeDef",
     "TestWindowSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeResourceRequestRequestTypeDef",
     "SchemaAttributeTypeDef",
     "StopResourceRequestRequestTypeDef",
     "TimeSeriesConditionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatasetGroupRequestRequestTypeDef",
+    "DataConfigOutputTypeDef",
     "DataConfigTypeDef",
     "PredictorBaselineTypeDef",
     "CreateDatasetGroupRequestRequestTypeDef",
     "CreateMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateAutoPredictorResponseTypeDef",
+    "CreateDatasetGroupResponseTypeDef",
+    "CreateDatasetImportJobResponseTypeDef",
+    "CreateDatasetResponseTypeDef",
+    "CreateExplainabilityExportResponseTypeDef",
+    "CreateExplainabilityResponseTypeDef",
+    "CreateForecastExportJobResponseTypeDef",
+    "CreateForecastResponseTypeDef",
+    "CreateMonitorResponseTypeDef",
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    "CreatePredictorResponseTypeDef",
+    "CreateWhatIfAnalysisResponseTypeDef",
+    "CreateWhatIfForecastExportResponseTypeDef",
+    "CreateWhatIfForecastResponseTypeDef",
+    "DescribeDatasetGroupResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "ExplainabilitySummaryTypeDef",
     "DataDestinationTypeDef",
     "DataSourceTypeDef",
     "ListDatasetGroupsResponseTypeDef",
     "ListDatasetsResponseTypeDef",
     "PredictorSummaryTypeDef",
+    "FeaturizationOutputTypeDef",
     "FeaturizationTypeDef",
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     "ListDatasetImportJobsRequestRequestTypeDef",
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     "ListExplainabilitiesRequestRequestTypeDef",
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     "ListExplainabilityExportsRequestRequestTypeDef",
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     "ListForecastExportJobsRequestRequestTypeDef",
-    "ListForecastsRequestListForecastsPaginateTypeDef",
     "ListForecastsRequestRequestTypeDef",
-    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     "ListMonitorEvaluationsRequestRequestTypeDef",
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     "ListMonitorsRequestRequestTypeDef",
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     "ListPredictorBacktestExportJobsRequestRequestTypeDef",
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     "ListPredictorsRequestRequestTypeDef",
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     "ListWhatIfAnalysesRequestRequestTypeDef",
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     "ListWhatIfForecastExportsRequestRequestTypeDef",
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListWhatIfForecastsRequestRequestTypeDef",
     "ListForecastsResponseTypeDef",
+    "InputDataConfigOutputTypeDef",
     "InputDataConfigTypeDef",
+    "ParameterRangesOutputTypeDef",
     "ParameterRangesTypeDef",
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+    "ListForecastsRequestListForecastsPaginateTypeDef",
+    "ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     "ListMonitorsResponseTypeDef",
     "ListWhatIfAnalysesResponseTypeDef",
     "ListWhatIfForecastsResponseTypeDef",
     "MetricsTypeDef",
     "PredictorMonitorEvaluationTypeDef",
     "PredictorExecutionTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
+    "TimeSeriesTransformationOutputTypeDef",
     "TimeSeriesTransformationTypeDef",
-    "CreateAutoPredictorRequestRequestTypeDef",
     "DescribeAutoPredictorResponseTypeDef",
+    "CreateAutoPredictorRequestRequestTypeDef",
+    "DataConfigUnionTypeDef",
     "BaselineTypeDef",
     "ListExplainabilitiesResponseTypeDef",
     "CreateExplainabilityExportRequestRequestTypeDef",
     "CreateForecastExportJobRequestRequestTypeDef",
     "CreatePredictorBacktestExportJobRequestRequestTypeDef",
     "CreateWhatIfForecastExportRequestRequestTypeDef",
     "DescribeExplainabilityExportResponseTypeDef",
@@ -199,53 +210,84 @@
     "ForecastExportJobSummaryTypeDef",
     "PredictorBacktestExportJobSummaryTypeDef",
     "WhatIfForecastExportSummaryTypeDef",
     "CreateDatasetImportJobRequestRequestTypeDef",
     "DatasetImportJobSummaryTypeDef",
     "DescribeDatasetImportJobResponseTypeDef",
     "ListPredictorsResponseTypeDef",
+    "FeaturizationConfigOutputTypeDef",
     "FeaturizationConfigTypeDef",
+    "InputDataConfigUnionTypeDef",
+    "HyperParameterTuningJobConfigOutputTypeDef",
     "HyperParameterTuningJobConfigTypeDef",
     "WindowSummaryTypeDef",
     "ListMonitorEvaluationsResponseTypeDef",
     "PredictorExecutionDetailsTypeDef",
-    "CreateDatasetRequestRequestTypeDef",
-    "CreateExplainabilityRequestRequestTypeDef",
     "DescribeDatasetResponseTypeDef",
     "DescribeExplainabilityResponseTypeDef",
+    "TimeSeriesIdentifiersOutputTypeDef",
+    "TimeSeriesReplacementsDataSourceOutputTypeDef",
+    "CreateDatasetRequestRequestTypeDef",
+    "CreateExplainabilityRequestRequestTypeDef",
+    "SchemaUnionTypeDef",
     "TimeSeriesIdentifiersTypeDef",
     "TimeSeriesReplacementsDataSourceTypeDef",
+    "TimeSeriesTransformationUnionTypeDef",
     "DescribeMonitorResponseTypeDef",
     "ListExplainabilityExportsResponseTypeDef",
     "ListForecastExportJobsResponseTypeDef",
     "ListPredictorBacktestExportJobsResponseTypeDef",
     "ListWhatIfForecastExportsResponseTypeDef",
     "ListDatasetImportJobsResponseTypeDef",
+    "FeaturizationConfigUnionTypeDef",
     "CreatePredictorRequestRequestTypeDef",
+    "HyperParameterTuningJobConfigUnionTypeDef",
     "EvaluationResultTypeDef",
     "DescribePredictorResponseTypeDef",
+    "TimeSeriesSelectorOutputTypeDef",
+    "DescribeWhatIfForecastResponseTypeDef",
     "TimeSeriesSelectorTypeDef",
+    "TimeSeriesReplacementsDataSourceUnionTypeDef",
     "CreateWhatIfForecastRequestRequestTypeDef",
-    "DescribeWhatIfForecastResponseTypeDef",
     "GetAccuracyMetricsResponseTypeDef",
-    "CreateForecastRequestRequestTypeDef",
-    "CreateWhatIfAnalysisRequestRequestTypeDef",
     "DescribeForecastResponseTypeDef",
     "DescribeWhatIfAnalysisResponseTypeDef",
+    "CreateForecastRequestRequestTypeDef",
+    "CreateWhatIfAnalysisRequestRequestTypeDef",
+    "TimeSeriesSelectorUnionTypeDef",
 )
 
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "AttributeName": str,
         "Operation": OperationType,
         "Value": float,
     },
 )
 
+_RequiredAdditionalDatasetOutputTypeDef = TypedDict(
+    "_RequiredAdditionalDatasetOutputTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAdditionalDatasetOutputTypeDef = TypedDict(
+    "_OptionalAdditionalDatasetOutputTypeDef",
+    {
+        "Configuration": Dict[str, List[str]],
+    },
+    total=False,
+)
+
+class AdditionalDatasetOutputTypeDef(
+    _RequiredAdditionalDatasetOutputTypeDef, _OptionalAdditionalDatasetOutputTypeDef
+):
+    pass
+
 _RequiredAdditionalDatasetTypeDef = TypedDict(
     "_RequiredAdditionalDatasetTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalAdditionalDatasetTypeDef = TypedDict(
@@ -257,14 +299,22 @@
 )
 
 class AdditionalDatasetTypeDef(
     _RequiredAdditionalDatasetTypeDef, _OptionalAdditionalDatasetTypeDef
 ):
     pass
 
+AttributeConfigOutputTypeDef = TypedDict(
+    "AttributeConfigOutputTypeDef",
+    {
+        "AttributeName": str,
+        "Transformations": Dict[str, str],
+    },
+)
+
 AttributeConfigTypeDef = TypedDict(
     "AttributeConfigTypeDef",
     {
         "AttributeName": str,
         "Transformations": Mapping[str, str],
     },
 )
@@ -274,14 +324,22 @@
     {
         "Name": str,
         "Value": float,
     },
     total=False,
 )
 
+CategoricalParameterRangeOutputTypeDef = TypedDict(
+    "CategoricalParameterRangeOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
+
 CategoricalParameterRangeTypeDef = TypedDict(
     "CategoricalParameterRangeTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -337,143 +395,42 @@
         "DayOfMonth": int,
         "DayOfWeek": DayOfWeekType,
         "Hour": int,
     },
     total=False,
 )
 
-CreateAutoPredictorResponseTypeDef = TypedDict(
-    "CreateAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetGroupResponseTypeDef = TypedDict(
-    "CreateDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetImportJobResponseTypeDef = TypedDict(
-    "CreateDatasetImportJobResponseTypeDef",
-    {
-        "DatasetImportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateDatasetResponseTypeDef = TypedDict(
-    "CreateDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateExplainabilityExportResponseTypeDef = TypedDict(
-    "CreateExplainabilityExportResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ExplainabilityExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ExplainabilityConfigTypeDef = TypedDict(
     "ExplainabilityConfigTypeDef",
     {
         "TimeSeriesGranularity": TimeSeriesGranularityType,
         "TimePointGranularity": TimePointGranularityType,
     },
 )
 
-CreateExplainabilityResponseTypeDef = TypedDict(
-    "CreateExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastExportJobResponseTypeDef = TypedDict(
-    "CreateForecastExportJobResponseTypeDef",
-    {
-        "ForecastExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateForecastResponseTypeDef = TypedDict(
-    "CreateForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateMonitorResponseTypeDef = TypedDict(
-    "CreateMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
-    "CreatePredictorBacktestExportJobResponseTypeDef",
-    {
-        "PredictorBacktestExportJobArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluationParametersTypeDef = TypedDict(
     "EvaluationParametersTypeDef",
     {
         "NumberOfBacktestWindows": int,
         "BackTestWindowOffset": int,
     },
     total=False,
 )
 
-CreatePredictorResponseTypeDef = TypedDict(
-    "CreatePredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfAnalysisResponseTypeDef = TypedDict(
-    "CreateWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastExportResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastExportResponseTypeDef",
-    {
-        "WhatIfForecastExportArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateWhatIfForecastResponseTypeDef = TypedDict(
-    "CreateWhatIfForecastResponseTypeDef",
-    {
-        "WhatIfForecastArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ConfigTypeDef = TypedDict(
     "_RequiredS3ConfigTypeDef",
     {
         "Path": str,
         "RoleArn": str,
     },
 )
@@ -647,28 +604,14 @@
 DescribeDatasetGroupRequestRequestTypeDef = TypedDict(
     "DescribeDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 
-DescribeDatasetGroupResponseTypeDef = TypedDict(
-    "DescribeDatasetGroupResponseTypeDef",
-    {
-        "DatasetGroupName": str,
-        "DatasetGroupArn": str,
-        "DatasetArns": List[str],
-        "Domain": DomainType,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDatasetImportJobRequestRequestTypeDef = TypedDict(
     "DescribeDatasetImportJobRequestRequestTypeDef",
     {
         "DatasetImportJobArn": str,
     },
 )
 
@@ -764,33 +707,45 @@
 DescribeWhatIfForecastRequestRequestTypeDef = TypedDict(
     "DescribeWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastArn": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorMetricTypeDef = TypedDict(
     "ErrorMetricTypeDef",
     {
         "ForecastType": str,
         "WAPE": float,
         "RMSE": float,
         "MASE": float,
         "MAPE": float,
     },
     total=False,
 )
 
+_RequiredFeaturizationMethodOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodName": Literal["filling"],
+    },
+)
+_OptionalFeaturizationMethodOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationMethodOutputTypeDef",
+    {
+        "FeaturizationMethodParameters": Dict[str, str],
+    },
+    total=False,
+)
+
+class FeaturizationMethodOutputTypeDef(
+    _RequiredFeaturizationMethodOutputTypeDef, _OptionalFeaturizationMethodOutputTypeDef
+):
+    pass
+
 _RequiredFeaturizationMethodTypeDef = TypedDict(
     "_RequiredFeaturizationMethodTypeDef",
     {
         "FeaturizationMethodName": Literal["filling"],
     },
 )
 _OptionalFeaturizationMethodTypeDef = TypedDict(
@@ -863,39 +818,33 @@
 )
 
 class IntegerParameterRangeTypeDef(
     _RequiredIntegerParameterRangeTypeDef, _OptionalIntegerParameterRangeTypeDef
 ):
     pass
 
-ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
-    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDatasetGroupsRequestRequestTypeDef = TypedDict(
     "ListDatasetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
-    "ListDatasetsRequestListDatasetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDatasetsRequestRequestTypeDef = TypedDict(
     "ListDatasetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -973,24 +922,14 @@
         "DatasetImportJobArn": str,
         "ForecastArn": str,
         "PredictorArn": str,
     },
     total=False,
 )
 
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
 PredictorEventTypeDef = TypedDict(
     "PredictorEventTypeDef",
     {
         "Detail": str,
         "Datetime": datetime,
     },
     total=False,
@@ -1003,25 +942,14 @@
         "TestWindowEnd": datetime,
         "Status": str,
         "Message": str,
     },
     total=False,
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
 ResumeResourceRequestRequestTypeDef = TypedDict(
     "ResumeResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -1062,14 +990,32 @@
     "UpdateDatasetGroupRequestRequestTypeDef",
     {
         "DatasetGroupArn": str,
         "DatasetArns": Sequence[str],
     },
 )
 
+_RequiredDataConfigOutputTypeDef = TypedDict(
+    "_RequiredDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalDataConfigOutputTypeDef = TypedDict(
+    "_OptionalDataConfigOutputTypeDef",
+    {
+        "AttributeConfigs": List[AttributeConfigOutputTypeDef],
+        "AdditionalDatasets": List[AdditionalDatasetOutputTypeDef],
+    },
+    total=False,
+)
+
+class DataConfigOutputTypeDef(_RequiredDataConfigOutputTypeDef, _OptionalDataConfigOutputTypeDef):
+    pass
+
 _RequiredDataConfigTypeDef = TypedDict(
     "_RequiredDataConfigTypeDef",
     {
         "DatasetGroupArn": str,
     },
 )
 _OptionalDataConfigTypeDef = TypedDict(
@@ -1130,30 +1076,163 @@
 )
 
 class CreateMonitorRequestRequestTypeDef(
     _RequiredCreateMonitorRequestRequestTypeDef, _OptionalCreateMonitorRequestRequestTypeDef
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateAutoPredictorResponseTypeDef = TypedDict(
+    "CreateAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetGroupResponseTypeDef = TypedDict(
+    "CreateDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetImportJobResponseTypeDef = TypedDict(
+    "CreateDatasetImportJobResponseTypeDef",
+    {
+        "DatasetImportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDatasetResponseTypeDef = TypedDict(
+    "CreateDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityExportResponseTypeDef = TypedDict(
+    "CreateExplainabilityExportResponseTypeDef",
+    {
+        "ExplainabilityExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateExplainabilityResponseTypeDef = TypedDict(
+    "CreateExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastExportJobResponseTypeDef = TypedDict(
+    "CreateForecastExportJobResponseTypeDef",
+    {
+        "ForecastExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateForecastResponseTypeDef = TypedDict(
+    "CreateForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMonitorResponseTypeDef = TypedDict(
+    "CreateMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorBacktestExportJobResponseTypeDef = TypedDict(
+    "CreatePredictorBacktestExportJobResponseTypeDef",
+    {
+        "PredictorBacktestExportJobArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePredictorResponseTypeDef = TypedDict(
+    "CreatePredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfAnalysisResponseTypeDef = TypedDict(
+    "CreateWhatIfAnalysisResponseTypeDef",
+    {
+        "WhatIfAnalysisArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastExportResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastExportResponseTypeDef",
+    {
+        "WhatIfForecastExportArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateWhatIfForecastResponseTypeDef = TypedDict(
+    "CreateWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDatasetGroupResponseTypeDef = TypedDict(
+    "DescribeDatasetGroupResponseTypeDef",
+    {
+        "DatasetGroupName": str,
+        "DatasetGroupArn": str,
+        "DatasetArns": List[str],
+        "Domain": DomainType,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ExplainabilitySummaryTypeDef = TypedDict(
     "ExplainabilitySummaryTypeDef",
     {
         "ExplainabilityArn": str,
         "ExplainabilityName": str,
         "ResourceArn": str,
         "ExplainabilityConfig": ExplainabilityConfigTypeDef,
@@ -1180,24 +1259,24 @@
 )
 
 ListDatasetGroupsResponseTypeDef = TypedDict(
     "ListDatasetGroupsResponseTypeDef",
     {
         "DatasetGroups": List[DatasetGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetsResponseTypeDef = TypedDict(
     "ListDatasetsResponseTypeDef",
     {
         "Datasets": List[DatasetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorSummaryTypeDef = TypedDict(
     "PredictorSummaryTypeDef",
     {
         "PredictorArn": str,
@@ -1209,14 +1288,33 @@
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
     },
     total=False,
 )
 
+_RequiredFeaturizationOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationOutputTypeDef",
+    {
+        "AttributeName": str,
+    },
+)
+_OptionalFeaturizationOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationOutputTypeDef",
+    {
+        "FeaturizationPipeline": List[FeaturizationMethodOutputTypeDef],
+    },
+    total=False,
+)
+
+class FeaturizationOutputTypeDef(
+    _RequiredFeaturizationOutputTypeDef, _OptionalFeaturizationOutputTypeDef
+):
+    pass
+
 _RequiredFeaturizationTypeDef = TypedDict(
     "_RequiredFeaturizationTypeDef",
     {
         "AttributeName": str,
     },
 )
 _OptionalFeaturizationTypeDef = TypedDict(
@@ -1226,326 +1324,371 @@
     },
     total=False,
 )
 
 class FeaturizationTypeDef(_RequiredFeaturizationTypeDef, _OptionalFeaturizationTypeDef):
     pass
 
-ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
+ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListDatasetImportJobsRequestRequestTypeDef = TypedDict(
-    "ListDatasetImportJobsRequestRequestTypeDef",
+ListExplainabilitiesRequestRequestTypeDef = TypedDict(
+    "ListExplainabilitiesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
-    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
+ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilitiesRequestRequestTypeDef = TypedDict(
-    "ListExplainabilitiesRequestRequestTypeDef",
+ListForecastExportJobsRequestRequestTypeDef = TypedDict(
+    "ListForecastExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
+ListForecastsRequestRequestTypeDef = TypedDict(
+    "ListForecastsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListExplainabilityExportsRequestRequestTypeDef = TypedDict(
-    "ListExplainabilityExportsRequestRequestTypeDef",
+_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
+    {
+        "MonitorArn": str,
+    },
+)
+_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
-    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
+class ListMonitorEvaluationsRequestRequestTypeDef(
+    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
+    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
+):
+    pass
+
+ListMonitorsRequestRequestTypeDef = TypedDict(
+    "ListMonitorsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastExportJobsRequestRequestTypeDef = TypedDict(
-    "ListForecastExportJobsRequestRequestTypeDef",
+ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
-    "ListForecastsRequestListForecastsPaginateTypeDef",
+ListPredictorsRequestRequestTypeDef = TypedDict(
+    "ListPredictorsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-ListForecastsRequestRequestTypeDef = TypedDict(
-    "ListForecastsRequestRequestTypeDef",
+ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
-_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestRequestTypeDef",
     {
-        "MonitorArn": str,
+        "NextToken": str,
+        "MaxResults": int,
+        "Filters": Sequence[FilterTypeDef],
     },
+    total=False,
 )
-_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+
+ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
-    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
-    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+ListForecastsResponseTypeDef = TypedDict(
+    "ListForecastsResponseTypeDef",
+    {
+        "Forecasts": List[ForecastSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredInputDataConfigOutputTypeDef = TypedDict(
+    "_RequiredInputDataConfigOutputTypeDef",
+    {
+        "DatasetGroupArn": str,
+    },
+)
+_OptionalInputDataConfigOutputTypeDef = TypedDict(
+    "_OptionalInputDataConfigOutputTypeDef",
+    {
+        "SupplementaryFeatures": List[SupplementaryFeatureTypeDef],
+    },
+    total=False,
+)
+
+class InputDataConfigOutputTypeDef(
+    _RequiredInputDataConfigOutputTypeDef, _OptionalInputDataConfigOutputTypeDef
 ):
     pass
 
-_RequiredListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredListMonitorEvaluationsRequestRequestTypeDef",
+_RequiredInputDataConfigTypeDef = TypedDict(
+    "_RequiredInputDataConfigTypeDef",
     {
-        "MonitorArn": str,
+        "DatasetGroupArn": str,
     },
 )
-_OptionalListMonitorEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalListMonitorEvaluationsRequestRequestTypeDef",
+_OptionalInputDataConfigTypeDef = TypedDict(
+    "_OptionalInputDataConfigTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filters": Sequence[FilterTypeDef],
+        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
     },
     total=False,
 )
 
-class ListMonitorEvaluationsRequestRequestTypeDef(
-    _RequiredListMonitorEvaluationsRequestRequestTypeDef,
-    _OptionalListMonitorEvaluationsRequestRequestTypeDef,
-):
+class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
     pass
 
-ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
-    "ListMonitorsRequestListMonitorsPaginateTypeDef",
+ParameterRangesOutputTypeDef = TypedDict(
+    "ParameterRangesOutputTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "CategoricalParameterRanges": List[CategoricalParameterRangeOutputTypeDef],
+        "ContinuousParameterRanges": List[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": List[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListMonitorsRequestRequestTypeDef = TypedDict(
-    "ListMonitorsRequestRequestTypeDef",
+ParameterRangesTypeDef = TypedDict(
+    "ParameterRangesTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
-        "Filters": Sequence[FilterTypeDef],
+        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
+        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
+        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
+ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef = TypedDict(
+    "ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorBacktestExportJobsRequestRequestTypeDef = TypedDict(
-    "ListPredictorBacktestExportJobsRequestRequestTypeDef",
+ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef = TypedDict(
+    "ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
-    "ListPredictorsRequestListPredictorsPaginateTypeDef",
+ListDatasetsRequestListDatasetsPaginateTypeDef = TypedDict(
+    "ListDatasetsRequestListDatasetsPaginateTypeDef",
     {
-        "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListPredictorsRequestRequestTypeDef = TypedDict(
-    "ListPredictorsRequestRequestTypeDef",
+ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef = TypedDict(
+    "ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
+ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef = TypedDict(
+    "ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfAnalysesRequestRequestTypeDef = TypedDict(
-    "ListWhatIfAnalysesRequestRequestTypeDef",
+ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef = TypedDict(
+    "ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
+ListForecastsRequestListForecastsPaginateTypeDef = TypedDict(
+    "ListForecastsRequestListForecastsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastExportsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastExportsRequestRequestTypeDef",
+_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
+    {
+        "MonitorArn": str,
+    },
+)
+_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef = TypedDict(
+    "_OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
+class ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef(
+    _RequiredListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    _OptionalListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+):
+    pass
+
+ListMonitorsRequestListMonitorsPaginateTypeDef = TypedDict(
+    "ListMonitorsRequestListMonitorsPaginateTypeDef",
     {
         "Filters": Sequence[FilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListWhatIfForecastsRequestRequestTypeDef = TypedDict(
-    "ListWhatIfForecastsRequestRequestTypeDef",
+ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef = TypedDict(
+    "ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListForecastsResponseTypeDef = TypedDict(
-    "ListForecastsResponseTypeDef",
+ListPredictorsRequestListPredictorsPaginateTypeDef = TypedDict(
+    "ListPredictorsRequestListPredictorsPaginateTypeDef",
     {
-        "Forecasts": List[ForecastSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredInputDataConfigTypeDef = TypedDict(
-    "_RequiredInputDataConfigTypeDef",
+ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef = TypedDict(
+    "ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef",
     {
-        "DatasetGroupArn": str,
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalInputDataConfigTypeDef = TypedDict(
-    "_OptionalInputDataConfigTypeDef",
+
+ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef",
     {
-        "SupplementaryFeatures": Sequence[SupplementaryFeatureTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class InputDataConfigTypeDef(_RequiredInputDataConfigTypeDef, _OptionalInputDataConfigTypeDef):
-    pass
-
-ParameterRangesTypeDef = TypedDict(
-    "ParameterRangesTypeDef",
+ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef = TypedDict(
+    "ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef",
     {
-        "CategoricalParameterRanges": Sequence[CategoricalParameterRangeTypeDef],
-        "ContinuousParameterRanges": Sequence[ContinuousParameterRangeTypeDef],
-        "IntegerParameterRanges": Sequence[IntegerParameterRangeTypeDef],
+        "Filters": Sequence[FilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitorsResponseTypeDef = TypedDict(
     "ListMonitorsResponseTypeDef",
     {
         "Monitors": List[MonitorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfAnalysesResponseTypeDef = TypedDict(
     "ListWhatIfAnalysesResponseTypeDef",
     {
         "WhatIfAnalyses": List[WhatIfAnalysisSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastsResponseTypeDef = TypedDict(
     "ListWhatIfForecastsResponseTypeDef",
     {
         "WhatIfForecasts": List[WhatIfForecastSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricsTypeDef = TypedDict(
     "MetricsTypeDef",
     {
         "RMSE": float,
@@ -1579,31 +1722,74 @@
     {
         "AlgorithmArn": str,
         "TestWindows": List[TestWindowSummaryTypeDef],
     },
     total=False,
 )
 
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
+    {
+        "Attributes": List[SchemaAttributeTypeDef],
+    },
+    total=False,
+)
+
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "Attributes": Sequence[SchemaAttributeTypeDef],
     },
     total=False,
 )
 
+TimeSeriesTransformationOutputTypeDef = TypedDict(
+    "TimeSeriesTransformationOutputTypeDef",
+    {
+        "Action": ActionTypeDef,
+        "TimeSeriesConditions": List[TimeSeriesConditionTypeDef],
+    },
+    total=False,
+)
+
 TimeSeriesTransformationTypeDef = TypedDict(
     "TimeSeriesTransformationTypeDef",
     {
         "Action": ActionTypeDef,
         "TimeSeriesConditions": Sequence[TimeSeriesConditionTypeDef],
     },
     total=False,
 )
 
+DescribeAutoPredictorResponseTypeDef = TypedDict(
+    "DescribeAutoPredictorResponseTypeDef",
+    {
+        "PredictorArn": str,
+        "PredictorName": str,
+        "ForecastHorizon": int,
+        "ForecastTypes": List[str],
+        "ForecastFrequency": str,
+        "ForecastDimensions": List[str],
+        "DatasetImportJobArns": List[str],
+        "DataConfig": DataConfigOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "OptimizationMetric": OptimizationMetricType,
+        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
+        "MonitorInfo": MonitorInfoTypeDef,
+        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateAutoPredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAutoPredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
     },
 )
 _OptionalCreateAutoPredictorRequestRequestTypeDef = TypedDict(
@@ -1627,54 +1813,29 @@
 
 class CreateAutoPredictorRequestRequestTypeDef(
     _RequiredCreateAutoPredictorRequestRequestTypeDef,
     _OptionalCreateAutoPredictorRequestRequestTypeDef,
 ):
     pass
 
-DescribeAutoPredictorResponseTypeDef = TypedDict(
-    "DescribeAutoPredictorResponseTypeDef",
-    {
-        "PredictorArn": str,
-        "PredictorName": str,
-        "ForecastHorizon": int,
-        "ForecastTypes": List[str],
-        "ForecastFrequency": str,
-        "ForecastDimensions": List[str],
-        "DatasetImportJobArns": List[str],
-        "DataConfig": DataConfigTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "ReferencePredictorSummary": ReferencePredictorSummaryTypeDef,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "OptimizationMetric": OptimizationMetricType,
-        "ExplainabilityInfo": ExplainabilityInfoTypeDef,
-        "MonitorInfo": MonitorInfoTypeDef,
-        "TimeAlignmentBoundary": TimeAlignmentBoundaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+DataConfigUnionTypeDef = Union[DataConfigTypeDef, DataConfigOutputTypeDef]
 BaselineTypeDef = TypedDict(
     "BaselineTypeDef",
     {
         "PredictorBaseline": PredictorBaselineTypeDef,
     },
     total=False,
 )
 
 ListExplainabilitiesResponseTypeDef = TypedDict(
     "ListExplainabilitiesResponseTypeDef",
     {
         "Explainabilities": List[ExplainabilitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateExplainabilityExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateExplainabilityExportRequestRequestTypeDef",
     {
         "ExplainabilityExportName": str,
@@ -1774,15 +1935,15 @@
         "ExplainabilityArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeForecastExportJobResponseTypeDef = TypedDict(
     "DescribeForecastExportJobResponseTypeDef",
     {
         "ForecastExportJobArn": str,
@@ -1790,15 +1951,15 @@
         "ForecastArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePredictorBacktestExportJobResponseTypeDef = TypedDict(
     "DescribePredictorBacktestExportJobResponseTypeDef",
     {
         "PredictorBacktestExportJobArn": str,
@@ -1806,15 +1967,15 @@
         "PredictorArn": str,
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeWhatIfForecastExportResponseTypeDef = TypedDict(
     "DescribeWhatIfForecastExportResponseTypeDef",
     {
         "WhatIfForecastExportArn": str,
@@ -1823,15 +1984,15 @@
         "Destination": DataDestinationTypeDef,
         "Message": str,
         "Status": str,
         "CreationTime": datetime,
         "EstimatedTimeRemainingInMinutes": int,
         "LastModificationTime": datetime,
         "Format": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExplainabilityExportSummaryTypeDef = TypedDict(
     "ExplainabilityExportSummaryTypeDef",
     {
         "ExplainabilityExportArn": str,
@@ -1947,27 +2108,47 @@
         "DataSize": float,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "Format": str,
         "ImportMode": ImportModeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPredictorsResponseTypeDef = TypedDict(
     "ListPredictorsResponseTypeDef",
     {
         "Predictors": List[PredictorSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredFeaturizationConfigOutputTypeDef = TypedDict(
+    "_RequiredFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastFrequency": str,
+    },
+)
+_OptionalFeaturizationConfigOutputTypeDef = TypedDict(
+    "_OptionalFeaturizationConfigOutputTypeDef",
+    {
+        "ForecastDimensions": List[str],
+        "Featurizations": List[FeaturizationOutputTypeDef],
+    },
+    total=False,
+)
+
+class FeaturizationConfigOutputTypeDef(
+    _RequiredFeaturizationConfigOutputTypeDef, _OptionalFeaturizationConfigOutputTypeDef
+):
+    pass
+
 _RequiredFeaturizationConfigTypeDef = TypedDict(
     "_RequiredFeaturizationConfigTypeDef",
     {
         "ForecastFrequency": str,
     },
 )
 _OptionalFeaturizationConfigTypeDef = TypedDict(
@@ -1980,14 +2161,23 @@
 )
 
 class FeaturizationConfigTypeDef(
     _RequiredFeaturizationConfigTypeDef, _OptionalFeaturizationConfigTypeDef
 ):
     pass
 
+InputDataConfigUnionTypeDef = Union[InputDataConfigTypeDef, InputDataConfigOutputTypeDef]
+HyperParameterTuningJobConfigOutputTypeDef = TypedDict(
+    "HyperParameterTuningJobConfigOutputTypeDef",
+    {
+        "ParameterRanges": ParameterRangesOutputTypeDef,
+    },
+    total=False,
+)
+
 HyperParameterTuningJobConfigTypeDef = TypedDict(
     "HyperParameterTuningJobConfigTypeDef",
     {
         "ParameterRanges": ParameterRangesTypeDef,
     },
     total=False,
 )
@@ -2005,26 +2195,96 @@
 )
 
 ListMonitorEvaluationsResponseTypeDef = TypedDict(
     "ListMonitorEvaluationsResponseTypeDef",
     {
         "NextToken": str,
         "PredictorMonitorEvaluations": List[PredictorMonitorEvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PredictorExecutionDetailsTypeDef = TypedDict(
     "PredictorExecutionDetailsTypeDef",
     {
         "PredictorExecutions": List[PredictorExecutionTypeDef],
     },
     total=False,
 )
 
+DescribeDatasetResponseTypeDef = TypedDict(
+    "DescribeDatasetResponseTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": str,
+        "Domain": DomainType,
+        "DatasetType": DatasetTypeType,
+        "DataFrequency": str,
+        "Schema": SchemaOutputTypeDef,
+        "EncryptionConfig": EncryptionConfigTypeDef,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeExplainabilityResponseTypeDef = TypedDict(
+    "DescribeExplainabilityResponseTypeDef",
+    {
+        "ExplainabilityArn": str,
+        "ExplainabilityName": str,
+        "ResourceArn": str,
+        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
+        "EnableVisualization": bool,
+        "DataSource": DataSourceTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "StartDateTime": str,
+        "EndDateTime": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Message": str,
+        "Status": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TimeSeriesIdentifiersOutputTypeDef = TypedDict(
+    "TimeSeriesIdentifiersOutputTypeDef",
+    {
+        "DataSource": DataSourceTypeDef,
+        "Schema": SchemaOutputTypeDef,
+        "Format": str,
+    },
+    total=False,
+)
+
+_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_RequiredTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "S3Config": S3ConfigTypeDef,
+        "Schema": SchemaOutputTypeDef,
+    },
+)
+_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef = TypedDict(
+    "_OptionalTimeSeriesReplacementsDataSourceOutputTypeDef",
+    {
+        "Format": str,
+        "TimestampFormat": str,
+    },
+    total=False,
+)
+
+class TimeSeriesReplacementsDataSourceOutputTypeDef(
+    _RequiredTimeSeriesReplacementsDataSourceOutputTypeDef,
+    _OptionalTimeSeriesReplacementsDataSourceOutputTypeDef,
+):
+    pass
+
 _RequiredCreateDatasetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatasetRequestRequestTypeDef",
     {
         "DatasetName": str,
         "Domain": DomainType,
         "DatasetType": DatasetTypeType,
         "Schema": SchemaTypeDef,
@@ -2068,52 +2328,15 @@
 
 class CreateExplainabilityRequestRequestTypeDef(
     _RequiredCreateExplainabilityRequestRequestTypeDef,
     _OptionalCreateExplainabilityRequestRequestTypeDef,
 ):
     pass
 
-DescribeDatasetResponseTypeDef = TypedDict(
-    "DescribeDatasetResponseTypeDef",
-    {
-        "DatasetArn": str,
-        "DatasetName": str,
-        "Domain": DomainType,
-        "DatasetType": DatasetTypeType,
-        "DataFrequency": str,
-        "Schema": SchemaTypeDef,
-        "EncryptionConfig": EncryptionConfigTypeDef,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeExplainabilityResponseTypeDef = TypedDict(
-    "DescribeExplainabilityResponseTypeDef",
-    {
-        "ExplainabilityArn": str,
-        "ExplainabilityName": str,
-        "ResourceArn": str,
-        "ExplainabilityConfig": ExplainabilityConfigTypeDef,
-        "EnableVisualization": bool,
-        "DataSource": DataSourceTypeDef,
-        "Schema": SchemaTypeDef,
-        "StartDateTime": str,
-        "EndDateTime": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Message": str,
-        "Status": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 TimeSeriesIdentifiersTypeDef = TypedDict(
     "TimeSeriesIdentifiersTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "Schema": SchemaTypeDef,
         "Format": str,
     },
@@ -2138,77 +2361,83 @@
 
 class TimeSeriesReplacementsDataSourceTypeDef(
     _RequiredTimeSeriesReplacementsDataSourceTypeDef,
     _OptionalTimeSeriesReplacementsDataSourceTypeDef,
 ):
     pass
 
+TimeSeriesTransformationUnionTypeDef = Union[
+    TimeSeriesTransformationTypeDef, TimeSeriesTransformationOutputTypeDef
+]
 DescribeMonitorResponseTypeDef = TypedDict(
     "DescribeMonitorResponseTypeDef",
     {
         "MonitorName": str,
         "MonitorArn": str,
         "ResourceArn": str,
         "Status": str,
         "LastEvaluationTime": datetime,
         "LastEvaluationState": str,
         "Baseline": BaselineTypeDef,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "EstimatedEvaluationTimeRemainingInMinutes": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListExplainabilityExportsResponseTypeDef = TypedDict(
     "ListExplainabilityExportsResponseTypeDef",
     {
         "ExplainabilityExports": List[ExplainabilityExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListForecastExportJobsResponseTypeDef = TypedDict(
     "ListForecastExportJobsResponseTypeDef",
     {
         "ForecastExportJobs": List[ForecastExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPredictorBacktestExportJobsResponseTypeDef = TypedDict(
     "ListPredictorBacktestExportJobsResponseTypeDef",
     {
         "PredictorBacktestExportJobs": List[PredictorBacktestExportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWhatIfForecastExportsResponseTypeDef = TypedDict(
     "ListWhatIfForecastExportsResponseTypeDef",
     {
         "WhatIfForecastExports": List[WhatIfForecastExportSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatasetImportJobsResponseTypeDef = TypedDict(
     "ListDatasetImportJobsResponseTypeDef",
     {
         "DatasetImportJobs": List[DatasetImportJobSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FeaturizationConfigUnionTypeDef = Union[
+    FeaturizationConfigTypeDef, FeaturizationConfigOutputTypeDef
+]
 _RequiredCreatePredictorRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePredictorRequestRequestTypeDef",
     {
         "PredictorName": str,
         "ForecastHorizon": int,
         "InputDataConfig": InputDataConfigTypeDef,
         "FeaturizationConfig": FeaturizationConfigTypeDef,
@@ -2233,14 +2462,17 @@
 )
 
 class CreatePredictorRequestRequestTypeDef(
     _RequiredCreatePredictorRequestRequestTypeDef, _OptionalCreatePredictorRequestRequestTypeDef
 ):
     pass
 
+HyperParameterTuningJobConfigUnionTypeDef = Union[
+    HyperParameterTuningJobConfigTypeDef, HyperParameterTuningJobConfigOutputTypeDef
+]
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "AlgorithmArn": str,
         "TestWindows": List[WindowSummaryTypeDef],
     },
     total=False,
@@ -2256,88 +2488,133 @@
         "ForecastHorizon": int,
         "ForecastTypes": List[str],
         "PerformAutoML": bool,
         "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
         "PerformHPO": bool,
         "TrainingParameters": Dict[str, str],
         "EvaluationParameters": EvaluationParametersTypeDef,
-        "HPOConfig": HyperParameterTuningJobConfigTypeDef,
-        "InputDataConfig": InputDataConfigTypeDef,
-        "FeaturizationConfig": FeaturizationConfigTypeDef,
+        "HPOConfig": HyperParameterTuningJobConfigOutputTypeDef,
+        "InputDataConfig": InputDataConfigOutputTypeDef,
+        "FeaturizationConfig": FeaturizationConfigOutputTypeDef,
         "EncryptionConfig": EncryptionConfigTypeDef,
         "PredictorExecutionDetails": PredictorExecutionDetailsTypeDef,
         "EstimatedTimeRemainingInMinutes": int,
         "IsAutoPredictor": bool,
         "DatasetImportJobArns": List[str],
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
         "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TimeSeriesSelectorOutputTypeDef = TypedDict(
+    "TimeSeriesSelectorOutputTypeDef",
+    {
+        "TimeSeriesIdentifiers": TimeSeriesIdentifiersOutputTypeDef,
+    },
+    total=False,
+)
+
+DescribeWhatIfForecastResponseTypeDef = TypedDict(
+    "DescribeWhatIfForecastResponseTypeDef",
+    {
+        "WhatIfForecastName": str,
+        "WhatIfForecastArn": str,
+        "WhatIfAnalysisArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesTransformations": List[TimeSeriesTransformationOutputTypeDef],
+        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceOutputTypeDef,
+        "ForecastTypes": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TimeSeriesSelectorTypeDef = TypedDict(
     "TimeSeriesSelectorTypeDef",
     {
         "TimeSeriesIdentifiers": TimeSeriesIdentifiersTypeDef,
     },
     total=False,
 )
 
+TimeSeriesReplacementsDataSourceUnionTypeDef = Union[
+    TimeSeriesReplacementsDataSourceTypeDef, TimeSeriesReplacementsDataSourceOutputTypeDef
+]
 _RequiredCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateWhatIfForecastRequestRequestTypeDef",
     {
         "WhatIfForecastName": str,
         "WhatIfAnalysisArn": str,
     },
 )
 _OptionalCreateWhatIfForecastRequestRequestTypeDef = TypedDict(
     "_OptionalCreateWhatIfForecastRequestRequestTypeDef",
     {
-        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationTypeDef],
+        "TimeSeriesTransformations": Sequence[TimeSeriesTransformationUnionTypeDef],
         "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
 class CreateWhatIfForecastRequestRequestTypeDef(
     _RequiredCreateWhatIfForecastRequestRequestTypeDef,
     _OptionalCreateWhatIfForecastRequestRequestTypeDef,
 ):
     pass
 
-DescribeWhatIfForecastResponseTypeDef = TypedDict(
-    "DescribeWhatIfForecastResponseTypeDef",
+GetAccuracyMetricsResponseTypeDef = TypedDict(
+    "GetAccuracyMetricsResponseTypeDef",
     {
-        "WhatIfForecastName": str,
-        "WhatIfForecastArn": str,
-        "WhatIfAnalysisArn": str,
+        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
+        "IsAutoPredictor": bool,
+        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
+        "OptimizationMetric": OptimizationMetricType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeForecastResponseTypeDef = TypedDict(
+    "DescribeForecastResponseTypeDef",
+    {
+        "ForecastArn": str,
+        "ForecastName": str,
+        "ForecastTypes": List[str],
+        "PredictorArn": str,
+        "DatasetGroupArn": str,
         "EstimatedTimeRemainingInMinutes": int,
         "Status": str,
         "Message": str,
         "CreationTime": datetime,
         "LastModificationTime": datetime,
-        "TimeSeriesTransformations": List[TimeSeriesTransformationTypeDef],
-        "TimeSeriesReplacementsDataSource": TimeSeriesReplacementsDataSourceTypeDef,
-        "ForecastTypes": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAccuracyMetricsResponseTypeDef = TypedDict(
-    "GetAccuracyMetricsResponseTypeDef",
+DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
+    "DescribeWhatIfAnalysisResponseTypeDef",
     {
-        "PredictorEvaluationResults": List[EvaluationResultTypeDef],
-        "IsAutoPredictor": bool,
-        "AutoMLOverrideStrategy": AutoMLOverrideStrategyType,
-        "OptimizationMetric": OptimizationMetricType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "WhatIfAnalysisName": str,
+        "WhatIfAnalysisArn": str,
+        "ForecastArn": str,
+        "EstimatedTimeRemainingInMinutes": int,
+        "Status": str,
+        "Message": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "TimeSeriesSelector": TimeSeriesSelectorOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateForecastRequestRequestTypeDef = TypedDict(
     "_RequiredCreateForecastRequestRequestTypeDef",
     {
         "ForecastName": str,
@@ -2377,40 +2654,8 @@
 
 class CreateWhatIfAnalysisRequestRequestTypeDef(
     _RequiredCreateWhatIfAnalysisRequestRequestTypeDef,
     _OptionalCreateWhatIfAnalysisRequestRequestTypeDef,
 ):
     pass
 
-DescribeForecastResponseTypeDef = TypedDict(
-    "DescribeForecastResponseTypeDef",
-    {
-        "ForecastArn": str,
-        "ForecastName": str,
-        "ForecastTypes": List[str],
-        "PredictorArn": str,
-        "DatasetGroupArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeWhatIfAnalysisResponseTypeDef = TypedDict(
-    "DescribeWhatIfAnalysisResponseTypeDef",
-    {
-        "WhatIfAnalysisName": str,
-        "WhatIfAnalysisArn": str,
-        "ForecastArn": str,
-        "EstimatedTimeRemainingInMinutes": int,
-        "Status": str,
-        "Message": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "TimeSeriesSelector": TimeSeriesSelectorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
+TimeSeriesSelectorUnionTypeDef = Union[TimeSeriesSelectorTypeDef, TimeSeriesSelectorOutputTypeDef]
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/PKG-INFO` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-forecast
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ForecastService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ForecastService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore forecast type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore forecast type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-forecast"></a>
 
 # types-aiobotocore-forecast
 
 [![PyPI - types-aiobotocore-forecast](https://img.shields.io/pypi/v/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-forecast.svg?color=blue)](https://pypi.org/project/types-aiobotocore-forecast)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-forecast?color=blue)](https://pypistats.org/packages/types-aiobotocore-forecast)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-forecast)](https://pepy.tech/project/types-aiobotocore-forecast)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ForecastService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/forecast.html#ForecastService)
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
 [types-aiobotocore-forecast docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_forecast/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +73,15 @@
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
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
@@ -383,49 +382,39 @@
 )
 
 
 def check_value(value: AttributeTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_forecast.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_forecast.type_defs import (
     ActionTypeDef,
+    AdditionalDatasetOutputTypeDef,
     AdditionalDatasetTypeDef,
+    AttributeConfigOutputTypeDef,
     AttributeConfigTypeDef,
     BaselineMetricTypeDef,
+    CategoricalParameterRangeOutputTypeDef,
     CategoricalParameterRangeTypeDef,
     ContinuousParameterRangeTypeDef,
     EncryptionConfigTypeDef,
     MonitorConfigTypeDef,
     TagTypeDef,
     TimeAlignmentBoundaryTypeDef,
-    CreateAutoPredictorResponseTypeDef,
-    CreateDatasetGroupResponseTypeDef,
-    CreateDatasetImportJobResponseTypeDef,
-    CreateDatasetResponseTypeDef,
-    CreateExplainabilityExportResponseTypeDef,
+    ResponseMetadataTypeDef,
     ExplainabilityConfigTypeDef,
-    CreateExplainabilityResponseTypeDef,
-    CreateForecastExportJobResponseTypeDef,
-    CreateForecastResponseTypeDef,
-    CreateMonitorResponseTypeDef,
-    CreatePredictorBacktestExportJobResponseTypeDef,
     EvaluationParametersTypeDef,
-    CreatePredictorResponseTypeDef,
-    CreateWhatIfAnalysisResponseTypeDef,
-    CreateWhatIfForecastExportResponseTypeDef,
-    CreateWhatIfForecastResponseTypeDef,
     S3ConfigTypeDef,
     DatasetGroupSummaryTypeDef,
     DatasetSummaryTypeDef,
     DeleteDatasetGroupRequestRequestTypeDef,
     DeleteDatasetImportJobRequestRequestTypeDef,
     DeleteDatasetRequestRequestTypeDef,
     DeleteExplainabilityExportRequestRequestTypeDef,
@@ -440,107 +429,128 @@
     DeleteWhatIfForecastExportRequestRequestTypeDef,
     DeleteWhatIfForecastRequestRequestTypeDef,
     DescribeAutoPredictorRequestRequestTypeDef,
     ExplainabilityInfoTypeDef,
     MonitorInfoTypeDef,
     ReferencePredictorSummaryTypeDef,
     DescribeDatasetGroupRequestRequestTypeDef,
-    DescribeDatasetGroupResponseTypeDef,
     DescribeDatasetImportJobRequestRequestTypeDef,
     StatisticsTypeDef,
     DescribeDatasetRequestRequestTypeDef,
     DescribeExplainabilityExportRequestRequestTypeDef,
     DescribeExplainabilityRequestRequestTypeDef,
     DescribeForecastExportJobRequestRequestTypeDef,
     DescribeForecastRequestRequestTypeDef,
     DescribeMonitorRequestRequestTypeDef,
     DescribePredictorBacktestExportJobRequestRequestTypeDef,
     DescribePredictorRequestRequestTypeDef,
     DescribeWhatIfAnalysisRequestRequestTypeDef,
     DescribeWhatIfForecastExportRequestRequestTypeDef,
     DescribeWhatIfForecastRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ErrorMetricTypeDef,
+    FeaturizationMethodOutputTypeDef,
     FeaturizationMethodTypeDef,
     FilterTypeDef,
     ForecastSummaryTypeDef,
     GetAccuracyMetricsRequestRequestTypeDef,
     SupplementaryFeatureTypeDef,
     IntegerParameterRangeTypeDef,
-    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDatasetGroupsRequestRequestTypeDef,
-    ListDatasetsRequestListDatasetsPaginateTypeDef,
     ListDatasetsRequestRequestTypeDef,
     MonitorSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     WhatIfAnalysisSummaryTypeDef,
     WhatIfForecastSummaryTypeDef,
     MetricResultTypeDef,
     WeightedQuantileLossTypeDef,
     MonitorDataSourceTypeDef,
-    PaginatorConfigTypeDef,
     PredictorEventTypeDef,
     TestWindowSummaryTypeDef,
-    ResponseMetadataTypeDef,
     ResumeResourceRequestRequestTypeDef,
     SchemaAttributeTypeDef,
     StopResourceRequestRequestTypeDef,
     TimeSeriesConditionTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatasetGroupRequestRequestTypeDef,
+    DataConfigOutputTypeDef,
     DataConfigTypeDef,
     PredictorBaselineTypeDef,
     CreateDatasetGroupRequestRequestTypeDef,
     CreateMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateAutoPredictorResponseTypeDef,
+    CreateDatasetGroupResponseTypeDef,
+    CreateDatasetImportJobResponseTypeDef,
+    CreateDatasetResponseTypeDef,
+    CreateExplainabilityExportResponseTypeDef,
+    CreateExplainabilityResponseTypeDef,
+    CreateForecastExportJobResponseTypeDef,
+    CreateForecastResponseTypeDef,
+    CreateMonitorResponseTypeDef,
+    CreatePredictorBacktestExportJobResponseTypeDef,
+    CreatePredictorResponseTypeDef,
+    CreateWhatIfAnalysisResponseTypeDef,
+    CreateWhatIfForecastExportResponseTypeDef,
+    CreateWhatIfForecastResponseTypeDef,
+    DescribeDatasetGroupResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ListTagsForResourceResponseTypeDef,
     ExplainabilitySummaryTypeDef,
     DataDestinationTypeDef,
     DataSourceTypeDef,
     ListDatasetGroupsResponseTypeDef,
     ListDatasetsResponseTypeDef,
     PredictorSummaryTypeDef,
+    FeaturizationOutputTypeDef,
     FeaturizationTypeDef,
-    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
     ListDatasetImportJobsRequestRequestTypeDef,
-    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
     ListExplainabilitiesRequestRequestTypeDef,
-    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
     ListExplainabilityExportsRequestRequestTypeDef,
-    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
     ListForecastExportJobsRequestRequestTypeDef,
-    ListForecastsRequestListForecastsPaginateTypeDef,
     ListForecastsRequestRequestTypeDef,
-    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
     ListMonitorEvaluationsRequestRequestTypeDef,
-    ListMonitorsRequestListMonitorsPaginateTypeDef,
     ListMonitorsRequestRequestTypeDef,
-    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
     ListPredictorBacktestExportJobsRequestRequestTypeDef,
-    ListPredictorsRequestListPredictorsPaginateTypeDef,
     ListPredictorsRequestRequestTypeDef,
-    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
     ListWhatIfAnalysesRequestRequestTypeDef,
-    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
     ListWhatIfForecastExportsRequestRequestTypeDef,
-    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListWhatIfForecastsRequestRequestTypeDef,
     ListForecastsResponseTypeDef,
+    InputDataConfigOutputTypeDef,
     InputDataConfigTypeDef,
+    ParameterRangesOutputTypeDef,
     ParameterRangesTypeDef,
+    ListDatasetGroupsRequestListDatasetGroupsPaginateTypeDef,
+    ListDatasetImportJobsRequestListDatasetImportJobsPaginateTypeDef,
+    ListDatasetsRequestListDatasetsPaginateTypeDef,
+    ListExplainabilitiesRequestListExplainabilitiesPaginateTypeDef,
+    ListExplainabilityExportsRequestListExplainabilityExportsPaginateTypeDef,
+    ListForecastExportJobsRequestListForecastExportJobsPaginateTypeDef,
+    ListForecastsRequestListForecastsPaginateTypeDef,
+    ListMonitorEvaluationsRequestListMonitorEvaluationsPaginateTypeDef,
+    ListMonitorsRequestListMonitorsPaginateTypeDef,
+    ListPredictorBacktestExportJobsRequestListPredictorBacktestExportJobsPaginateTypeDef,
+    ListPredictorsRequestListPredictorsPaginateTypeDef,
+    ListWhatIfAnalysesRequestListWhatIfAnalysesPaginateTypeDef,
+    ListWhatIfForecastExportsRequestListWhatIfForecastExportsPaginateTypeDef,
+    ListWhatIfForecastsRequestListWhatIfForecastsPaginateTypeDef,
     ListMonitorsResponseTypeDef,
     ListWhatIfAnalysesResponseTypeDef,
     ListWhatIfForecastsResponseTypeDef,
     MetricsTypeDef,
     PredictorMonitorEvaluationTypeDef,
     PredictorExecutionTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
+    TimeSeriesTransformationOutputTypeDef,
     TimeSeriesTransformationTypeDef,
-    CreateAutoPredictorRequestRequestTypeDef,
     DescribeAutoPredictorResponseTypeDef,
+    CreateAutoPredictorRequestRequestTypeDef,
+    DataConfigUnionTypeDef,
     BaselineTypeDef,
     ListExplainabilitiesResponseTypeDef,
     CreateExplainabilityExportRequestRequestTypeDef,
     CreateForecastExportJobRequestRequestTypeDef,
     CreatePredictorBacktestExportJobRequestRequestTypeDef,
     CreateWhatIfForecastExportRequestRequestTypeDef,
     DescribeExplainabilityExportResponseTypeDef,
@@ -551,46 +561,58 @@
     ForecastExportJobSummaryTypeDef,
     PredictorBacktestExportJobSummaryTypeDef,
     WhatIfForecastExportSummaryTypeDef,
     CreateDatasetImportJobRequestRequestTypeDef,
     DatasetImportJobSummaryTypeDef,
     DescribeDatasetImportJobResponseTypeDef,
     ListPredictorsResponseTypeDef,
+    FeaturizationConfigOutputTypeDef,
     FeaturizationConfigTypeDef,
+    InputDataConfigUnionTypeDef,
+    HyperParameterTuningJobConfigOutputTypeDef,
     HyperParameterTuningJobConfigTypeDef,
     WindowSummaryTypeDef,
     ListMonitorEvaluationsResponseTypeDef,
     PredictorExecutionDetailsTypeDef,
-    CreateDatasetRequestRequestTypeDef,
-    CreateExplainabilityRequestRequestTypeDef,
     DescribeDatasetResponseTypeDef,
     DescribeExplainabilityResponseTypeDef,
+    TimeSeriesIdentifiersOutputTypeDef,
+    TimeSeriesReplacementsDataSourceOutputTypeDef,
+    CreateDatasetRequestRequestTypeDef,
+    CreateExplainabilityRequestRequestTypeDef,
+    SchemaUnionTypeDef,
     TimeSeriesIdentifiersTypeDef,
     TimeSeriesReplacementsDataSourceTypeDef,
+    TimeSeriesTransformationUnionTypeDef,
     DescribeMonitorResponseTypeDef,
     ListExplainabilityExportsResponseTypeDef,
     ListForecastExportJobsResponseTypeDef,
     ListPredictorBacktestExportJobsResponseTypeDef,
     ListWhatIfForecastExportsResponseTypeDef,
     ListDatasetImportJobsResponseTypeDef,
+    FeaturizationConfigUnionTypeDef,
     CreatePredictorRequestRequestTypeDef,
+    HyperParameterTuningJobConfigUnionTypeDef,
     EvaluationResultTypeDef,
     DescribePredictorResponseTypeDef,
+    TimeSeriesSelectorOutputTypeDef,
+    DescribeWhatIfForecastResponseTypeDef,
     TimeSeriesSelectorTypeDef,
+    TimeSeriesReplacementsDataSourceUnionTypeDef,
     CreateWhatIfForecastRequestRequestTypeDef,
-    DescribeWhatIfForecastResponseTypeDef,
     GetAccuracyMetricsResponseTypeDef,
-    CreateForecastRequestRequestTypeDef,
-    CreateWhatIfAnalysisRequestRequestTypeDef,
     DescribeForecastResponseTypeDef,
     DescribeWhatIfAnalysisResponseTypeDef,
+    CreateForecastRequestRequestTypeDef,
+    CreateWhatIfAnalysisRequestRequestTypeDef,
+    TimeSeriesSelectorUnionTypeDef,
 )
 
 
-def get_structure() -> ActionTypeDef:
+def get_value() -> ActionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-forecast-2.5.2/types_aiobotocore_forecast.egg-info/SOURCES.txt` & `types-aiobotocore-forecast-2.5.2.post1/types_aiobotocore_forecast.egg-info/SOURCES.txt`

 * *Files identical despite different names*


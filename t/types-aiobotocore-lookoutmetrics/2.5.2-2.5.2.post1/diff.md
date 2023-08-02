# Comparing `tmp/types-aiobotocore-lookoutmetrics-2.5.2.tar.gz` & `tmp/types-aiobotocore-lookoutmetrics-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lookoutmetrics-2.5.2.tar", last modified: Sat Jul  8 01:43:55 2023, max compression
+gzip compressed data, was "types-aiobotocore-lookoutmetrics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:35 2023, max compression
```

## Comparing `types-aiobotocore-lookoutmetrics-2.5.2.tar` & `types-aiobotocore-lookoutmetrics-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.666471 types-aiobotocore-lookoutmetrics-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-07-08 01:43:55.666471 types-aiobotocore-lookoutmetrics-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15173 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:55.666471 types-aiobotocore-lookoutmetrics-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.650471 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24304 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24266 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    36567 2023-07-08 01:34:24.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    36534 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:23.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.666471 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16766 2023-07-08 01:43:55.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-08 01:43:55.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:43:55.000000 types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15615 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24349 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24311 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    40126 2023-08-02 14:42:34.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40093 2023-08-02 14:42:34.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:33.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:35.901533 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17161 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:35.000000 types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/LICENSE` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/PKG-INFO` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutmetrics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LookoutMetrics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LookoutMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lookoutmetrics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lookoutmetrics"></a>
 
 # types-aiobotocore-lookoutmetrics
 
 [![PyPI - types-aiobotocore-lookoutmetrics](https://img.shields.io/pypi/v/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lookoutmetrics?color=blue)](https://pypistats.org/packages/types-aiobotocore-lookoutmetrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutmetrics)](https://pepy.tech/project/types-aiobotocore-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LookoutMetrics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [types-aiobotocore-lookoutmetrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -294,45 +293,45 @@
 )
 
 
 def check_value(value: AggregationFunctionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lookoutmetrics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lookoutmetrics.type_defs import (
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
+    DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AppFlowConfigTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
-    CreateMetricSetResponseTypeDef,
+    CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
@@ -342,88 +341,101 @@
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
     JsonFormatDescriptorTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
-    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
-    ListAlertsResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
+    CreateMetricSetResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
+    GetSampleDataResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
+    FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
+    RDSSourceConfigOutputTypeDef,
+    RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
+    AlertFiltersUnionTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
+    S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
-    CreateMetricSetRequestRequestTypeDef,
     DescribeMetricSetResponseTypeDef,
+    CreateMetricSetRequestRequestTypeDef,
+    MetricSourceUnionTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_value() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/README.md` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-lookoutmetrics"></a>
 
 # types-aiobotocore-lookoutmetrics
 
 [![PyPI - types-aiobotocore-lookoutmetrics](https://img.shields.io/pypi/v/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lookoutmetrics?color=blue)](https://pypistats.org/packages/types-aiobotocore-lookoutmetrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutmetrics)](https://pepy.tech/project/types-aiobotocore-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LookoutMetrics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [types-aiobotocore-lookoutmetrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -261,45 +261,45 @@
 )
 
 
 def check_value(value: AggregationFunctionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lookoutmetrics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lookoutmetrics.type_defs import (
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
+    DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AppFlowConfigTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
-    CreateMetricSetResponseTypeDef,
+    CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
@@ -309,88 +309,101 @@
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
     JsonFormatDescriptorTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
-    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
-    ListAlertsResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
+    CreateMetricSetResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
+    GetSampleDataResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
+    FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
+    RDSSourceConfigOutputTypeDef,
+    RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
+    AlertFiltersUnionTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
+    S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
-    CreateMetricSetRequestRequestTypeDef,
     DescribeMetricSetResponseTypeDef,
+    CreateMetricSetRequestRequestTypeDef,
+    MetricSourceUnionTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_value() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/setup.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lookoutmetrics",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_lookoutmetrics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LookoutMetrics 2.5.2 service generated with"
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
-    keywords="aiobotocore lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore lookoutmetrics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lookoutmetrics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/"
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/__main__.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LookoutMetrics 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.LookoutMetrics 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics\nOther"
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

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/client.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
-    AlertFiltersTypeDef,
+    AlertFiltersUnionTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     CreateMetricSetResponseTypeDef,
@@ -42,16 +42,16 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricSetDimensionFilterTypeDef,
-    MetricSourceTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
+    MetricSourceUnionTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
 )
@@ -132,15 +132,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_alert)
         """
@@ -163,23 +163,23 @@
 
     async def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: MetricSourceTypeDef,
+        MetricSource: MetricSourceUnionTypeDef,
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_metric_set)
         """
@@ -445,15 +445,15 @@
     async def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_alert)
         """
@@ -479,16 +479,16 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: MetricSourceTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        MetricSource: MetricSourceUnionTypeDef = ...,
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/client.pyi` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import FrequencyType, RelationshipTypeType
 from .type_defs import (
     ActionTypeDef,
-    AlertFiltersTypeDef,
+    AlertFiltersUnionTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AutoDetectionMetricSourceTypeDef,
     CreateAlertResponseTypeDef,
     CreateAnomalyDetectorResponseTypeDef,
     CreateMetricSetResponseTypeDef,
@@ -42,16 +42,16 @@
     ListAlertsResponseTypeDef,
     ListAnomalyDetectorsResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
     ListMetricSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MetricSetDimensionFilterTypeDef,
-    MetricSourceTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
+    MetricSourceUnionTypeDef,
     MetricTypeDef,
     SampleDataS3SourceConfigTypeDef,
     TimestampColumnTypeDef,
     UpdateAlertResponseTypeDef,
     UpdateAnomalyDetectorResponseTypeDef,
     UpdateMetricSetResponseTypeDef,
 )
@@ -124,15 +124,15 @@
         *,
         AlertName: str,
         AnomalyDetectorArn: str,
         Action: ActionTypeDef,
         AlertSensitivityThreshold: int = ...,
         AlertDescription: str = ...,
         Tags: Mapping[str, str] = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> CreateAlertResponseTypeDef:
         """
         Creates an alert for an anomaly detector.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_alert)
         """
@@ -153,23 +153,23 @@
         """
     async def create_metric_set(
         self,
         *,
         AnomalyDetectorArn: str,
         MetricSetName: str,
         MetricList: Sequence[MetricTypeDef],
-        MetricSource: MetricSourceTypeDef,
+        MetricSource: MetricSourceUnionTypeDef,
         MetricSetDescription: str = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
         Timezone: str = ...,
         Tags: Mapping[str, str] = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> CreateMetricSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.create_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#create_metric_set)
         """
@@ -411,15 +411,15 @@
     async def update_alert(
         self,
         *,
         AlertArn: str,
         AlertDescription: str = ...,
         AlertSensitivityThreshold: int = ...,
         Action: ActionTypeDef = ...,
-        AlertFilters: AlertFiltersTypeDef = ...
+        AlertFilters: AlertFiltersUnionTypeDef = ...
     ) -> UpdateAlertResponseTypeDef:
         """
         Make changes to an existing alert.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_alert)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_alert)
         """
@@ -443,16 +443,16 @@
         MetricSetArn: str,
         MetricSetDescription: str = ...,
         MetricList: Sequence[MetricTypeDef] = ...,
         Offset: int = ...,
         TimestampColumn: TimestampColumnTypeDef = ...,
         DimensionList: Sequence[str] = ...,
         MetricSetFrequency: FrequencyType = ...,
-        MetricSource: MetricSourceTypeDef = ...,
-        DimensionFilterList: Sequence[MetricSetDimensionFilterTypeDef] = ...
+        MetricSource: MetricSourceUnionTypeDef = ...,
+        DimensionFilterList: Sequence[MetricSetDimensionFilterUnionTypeDef] = ...
     ) -> UpdateMetricSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics.Client.update_metric_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/client/#update_metric_set)
         """
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/literals.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/literals.pyi` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/type_defs.py` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
-    data: LambdaConfigurationTypeDef = {...}
+    data: LambdaConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregationFunctionType,
     AlertStatusType,
     AlertTypeType,
     AnomalyDetectionTaskStatusType,
     AnomalyDetectorFailureTypeType,
@@ -41,33 +41,33 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
+    "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
     "AppFlowConfigTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
-    "CreateAlertResponseTypeDef",
-    "CreateAnomalyDetectorResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
-    "CreateMetricSetResponseTypeDef",
+    "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
@@ -77,79 +77,92 @@
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
     "JsonFormatDescriptorTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
-    "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlertResponseTypeDef",
-    "UpdateAnomalyDetectorResponseTypeDef",
-    "UpdateMetricSetResponseTypeDef",
     "ActionTypeDef",
+    "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
-    "ListAlertsResponseTypeDef",
-    "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
-    "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
+    "CreateAlertResponseTypeDef",
+    "CreateAnomalyDetectorResponseTypeDef",
+    "CreateMetricSetResponseTypeDef",
+    "DescribeAnomalyDetectorResponseTypeDef",
+    "GetSampleDataResponseTypeDef",
+    "ListAlertsResponseTypeDef",
+    "ListAnomalyDetectorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateAlertResponseTypeDef",
+    "UpdateAnomalyDetectorResponseTypeDef",
+    "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
+    "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
+    "MetricSetDimensionFilterOutputTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
+    "RDSSourceConfigOutputTypeDef",
+    "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
+    "AlertFiltersUnionTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
+    "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
+    "MetricSetDimensionFilterUnionTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
+    "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
-    "CreateMetricSetRequestRequestTypeDef",
     "DescribeMetricSetResponseTypeDef",
+    "CreateMetricSetRequestRequestTypeDef",
+    "MetricSourceUnionTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
@@ -184,14 +197,23 @@
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
+DimensionFilterOutputTypeDef = TypedDict(
+    "DimensionFilterOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueList": List[str],
+    },
+    total=False,
+)
+
 DimensionFilterTypeDef = TypedDict(
     "DimensionFilterTypeDef",
     {
         "DimensionName": str,
         "DimensionValueList": Sequence[str],
     },
     total=False,
@@ -335,27 +357,22 @@
 BackTestAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-CreateAlertResponseTypeDef = TypedDict(
-    "CreateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalyDetectorResponseTypeDef = TypedDict(
-    "CreateAnomalyDetectorResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "MetricName": str,
@@ -380,20 +397,25 @@
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
-CreateMetricSetResponseTypeDef = TypedDict(
-    "CreateMetricSetResponseTypeDef",
+CsvFormatDescriptorOutputTypeDef = TypedDict(
+    "CsvFormatDescriptorOutputTypeDef",
     {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FileCompression": CSVFileCompressionType,
+        "Charset": str,
+        "ContainsHeader": bool,
+        "Delimiter": str,
+        "HeaderList": List[str],
+        "QuoteSymbol": str,
     },
+    total=False,
 )
 
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
@@ -562,23 +584,14 @@
     {
         "TimeSeriesId": str,
         "IsAnomaly": bool,
     },
     total=False,
 )
 
-GetSampleDataResponseTypeDef = TypedDict(
-    "GetSampleDataResponseTypeDef",
-    {
-        "HeaderValues": List[str],
-        "SampleRows": List[List[str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InterMetricImpactDetailsTypeDef = TypedDict(
     "InterMetricImpactDetailsTypeDef",
     {
         "MetricName": str,
         "AnomalyGroupId": str,
         "RelationshipType": RelationshipTypeType,
         "ContributionPercentage": float,
@@ -706,41 +719,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubnetIdList": List[str],
+        "SecurityGroupIdList": List[str],
     },
 )
 
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -749,80 +751,39 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAlertResponseTypeDef = TypedDict(
-    "UpdateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalyDetectorResponseTypeDef = TypedDict(
-    "UpdateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMetricSetResponseTypeDef = TypedDict(
-    "UpdateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
 )
 
-AlertFiltersTypeDef = TypedDict(
-    "AlertFiltersTypeDef",
+AlertFiltersOutputTypeDef = TypedDict(
+    "AlertFiltersOutputTypeDef",
     {
-        "MetricList": Sequence[str],
-        "DimensionFilterList": Sequence[DimensionFilterTypeDef],
+        "MetricList": List[str],
+        "DimensionFilterList": List[DimensionFilterOutputTypeDef],
     },
     total=False,
 )
 
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "AlertSummaryList": List[AlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAnomalyDetectorResponseTypeDef = TypedDict(
-    "DescribeAnomalyDetectorResponseTypeDef",
+AlertFiltersTypeDef = TypedDict(
+    "AlertFiltersTypeDef",
     {
-        "AnomalyDetectorArn": str,
-        "AnomalyDetectorName": str,
-        "AnomalyDetectorDescription": str,
-        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Status": AnomalyDetectorStatusType,
-        "FailureReason": str,
-        "KmsKeyArn": str,
-        "FailureType": AnomalyDetectorFailureTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MetricList": Sequence[str],
+        "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
+    total=False,
 )
 
 _RequiredCreateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorName": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
@@ -866,23 +827,14 @@
 class UpdateAnomalyDetectorRequestRequestTypeDef(
     _RequiredUpdateAnomalyDetectorRequestRequestTypeDef,
     _OptionalUpdateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
 
-ListAnomalyDetectorsResponseTypeDef = TypedDict(
-    "ListAnomalyDetectorsResponseTypeDef",
-    {
-        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnomalyGroupStatisticsTypeDef = TypedDict(
     "AnomalyGroupStatisticsTypeDef",
     {
         "EvaluationStartDate": str,
         "TotalCount": int,
         "ItemizedMetricStatsList": List[ItemizedMetricStatsTypeDef],
     },
@@ -957,29 +909,129 @@
     "AutoDetectionMetricSourceTypeDef",
     {
         "S3SourceConfig": AutoDetectionS3SourceConfigTypeDef,
     },
     total=False,
 )
 
+CreateAlertResponseTypeDef = TypedDict(
+    "CreateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalyDetectorResponseTypeDef = TypedDict(
+    "CreateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMetricSetResponseTypeDef = TypedDict(
+    "CreateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAnomalyDetectorResponseTypeDef = TypedDict(
+    "DescribeAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "AnomalyDetectorName": str,
+        "AnomalyDetectorDescription": str,
+        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Status": AnomalyDetectorStatusType,
+        "FailureReason": str,
+        "KmsKeyArn": str,
+        "FailureType": AnomalyDetectorFailureTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSampleDataResponseTypeDef = TypedDict(
+    "GetSampleDataResponseTypeDef",
+    {
+        "HeaderValues": List[str],
+        "SampleRows": List[List[str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "AlertSummaryList": List[AlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAnomalyDetectorsResponseTypeDef = TypedDict(
+    "ListAnomalyDetectorsResponseTypeDef",
+    {
+        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlertResponseTypeDef = TypedDict(
+    "UpdateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyDetectorResponseTypeDef = TypedDict(
+    "UpdateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMetricSetResponseTypeDef = TypedDict(
+    "UpdateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MetricSetDataQualityMetricTypeDef = TypedDict(
     "MetricSetDataQualityMetricTypeDef",
     {
         "MetricSetArn": str,
         "DataQualityMetricList": List[DataQualityMetricTypeDef],
     },
     total=False,
 )
 
 DescribeAnomalyDetectionExecutionsResponseTypeDef = TypedDict(
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     {
         "ExecutionList": List[ExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DimensionContributionTypeDef = TypedDict(
     "DimensionContributionTypeDef",
     {
         "DimensionName": str,
@@ -993,57 +1045,105 @@
     {
         "TimeSeriesId": str,
         "DimensionList": List[DimensionNameValueTypeDef],
         "MetricValueList": List[float],
     },
 )
 
+FileFormatDescriptorOutputTypeDef = TypedDict(
+    "FileFormatDescriptorOutputTypeDef",
+    {
+        "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
+        "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
+    },
+    total=False,
+)
+
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorTypeDef,
         "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
+MetricSetDimensionFilterOutputTypeDef = TypedDict(
+    "MetricSetDimensionFilterOutputTypeDef",
+    {
+        "Name": str,
+        "FilterList": List[FilterTypeDef],
+    },
+    total=False,
+)
+
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
         "Name": str,
         "FilterList": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 GetFeedbackResponseTypeDef = TypedDict(
     "GetFeedbackResponseTypeDef",
     {
         "AnomalyGroupTimeSeriesFeedback": List[TimeSeriesFeedbackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnomalyGroupRelatedMetricsResponseTypeDef = TypedDict(
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     {
         "InterMetricImpactList": List[InterMetricImpactDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricSetsResponseTypeDef = TypedDict(
     "ListMetricSetsResponseTypeDef",
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RDSSourceConfigOutputTypeDef = TypedDict(
+    "RDSSourceConfigOutputTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
     },
+    total=False,
+)
+
+RedshiftSourceConfigOutputTypeDef = TypedDict(
+    "RedshiftSourceConfigOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+    },
+    total=False,
 )
 
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DatabaseHost": str,
@@ -1081,19 +1181,20 @@
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
         "LastModificationTime": datetime,
         "CreationTime": datetime,
-        "AlertFilters": AlertFiltersTypeDef,
+        "AlertFilters": AlertFiltersOutputTypeDef,
     },
     total=False,
 )
 
+AlertFiltersUnionTypeDef = Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef]
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
         "AlertName": str,
         "AnomalyDetectorArn": str,
         "Action": ActionTypeDef,
     },
@@ -1142,15 +1243,15 @@
 
 ListAnomalyGroupSummariesResponseTypeDef = TypedDict(
     "ListAnomalyGroupSummariesResponseTypeDef",
     {
         "AnomalyGroupSummaryList": List[AnomalyGroupSummaryTypeDef],
         "AnomalyGroupStatistics": AnomalyGroupStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedCsvFormatDescriptorTypeDef = TypedDict(
     "DetectedCsvFormatDescriptorTypeDef",
     {
         "FileCompression": DetectedFieldTypeDef,
@@ -1201,18 +1302,29 @@
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     {
         "AnomalyGroupId": str,
         "MetricName": str,
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+S3SourceConfigOutputTypeDef = TypedDict(
+    "S3SourceConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "TemplatedPathList": List[str],
+        "HistoricalDataPathList": List[str],
+        "FileFormatDescriptor": FileFormatDescriptorOutputTypeDef,
+    },
+    total=False,
+)
+
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
         "FileFormatDescriptor": FileFormatDescriptorTypeDef,
@@ -1239,19 +1351,22 @@
 
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
 
+MetricSetDimensionFilterUnionTypeDef = Union[
+    MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef
+]
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedFileFormatDescriptorTypeDef = TypedDict(
     "DetectedFileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": DetectedCsvFormatDescriptorTypeDef,
@@ -1260,28 +1375,41 @@
     total=False,
 )
 
 GetDataQualityMetricsResponseTypeDef = TypedDict(
     "GetDataQualityMetricsResponseTypeDef",
     {
         "AnomalyDetectorDataQualityMetricList": List[AnomalyDetectorDataQualityMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricLevelImpactTypeDef = TypedDict(
     "MetricLevelImpactTypeDef",
     {
         "MetricName": str,
         "NumTimeSeries": int,
         "ContributionMatrix": ContributionMatrixTypeDef,
     },
     total=False,
 )
 
+MetricSourceOutputTypeDef = TypedDict(
+    "MetricSourceOutputTypeDef",
+    {
+        "S3SourceConfig": S3SourceConfigOutputTypeDef,
+        "AppFlowConfig": AppFlowConfigTypeDef,
+        "CloudWatchConfig": CloudWatchConfigTypeDef,
+        "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
+        "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
+        "AthenaSourceConfig": AthenaSourceConfigTypeDef,
+    },
+    total=False,
+)
+
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
         "S3SourceConfig": S3SourceConfigTypeDef,
         "AppFlowConfig": AppFlowConfigTypeDef,
         "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigTypeDef,
@@ -1316,14 +1444,35 @@
         "AnomalyGroupScore": float,
         "PrimaryMetricName": str,
         "MetricLevelImpactList": List[MetricLevelImpactTypeDef],
     },
     total=False,
 )
 
+DescribeMetricSetResponseTypeDef = TypedDict(
+    "DescribeMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "AnomalyDetectorArn": str,
+        "MetricSetName": str,
+        "MetricSetDescription": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Offset": int,
+        "MetricList": List[MetricTypeDef],
+        "TimestampColumn": TimestampColumnTypeDef,
+        "DimensionList": List[str],
+        "MetricSetFrequency": FrequencyType,
+        "Timezone": str,
+        "MetricSource": MetricSourceOutputTypeDef,
+        "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricList": Sequence[MetricTypeDef],
         "MetricSource": MetricSourceTypeDef,
@@ -1335,47 +1484,27 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
 
-DescribeMetricSetResponseTypeDef = TypedDict(
-    "DescribeMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "AnomalyDetectorArn": str,
-        "MetricSetName": str,
-        "MetricSetDescription": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Offset": int,
-        "MetricList": List[MetricTypeDef],
-        "TimestampColumn": TimestampColumnTypeDef,
-        "DimensionList": List[str],
-        "MetricSetFrequency": FrequencyType,
-        "Timezone": str,
-        "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+MetricSourceUnionTypeDef = Union[MetricSourceTypeDef, MetricSourceOutputTypeDef]
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1384,15 +1513,15 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
@@ -1408,15 +1537,15 @@
     total=False,
 )
 
 GetAnomalyGroupResponseTypeDef = TypedDict(
     "GetAnomalyGroupResponseTypeDef",
     {
         "AnomalyGroup": AnomalyGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedMetricSetConfigTypeDef = TypedDict(
     "DetectedMetricSetConfigTypeDef",
     {
         "Offset": DetectedFieldTypeDef,
@@ -1426,10 +1555,10 @@
     total=False,
 )
 
 DetectMetricSetConfigResponseTypeDef = TypedDict(
     "DetectMetricSetConfigResponseTypeDef",
     {
         "DetectedMetricSetConfig": DetectedMetricSetConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics/type_defs.pyi` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lookoutmetrics.type_defs import LambdaConfigurationTypeDef
 
-    data: LambdaConfigurationTypeDef = {...}
+    data: LambdaConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AggregationFunctionType,
     AlertStatusType,
     AlertTypeType,
     AnomalyDetectionTaskStatusType,
     AnomalyDetectorFailureTypeType,
@@ -40,33 +40,33 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "LambdaConfigurationTypeDef",
     "SNSConfigurationTypeDef",
     "ActivateAnomalyDetectorRequestRequestTypeDef",
+    "DimensionFilterOutputTypeDef",
     "DimensionFilterTypeDef",
     "AlertSummaryTypeDef",
     "AnomalyDetectorConfigSummaryTypeDef",
     "AnomalyDetectorConfigTypeDef",
     "AnomalyDetectorSummaryTypeDef",
     "ItemizedMetricStatsTypeDef",
     "AnomalyGroupSummaryTypeDef",
     "AnomalyGroupTimeSeriesFeedbackTypeDef",
     "AnomalyGroupTimeSeriesTypeDef",
     "AppFlowConfigTypeDef",
     "BackTestConfigurationTypeDef",
     "AttributeValueTypeDef",
     "AutoDetectionS3SourceConfigTypeDef",
     "BackTestAnomalyDetectorRequestRequestTypeDef",
-    "CreateAlertResponseTypeDef",
-    "CreateAnomalyDetectorResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "MetricTypeDef",
     "TimestampColumnTypeDef",
-    "CreateMetricSetResponseTypeDef",
+    "CsvFormatDescriptorOutputTypeDef",
     "CsvFormatDescriptorTypeDef",
     "DataQualityMetricTypeDef",
     "DeactivateAnomalyDetectorRequestRequestTypeDef",
     "DeleteAlertRequestRequestTypeDef",
     "DeleteAnomalyDetectorRequestRequestTypeDef",
     "DescribeAlertRequestRequestTypeDef",
     "DescribeAnomalyDetectionExecutionsRequestRequestTypeDef",
@@ -76,79 +76,92 @@
     "DimensionValueContributionTypeDef",
     "DimensionNameValueTypeDef",
     "JsonFormatDescriptorTypeDef",
     "FilterTypeDef",
     "GetAnomalyGroupRequestRequestTypeDef",
     "GetDataQualityMetricsRequestRequestTypeDef",
     "TimeSeriesFeedbackTypeDef",
-    "GetSampleDataResponseTypeDef",
     "InterMetricImpactDetailsTypeDef",
     "ListAlertsRequestRequestTypeDef",
     "ListAnomalyDetectorsRequestRequestTypeDef",
     "ListAnomalyGroupRelatedMetricsRequestRequestTypeDef",
     "ListAnomalyGroupSummariesRequestRequestTypeDef",
     "ListAnomalyGroupTimeSeriesRequestRequestTypeDef",
     "ListMetricSetsRequestRequestTypeDef",
     "MetricSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
+    "VpcConfigurationOutputTypeDef",
     "VpcConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAlertResponseTypeDef",
-    "UpdateAnomalyDetectorResponseTypeDef",
-    "UpdateMetricSetResponseTypeDef",
     "ActionTypeDef",
+    "AlertFiltersOutputTypeDef",
     "AlertFiltersTypeDef",
-    "ListAlertsResponseTypeDef",
-    "DescribeAnomalyDetectorResponseTypeDef",
     "CreateAnomalyDetectorRequestRequestTypeDef",
     "UpdateAnomalyDetectorRequestRequestTypeDef",
-    "ListAnomalyDetectorsResponseTypeDef",
     "AnomalyGroupStatisticsTypeDef",
     "PutFeedbackRequestRequestTypeDef",
     "GetFeedbackRequestRequestTypeDef",
     "AthenaSourceConfigTypeDef",
     "CloudWatchConfigTypeDef",
     "DetectedFieldTypeDef",
     "AutoDetectionMetricSourceTypeDef",
+    "CreateAlertResponseTypeDef",
+    "CreateAnomalyDetectorResponseTypeDef",
+    "CreateMetricSetResponseTypeDef",
+    "DescribeAnomalyDetectorResponseTypeDef",
+    "GetSampleDataResponseTypeDef",
+    "ListAlertsResponseTypeDef",
+    "ListAnomalyDetectorsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateAlertResponseTypeDef",
+    "UpdateAnomalyDetectorResponseTypeDef",
+    "UpdateMetricSetResponseTypeDef",
     "MetricSetDataQualityMetricTypeDef",
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     "DimensionContributionTypeDef",
     "TimeSeriesTypeDef",
+    "FileFormatDescriptorOutputTypeDef",
     "FileFormatDescriptorTypeDef",
+    "MetricSetDimensionFilterOutputTypeDef",
     "MetricSetDimensionFilterTypeDef",
     "GetFeedbackResponseTypeDef",
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     "ListMetricSetsResponseTypeDef",
+    "RDSSourceConfigOutputTypeDef",
+    "RedshiftSourceConfigOutputTypeDef",
     "RDSSourceConfigTypeDef",
     "RedshiftSourceConfigTypeDef",
     "AlertTypeDef",
+    "AlertFiltersUnionTypeDef",
     "CreateAlertRequestRequestTypeDef",
     "UpdateAlertRequestRequestTypeDef",
     "ListAnomalyGroupSummariesResponseTypeDef",
     "DetectedCsvFormatDescriptorTypeDef",
     "DetectedJsonFormatDescriptorTypeDef",
     "DetectMetricSetConfigRequestRequestTypeDef",
     "AnomalyDetectorDataQualityMetricTypeDef",
     "ContributionMatrixTypeDef",
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
+    "S3SourceConfigOutputTypeDef",
     "S3SourceConfigTypeDef",
     "SampleDataS3SourceConfigTypeDef",
+    "MetricSetDimensionFilterUnionTypeDef",
     "DescribeAlertResponseTypeDef",
     "DetectedFileFormatDescriptorTypeDef",
     "GetDataQualityMetricsResponseTypeDef",
     "MetricLevelImpactTypeDef",
+    "MetricSourceOutputTypeDef",
     "MetricSourceTypeDef",
     "GetSampleDataRequestRequestTypeDef",
     "DetectedS3SourceConfigTypeDef",
     "AnomalyGroupTypeDef",
-    "CreateMetricSetRequestRequestTypeDef",
     "DescribeMetricSetResponseTypeDef",
+    "CreateMetricSetRequestRequestTypeDef",
+    "MetricSourceUnionTypeDef",
     "UpdateMetricSetRequestRequestTypeDef",
     "DetectedMetricSourceTypeDef",
     "GetAnomalyGroupResponseTypeDef",
     "DetectedMetricSetConfigTypeDef",
     "DetectMetricSetConfigResponseTypeDef",
 )
 
@@ -181,14 +194,23 @@
 ActivateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "ActivateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
+DimensionFilterOutputTypeDef = TypedDict(
+    "DimensionFilterOutputTypeDef",
+    {
+        "DimensionName": str,
+        "DimensionValueList": List[str],
+    },
+    total=False,
+)
+
 DimensionFilterTypeDef = TypedDict(
     "DimensionFilterTypeDef",
     {
         "DimensionName": str,
         "DimensionValueList": Sequence[str],
     },
     total=False,
@@ -330,27 +352,22 @@
 BackTestAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "BackTestAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
     },
 )
 
-CreateAlertResponseTypeDef = TypedDict(
-    "CreateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalyDetectorResponseTypeDef = TypedDict(
-    "CreateAnomalyDetectorResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredMetricTypeDef = TypedDict(
     "_RequiredMetricTypeDef",
     {
         "MetricName": str,
@@ -373,20 +390,25 @@
     {
         "ColumnName": str,
         "ColumnFormat": str,
     },
     total=False,
 )
 
-CreateMetricSetResponseTypeDef = TypedDict(
-    "CreateMetricSetResponseTypeDef",
+CsvFormatDescriptorOutputTypeDef = TypedDict(
+    "CsvFormatDescriptorOutputTypeDef",
     {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "FileCompression": CSVFileCompressionType,
+        "Charset": str,
+        "ContainsHeader": bool,
+        "Delimiter": str,
+        "HeaderList": List[str],
+        "QuoteSymbol": str,
     },
+    total=False,
 )
 
 CsvFormatDescriptorTypeDef = TypedDict(
     "CsvFormatDescriptorTypeDef",
     {
         "FileCompression": CSVFileCompressionType,
         "Charset": str,
@@ -551,23 +573,14 @@
     {
         "TimeSeriesId": str,
         "IsAnomaly": bool,
     },
     total=False,
 )
 
-GetSampleDataResponseTypeDef = TypedDict(
-    "GetSampleDataResponseTypeDef",
-    {
-        "HeaderValues": List[str],
-        "SampleRows": List[List[str]],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InterMetricImpactDetailsTypeDef = TypedDict(
     "InterMetricImpactDetailsTypeDef",
     {
         "MetricName": str,
         "AnomalyGroupId": str,
         "RelationshipType": RelationshipTypeType,
         "ContributionPercentage": float,
@@ -689,41 +702,30 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+VpcConfigurationOutputTypeDef = TypedDict(
+    "VpcConfigurationOutputTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubnetIdList": List[str],
+        "SecurityGroupIdList": List[str],
     },
 )
 
 VpcConfigurationTypeDef = TypedDict(
     "VpcConfigurationTypeDef",
     {
         "SubnetIdList": Sequence[str],
         "SecurityGroupIdList": Sequence[str],
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -732,80 +734,39 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateAlertResponseTypeDef = TypedDict(
-    "UpdateAlertResponseTypeDef",
-    {
-        "AlertArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalyDetectorResponseTypeDef = TypedDict(
-    "UpdateAnomalyDetectorResponseTypeDef",
-    {
-        "AnomalyDetectorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateMetricSetResponseTypeDef = TypedDict(
-    "UpdateMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActionTypeDef = TypedDict(
     "ActionTypeDef",
     {
         "SNSConfiguration": SNSConfigurationTypeDef,
         "LambdaConfiguration": LambdaConfigurationTypeDef,
     },
     total=False,
 )
 
-AlertFiltersTypeDef = TypedDict(
-    "AlertFiltersTypeDef",
+AlertFiltersOutputTypeDef = TypedDict(
+    "AlertFiltersOutputTypeDef",
     {
-        "MetricList": Sequence[str],
-        "DimensionFilterList": Sequence[DimensionFilterTypeDef],
+        "MetricList": List[str],
+        "DimensionFilterList": List[DimensionFilterOutputTypeDef],
     },
     total=False,
 )
 
-ListAlertsResponseTypeDef = TypedDict(
-    "ListAlertsResponseTypeDef",
-    {
-        "AlertSummaryList": List[AlertSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAnomalyDetectorResponseTypeDef = TypedDict(
-    "DescribeAnomalyDetectorResponseTypeDef",
+AlertFiltersTypeDef = TypedDict(
+    "AlertFiltersTypeDef",
     {
-        "AnomalyDetectorArn": str,
-        "AnomalyDetectorName": str,
-        "AnomalyDetectorDescription": str,
-        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Status": AnomalyDetectorStatusType,
-        "FailureReason": str,
-        "KmsKeyArn": str,
-        "FailureType": AnomalyDetectorFailureTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MetricList": Sequence[str],
+        "DimensionFilterList": Sequence[DimensionFilterTypeDef],
     },
+    total=False,
 )
 
 _RequiredCreateAnomalyDetectorRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalyDetectorRequestRequestTypeDef",
     {
         "AnomalyDetectorName": str,
         "AnomalyDetectorConfig": AnomalyDetectorConfigTypeDef,
@@ -845,23 +806,14 @@
 
 class UpdateAnomalyDetectorRequestRequestTypeDef(
     _RequiredUpdateAnomalyDetectorRequestRequestTypeDef,
     _OptionalUpdateAnomalyDetectorRequestRequestTypeDef,
 ):
     pass
 
-ListAnomalyDetectorsResponseTypeDef = TypedDict(
-    "ListAnomalyDetectorsResponseTypeDef",
-    {
-        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AnomalyGroupStatisticsTypeDef = TypedDict(
     "AnomalyGroupStatisticsTypeDef",
     {
         "EvaluationStartDate": str,
         "TotalCount": int,
         "ItemizedMetricStatsList": List[ItemizedMetricStatsTypeDef],
     },
@@ -934,29 +886,129 @@
     "AutoDetectionMetricSourceTypeDef",
     {
         "S3SourceConfig": AutoDetectionS3SourceConfigTypeDef,
     },
     total=False,
 )
 
+CreateAlertResponseTypeDef = TypedDict(
+    "CreateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalyDetectorResponseTypeDef = TypedDict(
+    "CreateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMetricSetResponseTypeDef = TypedDict(
+    "CreateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAnomalyDetectorResponseTypeDef = TypedDict(
+    "DescribeAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "AnomalyDetectorName": str,
+        "AnomalyDetectorDescription": str,
+        "AnomalyDetectorConfig": AnomalyDetectorConfigSummaryTypeDef,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Status": AnomalyDetectorStatusType,
+        "FailureReason": str,
+        "KmsKeyArn": str,
+        "FailureType": AnomalyDetectorFailureTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSampleDataResponseTypeDef = TypedDict(
+    "GetSampleDataResponseTypeDef",
+    {
+        "HeaderValues": List[str],
+        "SampleRows": List[List[str]],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAlertsResponseTypeDef = TypedDict(
+    "ListAlertsResponseTypeDef",
+    {
+        "AlertSummaryList": List[AlertSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAnomalyDetectorsResponseTypeDef = TypedDict(
+    "ListAnomalyDetectorsResponseTypeDef",
+    {
+        "AnomalyDetectorSummaryList": List[AnomalyDetectorSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAlertResponseTypeDef = TypedDict(
+    "UpdateAlertResponseTypeDef",
+    {
+        "AlertArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyDetectorResponseTypeDef = TypedDict(
+    "UpdateAnomalyDetectorResponseTypeDef",
+    {
+        "AnomalyDetectorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateMetricSetResponseTypeDef = TypedDict(
+    "UpdateMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 MetricSetDataQualityMetricTypeDef = TypedDict(
     "MetricSetDataQualityMetricTypeDef",
     {
         "MetricSetArn": str,
         "DataQualityMetricList": List[DataQualityMetricTypeDef],
     },
     total=False,
 )
 
 DescribeAnomalyDetectionExecutionsResponseTypeDef = TypedDict(
     "DescribeAnomalyDetectionExecutionsResponseTypeDef",
     {
         "ExecutionList": List[ExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DimensionContributionTypeDef = TypedDict(
     "DimensionContributionTypeDef",
     {
         "DimensionName": str,
@@ -970,57 +1022,105 @@
     {
         "TimeSeriesId": str,
         "DimensionList": List[DimensionNameValueTypeDef],
         "MetricValueList": List[float],
     },
 )
 
+FileFormatDescriptorOutputTypeDef = TypedDict(
+    "FileFormatDescriptorOutputTypeDef",
+    {
+        "CsvFormatDescriptor": CsvFormatDescriptorOutputTypeDef,
+        "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
+    },
+    total=False,
+)
+
 FileFormatDescriptorTypeDef = TypedDict(
     "FileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": CsvFormatDescriptorTypeDef,
         "JsonFormatDescriptor": JsonFormatDescriptorTypeDef,
     },
     total=False,
 )
 
+MetricSetDimensionFilterOutputTypeDef = TypedDict(
+    "MetricSetDimensionFilterOutputTypeDef",
+    {
+        "Name": str,
+        "FilterList": List[FilterTypeDef],
+    },
+    total=False,
+)
+
 MetricSetDimensionFilterTypeDef = TypedDict(
     "MetricSetDimensionFilterTypeDef",
     {
         "Name": str,
         "FilterList": Sequence[FilterTypeDef],
     },
     total=False,
 )
 
 GetFeedbackResponseTypeDef = TypedDict(
     "GetFeedbackResponseTypeDef",
     {
         "AnomalyGroupTimeSeriesFeedback": List[TimeSeriesFeedbackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAnomalyGroupRelatedMetricsResponseTypeDef = TypedDict(
     "ListAnomalyGroupRelatedMetricsResponseTypeDef",
     {
         "InterMetricImpactList": List[InterMetricImpactDetailsTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricSetsResponseTypeDef = TypedDict(
     "ListMetricSetsResponseTypeDef",
     {
         "MetricSetSummaryList": List[MetricSetSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RDSSourceConfigOutputTypeDef = TypedDict(
+    "RDSSourceConfigOutputTypeDef",
+    {
+        "DBInstanceIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
     },
+    total=False,
+)
+
+RedshiftSourceConfigOutputTypeDef = TypedDict(
+    "RedshiftSourceConfigOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DatabaseHost": str,
+        "DatabasePort": int,
+        "SecretManagerArn": str,
+        "DatabaseName": str,
+        "TableName": str,
+        "RoleArn": str,
+        "VpcConfiguration": VpcConfigurationOutputTypeDef,
+    },
+    total=False,
 )
 
 RDSSourceConfigTypeDef = TypedDict(
     "RDSSourceConfigTypeDef",
     {
         "DBInstanceIdentifier": str,
         "DatabaseHost": str,
@@ -1058,19 +1158,20 @@
         "AnomalyDetectorArn": str,
         "AlertName": str,
         "AlertSensitivityThreshold": int,
         "AlertType": AlertTypeType,
         "AlertStatus": AlertStatusType,
         "LastModificationTime": datetime,
         "CreationTime": datetime,
-        "AlertFilters": AlertFiltersTypeDef,
+        "AlertFilters": AlertFiltersOutputTypeDef,
     },
     total=False,
 )
 
+AlertFiltersUnionTypeDef = Union[AlertFiltersTypeDef, AlertFiltersOutputTypeDef]
 _RequiredCreateAlertRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAlertRequestRequestTypeDef",
     {
         "AlertName": str,
         "AnomalyDetectorArn": str,
         "Action": ActionTypeDef,
     },
@@ -1115,15 +1216,15 @@
 
 ListAnomalyGroupSummariesResponseTypeDef = TypedDict(
     "ListAnomalyGroupSummariesResponseTypeDef",
     {
         "AnomalyGroupSummaryList": List[AnomalyGroupSummaryTypeDef],
         "AnomalyGroupStatistics": AnomalyGroupStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedCsvFormatDescriptorTypeDef = TypedDict(
     "DetectedCsvFormatDescriptorTypeDef",
     {
         "FileCompression": DetectedFieldTypeDef,
@@ -1174,18 +1275,29 @@
     "ListAnomalyGroupTimeSeriesResponseTypeDef",
     {
         "AnomalyGroupId": str,
         "MetricName": str,
         "TimestampList": List[str],
         "NextToken": str,
         "TimeSeriesList": List[TimeSeriesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+S3SourceConfigOutputTypeDef = TypedDict(
+    "S3SourceConfigOutputTypeDef",
+    {
+        "RoleArn": str,
+        "TemplatedPathList": List[str],
+        "HistoricalDataPathList": List[str],
+        "FileFormatDescriptor": FileFormatDescriptorOutputTypeDef,
+    },
+    total=False,
+)
+
 S3SourceConfigTypeDef = TypedDict(
     "S3SourceConfigTypeDef",
     {
         "RoleArn": str,
         "TemplatedPathList": Sequence[str],
         "HistoricalDataPathList": Sequence[str],
         "FileFormatDescriptor": FileFormatDescriptorTypeDef,
@@ -1210,19 +1322,22 @@
 )
 
 class SampleDataS3SourceConfigTypeDef(
     _RequiredSampleDataS3SourceConfigTypeDef, _OptionalSampleDataS3SourceConfigTypeDef
 ):
     pass
 
+MetricSetDimensionFilterUnionTypeDef = Union[
+    MetricSetDimensionFilterTypeDef, MetricSetDimensionFilterOutputTypeDef
+]
 DescribeAlertResponseTypeDef = TypedDict(
     "DescribeAlertResponseTypeDef",
     {
         "Alert": AlertTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedFileFormatDescriptorTypeDef = TypedDict(
     "DetectedFileFormatDescriptorTypeDef",
     {
         "CsvFormatDescriptor": DetectedCsvFormatDescriptorTypeDef,
@@ -1231,28 +1346,41 @@
     total=False,
 )
 
 GetDataQualityMetricsResponseTypeDef = TypedDict(
     "GetDataQualityMetricsResponseTypeDef",
     {
         "AnomalyDetectorDataQualityMetricList": List[AnomalyDetectorDataQualityMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MetricLevelImpactTypeDef = TypedDict(
     "MetricLevelImpactTypeDef",
     {
         "MetricName": str,
         "NumTimeSeries": int,
         "ContributionMatrix": ContributionMatrixTypeDef,
     },
     total=False,
 )
 
+MetricSourceOutputTypeDef = TypedDict(
+    "MetricSourceOutputTypeDef",
+    {
+        "S3SourceConfig": S3SourceConfigOutputTypeDef,
+        "AppFlowConfig": AppFlowConfigTypeDef,
+        "CloudWatchConfig": CloudWatchConfigTypeDef,
+        "RDSSourceConfig": RDSSourceConfigOutputTypeDef,
+        "RedshiftSourceConfig": RedshiftSourceConfigOutputTypeDef,
+        "AthenaSourceConfig": AthenaSourceConfigTypeDef,
+    },
+    total=False,
+)
+
 MetricSourceTypeDef = TypedDict(
     "MetricSourceTypeDef",
     {
         "S3SourceConfig": S3SourceConfigTypeDef,
         "AppFlowConfig": AppFlowConfigTypeDef,
         "CloudWatchConfig": CloudWatchConfigTypeDef,
         "RDSSourceConfig": RDSSourceConfigTypeDef,
@@ -1287,14 +1415,35 @@
         "AnomalyGroupScore": float,
         "PrimaryMetricName": str,
         "MetricLevelImpactList": List[MetricLevelImpactTypeDef],
     },
     total=False,
 )
 
+DescribeMetricSetResponseTypeDef = TypedDict(
+    "DescribeMetricSetResponseTypeDef",
+    {
+        "MetricSetArn": str,
+        "AnomalyDetectorArn": str,
+        "MetricSetName": str,
+        "MetricSetDescription": str,
+        "CreationTime": datetime,
+        "LastModificationTime": datetime,
+        "Offset": int,
+        "MetricList": List[MetricTypeDef],
+        "TimestampColumn": TimestampColumnTypeDef,
+        "DimensionList": List[str],
+        "MetricSetFrequency": FrequencyType,
+        "Timezone": str,
+        "MetricSource": MetricSourceOutputTypeDef,
+        "DimensionFilterList": List[MetricSetDimensionFilterOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMetricSetRequestRequestTypeDef",
     {
         "AnomalyDetectorArn": str,
         "MetricSetName": str,
         "MetricList": Sequence[MetricTypeDef],
         "MetricSource": MetricSourceTypeDef,
@@ -1306,45 +1455,25 @@
         "MetricSetDescription": str,
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "Timezone": str,
         "Tags": Mapping[str, str],
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 class CreateMetricSetRequestRequestTypeDef(
     _RequiredCreateMetricSetRequestRequestTypeDef, _OptionalCreateMetricSetRequestRequestTypeDef
 ):
     pass
 
-DescribeMetricSetResponseTypeDef = TypedDict(
-    "DescribeMetricSetResponseTypeDef",
-    {
-        "MetricSetArn": str,
-        "AnomalyDetectorArn": str,
-        "MetricSetName": str,
-        "MetricSetDescription": str,
-        "CreationTime": datetime,
-        "LastModificationTime": datetime,
-        "Offset": int,
-        "MetricList": List[MetricTypeDef],
-        "TimestampColumn": TimestampColumnTypeDef,
-        "DimensionList": List[str],
-        "MetricSetFrequency": FrequencyType,
-        "Timezone": str,
-        "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": List[MetricSetDimensionFilterTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+MetricSourceUnionTypeDef = Union[MetricSourceTypeDef, MetricSourceOutputTypeDef]
 _RequiredUpdateMetricSetRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMetricSetRequestRequestTypeDef",
     {
         "MetricSetArn": str,
     },
 )
 _OptionalUpdateMetricSetRequestRequestTypeDef = TypedDict(
@@ -1353,15 +1482,15 @@
         "MetricSetDescription": str,
         "MetricList": Sequence[MetricTypeDef],
         "Offset": int,
         "TimestampColumn": TimestampColumnTypeDef,
         "DimensionList": Sequence[str],
         "MetricSetFrequency": FrequencyType,
         "MetricSource": MetricSourceTypeDef,
-        "DimensionFilterList": Sequence[MetricSetDimensionFilterTypeDef],
+        "DimensionFilterList": Sequence[MetricSetDimensionFilterUnionTypeDef],
     },
     total=False,
 )
 
 class UpdateMetricSetRequestRequestTypeDef(
     _RequiredUpdateMetricSetRequestRequestTypeDef, _OptionalUpdateMetricSetRequestRequestTypeDef
 ):
@@ -1375,15 +1504,15 @@
     total=False,
 )
 
 GetAnomalyGroupResponseTypeDef = TypedDict(
     "GetAnomalyGroupResponseTypeDef",
     {
         "AnomalyGroup": AnomalyGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectedMetricSetConfigTypeDef = TypedDict(
     "DetectedMetricSetConfigTypeDef",
     {
         "Offset": DetectedFieldTypeDef,
@@ -1393,10 +1522,10 @@
     total=False,
 )
 
 DetectMetricSetConfigResponseTypeDef = TypedDict(
     "DetectMetricSetConfigResponseTypeDef",
     {
         "DetectedMetricSetConfig": DetectedMetricSetConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lookoutmetrics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LookoutMetrics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LookoutMetrics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lookoutmetrics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lookoutmetrics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lookoutmetrics"></a>
 
 # types-aiobotocore-lookoutmetrics
 
 [![PyPI - types-aiobotocore-lookoutmetrics](https://img.shields.io/pypi/v/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lookoutmetrics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lookoutmetrics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lookoutmetrics?color=blue)](https://pypistats.org/packages/types-aiobotocore-lookoutmetrics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lookoutmetrics)](https://pepy.tech/project/types-aiobotocore-lookoutmetrics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LookoutMetrics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lookoutmetrics.html#LookoutMetrics)
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
 [types-aiobotocore-lookoutmetrics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lookoutmetrics/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -294,45 +293,45 @@
 )
 
 
 def check_value(value: AggregationFunctionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lookoutmetrics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lookoutmetrics.type_defs import (
     LambdaConfigurationTypeDef,
     SNSConfigurationTypeDef,
     ActivateAnomalyDetectorRequestRequestTypeDef,
+    DimensionFilterOutputTypeDef,
     DimensionFilterTypeDef,
     AlertSummaryTypeDef,
     AnomalyDetectorConfigSummaryTypeDef,
     AnomalyDetectorConfigTypeDef,
     AnomalyDetectorSummaryTypeDef,
     ItemizedMetricStatsTypeDef,
     AnomalyGroupSummaryTypeDef,
     AnomalyGroupTimeSeriesFeedbackTypeDef,
     AnomalyGroupTimeSeriesTypeDef,
     AppFlowConfigTypeDef,
     BackTestConfigurationTypeDef,
     AttributeValueTypeDef,
     AutoDetectionS3SourceConfigTypeDef,
     BackTestAnomalyDetectorRequestRequestTypeDef,
-    CreateAlertResponseTypeDef,
-    CreateAnomalyDetectorResponseTypeDef,
+    ResponseMetadataTypeDef,
     MetricTypeDef,
     TimestampColumnTypeDef,
-    CreateMetricSetResponseTypeDef,
+    CsvFormatDescriptorOutputTypeDef,
     CsvFormatDescriptorTypeDef,
     DataQualityMetricTypeDef,
     DeactivateAnomalyDetectorRequestRequestTypeDef,
     DeleteAlertRequestRequestTypeDef,
     DeleteAnomalyDetectorRequestRequestTypeDef,
     DescribeAlertRequestRequestTypeDef,
     DescribeAnomalyDetectionExecutionsRequestRequestTypeDef,
@@ -342,88 +341,101 @@
     DimensionValueContributionTypeDef,
     DimensionNameValueTypeDef,
     JsonFormatDescriptorTypeDef,
     FilterTypeDef,
     GetAnomalyGroupRequestRequestTypeDef,
     GetDataQualityMetricsRequestRequestTypeDef,
     TimeSeriesFeedbackTypeDef,
-    GetSampleDataResponseTypeDef,
     InterMetricImpactDetailsTypeDef,
     ListAlertsRequestRequestTypeDef,
     ListAnomalyDetectorsRequestRequestTypeDef,
     ListAnomalyGroupRelatedMetricsRequestRequestTypeDef,
     ListAnomalyGroupSummariesRequestRequestTypeDef,
     ListAnomalyGroupTimeSeriesRequestRequestTypeDef,
     ListMetricSetsRequestRequestTypeDef,
     MetricSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
+    VpcConfigurationOutputTypeDef,
     VpcConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAlertResponseTypeDef,
-    UpdateAnomalyDetectorResponseTypeDef,
-    UpdateMetricSetResponseTypeDef,
     ActionTypeDef,
+    AlertFiltersOutputTypeDef,
     AlertFiltersTypeDef,
-    ListAlertsResponseTypeDef,
-    DescribeAnomalyDetectorResponseTypeDef,
     CreateAnomalyDetectorRequestRequestTypeDef,
     UpdateAnomalyDetectorRequestRequestTypeDef,
-    ListAnomalyDetectorsResponseTypeDef,
     AnomalyGroupStatisticsTypeDef,
     PutFeedbackRequestRequestTypeDef,
     GetFeedbackRequestRequestTypeDef,
     AthenaSourceConfigTypeDef,
     CloudWatchConfigTypeDef,
     DetectedFieldTypeDef,
     AutoDetectionMetricSourceTypeDef,
+    CreateAlertResponseTypeDef,
+    CreateAnomalyDetectorResponseTypeDef,
+    CreateMetricSetResponseTypeDef,
+    DescribeAnomalyDetectorResponseTypeDef,
+    GetSampleDataResponseTypeDef,
+    ListAlertsResponseTypeDef,
+    ListAnomalyDetectorsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateAlertResponseTypeDef,
+    UpdateAnomalyDetectorResponseTypeDef,
+    UpdateMetricSetResponseTypeDef,
     MetricSetDataQualityMetricTypeDef,
     DescribeAnomalyDetectionExecutionsResponseTypeDef,
     DimensionContributionTypeDef,
     TimeSeriesTypeDef,
+    FileFormatDescriptorOutputTypeDef,
     FileFormatDescriptorTypeDef,
+    MetricSetDimensionFilterOutputTypeDef,
     MetricSetDimensionFilterTypeDef,
     GetFeedbackResponseTypeDef,
     ListAnomalyGroupRelatedMetricsResponseTypeDef,
     ListMetricSetsResponseTypeDef,
+    RDSSourceConfigOutputTypeDef,
+    RedshiftSourceConfigOutputTypeDef,
     RDSSourceConfigTypeDef,
     RedshiftSourceConfigTypeDef,
     AlertTypeDef,
+    AlertFiltersUnionTypeDef,
     CreateAlertRequestRequestTypeDef,
     UpdateAlertRequestRequestTypeDef,
     ListAnomalyGroupSummariesResponseTypeDef,
     DetectedCsvFormatDescriptorTypeDef,
     DetectedJsonFormatDescriptorTypeDef,
     DetectMetricSetConfigRequestRequestTypeDef,
     AnomalyDetectorDataQualityMetricTypeDef,
     ContributionMatrixTypeDef,
     ListAnomalyGroupTimeSeriesResponseTypeDef,
+    S3SourceConfigOutputTypeDef,
     S3SourceConfigTypeDef,
     SampleDataS3SourceConfigTypeDef,
+    MetricSetDimensionFilterUnionTypeDef,
     DescribeAlertResponseTypeDef,
     DetectedFileFormatDescriptorTypeDef,
     GetDataQualityMetricsResponseTypeDef,
     MetricLevelImpactTypeDef,
+    MetricSourceOutputTypeDef,
     MetricSourceTypeDef,
     GetSampleDataRequestRequestTypeDef,
     DetectedS3SourceConfigTypeDef,
     AnomalyGroupTypeDef,
-    CreateMetricSetRequestRequestTypeDef,
     DescribeMetricSetResponseTypeDef,
+    CreateMetricSetRequestRequestTypeDef,
+    MetricSourceUnionTypeDef,
     UpdateMetricSetRequestRequestTypeDef,
     DetectedMetricSourceTypeDef,
     GetAnomalyGroupResponseTypeDef,
     DetectedMetricSetConfigTypeDef,
     DetectMetricSetConfigResponseTypeDef,
 )
 
 
-def get_structure() -> LambdaConfigurationTypeDef:
+def get_value() -> LambdaConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lookoutmetrics-2.5.2/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt` & `types-aiobotocore-lookoutmetrics-2.5.2.post1/types_aiobotocore_lookoutmetrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


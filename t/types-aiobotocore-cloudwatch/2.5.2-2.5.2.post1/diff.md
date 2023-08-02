# Comparing `tmp/types-aiobotocore-cloudwatch-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudwatch-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudwatch-2.5.2.tar", last modified: Sat Jul  8 01:43:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudwatch-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:02 2023, max compression
```

## Comparing `types-aiobotocore-cloudwatch-2.5.2.tar` & `types-aiobotocore-cloudwatch-2.5.2.post1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.421861 types-aiobotocore-cloudwatch-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21529 2023-07-08 01:43:23.421861 types-aiobotocore-cloudwatch-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19952 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:23.421861 types-aiobotocore-cloudwatch-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.421861 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34952 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    34897 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25830 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/service_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    25782 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/service_resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    42515 2023-07-08 01:27:18.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42470 2023-07-08 01:27:17.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-08 01:27:16.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:23.421861 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21529 2023-07-08 01:43:23.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-07-08 01:43:23.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:23.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:23.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:23.000000 types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    22083 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20553 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34985 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34930 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11144 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11142 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9229 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25869 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25821 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    46361 2023-08-02 14:34:50.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46312 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:48.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-08-02 14:34:49.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:02.281627 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22083 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:02.000000 types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/LICENSE` & `types-aiobotocore-cloudwatch-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2/PKG-INFO` & `types-aiobotocore-cloudwatch-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudwatch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatch 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatch 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudwatch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudwatch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudwatch"></a>
 
 # types-aiobotocore-cloudwatch
 
 [![PyPI - types-aiobotocore-cloudwatch](https://img.shields.io/pypi/v/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudwatch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudwatch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudwatch)](https://pepy.tech/project/types-aiobotocore-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [types-aiobotocore-cloudwatch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -439,95 +438,100 @@
 )
 
 
 def check_value(value: ActionsSuppressedByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudwatch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
-    RangeTypeDef,
+    RangeOutputTypeDef,
     DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
-    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
-    DescribeAlarmHistoryInputRequestTypeDef,
+    TimestampTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetDashboardOutputTypeDef,
-    GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
-    MetricStreamFilterTypeDef,
+    MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
+    MetricStreamFilterTypeDef,
     MetricStreamStatisticsMetricTypeDef,
-    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
-    PutMetricStreamOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
-    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    GetMetricStatisticsInputRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
+    GetDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
+    PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    DescribeAlarmHistoryInputRequestTypeDef,
+    GetInsightRuleReportInputRequestTypeDef,
+    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    GetMetricStatisticsInputRequestTypeDef,
+    RangeTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
@@ -535,41 +539,52 @@
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
+    MetricStatOutputTypeDef,
     MetricStatTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
-    PutMetricStreamInputRequestTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
-    GetMetricDataInputGetMetricDataPaginateTypeDef,
-    GetMetricDataInputRequestTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
+    PutMetricStreamInputRequestTypeDef,
     MetricAlarmTypeDef,
+    MetricMathAnomalyDetectorOutputTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
-    PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
+    GetMetricDataInputGetMetricDataPaginateTypeDef,
+    GetMetricDataInputRequestTypeDef,
+    PutMetricAlarmInputRequestTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
     PutAnomalyDetectorInputRequestTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
 )
 
 
-def get_structure() -> AlarmHistoryItemTypeDef:
+def get_value() -> AlarmHistoryItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/README.md` & `types-aiobotocore-cloudwatch-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudwatch"></a>
 
 # types-aiobotocore-cloudwatch
 
 [![PyPI - types-aiobotocore-cloudwatch](https://img.shields.io/pypi/v/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudwatch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudwatch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudwatch)](https://pepy.tech/project/types-aiobotocore-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [types-aiobotocore-cloudwatch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -45,15 +45,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -406,95 +406,100 @@
 )
 
 
 def check_value(value: ActionsSuppressedByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudwatch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
-    RangeTypeDef,
+    RangeOutputTypeDef,
     DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
-    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
-    DescribeAlarmHistoryInputRequestTypeDef,
+    TimestampTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetDashboardOutputTypeDef,
-    GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
-    MetricStreamFilterTypeDef,
+    MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
+    MetricStreamFilterTypeDef,
     MetricStreamStatisticsMetricTypeDef,
-    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
-    PutMetricStreamOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
-    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    GetMetricStatisticsInputRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
+    GetDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
+    PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    DescribeAlarmHistoryInputRequestTypeDef,
+    GetInsightRuleReportInputRequestTypeDef,
+    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    GetMetricStatisticsInputRequestTypeDef,
+    RangeTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
@@ -502,41 +507,52 @@
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
+    MetricStatOutputTypeDef,
     MetricStatTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
-    PutMetricStreamInputRequestTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
-    GetMetricDataInputGetMetricDataPaginateTypeDef,
-    GetMetricDataInputRequestTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
+    PutMetricStreamInputRequestTypeDef,
     MetricAlarmTypeDef,
+    MetricMathAnomalyDetectorOutputTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
-    PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
+    GetMetricDataInputGetMetricDataPaginateTypeDef,
+    GetMetricDataInputRequestTypeDef,
+    PutMetricAlarmInputRequestTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
     PutAnomalyDetectorInputRequestTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
 )
 
 
-def get_structure() -> AlarmHistoryItemTypeDef:
+def get_value() -> AlarmHistoryItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/setup.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudwatch",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudwatch"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatch 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudwatch type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudwatch type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudwatch": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/"
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/__init__.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 )
 from .service_resource import CloudWatchServiceResource
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 Client = CloudWatchClient
 
 
+ServiceResource = CloudWatchServiceResource
+
+
 __all__ = (
     "AlarmExistsWaiter",
     "Client",
     "CloudWatchClient",
     "CloudWatchServiceResource",
     "CompositeAlarmExistsWaiter",
     "DescribeAlarmHistoryPaginator",
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/__init__.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
     ListMetricsPaginator,
 )
 from .service_resource import CloudWatchServiceResource
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 Client = CloudWatchClient
 
+ServiceResource = CloudWatchServiceResource
+
 __all__ = (
     "AlarmExistsWaiter",
     "Client",
     "CloudWatchClient",
     "CloudWatchServiceResource",
     "CompositeAlarmExistsWaiter",
     "DescribeAlarmHistoryPaginator",
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/__main__.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudWatch 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudWatch 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch\nOther"
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

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/client.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("cloudwatch") as client:
         client: CloudWatchClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
@@ -37,15 +36,15 @@
     DescribeAlarmsPaginator,
     DescribeAnomalyDetectorsPaginator,
     GetMetricDataPaginator,
     ListDashboardsPaginator,
     ListMetricsPaginator,
 )
 from .type_defs import (
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
     DescribeInsightRulesOutputTypeDef,
     DimensionFilterTypeDef,
@@ -62,24 +61,25 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricDatumTypeDef,
-    MetricMathAnomalyDetectorTypeDef,
-    MetricStreamFilterTypeDef,
-    MetricStreamStatisticsConfigurationTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
-    SingleMetricAnomalyDetectorTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -157,16 +157,16 @@
     async def delete_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -199,16 +199,16 @@
 
     async def describe_alarm_history(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -343,16 +343,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_dashboard)
         """
 
     async def get_insight_rule_report(
         self,
         *,
         RuleName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         MaxContributorCount: int = ...,
         Metrics: Sequence[str] = ...,
         OrderBy: str = ...
     ) -> GetInsightRuleReportOutputTypeDef:
         """
         This operation returns the time series data collected by a Contributor Insights
@@ -361,17 +361,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_insight_rule_report)
         """
 
     async def get_metric_data(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
         LabelOptions: LabelOptionsTypeDef = ...
     ) -> GetMetricDataOutputTypeDef:
         """
         You can use the `GetMetricData` API to retrieve CloudWatch metric values.
@@ -381,16 +381,16 @@
         """
 
     async def get_metric_statistics(
         self,
         *,
         Namespace: str,
         MetricName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
@@ -479,17 +479,17 @@
     async def put_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        Configuration: AnomalyDetectorConfigurationTypeDef = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_anomaly_detector)
         """
@@ -571,15 +571,15 @@
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
-        Metrics: Sequence[MetricDataQueryTypeDef] = ...,
+        Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ThresholdMetricId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights query.
 
@@ -600,18 +600,18 @@
     async def put_metric_stream(
         self,
         *,
         Name: str,
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
-        IncludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
-        ExcludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
+        IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
+        ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationTypeDef] = ...,
+        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,
         IncludeLinkedAccountsMetrics: bool = ...
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_metric_stream)
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/client.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("cloudwatch") as client:
         client: CloudWatchClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
@@ -37,15 +36,15 @@
     DescribeAlarmsPaginator,
     DescribeAnomalyDetectorsPaginator,
     GetMetricDataPaginator,
     ListDashboardsPaginator,
     ListMetricsPaginator,
 )
 from .type_defs import (
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
     DeleteInsightRulesOutputTypeDef,
     DescribeAlarmHistoryOutputTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
     DescribeInsightRulesOutputTypeDef,
     DimensionFilterTypeDef,
@@ -62,24 +61,25 @@
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     ListMetricsOutputTypeDef,
     ListMetricStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricDatumTypeDef,
-    MetricMathAnomalyDetectorTypeDef,
-    MetricStreamFilterTypeDef,
-    MetricStreamStatisticsConfigurationTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
     PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
     PutMetricStreamOutputTypeDef,
-    SingleMetricAnomalyDetectorTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 from .waiter import AlarmExistsWaiter, CompositeAlarmExistsWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -149,16 +149,16 @@
     async def delete_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes the specified anomaly detection model from your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.delete_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#delete_anomaly_detector)
         """
@@ -187,16 +187,16 @@
         """
     async def describe_alarm_history(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -320,16 +320,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_dashboard)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_dashboard)
         """
     async def get_insight_rule_report(
         self,
         *,
         RuleName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         MaxContributorCount: int = ...,
         Metrics: Sequence[str] = ...,
         OrderBy: str = ...
     ) -> GetInsightRuleReportOutputTypeDef:
         """
         This operation returns the time series data collected by a Contributor Insights
@@ -337,17 +337,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.get_insight_rule_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_insight_rule_report)
         """
     async def get_metric_data(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...,
         ScanBy: ScanByType = ...,
         MaxDatapoints: int = ...,
         LabelOptions: LabelOptionsTypeDef = ...
     ) -> GetMetricDataOutputTypeDef:
         """
         You can use the `GetMetricData` API to retrieve CloudWatch metric values.
@@ -356,16 +356,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#get_metric_data)
         """
     async def get_metric_statistics(
         self,
         *,
         Namespace: str,
         MetricName: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
@@ -446,17 +446,17 @@
     async def put_anomaly_detector(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Stat: str = ...,
-        Configuration: AnomalyDetectorConfigurationTypeDef = ...,
-        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorTypeDef = ...,
-        MetricMathAnomalyDetector: MetricMathAnomalyDetectorTypeDef = ...
+        Configuration: AnomalyDetectorConfigurationUnionTypeDef = ...,
+        SingleMetricAnomalyDetector: SingleMetricAnomalyDetectorUnionTypeDef = ...,
+        MetricMathAnomalyDetector: MetricMathAnomalyDetectorUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Creates an anomaly detection model for a CloudWatch metric.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_anomaly_detector)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_anomaly_detector)
         """
@@ -533,15 +533,15 @@
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Period: int = ...,
         Unit: StandardUnitType = ...,
         DatapointsToAlarm: int = ...,
         Threshold: float = ...,
         TreatMissingData: str = ...,
         EvaluateLowSampleCountPercentile: str = ...,
-        Metrics: Sequence[MetricDataQueryTypeDef] = ...,
+        Metrics: Sequence[MetricDataQueryUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         ThresholdMetricId: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an alarm and associates it with the specified metric, metric
         math expression, anomaly detection model, or Metrics Insights query.
 
@@ -560,18 +560,18 @@
     async def put_metric_stream(
         self,
         *,
         Name: str,
         FirehoseArn: str,
         RoleArn: str,
         OutputFormat: MetricStreamOutputFormatType,
-        IncludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
-        ExcludeFilters: Sequence[MetricStreamFilterTypeDef] = ...,
+        IncludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
+        ExcludeFilters: Sequence[MetricStreamFilterUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationTypeDef] = ...,
+        StatisticsConfigurations: Sequence[MetricStreamStatisticsConfigurationUnionTypeDef] = ...,
         IncludeLinkedAccountsMetrics: bool = ...
     ) -> PutMetricStreamOutputTypeDef:
         """
         Creates or updates a metric stream.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Client.put_metric_stream)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/client/#put_metric_stream)
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/literals.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/literals.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/paginator.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         describe_anomaly_detectors_paginator: DescribeAnomalyDetectorsPaginator = client.get_paginator("describe_anomaly_detectors")
         get_metric_data_paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
         list_dashboards_paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
         list_metrics_paginator: ListMetricsPaginator = client.get_paginator("list_metrics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
@@ -50,16 +49,17 @@
     DescribeAnomalyDetectorsOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricDataOutputTypeDef,
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListMetricsOutputTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -92,18 +92,18 @@
 
     def paginate(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 
@@ -119,15 +119,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAlarmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmspaginator)
         """
 
 
@@ -140,15 +140,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAnomalyDetectorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 
@@ -157,35 +157,35 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 
 class ListDashboardsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, DashboardNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DashboardNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDashboardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listdashboardspaginator)
         """
 
 
@@ -200,13 +200,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMetricsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/paginator.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -27,16 +27,15 @@
         describe_anomaly_detectors_paginator: DescribeAnomalyDetectorsPaginator = client.get_paginator("describe_anomaly_detectors")
         get_metric_data_paginator: GetMetricDataPaginator = client.get_paginator("get_metric_data")
         list_dashboards_paginator: ListDashboardsPaginator = client.get_paginator("list_dashboards")
         list_metrics_paginator: ListMetricsPaginator = client.get_paginator("list_metrics")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     AlarmTypeType,
     AnomalyDetectorTypeType,
@@ -50,16 +49,17 @@
     DescribeAnomalyDetectorsOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricDataOutputTypeDef,
     LabelOptionsTypeDef,
     ListDashboardsOutputTypeDef,
     ListMetricsOutputTypeDef,
-    MetricDataQueryTypeDef,
+    MetricDataQueryUnionTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -88,18 +88,18 @@
 
     def paginate(
         self,
         *,
         AlarmName: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         ScanBy: ScanByType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAlarmHistoryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarmHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmhistorypaginator)
         """
 
 class DescribeAlarmsPaginator(AioPaginator):
@@ -114,15 +114,15 @@
         AlarmNames: Sequence[str] = ...,
         AlarmNamePrefix: str = ...,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         ChildrenOfAlarmName: str = ...,
         ParentsOfAlarmName: str = ...,
         StateValue: StateValueType = ...,
         ActionPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAlarmsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAlarms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describealarmspaginator)
         """
 
 class DescribeAnomalyDetectorsPaginator(AioPaginator):
@@ -134,15 +134,15 @@
     def paginate(
         self,
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         AnomalyDetectorTypes: Sequence[AnomalyDetectorTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAnomalyDetectorsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.DescribeAnomalyDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#describeanomalydetectorspaginator)
         """
 
 class GetMetricDataPaginator(AioPaginator):
@@ -150,34 +150,34 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
     """
 
     def paginate(
         self,
         *,
-        MetricDataQueries: Sequence[MetricDataQueryTypeDef],
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        MetricDataQueries: Sequence[MetricDataQueryUnionTypeDef],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         ScanBy: ScanByType = ...,
         LabelOptions: LabelOptionsTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetMetricDataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.GetMetricData.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#getmetricdatapaginator)
         """
 
 class ListDashboardsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listdashboardspaginator)
     """
 
     def paginate(
-        self, *, DashboardNamePrefix: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DashboardNamePrefix: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDashboardsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListDashboards.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listdashboardspaginator)
         """
 
 class ListMetricsPaginator(AioPaginator):
@@ -191,13 +191,13 @@
         *,
         Namespace: str = ...,
         MetricName: str = ...,
         Dimensions: Sequence[DimensionFilterTypeDef] = ...,
         RecentlyActive: Literal["PT3H"] = ...,
         IncludeLinkedAccounts: bool = ...,
         OwningAccount: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMetricsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Paginator.ListMetrics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/paginators/#listmetricspaginator)
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/service_resource.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         my_alarm: cloudwatch_resources.Alarm = resource.Alarm(...)
         my_metric: cloudwatch_resources.Metric = resource.Metric(...)
 ```
 """
 import sys
 from datetime import datetime
-from typing import AsyncIterator, Awaitable, List, NoReturn, Sequence, Union
+from typing import AsyncIterator, Awaitable, List, NoReturn, Sequence
 
 from .client import CloudWatchClient
 from .literals import (
     AlarmTypeType,
     ComparisonOperatorType,
     HistoryItemTypeType,
     ScanByType,
@@ -34,16 +34,18 @@
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
@@ -329,15 +331,15 @@
     unit: Awaitable[StandardUnitType]
     evaluation_periods: Awaitable[int]
     datapoints_to_alarm: Awaitable[int]
     threshold: Awaitable[float]
     comparison_operator: Awaitable[ComparisonOperatorType]
     treat_missing_data: Awaitable[str]
     evaluate_low_sample_count_percentile: Awaitable[str]
-    metrics: Awaitable[List[MetricDataQueryTypeDef]]
+    metrics: Awaitable[List[MetricDataQueryOutputTypeDef]]
     threshold_metric_id: Awaitable[str]
     evaluation_state: Awaitable[Literal["PARTIAL_DATA"]]
     state_transitioned_timestamp: Awaitable[datetime]
     name: str
     metric: "Metric"
 
     async def delete(self) -> None:
@@ -349,16 +351,16 @@
         """
 
     async def describe_history(
         self,
         *,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -441,16 +443,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricget_available_subresources-method)
         """
 
     async def get_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/service_resource.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/service_resource.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
         my_alarm: cloudwatch_resources.Alarm = resource.Alarm(...)
         my_metric: cloudwatch_resources.Metric = resource.Metric(...)
 ```
 """
 import sys
 from datetime import datetime
-from typing import AsyncIterator, Awaitable, List, NoReturn, Sequence, Union
+from typing import AsyncIterator, Awaitable, List, NoReturn, Sequence
 
 from .client import CloudWatchClient
 from .literals import (
     AlarmTypeType,
     ComparisonOperatorType,
     HistoryItemTypeType,
     ScanByType,
@@ -34,16 +34,18 @@
     StatisticType,
 )
 from .type_defs import (
     DescribeAlarmHistoryOutputTypeDef,
     DimensionFilterTypeDef,
     DimensionTypeDef,
     GetMetricStatisticsOutputTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 try:
     from aioboto3.resources.base import AIOBoto3ServiceResource
 except (ModuleNotFoundError, ImportError):
     from builtins import object as AIOBoto3ServiceResource
 try:
@@ -300,15 +302,15 @@
     unit: Awaitable[StandardUnitType]
     evaluation_periods: Awaitable[int]
     datapoints_to_alarm: Awaitable[int]
     threshold: Awaitable[float]
     comparison_operator: Awaitable[ComparisonOperatorType]
     treat_missing_data: Awaitable[str]
     evaluate_low_sample_count_percentile: Awaitable[str]
-    metrics: Awaitable[List[MetricDataQueryTypeDef]]
+    metrics: Awaitable[List[MetricDataQueryOutputTypeDef]]
     threshold_metric_id: Awaitable[str]
     evaluation_state: Awaitable[Literal["PARTIAL_DATA"]]
     state_transitioned_timestamp: Awaitable[datetime]
     name: str
     metric: "Metric"
 
     async def delete(self) -> None:
@@ -319,16 +321,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#alarmdelete-method)
         """
     async def describe_history(
         self,
         *,
         AlarmTypes: Sequence[AlarmTypeType] = ...,
         HistoryItemType: HistoryItemTypeType = ...,
-        StartDate: Union[datetime, str] = ...,
-        EndDate: Union[datetime, str] = ...,
+        StartDate: TimestampTypeDef = ...,
+        EndDate: TimestampTypeDef = ...,
         MaxRecords: int = ...,
         NextToken: str = ...,
         ScanBy: ScanByType = ...
     ) -> DescribeAlarmHistoryOutputTypeDef:
         """
         Retrieves the history for the specified alarm.
 
@@ -402,16 +404,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch.Metric.get_available_subresources)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/service_resource/#metricget_available_subresources-method)
         """
     async def get_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         Period: int,
         Dimensions: Sequence[DimensionTypeDef] = ...,
         Statistics: Sequence[StatisticType] = ...,
         ExtendedStatistics: Sequence[str] = ...,
         Unit: StandardUnitType = ...
     ) -> GetMetricStatisticsOutputTypeDef:
         """
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/type_defs.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudwatch.type_defs import AlarmHistoryItemTypeDef
 
-    data: AlarmHistoryItemTypeDef = {...}
+    data: AlarmHistoryItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,88 +35,92 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AlarmHistoryItemTypeDef",
-    "RangeTypeDef",
+    "RangeOutputTypeDef",
     "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
-    "DescribeAlarmHistoryInputRequestTypeDef",
+    "TimestampTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
-    "GetDashboardOutputTypeDef",
-    "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
-    "MetricStreamFilterTypeDef",
+    "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
-    "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
+    "MetricStreamFilterTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
-    "PutMetricStreamOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "DescribeAlarmHistoryOutputTypeDef",
-    "AnomalyDetectorConfigurationTypeDef",
+    "AnomalyDetectorConfigurationOutputTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
-    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    "GetMetricStatisticsInputRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
+    "SingleMetricAnomalyDetectorOutputTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
     "DeleteInsightRulesOutputTypeDef",
+    "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
+    "GetDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
+    "GetMetricWidgetImageOutputTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
+    "PutMetricStreamOutputTypeDef",
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    "GetInsightRuleReportInputRequestTypeDef",
+    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    "GetMetricStatisticsInputRequestTypeDef",
+    "RangeTypeDef",
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
@@ -124,35 +128,46 @@
     "ListTagsForResourceOutputTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
+    "MetricStreamFilterUnionTypeDef",
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
+    "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
+    "SingleMetricAnomalyDetectorUnionTypeDef",
+    "AnomalyDetectorConfigurationTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
-    "PutMetricStreamInputRequestTypeDef",
+    "MetricStreamStatisticsConfigurationUnionTypeDef",
+    "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
-    "GetMetricDataInputGetMetricDataPaginateTypeDef",
-    "GetMetricDataInputRequestTypeDef",
+    "AnomalyDetectorConfigurationUnionTypeDef",
+    "PutMetricStreamInputRequestTypeDef",
     "MetricAlarmTypeDef",
+    "MetricMathAnomalyDetectorOutputTypeDef",
+    "MetricDataQueryUnionTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
-    "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
     "AnomalyDetectorTypeDef",
+    "GetMetricDataInputGetMetricDataPaginateTypeDef",
+    "GetMetricDataInputRequestTypeDef",
+    "PutMetricAlarmInputRequestTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
+    "MetricMathAnomalyDetectorUnionTypeDef",
     "PutAnomalyDetectorInputRequestTypeDef",
     "DescribeAnomalyDetectorsOutputTypeDef",
 )
 
 AlarmHistoryItemTypeDef = TypedDict(
     "AlarmHistoryItemTypeDef",
     {
@@ -162,16 +177,16 @@
         "HistoryItemType": HistoryItemTypeType,
         "HistorySummary": str,
         "HistoryData": str,
     },
     total=False,
 )
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
+RangeOutputTypeDef = TypedDict(
+    "RangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
 DimensionTypeDef = TypedDict(
@@ -271,88 +286,52 @@
         "ExceptionType": str,
         "FailureCode": str,
         "FailureDescription": str,
     },
     total=False,
 )
 
-DeleteMetricStreamInputRequestTypeDef = TypedDict(
-    "DeleteMetricStreamInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
-DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+DeleteMetricStreamInputRequestTypeDef = TypedDict(
+    "DeleteMetricStreamInputRequestTypeDef",
     {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "ScanBy": ScanByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
     },
-    total=False,
 )
 
-DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputRequestTypeDef",
+TimestampTypeDef = Union[datetime, str]
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    {
-        "AlarmNames": Sequence[str],
-        "AlarmNamePrefix": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "ChildrenOfAlarmName": str,
-        "ParentsOfAlarmName": str,
-        "StateValue": StateValueType,
-        "ActionPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAlarmsInputRequestTypeDef = TypedDict(
     "DescribeAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "ChildrenOfAlarmName": str,
@@ -387,59 +366,48 @@
     "_OptionalInsightRuleTypeDef",
     {
         "ManagedRule": bool,
     },
     total=False,
 )
 
-
 class InsightRuleTypeDef(_RequiredInsightRuleTypeDef, _OptionalInsightRuleTypeDef):
     pass
 
-
 _RequiredDimensionFilterTypeDef = TypedDict(
     "_RequiredDimensionFilterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDimensionFilterTypeDef = TypedDict(
     "_OptionalDimensionFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class DimensionFilterTypeDef(_RequiredDimensionFilterTypeDef, _OptionalDimensionFilterTypeDef):
     pass
 
-
 DisableAlarmActionsInputRequestTypeDef = TypedDict(
     "DisableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
 DisableInsightRulesInputRequestTypeDef = TypedDict(
     "DisableInsightRulesInputRequestTypeDef",
     {
         "RuleNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableAlarmActionsInputRequestTypeDef = TypedDict(
     "EnableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
@@ -453,51 +421,14 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
-GetDashboardOutputTypeDef = TypedDict(
-    "GetDashboardOutputTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardBody": str,
-        "DashboardName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetInsightRuleReportInputRequestTypeDef",
-    {
-        "RuleName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetInsightRuleReportInputRequestTypeDef",
-    {
-        "MaxContributorCount": int,
-        "Metrics": Sequence[str],
-        "OrderBy": str,
-    },
-    total=False,
-)
-
-
-class GetInsightRuleReportInputRequestTypeDef(
-    _RequiredGetInsightRuleReportInputRequestTypeDef,
-    _OptionalGetInsightRuleReportInputRequestTypeDef,
-):
-    pass
-
-
 _RequiredInsightRuleMetricDatapointTypeDef = TypedDict(
     "_RequiredInsightRuleMetricDatapointTypeDef",
     {
         "Timestamp": datetime,
     },
 )
 _OptionalInsightRuleMetricDatapointTypeDef = TypedDict(
@@ -510,21 +441,19 @@
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
     total=False,
 )
 
-
 class InsightRuleMetricDatapointTypeDef(
     _RequiredInsightRuleMetricDatapointTypeDef, _OptionalInsightRuleMetricDatapointTypeDef
 ):
     pass
 
-
 LabelOptionsTypeDef = TypedDict(
     "LabelOptionsTypeDef",
     {
         "Timezone": str,
     },
     total=False,
 )
@@ -541,16 +470,16 @@
 GetMetricStreamInputRequestTypeDef = TypedDict(
     "GetMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-MetricStreamFilterTypeDef = TypedDict(
-    "MetricStreamFilterTypeDef",
+MetricStreamFilterOutputTypeDef = TypedDict(
+    "MetricStreamFilterOutputTypeDef",
     {
         "Namespace": str,
         "MetricNames": List[str],
     },
     total=False,
 )
 
@@ -564,47 +493,28 @@
     "_OptionalGetMetricWidgetImageInputRequestTypeDef",
     {
         "OutputFormat": str,
     },
     total=False,
 )
 
-
 class GetMetricWidgetImageInputRequestTypeDef(
     _RequiredGetMetricWidgetImageInputRequestTypeDef,
     _OptionalGetMetricWidgetImageInputRequestTypeDef,
 ):
     pass
 
-
-GetMetricWidgetImageOutputTypeDef = TypedDict(
-    "GetMetricWidgetImageOutputTypeDef",
-    {
-        "MetricWidgetImage": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 InsightRuleContributorDatapointTypeDef = TypedDict(
     "InsightRuleContributorDatapointTypeDef",
     {
         "Timestamp": datetime,
         "ApproximateValue": float,
     },
 )
 
-ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
-    {
-        "DashboardNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDashboardsInputRequestTypeDef = TypedDict(
     "ListDashboardsInputRequestTypeDef",
     {
         "DashboardNamePrefix": str,
         "NextToken": str,
     },
     total=False,
@@ -621,22 +531,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListManagedInsightRulesInputRequestTypeDef(
     _RequiredListManagedInsightRulesInputRequestTypeDef,
     _OptionalListManagedInsightRulesInputRequestTypeDef,
 ):
     pass
 
-
 ListMetricStreamsInputRequestTypeDef = TypedDict(
     "ListMetricStreamsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -685,59 +593,39 @@
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
 )
 
-MetricStreamStatisticsMetricTypeDef = TypedDict(
-    "MetricStreamStatisticsMetricTypeDef",
+MetricStreamFilterTypeDef = TypedDict(
+    "MetricStreamFilterTypeDef",
     {
         "Namespace": str,
-        "MetricName": str,
+        "MetricNames": Sequence[str],
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+MetricStreamStatisticsMetricTypeDef = TypedDict(
+    "MetricStreamStatisticsMetricTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Namespace": str,
+        "MetricName": str,
     },
-    total=False,
 )
 
 PutDashboardInputRequestTypeDef = TypedDict(
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
-PutMetricStreamOutputTypeDef = TypedDict(
-    "PutMetricStreamOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
@@ -745,21 +633,19 @@
     "_OptionalSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateReasonData": str,
     },
     total=False,
 )
 
-
 class SetAlarmStateInputAlarmSetStateTypeDef(
     _RequiredSetAlarmStateInputAlarmSetStateTypeDef, _OptionalSetAlarmStateInputAlarmSetStateTypeDef
 ):
     pass
 
-
 _RequiredSetAlarmStateInputRequestTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputRequestTypeDef",
     {
         "AlarmName": str,
         "StateValue": StateValueType,
         "StateReason": str,
     },
@@ -768,21 +654,19 @@
     "_OptionalSetAlarmStateInputRequestTypeDef",
     {
         "StateReasonData": str,
     },
     total=False,
 )
 
-
 class SetAlarmStateInputRequestTypeDef(
     _RequiredSetAlarmStateInputRequestTypeDef, _OptionalSetAlarmStateInputRequestTypeDef
 ):
     pass
 
-
 StartMetricStreamsInputRequestTypeDef = TypedDict(
     "StartMetricStreamsInputRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
@@ -797,27 +681,18 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-DescribeAlarmHistoryOutputTypeDef = TypedDict(
-    "DescribeAlarmHistoryOutputTypeDef",
-    {
-        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AnomalyDetectorConfigurationTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationTypeDef",
+AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationOutputTypeDef",
     {
-        "ExcludedTimeRanges": List[RangeTypeDef],
+        "ExcludedTimeRanges": List[RangeOutputTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
@@ -834,179 +709,336 @@
         "Dimensions": Sequence[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
-
 class DescribeAlarmsForMetricInputRequestTypeDef(
     _RequiredDescribeAlarmsForMetricInputRequestTypeDef,
     _OptionalDescribeAlarmsForMetricInputRequestTypeDef,
 ):
     pass
 
-
-DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputRequestTypeDef",
+MetricOutputTypeDef = TypedDict(
+    "MetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+    },
+    total=False,
+)
+
+MetricTypeDef = TypedDict(
+    "MetricTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
-        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
     },
     total=False,
 )
 
+SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
+SingleMetricAnomalyDetectorTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
+DeleteInsightRulesOutputTypeDef = TypedDict(
+    "DeleteInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryOutputTypeDef = TypedDict(
+    "DescribeAlarmHistoryOutputTypeDef",
+    {
+        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableInsightRulesOutputTypeDef = TypedDict(
+    "DisableInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
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
+EnableInsightRulesOutputTypeDef = TypedDict(
+    "EnableInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardOutputTypeDef = TypedDict(
+    "GetDashboardOutputTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardBody": str,
+        "DashboardName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricStatisticsOutputTypeDef = TypedDict(
+    "GetMetricStatisticsOutputTypeDef",
+    {
+        "Label": str,
+        "Datapoints": List[DatapointTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricWidgetImageOutputTypeDef = TypedDict(
+    "GetMetricWidgetImageOutputTypeDef",
+    {
+        "MetricWidgetImage": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
+    {
+        "DashboardEntries": List[DashboardEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
+    {
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutManagedInsightRulesOutputTypeDef = TypedDict(
+    "PutManagedInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMetricStreamOutputTypeDef = TypedDict(
+    "PutMetricStreamOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    {
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_RequiredGetInsightRuleReportInputRequestTypeDef",
+    {
+        "RuleName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_OptionalGetInsightRuleReportInputRequestTypeDef",
+    {
+        "MaxContributorCount": int,
+        "Metrics": Sequence[str],
+        "OrderBy": str,
+    },
+    total=False,
+)
+
+class GetInsightRuleReportInputRequestTypeDef(
+    _RequiredGetInsightRuleReportInputRequestTypeDef,
+    _OptionalGetInsightRuleReportInputRequestTypeDef,
+):
+    pass
+
 _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
     "_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Period": int,
     },
 )
 _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
     "_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "Statistics": Sequence[StatisticType],
         "ExtendedStatistics": Sequence[str],
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
-
 class GetMetricStatisticsInputMetricGetStatisticsTypeDef(
     _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef,
     _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef,
 ):
     pass
 
-
 _RequiredGetMetricStatisticsInputRequestTypeDef = TypedDict(
     "_RequiredGetMetricStatisticsInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Period": int,
     },
 )
 _OptionalGetMetricStatisticsInputRequestTypeDef = TypedDict(
     "_OptionalGetMetricStatisticsInputRequestTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "Statistics": Sequence[StatisticType],
         "ExtendedStatistics": Sequence[str],
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
-
 class GetMetricStatisticsInputRequestTypeDef(
     _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
 ):
     pass
 
-
-MetricTypeDef = TypedDict(
-    "MetricTypeDef",
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
     {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
-    total=False,
 )
 
-SingleMetricAnomalyDetectorTypeDef = TypedDict(
-    "SingleMetricAnomalyDetectorTypeDef",
+DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Stat": str,
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "ScanBy": ScanByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
-    {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
-    {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMetricStatisticsOutputTypeDef = TypedDict(
-    "GetMetricStatisticsOutputTypeDef",
-    {
-        "Label": str,
-        "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteInsightRulesOutputTypeDef = TypedDict(
-    "DeleteInsightRulesOutputTypeDef",
-    {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DisableInsightRulesOutputTypeDef = TypedDict(
-    "DisableInsightRulesOutputTypeDef",
+DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmNames": Sequence[str],
+        "AlarmNamePrefix": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "ChildrenOfAlarmName": str,
+        "ParentsOfAlarmName": str,
+        "StateValue": StateValueType,
+        "ActionPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-EnableInsightRulesOutputTypeDef = TypedDict(
-    "EnableInsightRulesOutputTypeDef",
+DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PutManagedInsightRulesOutputTypeDef = TypedDict(
-    "PutManagedInsightRulesOutputTypeDef",
+ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DashboardNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeAlarmsInputAlarmExistsWaitTypeDef = TypedDict(
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
@@ -1040,28 +1072,28 @@
 )
 
 DescribeInsightRulesOutputTypeDef = TypedDict(
     "DescribeInsightRulesOutputTypeDef",
     {
         "NextToken": str,
         "InsightRules": List[InsightRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricsInputListMetricsPaginateTypeDef = TypedDict(
     "ListMetricsInputListMetricsPaginateTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionFilterTypeDef],
         "RecentlyActive": Literal["PT3H"],
         "IncludeLinkedAccounts": bool,
         "OwningAccount": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMetricsInputRequestTypeDef = TypedDict(
     "ListMetricsInputRequestTypeDef",
     {
@@ -1099,23 +1131,23 @@
 )
 
 ListMetricStreamsOutputTypeDef = TypedDict(
     "ListMetricStreamsOutputTypeDef",
     {
         "NextToken": str,
         "Entries": List[MetricStreamEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
@@ -1126,19 +1158,17 @@
     "_OptionalManagedRuleTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class ManagedRuleTypeDef(_RequiredManagedRuleTypeDef, _OptionalManagedRuleTypeDef):
     pass
 
-
 _RequiredPutCompositeAlarmInputRequestTypeDef = TypedDict(
     "_RequiredPutCompositeAlarmInputRequestTypeDef",
     {
         "AlarmName": str,
         "AlarmRule": str,
     },
 )
@@ -1154,21 +1184,19 @@
         "ActionsSuppressor": str,
         "ActionsSuppressorWaitPeriod": int,
         "ActionsSuppressorExtensionPeriod": int,
     },
     total=False,
 )
 
-
 class PutCompositeAlarmInputRequestTypeDef(
     _RequiredPutCompositeAlarmInputRequestTypeDef, _OptionalPutCompositeAlarmInputRequestTypeDef
 ):
     pass
 
-
 _RequiredPutInsightRuleInputRequestTypeDef = TypedDict(
     "_RequiredPutInsightRuleInputRequestTypeDef",
     {
         "RuleName": str,
         "RuleDefinition": str,
     },
 )
@@ -1177,21 +1205,19 @@
     {
         "RuleState": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutInsightRuleInputRequestTypeDef(
     _RequiredPutInsightRuleInputRequestTypeDef, _OptionalPutInsightRuleInputRequestTypeDef
 ):
     pass
 
-
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1212,47 +1238,73 @@
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "Value": float,
         "StatisticValues": StatisticSetTypeDef,
         "Values": Sequence[float],
         "Counts": Sequence[float],
         "Unit": StandardUnitType,
         "StorageResolution": int,
     },
     total=False,
 )
 
-
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
+MetricStreamFilterUnionTypeDef = Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
+MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
+    {
+        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": List[str],
+    },
+)
 
 MetricStreamStatisticsConfigurationTypeDef = TypedDict(
     "MetricStreamStatisticsConfigurationTypeDef",
     {
-        "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
-        "AdditionalStatistics": List[str],
+        "IncludeMetrics": Sequence[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": Sequence[str],
     },
 )
 
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
-        "Metrics": List[MetricTypeDef],
+        "Metrics": List[MetricOutputTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Period": int,
+        "Stat": str,
     },
 )
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
+    {
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
 
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Period": int,
         "Stat": str,
@@ -1262,39 +1314,49 @@
     "_OptionalMetricStatTypeDef",
     {
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
-
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
+SingleMetricAnomalyDetectorUnionTypeDef = Union[
+    SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
+]
+AnomalyDetectorConfigurationTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationTypeDef",
+    {
+        "ExcludedTimeRanges": Sequence[RangeTypeDef],
+        "MetricTimezone": str,
+    },
+    total=False,
+)
 
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightRuleReportOutputTypeDef = TypedDict(
     "GetInsightRuleReportOutputTypeDef",
     {
         "KeyLabels": List[str],
         "AggregationStatistic": str,
         "AggregateValue": float,
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutManagedInsightRulesInputRequestTypeDef = TypedDict(
     "PutManagedInsightRulesInputRequestTypeDef",
     {
         "ManagedRules": Sequence[ManagedRuleTypeDef],
@@ -1302,15 +1364,15 @@
 )
 
 ListManagedInsightRulesOutputTypeDef = TypedDict(
     "ListManagedInsightRulesOutputTypeDef",
     {
         "ManagedRules": List[ManagedRuleDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
@@ -1319,56 +1381,55 @@
 )
 
 GetMetricStreamOutputTypeDef = TypedDict(
     "GetMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
-        "IncludeFilters": List[MetricStreamFilterTypeDef],
-        "ExcludeFilters": List[MetricStreamFilterTypeDef],
+        "IncludeFilters": List[MetricStreamFilterOutputTypeDef],
+        "ExcludeFilters": List[MetricStreamFilterOutputTypeDef],
         "FirehoseArn": str,
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
-        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
+        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricStreamInputRequestTypeDef",
+MetricStreamStatisticsConfigurationUnionTypeDef = Union[
+    MetricStreamStatisticsConfigurationTypeDef, MetricStreamStatisticsConfigurationOutputTypeDef
+]
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
     {
-        "Name": str,
-        "FirehoseArn": str,
-        "RoleArn": str,
-        "OutputFormat": MetricStreamOutputFormatType,
+        "Id": str,
     },
 )
-_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricStreamInputRequestTypeDef",
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
     {
-        "IncludeFilters": Sequence[MetricStreamFilterTypeDef],
-        "ExcludeFilters": Sequence[MetricStreamFilterTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationTypeDef],
-        "IncludeLinkedAccountsMetrics": bool,
+        "MetricStat": MetricStatOutputTypeDef,
+        "Expression": str,
+        "Label": str,
+        "ReturnData": bool,
+        "Period": int,
+        "AccountId": str,
     },
     total=False,
 )
 
-
-class PutMetricStreamInputRequestTypeDef(
-    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
 ):
     pass
 
-
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -1380,71 +1441,46 @@
         "ReturnData": bool,
         "Period": int,
         "AccountId": str,
     },
     total=False,
 )
 
-
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
-
-_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "ScanBy": ScanByType,
-        "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetMetricDataInputGetMetricDataPaginateTypeDef(
-    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
-    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputRequestTypeDef",
+AnomalyDetectorConfigurationUnionTypeDef = Union[
+    AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
+]
+_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricStreamInputRequestTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "Name": str,
+        "FirehoseArn": str,
+        "RoleArn": str,
+        "OutputFormat": MetricStreamOutputFormatType,
     },
 )
-_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputRequestTypeDef",
+_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricStreamInputRequestTypeDef",
     {
-        "NextToken": str,
-        "ScanBy": ScanByType,
-        "MaxDatapoints": int,
-        "LabelOptions": LabelOptionsTypeDef,
+        "IncludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "ExcludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationUnionTypeDef],
+        "IncludeLinkedAccountsMetrics": bool,
     },
     total=False,
 )
 
-
-class GetMetricDataInputRequestTypeDef(
-    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
+class PutMetricStreamInputRequestTypeDef(
+    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
 ):
     pass
 
-
 MetricAlarmTypeDef = TypedDict(
     "MetricAlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmArn": str,
         "AlarmDescription": str,
         "AlarmConfigurationUpdatedTimestamp": datetime,
@@ -1465,22 +1501,31 @@
         "Unit": StandardUnitType,
         "EvaluationPeriods": int,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "ComparisonOperator": ComparisonOperatorType,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": List[MetricDataQueryTypeDef],
+        "Metrics": List[MetricDataQueryOutputTypeDef],
         "ThresholdMetricId": str,
         "EvaluationState": Literal["PARTIAL_DATA"],
         "StateTransitionedTimestamp": datetime,
     },
     total=False,
 )
 
+MetricMathAnomalyDetectorOutputTypeDef = TypedDict(
+    "MetricMathAnomalyDetectorOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
+MetricDataQueryUnionTypeDef = Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1513,21 +1558,100 @@
         "Metrics": Sequence[MetricDataQueryTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ThresholdMetricId": str,
     },
     total=False,
 )
 
-
 class PutMetricAlarmInputMetricPutAlarmTypeDef(
     _RequiredPutMetricAlarmInputMetricPutAlarmTypeDef,
     _OptionalPutMetricAlarmInputMetricPutAlarmTypeDef,
 ):
     pass
 
+DescribeAlarmsForMetricOutputTypeDef = TypedDict(
+    "DescribeAlarmsForMetricOutputTypeDef",
+    {
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmsOutputTypeDef = TypedDict(
+    "DescribeAlarmsOutputTypeDef",
+    {
+        "CompositeAlarms": List[CompositeAlarmTypeDef],
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AnomalyDetectorTypeDef = TypedDict(
+    "AnomalyDetectorTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "ScanBy": ScanByType,
+        "LabelOptions": LabelOptionsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetMetricDataInputGetMetricDataPaginateTypeDef(
+    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
+    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
+):
+    pass
+
+_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputRequestTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "ScanBy": ScanByType,
+        "MaxDatapoints": int,
+        "LabelOptions": LabelOptionsTypeDef,
+    },
+    total=False,
+)
+
+class GetMetricDataInputRequestTypeDef(
+    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
+):
+    pass
 
 _RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricAlarmInputRequestTypeDef",
     {
         "AlarmName": str,
         "EvaluationPeriods": int,
         "ComparisonOperator": ComparisonOperatorType,
@@ -1548,74 +1672,42 @@
         "Dimensions": Sequence[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": Sequence[MetricDataQueryTypeDef],
+        "Metrics": Sequence[MetricDataQueryUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ThresholdMetricId": str,
     },
     total=False,
 )
 
-
 class PutMetricAlarmInputRequestTypeDef(
     _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
 ):
     pass
 
-
-DescribeAlarmsForMetricOutputTypeDef = TypedDict(
-    "DescribeAlarmsForMetricOutputTypeDef",
-    {
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAlarmsOutputTypeDef = TypedDict(
-    "DescribeAlarmsOutputTypeDef",
-    {
-        "CompositeAlarms": List[CompositeAlarmTypeDef],
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AnomalyDetectorTypeDef = TypedDict(
-    "AnomalyDetectorTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
-        "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationTypeDef,
-        "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
-    },
-    total=False,
-)
-
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
+MetricMathAnomalyDetectorUnionTypeDef = Union[
+    MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
+]
 PutAnomalyDetectorInputRequestTypeDef = TypedDict(
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
@@ -1627,10 +1719,10 @@
 )
 
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/type_defs.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudwatch.type_defs import AlarmHistoryItemTypeDef
 
-    data: AlarmHistoryItemTypeDef = {...}
+    data: AlarmHistoryItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -35,87 +35,93 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AlarmHistoryItemTypeDef",
-    "RangeTypeDef",
+    "RangeOutputTypeDef",
     "DimensionTypeDef",
     "CompositeAlarmTypeDef",
     "DashboardEntryTypeDef",
     "DashboardValidationMessageTypeDef",
     "DatapointTypeDef",
     "DeleteAlarmsInputRequestTypeDef",
     "DeleteDashboardsInputRequestTypeDef",
     "DeleteInsightRulesInputRequestTypeDef",
     "PartialFailureTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteMetricStreamInputRequestTypeDef",
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
-    "DescribeAlarmHistoryInputRequestTypeDef",
+    "TimestampTypeDef",
+    "PaginatorConfigTypeDef",
     "WaiterConfigTypeDef",
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     "DescribeAlarmsInputRequestTypeDef",
     "DescribeInsightRulesInputRequestTypeDef",
     "InsightRuleTypeDef",
     "DimensionFilterTypeDef",
     "DisableAlarmActionsInputRequestTypeDef",
     "DisableInsightRulesInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EnableAlarmActionsInputRequestTypeDef",
     "EnableInsightRulesInputRequestTypeDef",
     "GetDashboardInputRequestTypeDef",
-    "GetDashboardOutputTypeDef",
-    "GetInsightRuleReportInputRequestTypeDef",
     "InsightRuleMetricDatapointTypeDef",
     "LabelOptionsTypeDef",
     "MessageDataTypeDef",
     "GetMetricStreamInputRequestTypeDef",
-    "MetricStreamFilterTypeDef",
+    "MetricStreamFilterOutputTypeDef",
     "GetMetricWidgetImageInputRequestTypeDef",
-    "GetMetricWidgetImageOutputTypeDef",
     "InsightRuleContributorDatapointTypeDef",
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "ListDashboardsInputRequestTypeDef",
     "ListManagedInsightRulesInputRequestTypeDef",
     "ListMetricStreamsInputRequestTypeDef",
     "MetricStreamEntryTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "TagTypeDef",
     "ManagedRuleStateTypeDef",
     "StatisticSetTypeDef",
+    "MetricStreamFilterTypeDef",
     "MetricStreamStatisticsMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "PutDashboardInputRequestTypeDef",
-    "PutMetricStreamOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "SetAlarmStateInputAlarmSetStateTypeDef",
     "SetAlarmStateInputRequestTypeDef",
     "StartMetricStreamsInputRequestTypeDef",
     "StopMetricStreamsInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
-    "DescribeAlarmHistoryOutputTypeDef",
-    "AnomalyDetectorConfigurationTypeDef",
+    "AnomalyDetectorConfigurationOutputTypeDef",
     "DescribeAlarmsForMetricInputRequestTypeDef",
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     "DescribeAnomalyDetectorsInputRequestTypeDef",
-    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
-    "GetMetricStatisticsInputRequestTypeDef",
+    "MetricOutputTypeDef",
     "MetricTypeDef",
+    "SingleMetricAnomalyDetectorOutputTypeDef",
     "SingleMetricAnomalyDetectorTypeDef",
-    "ListDashboardsOutputTypeDef",
-    "PutDashboardOutputTypeDef",
-    "GetMetricStatisticsOutputTypeDef",
     "DeleteInsightRulesOutputTypeDef",
+    "DescribeAlarmHistoryOutputTypeDef",
     "DisableInsightRulesOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "EnableInsightRulesOutputTypeDef",
+    "GetDashboardOutputTypeDef",
+    "GetMetricStatisticsOutputTypeDef",
+    "GetMetricWidgetImageOutputTypeDef",
+    "ListDashboardsOutputTypeDef",
+    "PutDashboardOutputTypeDef",
     "PutManagedInsightRulesOutputTypeDef",
+    "PutMetricStreamOutputTypeDef",
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    "GetInsightRuleReportInputRequestTypeDef",
+    "GetMetricStatisticsInputMetricGetStatisticsTypeDef",
+    "GetMetricStatisticsInputRequestTypeDef",
+    "RangeTypeDef",
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     "DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef",
     "DescribeInsightRulesOutputTypeDef",
     "ListMetricsInputListMetricsPaginateTypeDef",
     "ListMetricsInputRequestTypeDef",
     "MetricDataResultTypeDef",
     "InsightRuleContributorTypeDef",
@@ -123,35 +129,46 @@
     "ListTagsForResourceOutputTypeDef",
     "ManagedRuleTypeDef",
     "PutCompositeAlarmInputRequestTypeDef",
     "PutInsightRuleInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
     "ManagedRuleDescriptionTypeDef",
     "MetricDatumTypeDef",
+    "MetricStreamFilterUnionTypeDef",
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
     "MetricStreamStatisticsConfigurationTypeDef",
     "ListMetricsOutputTypeDef",
+    "MetricStatOutputTypeDef",
     "MetricStatTypeDef",
+    "SingleMetricAnomalyDetectorUnionTypeDef",
+    "AnomalyDetectorConfigurationTypeDef",
     "GetMetricDataOutputTypeDef",
     "GetInsightRuleReportOutputTypeDef",
     "PutManagedInsightRulesInputRequestTypeDef",
     "ListManagedInsightRulesOutputTypeDef",
     "PutMetricDataInputRequestTypeDef",
     "GetMetricStreamOutputTypeDef",
-    "PutMetricStreamInputRequestTypeDef",
+    "MetricStreamStatisticsConfigurationUnionTypeDef",
+    "MetricDataQueryOutputTypeDef",
     "MetricDataQueryTypeDef",
-    "GetMetricDataInputGetMetricDataPaginateTypeDef",
-    "GetMetricDataInputRequestTypeDef",
+    "AnomalyDetectorConfigurationUnionTypeDef",
+    "PutMetricStreamInputRequestTypeDef",
     "MetricAlarmTypeDef",
+    "MetricMathAnomalyDetectorOutputTypeDef",
+    "MetricDataQueryUnionTypeDef",
     "MetricMathAnomalyDetectorTypeDef",
     "PutMetricAlarmInputMetricPutAlarmTypeDef",
-    "PutMetricAlarmInputRequestTypeDef",
     "DescribeAlarmsForMetricOutputTypeDef",
     "DescribeAlarmsOutputTypeDef",
     "AnomalyDetectorTypeDef",
+    "GetMetricDataInputGetMetricDataPaginateTypeDef",
+    "GetMetricDataInputRequestTypeDef",
+    "PutMetricAlarmInputRequestTypeDef",
     "DeleteAnomalyDetectorInputRequestTypeDef",
+    "MetricMathAnomalyDetectorUnionTypeDef",
     "PutAnomalyDetectorInputRequestTypeDef",
     "DescribeAnomalyDetectorsOutputTypeDef",
 )
 
 AlarmHistoryItemTypeDef = TypedDict(
     "AlarmHistoryItemTypeDef",
     {
@@ -161,16 +178,16 @@
         "HistoryItemType": HistoryItemTypeType,
         "HistorySummary": str,
         "HistoryData": str,
     },
     total=False,
 )
 
-RangeTypeDef = TypedDict(
-    "RangeTypeDef",
+RangeOutputTypeDef = TypedDict(
+    "RangeOutputTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
     },
 )
 
 DimensionTypeDef = TypedDict(
@@ -270,88 +287,52 @@
         "ExceptionType": str,
         "FailureCode": str,
         "FailureDescription": str,
     },
     total=False,
 )
 
-DeleteMetricStreamInputRequestTypeDef = TypedDict(
-    "DeleteMetricStreamInputRequestTypeDef",
-    {
-        "Name": str,
-    },
-)
-
-DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
-    total=False,
 )
 
-DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
+DeleteMetricStreamInputRequestTypeDef = TypedDict(
+    "DeleteMetricStreamInputRequestTypeDef",
     {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "ScanBy": ScanByType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Name": str,
     },
-    total=False,
 )
 
-DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
-    "DescribeAlarmHistoryInputRequestTypeDef",
+TimestampTypeDef = Union[datetime, str]
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AlarmName": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "HistoryItemType": HistoryItemTypeType,
-        "StartDate": Union[datetime, str],
-        "EndDate": Union[datetime, str],
-        "MaxRecords": int,
-        "NextToken": str,
-        "ScanBy": ScanByType,
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 WaiterConfigTypeDef = TypedDict(
     "WaiterConfigTypeDef",
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
-    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
-    {
-        "AlarmNames": Sequence[str],
-        "AlarmNamePrefix": str,
-        "AlarmTypes": Sequence[AlarmTypeType],
-        "ChildrenOfAlarmName": str,
-        "ParentsOfAlarmName": str,
-        "StateValue": StateValueType,
-        "ActionPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeAlarmsInputRequestTypeDef = TypedDict(
     "DescribeAlarmsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
         "AlarmTypes": Sequence[AlarmTypeType],
         "ChildrenOfAlarmName": str,
@@ -386,55 +367,52 @@
     "_OptionalInsightRuleTypeDef",
     {
         "ManagedRule": bool,
     },
     total=False,
 )
 
+
 class InsightRuleTypeDef(_RequiredInsightRuleTypeDef, _OptionalInsightRuleTypeDef):
     pass
 
+
 _RequiredDimensionFilterTypeDef = TypedDict(
     "_RequiredDimensionFilterTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDimensionFilterTypeDef = TypedDict(
     "_OptionalDimensionFilterTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class DimensionFilterTypeDef(_RequiredDimensionFilterTypeDef, _OptionalDimensionFilterTypeDef):
     pass
 
+
 DisableAlarmActionsInputRequestTypeDef = TypedDict(
     "DisableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
 DisableInsightRulesInputRequestTypeDef = TypedDict(
     "DisableInsightRulesInputRequestTypeDef",
     {
         "RuleNames": Sequence[str],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnableAlarmActionsInputRequestTypeDef = TypedDict(
     "EnableAlarmActionsInputRequestTypeDef",
     {
         "AlarmNames": Sequence[str],
     },
 )
 
@@ -448,49 +426,14 @@
 GetDashboardInputRequestTypeDef = TypedDict(
     "GetDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
     },
 )
 
-GetDashboardOutputTypeDef = TypedDict(
-    "GetDashboardOutputTypeDef",
-    {
-        "DashboardArn": str,
-        "DashboardBody": str,
-        "DashboardName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_RequiredGetInsightRuleReportInputRequestTypeDef",
-    {
-        "RuleName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "Period": int,
-    },
-)
-_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
-    "_OptionalGetInsightRuleReportInputRequestTypeDef",
-    {
-        "MaxContributorCount": int,
-        "Metrics": Sequence[str],
-        "OrderBy": str,
-    },
-    total=False,
-)
-
-class GetInsightRuleReportInputRequestTypeDef(
-    _RequiredGetInsightRuleReportInputRequestTypeDef,
-    _OptionalGetInsightRuleReportInputRequestTypeDef,
-):
-    pass
-
 _RequiredInsightRuleMetricDatapointTypeDef = TypedDict(
     "_RequiredInsightRuleMetricDatapointTypeDef",
     {
         "Timestamp": datetime,
     },
 )
 _OptionalInsightRuleMetricDatapointTypeDef = TypedDict(
@@ -503,19 +446,21 @@
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
     total=False,
 )
 
+
 class InsightRuleMetricDatapointTypeDef(
     _RequiredInsightRuleMetricDatapointTypeDef, _OptionalInsightRuleMetricDatapointTypeDef
 ):
     pass
 
+
 LabelOptionsTypeDef = TypedDict(
     "LabelOptionsTypeDef",
     {
         "Timezone": str,
     },
     total=False,
 )
@@ -532,16 +477,16 @@
 GetMetricStreamInputRequestTypeDef = TypedDict(
     "GetMetricStreamInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-MetricStreamFilterTypeDef = TypedDict(
-    "MetricStreamFilterTypeDef",
+MetricStreamFilterOutputTypeDef = TypedDict(
+    "MetricStreamFilterOutputTypeDef",
     {
         "Namespace": str,
         "MetricNames": List[str],
     },
     total=False,
 )
 
@@ -555,45 +500,30 @@
     "_OptionalGetMetricWidgetImageInputRequestTypeDef",
     {
         "OutputFormat": str,
     },
     total=False,
 )
 
+
 class GetMetricWidgetImageInputRequestTypeDef(
     _RequiredGetMetricWidgetImageInputRequestTypeDef,
     _OptionalGetMetricWidgetImageInputRequestTypeDef,
 ):
     pass
 
-GetMetricWidgetImageOutputTypeDef = TypedDict(
-    "GetMetricWidgetImageOutputTypeDef",
-    {
-        "MetricWidgetImage": bytes,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 InsightRuleContributorDatapointTypeDef = TypedDict(
     "InsightRuleContributorDatapointTypeDef",
     {
         "Timestamp": datetime,
         "ApproximateValue": float,
     },
 )
 
-ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
-    "ListDashboardsInputListDashboardsPaginateTypeDef",
-    {
-        "DashboardNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDashboardsInputRequestTypeDef = TypedDict(
     "ListDashboardsInputRequestTypeDef",
     {
         "DashboardNamePrefix": str,
         "NextToken": str,
     },
     total=False,
@@ -610,20 +540,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListManagedInsightRulesInputRequestTypeDef(
     _RequiredListManagedInsightRulesInputRequestTypeDef,
     _OptionalListManagedInsightRulesInputRequestTypeDef,
 ):
     pass
 
+
 ListMetricStreamsInputRequestTypeDef = TypedDict(
     "ListMetricStreamsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -672,59 +604,39 @@
         "SampleCount": float,
         "Sum": float,
         "Minimum": float,
         "Maximum": float,
     },
 )
 
-MetricStreamStatisticsMetricTypeDef = TypedDict(
-    "MetricStreamStatisticsMetricTypeDef",
+MetricStreamFilterTypeDef = TypedDict(
+    "MetricStreamFilterTypeDef",
     {
         "Namespace": str,
-        "MetricName": str,
+        "MetricNames": Sequence[str],
     },
+    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+MetricStreamStatisticsMetricTypeDef = TypedDict(
+    "MetricStreamStatisticsMetricTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Namespace": str,
+        "MetricName": str,
     },
-    total=False,
 )
 
 PutDashboardInputRequestTypeDef = TypedDict(
     "PutDashboardInputRequestTypeDef",
     {
         "DashboardName": str,
         "DashboardBody": str,
     },
 )
 
-PutMetricStreamOutputTypeDef = TypedDict(
-    "PutMetricStreamOutputTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredSetAlarmStateInputAlarmSetStateTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateValue": StateValueType,
         "StateReason": str,
     },
 )
@@ -732,19 +644,21 @@
     "_OptionalSetAlarmStateInputAlarmSetStateTypeDef",
     {
         "StateReasonData": str,
     },
     total=False,
 )
 
+
 class SetAlarmStateInputAlarmSetStateTypeDef(
     _RequiredSetAlarmStateInputAlarmSetStateTypeDef, _OptionalSetAlarmStateInputAlarmSetStateTypeDef
 ):
     pass
 
+
 _RequiredSetAlarmStateInputRequestTypeDef = TypedDict(
     "_RequiredSetAlarmStateInputRequestTypeDef",
     {
         "AlarmName": str,
         "StateValue": StateValueType,
         "StateReason": str,
     },
@@ -753,19 +667,21 @@
     "_OptionalSetAlarmStateInputRequestTypeDef",
     {
         "StateReasonData": str,
     },
     total=False,
 )
 
+
 class SetAlarmStateInputRequestTypeDef(
     _RequiredSetAlarmStateInputRequestTypeDef, _OptionalSetAlarmStateInputRequestTypeDef
 ):
     pass
 
+
 StartMetricStreamsInputRequestTypeDef = TypedDict(
     "StartMetricStreamsInputRequestTypeDef",
     {
         "Names": Sequence[str],
     },
 )
 
@@ -780,27 +696,18 @@
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
 
-DescribeAlarmHistoryOutputTypeDef = TypedDict(
-    "DescribeAlarmHistoryOutputTypeDef",
+AnomalyDetectorConfigurationOutputTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationOutputTypeDef",
     {
-        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AnomalyDetectorConfigurationTypeDef = TypedDict(
-    "AnomalyDetectorConfigurationTypeDef",
-    {
-        "ExcludedTimeRanges": List[RangeTypeDef],
+        "ExcludedTimeRanges": List[RangeOutputTypeDef],
         "MetricTimezone": str,
     },
     total=False,
 )
 
 _RequiredDescribeAlarmsForMetricInputRequestTypeDef = TypedDict(
     "_RequiredDescribeAlarmsForMetricInputRequestTypeDef",
@@ -817,173 +724,344 @@
         "Dimensions": Sequence[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
+
 class DescribeAlarmsForMetricInputRequestTypeDef(
     _RequiredDescribeAlarmsForMetricInputRequestTypeDef,
     _OptionalDescribeAlarmsForMetricInputRequestTypeDef,
 ):
     pass
 
-DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
+
+DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputRequestTypeDef",
     {
+        "NextToken": str,
+        "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-DescribeAnomalyDetectorsInputRequestTypeDef = TypedDict(
-    "DescribeAnomalyDetectorsInputRequestTypeDef",
+MetricOutputTypeDef = TypedDict(
+    "MetricOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+    },
+    total=False,
+)
+
+MetricTypeDef = TypedDict(
+    "MetricTypeDef",
     {
-        "NextToken": str,
-        "MaxResults": int,
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
-        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
     },
     total=False,
 )
 
+SingleMetricAnomalyDetectorOutputTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorOutputTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
+SingleMetricAnomalyDetectorTypeDef = TypedDict(
+    "SingleMetricAnomalyDetectorTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "Stat": str,
+    },
+    total=False,
+)
+
+DeleteInsightRulesOutputTypeDef = TypedDict(
+    "DeleteInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryOutputTypeDef = TypedDict(
+    "DescribeAlarmHistoryOutputTypeDef",
+    {
+        "AlarmHistoryItems": List[AlarmHistoryItemTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableInsightRulesOutputTypeDef = TypedDict(
+    "DisableInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
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
+EnableInsightRulesOutputTypeDef = TypedDict(
+    "EnableInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDashboardOutputTypeDef = TypedDict(
+    "GetDashboardOutputTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardBody": str,
+        "DashboardName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricStatisticsOutputTypeDef = TypedDict(
+    "GetMetricStatisticsOutputTypeDef",
+    {
+        "Label": str,
+        "Datapoints": List[DatapointTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMetricWidgetImageOutputTypeDef = TypedDict(
+    "GetMetricWidgetImageOutputTypeDef",
+    {
+        "MetricWidgetImage": bytes,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDashboardsOutputTypeDef = TypedDict(
+    "ListDashboardsOutputTypeDef",
+    {
+        "DashboardEntries": List[DashboardEntryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutDashboardOutputTypeDef = TypedDict(
+    "PutDashboardOutputTypeDef",
+    {
+        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutManagedInsightRulesOutputTypeDef = TypedDict(
+    "PutManagedInsightRulesOutputTypeDef",
+    {
+        "Failures": List[PartialFailureTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutMetricStreamOutputTypeDef = TypedDict(
+    "PutMetricStreamOutputTypeDef",
+    {
+        "Arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef",
+    {
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+DescribeAlarmHistoryInputRequestTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputRequestTypeDef",
+    {
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "MaxRecords": int,
+        "NextToken": str,
+        "ScanBy": ScanByType,
+    },
+    total=False,
+)
+
+_RequiredGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_RequiredGetInsightRuleReportInputRequestTypeDef",
+    {
+        "RuleName": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "Period": int,
+    },
+)
+_OptionalGetInsightRuleReportInputRequestTypeDef = TypedDict(
+    "_OptionalGetInsightRuleReportInputRequestTypeDef",
+    {
+        "MaxContributorCount": int,
+        "Metrics": Sequence[str],
+        "OrderBy": str,
+    },
+    total=False,
+)
+
+
+class GetInsightRuleReportInputRequestTypeDef(
+    _RequiredGetInsightRuleReportInputRequestTypeDef,
+    _OptionalGetInsightRuleReportInputRequestTypeDef,
+):
+    pass
+
+
 _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
     "_RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Period": int,
     },
 )
 _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef = TypedDict(
     "_OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "Statistics": Sequence[StatisticType],
         "ExtendedStatistics": Sequence[str],
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
+
 class GetMetricStatisticsInputMetricGetStatisticsTypeDef(
     _RequiredGetMetricStatisticsInputMetricGetStatisticsTypeDef,
     _OptionalGetMetricStatisticsInputMetricGetStatisticsTypeDef,
 ):
     pass
 
+
 _RequiredGetMetricStatisticsInputRequestTypeDef = TypedDict(
     "_RequiredGetMetricStatisticsInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
         "Period": int,
     },
 )
 _OptionalGetMetricStatisticsInputRequestTypeDef = TypedDict(
     "_OptionalGetMetricStatisticsInputRequestTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
         "Statistics": Sequence[StatisticType],
         "ExtendedStatistics": Sequence[str],
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
+
 class GetMetricStatisticsInputRequestTypeDef(
     _RequiredGetMetricStatisticsInputRequestTypeDef, _OptionalGetMetricStatisticsInputRequestTypeDef
 ):
     pass
 
-MetricTypeDef = TypedDict(
-    "MetricTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-    },
-    total=False,
-)
-
-SingleMetricAnomalyDetectorTypeDef = TypedDict(
-    "SingleMetricAnomalyDetectorTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": Sequence[DimensionTypeDef],
-        "Stat": str,
-    },
-    total=False,
-)
-
-ListDashboardsOutputTypeDef = TypedDict(
-    "ListDashboardsOutputTypeDef",
-    {
-        "DashboardEntries": List[DashboardEntryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-PutDashboardOutputTypeDef = TypedDict(
-    "PutDashboardOutputTypeDef",
-    {
-        "DashboardValidationMessages": List[DashboardValidationMessageTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-GetMetricStatisticsOutputTypeDef = TypedDict(
-    "GetMetricStatisticsOutputTypeDef",
+RangeTypeDef = TypedDict(
+    "RangeTypeDef",
     {
-        "Label": str,
-        "Datapoints": List[DatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 
-DeleteInsightRulesOutputTypeDef = TypedDict(
-    "DeleteInsightRulesOutputTypeDef",
+DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef = TypedDict(
+    "DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmName": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "HistoryItemType": HistoryItemTypeType,
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "ScanBy": ScanByType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-DisableInsightRulesOutputTypeDef = TypedDict(
-    "DisableInsightRulesOutputTypeDef",
+DescribeAlarmsInputDescribeAlarmsPaginateTypeDef = TypedDict(
+    "DescribeAlarmsInputDescribeAlarmsPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AlarmNames": Sequence[str],
+        "AlarmNamePrefix": str,
+        "AlarmTypes": Sequence[AlarmTypeType],
+        "ChildrenOfAlarmName": str,
+        "ParentsOfAlarmName": str,
+        "StateValue": StateValueType,
+        "ActionPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-EnableInsightRulesOutputTypeDef = TypedDict(
-    "EnableInsightRulesOutputTypeDef",
+DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef = TypedDict(
+    "DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": Sequence[DimensionTypeDef],
+        "AnomalyDetectorTypes": Sequence[AnomalyDetectorTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-PutManagedInsightRulesOutputTypeDef = TypedDict(
-    "PutManagedInsightRulesOutputTypeDef",
+ListDashboardsInputListDashboardsPaginateTypeDef = TypedDict(
+    "ListDashboardsInputListDashboardsPaginateTypeDef",
     {
-        "Failures": List[PartialFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DashboardNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 DescribeAlarmsInputAlarmExistsWaitTypeDef = TypedDict(
     "DescribeAlarmsInputAlarmExistsWaitTypeDef",
     {
         "AlarmNames": Sequence[str],
         "AlarmNamePrefix": str,
@@ -1017,28 +1095,28 @@
 )
 
 DescribeInsightRulesOutputTypeDef = TypedDict(
     "DescribeInsightRulesOutputTypeDef",
     {
         "NextToken": str,
         "InsightRules": List[InsightRuleTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMetricsInputListMetricsPaginateTypeDef = TypedDict(
     "ListMetricsInputListMetricsPaginateTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionFilterTypeDef],
         "RecentlyActive": Literal["PT3H"],
         "IncludeLinkedAccounts": bool,
         "OwningAccount": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMetricsInputRequestTypeDef = TypedDict(
     "ListMetricsInputRequestTypeDef",
     {
@@ -1076,23 +1154,23 @@
 )
 
 ListMetricStreamsOutputTypeDef = TypedDict(
     "ListMetricStreamsOutputTypeDef",
     {
         "NextToken": str,
         "Entries": List[MetricStreamEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredManagedRuleTypeDef = TypedDict(
     "_RequiredManagedRuleTypeDef",
     {
         "TemplateName": str,
@@ -1103,17 +1181,19 @@
     "_OptionalManagedRuleTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class ManagedRuleTypeDef(_RequiredManagedRuleTypeDef, _OptionalManagedRuleTypeDef):
     pass
 
+
 _RequiredPutCompositeAlarmInputRequestTypeDef = TypedDict(
     "_RequiredPutCompositeAlarmInputRequestTypeDef",
     {
         "AlarmName": str,
         "AlarmRule": str,
     },
 )
@@ -1129,19 +1209,21 @@
         "ActionsSuppressor": str,
         "ActionsSuppressorWaitPeriod": int,
         "ActionsSuppressorExtensionPeriod": int,
     },
     total=False,
 )
 
+
 class PutCompositeAlarmInputRequestTypeDef(
     _RequiredPutCompositeAlarmInputRequestTypeDef, _OptionalPutCompositeAlarmInputRequestTypeDef
 ):
     pass
 
+
 _RequiredPutInsightRuleInputRequestTypeDef = TypedDict(
     "_RequiredPutInsightRuleInputRequestTypeDef",
     {
         "RuleName": str,
         "RuleDefinition": str,
     },
 )
@@ -1150,19 +1232,21 @@
     {
         "RuleState": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutInsightRuleInputRequestTypeDef(
     _RequiredPutInsightRuleInputRequestTypeDef, _OptionalPutInsightRuleInputRequestTypeDef
 ):
     pass
 
+
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -1183,45 +1267,77 @@
         "MetricName": str,
     },
 )
 _OptionalMetricDatumTypeDef = TypedDict(
     "_OptionalMetricDatumTypeDef",
     {
         "Dimensions": Sequence[DimensionTypeDef],
-        "Timestamp": Union[datetime, str],
+        "Timestamp": TimestampTypeDef,
         "Value": float,
         "StatisticValues": StatisticSetTypeDef,
         "Values": Sequence[float],
         "Counts": Sequence[float],
         "Unit": StandardUnitType,
         "StorageResolution": int,
     },
     total=False,
 )
 
+
 class MetricDatumTypeDef(_RequiredMetricDatumTypeDef, _OptionalMetricDatumTypeDef):
     pass
 
-MetricStreamStatisticsConfigurationTypeDef = TypedDict(
-    "MetricStreamStatisticsConfigurationTypeDef",
+
+MetricStreamFilterUnionTypeDef = Union[MetricStreamFilterTypeDef, MetricStreamFilterOutputTypeDef]
+MetricStreamStatisticsConfigurationOutputTypeDef = TypedDict(
+    "MetricStreamStatisticsConfigurationOutputTypeDef",
     {
         "IncludeMetrics": List[MetricStreamStatisticsMetricTypeDef],
         "AdditionalStatistics": List[str],
     },
 )
 
+MetricStreamStatisticsConfigurationTypeDef = TypedDict(
+    "MetricStreamStatisticsConfigurationTypeDef",
+    {
+        "IncludeMetrics": Sequence[MetricStreamStatisticsMetricTypeDef],
+        "AdditionalStatistics": Sequence[str],
+    },
+)
+
 ListMetricsOutputTypeDef = TypedDict(
     "ListMetricsOutputTypeDef",
     {
-        "Metrics": List[MetricTypeDef],
+        "Metrics": List[MetricOutputTypeDef],
         "NextToken": str,
         "OwningAccounts": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredMetricStatOutputTypeDef = TypedDict(
+    "_RequiredMetricStatOutputTypeDef",
+    {
+        "Metric": MetricOutputTypeDef,
+        "Period": int,
+        "Stat": str,
     },
 )
+_OptionalMetricStatOutputTypeDef = TypedDict(
+    "_OptionalMetricStatOutputTypeDef",
+    {
+        "Unit": StandardUnitType,
+    },
+    total=False,
+)
+
+
+class MetricStatOutputTypeDef(_RequiredMetricStatOutputTypeDef, _OptionalMetricStatOutputTypeDef):
+    pass
+
 
 _RequiredMetricStatTypeDef = TypedDict(
     "_RequiredMetricStatTypeDef",
     {
         "Metric": MetricTypeDef,
         "Period": int,
         "Stat": str,
@@ -1231,37 +1347,51 @@
     "_OptionalMetricStatTypeDef",
     {
         "Unit": StandardUnitType,
     },
     total=False,
 )
 
+
 class MetricStatTypeDef(_RequiredMetricStatTypeDef, _OptionalMetricStatTypeDef):
     pass
 
+
+SingleMetricAnomalyDetectorUnionTypeDef = Union[
+    SingleMetricAnomalyDetectorTypeDef, SingleMetricAnomalyDetectorOutputTypeDef
+]
+AnomalyDetectorConfigurationTypeDef = TypedDict(
+    "AnomalyDetectorConfigurationTypeDef",
+    {
+        "ExcludedTimeRanges": Sequence[RangeTypeDef],
+        "MetricTimezone": str,
+    },
+    total=False,
+)
+
 GetMetricDataOutputTypeDef = TypedDict(
     "GetMetricDataOutputTypeDef",
     {
         "MetricDataResults": List[MetricDataResultTypeDef],
         "NextToken": str,
         "Messages": List[MessageDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightRuleReportOutputTypeDef = TypedDict(
     "GetInsightRuleReportOutputTypeDef",
     {
         "KeyLabels": List[str],
         "AggregationStatistic": str,
         "AggregateValue": float,
         "ApproximateUniqueCount": int,
         "Contributors": List[InsightRuleContributorTypeDef],
         "MetricDatapoints": List[InsightRuleMetricDatapointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutManagedInsightRulesInputRequestTypeDef = TypedDict(
     "PutManagedInsightRulesInputRequestTypeDef",
     {
         "ManagedRules": Sequence[ManagedRuleTypeDef],
@@ -1269,15 +1399,15 @@
 )
 
 ListManagedInsightRulesOutputTypeDef = TypedDict(
     "ListManagedInsightRulesOutputTypeDef",
     {
         "ManagedRules": List[ManagedRuleDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutMetricDataInputRequestTypeDef = TypedDict(
     "PutMetricDataInputRequestTypeDef",
     {
         "Namespace": str,
@@ -1286,54 +1416,57 @@
 )
 
 GetMetricStreamOutputTypeDef = TypedDict(
     "GetMetricStreamOutputTypeDef",
     {
         "Arn": str,
         "Name": str,
-        "IncludeFilters": List[MetricStreamFilterTypeDef],
-        "ExcludeFilters": List[MetricStreamFilterTypeDef],
+        "IncludeFilters": List[MetricStreamFilterOutputTypeDef],
+        "ExcludeFilters": List[MetricStreamFilterOutputTypeDef],
         "FirehoseArn": str,
         "RoleArn": str,
         "State": str,
         "CreationDate": datetime,
         "LastUpdateDate": datetime,
         "OutputFormat": MetricStreamOutputFormatType,
-        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationTypeDef],
+        "StatisticsConfigurations": List[MetricStreamStatisticsConfigurationOutputTypeDef],
         "IncludeLinkedAccountsMetrics": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_RequiredPutMetricStreamInputRequestTypeDef",
+MetricStreamStatisticsConfigurationUnionTypeDef = Union[
+    MetricStreamStatisticsConfigurationTypeDef, MetricStreamStatisticsConfigurationOutputTypeDef
+]
+_RequiredMetricDataQueryOutputTypeDef = TypedDict(
+    "_RequiredMetricDataQueryOutputTypeDef",
     {
-        "Name": str,
-        "FirehoseArn": str,
-        "RoleArn": str,
-        "OutputFormat": MetricStreamOutputFormatType,
+        "Id": str,
     },
 )
-_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
-    "_OptionalPutMetricStreamInputRequestTypeDef",
+_OptionalMetricDataQueryOutputTypeDef = TypedDict(
+    "_OptionalMetricDataQueryOutputTypeDef",
     {
-        "IncludeFilters": Sequence[MetricStreamFilterTypeDef],
-        "ExcludeFilters": Sequence[MetricStreamFilterTypeDef],
-        "Tags": Sequence[TagTypeDef],
-        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationTypeDef],
-        "IncludeLinkedAccountsMetrics": bool,
+        "MetricStat": MetricStatOutputTypeDef,
+        "Expression": str,
+        "Label": str,
+        "ReturnData": bool,
+        "Period": int,
+        "AccountId": str,
     },
     total=False,
 )
 
-class PutMetricStreamInputRequestTypeDef(
-    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
+
+class MetricDataQueryOutputTypeDef(
+    _RequiredMetricDataQueryOutputTypeDef, _OptionalMetricDataQueryOutputTypeDef
 ):
     pass
 
+
 _RequiredMetricDataQueryTypeDef = TypedDict(
     "_RequiredMetricDataQueryTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalMetricDataQueryTypeDef = TypedDict(
@@ -1345,65 +1478,50 @@
         "ReturnData": bool,
         "Period": int,
         "AccountId": str,
     },
     total=False,
 )
 
+
 class MetricDataQueryTypeDef(_RequiredMetricDataQueryTypeDef, _OptionalMetricDataQueryTypeDef):
     pass
 
-_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
-    {
-        "ScanBy": ScanByType,
-        "LabelOptions": LabelOptionsTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
-class GetMetricDataInputGetMetricDataPaginateTypeDef(
-    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
-    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
-):
-    pass
-
-_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
-    "_RequiredGetMetricDataInputRequestTypeDef",
+AnomalyDetectorConfigurationUnionTypeDef = Union[
+    AnomalyDetectorConfigurationTypeDef, AnomalyDetectorConfigurationOutputTypeDef
+]
+_RequiredPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_RequiredPutMetricStreamInputRequestTypeDef",
     {
-        "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "Name": str,
+        "FirehoseArn": str,
+        "RoleArn": str,
+        "OutputFormat": MetricStreamOutputFormatType,
     },
 )
-_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
-    "_OptionalGetMetricDataInputRequestTypeDef",
+_OptionalPutMetricStreamInputRequestTypeDef = TypedDict(
+    "_OptionalPutMetricStreamInputRequestTypeDef",
     {
-        "NextToken": str,
-        "ScanBy": ScanByType,
-        "MaxDatapoints": int,
-        "LabelOptions": LabelOptionsTypeDef,
+        "IncludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "ExcludeFilters": Sequence[MetricStreamFilterUnionTypeDef],
+        "Tags": Sequence[TagTypeDef],
+        "StatisticsConfigurations": Sequence[MetricStreamStatisticsConfigurationUnionTypeDef],
+        "IncludeLinkedAccountsMetrics": bool,
     },
     total=False,
 )
 
-class GetMetricDataInputRequestTypeDef(
-    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
+
+class PutMetricStreamInputRequestTypeDef(
+    _RequiredPutMetricStreamInputRequestTypeDef, _OptionalPutMetricStreamInputRequestTypeDef
 ):
     pass
 
+
 MetricAlarmTypeDef = TypedDict(
     "MetricAlarmTypeDef",
     {
         "AlarmName": str,
         "AlarmArn": str,
         "AlarmDescription": str,
         "AlarmConfigurationUpdatedTimestamp": datetime,
@@ -1424,22 +1542,31 @@
         "Unit": StandardUnitType,
         "EvaluationPeriods": int,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "ComparisonOperator": ComparisonOperatorType,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": List[MetricDataQueryTypeDef],
+        "Metrics": List[MetricDataQueryOutputTypeDef],
         "ThresholdMetricId": str,
         "EvaluationState": Literal["PARTIAL_DATA"],
         "StateTransitionedTimestamp": datetime,
     },
     total=False,
 )
 
+MetricMathAnomalyDetectorOutputTypeDef = TypedDict(
+    "MetricMathAnomalyDetectorOutputTypeDef",
+    {
+        "MetricDataQueries": List[MetricDataQueryOutputTypeDef],
+    },
+    total=False,
+)
+
+MetricDataQueryUnionTypeDef = Union[MetricDataQueryTypeDef, MetricDataQueryOutputTypeDef]
 MetricMathAnomalyDetectorTypeDef = TypedDict(
     "MetricMathAnomalyDetectorTypeDef",
     {
         "MetricDataQueries": Sequence[MetricDataQueryTypeDef],
     },
     total=False,
 )
@@ -1472,20 +1599,107 @@
         "Metrics": Sequence[MetricDataQueryTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ThresholdMetricId": str,
     },
     total=False,
 )
 
+
 class PutMetricAlarmInputMetricPutAlarmTypeDef(
     _RequiredPutMetricAlarmInputMetricPutAlarmTypeDef,
     _OptionalPutMetricAlarmInputMetricPutAlarmTypeDef,
 ):
     pass
 
+
+DescribeAlarmsForMetricOutputTypeDef = TypedDict(
+    "DescribeAlarmsForMetricOutputTypeDef",
+    {
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAlarmsOutputTypeDef = TypedDict(
+    "DescribeAlarmsOutputTypeDef",
+    {
+        "CompositeAlarms": List[CompositeAlarmTypeDef],
+        "MetricAlarms": List[MetricAlarmTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AnomalyDetectorTypeDef = TypedDict(
+    "AnomalyDetectorTypeDef",
+    {
+        "Namespace": str,
+        "MetricName": str,
+        "Dimensions": List[DimensionTypeDef],
+        "Stat": str,
+        "Configuration": AnomalyDetectorConfigurationOutputTypeDef,
+        "StateValue": AnomalyDetectorStateValueType,
+        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorOutputTypeDef,
+        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputGetMetricDataPaginateTypeDef",
+    {
+        "ScanBy": ScanByType,
+        "LabelOptions": LabelOptionsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetMetricDataInputGetMetricDataPaginateTypeDef(
+    _RequiredGetMetricDataInputGetMetricDataPaginateTypeDef,
+    _OptionalGetMetricDataInputGetMetricDataPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetMetricDataInputRequestTypeDef = TypedDict(
+    "_RequiredGetMetricDataInputRequestTypeDef",
+    {
+        "MetricDataQueries": Sequence[MetricDataQueryUnionTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetMetricDataInputRequestTypeDef = TypedDict(
+    "_OptionalGetMetricDataInputRequestTypeDef",
+    {
+        "NextToken": str,
+        "ScanBy": ScanByType,
+        "MaxDatapoints": int,
+        "LabelOptions": LabelOptionsTypeDef,
+    },
+    total=False,
+)
+
+
+class GetMetricDataInputRequestTypeDef(
+    _RequiredGetMetricDataInputRequestTypeDef, _OptionalGetMetricDataInputRequestTypeDef
+):
+    pass
+
+
 _RequiredPutMetricAlarmInputRequestTypeDef = TypedDict(
     "_RequiredPutMetricAlarmInputRequestTypeDef",
     {
         "AlarmName": str,
         "EvaluationPeriods": int,
         "ComparisonOperator": ComparisonOperatorType,
     },
@@ -1505,72 +1719,44 @@
         "Dimensions": Sequence[DimensionTypeDef],
         "Period": int,
         "Unit": StandardUnitType,
         "DatapointsToAlarm": int,
         "Threshold": float,
         "TreatMissingData": str,
         "EvaluateLowSampleCountPercentile": str,
-        "Metrics": Sequence[MetricDataQueryTypeDef],
+        "Metrics": Sequence[MetricDataQueryUnionTypeDef],
         "Tags": Sequence[TagTypeDef],
         "ThresholdMetricId": str,
     },
     total=False,
 )
 
+
 class PutMetricAlarmInputRequestTypeDef(
     _RequiredPutMetricAlarmInputRequestTypeDef, _OptionalPutMetricAlarmInputRequestTypeDef
 ):
     pass
 
-DescribeAlarmsForMetricOutputTypeDef = TypedDict(
-    "DescribeAlarmsForMetricOutputTypeDef",
-    {
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeAlarmsOutputTypeDef = TypedDict(
-    "DescribeAlarmsOutputTypeDef",
-    {
-        "CompositeAlarms": List[CompositeAlarmTypeDef],
-        "MetricAlarms": List[MetricAlarmTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-AnomalyDetectorTypeDef = TypedDict(
-    "AnomalyDetectorTypeDef",
-    {
-        "Namespace": str,
-        "MetricName": str,
-        "Dimensions": List[DimensionTypeDef],
-        "Stat": str,
-        "Configuration": AnomalyDetectorConfigurationTypeDef,
-        "StateValue": AnomalyDetectorStateValueType,
-        "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
-        "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
-    },
-    total=False,
-)
 
 DeleteAnomalyDetectorInputRequestTypeDef = TypedDict(
     "DeleteAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
         "SingleMetricAnomalyDetector": SingleMetricAnomalyDetectorTypeDef,
         "MetricMathAnomalyDetector": MetricMathAnomalyDetectorTypeDef,
     },
     total=False,
 )
 
+MetricMathAnomalyDetectorUnionTypeDef = Union[
+    MetricMathAnomalyDetectorTypeDef, MetricMathAnomalyDetectorOutputTypeDef
+]
 PutAnomalyDetectorInputRequestTypeDef = TypedDict(
     "PutAnomalyDetectorInputRequestTypeDef",
     {
         "Namespace": str,
         "MetricName": str,
         "Dimensions": Sequence[DimensionTypeDef],
         "Stat": str,
@@ -1582,10 +1768,10 @@
 )
 
 DescribeAnomalyDetectorsOutputTypeDef = TypedDict(
     "DescribeAnomalyDetectorsOutputTypeDef",
     {
         "AnomalyDetectors": List[AnomalyDetectorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/waiter.py` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch/waiter.pyi` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/PKG-INFO` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudwatch
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatch 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatch 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudwatch type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudwatch type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudwatch"></a>
 
 # types-aiobotocore-cloudwatch
 
 [![PyPI - types-aiobotocore-cloudwatch](https://img.shields.io/pypi/v/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudwatch.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudwatch)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudwatch?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudwatch)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudwatch)](https://pepy.tech/project/types-aiobotocore-cloudwatch)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatch 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudwatch.html#CloudWatch)
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
 [types-aiobotocore-cloudwatch docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudwatch/).
 
 See how it helps to find and fix potential bugs:
 
@@ -78,15 +77,15 @@
     - [Client annotations](#client-annotations)
     - [Paginators annotations](#paginators-annotations)
     - [Waiters annotations](#waiters-annotations)
     - [Service Resource annotations](#service-resource-annotations)
     - [Other resources annotations](#other-resources-annotations)
     - [Collections annotations](#collections-annotations)
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
@@ -439,95 +438,100 @@
 )
 
 
 def check_value(value: ActionsSuppressedByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudwatch.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudwatch.type_defs import (
     AlarmHistoryItemTypeDef,
-    RangeTypeDef,
+    RangeOutputTypeDef,
     DimensionTypeDef,
     CompositeAlarmTypeDef,
     DashboardEntryTypeDef,
     DashboardValidationMessageTypeDef,
     DatapointTypeDef,
     DeleteAlarmsInputRequestTypeDef,
     DeleteDashboardsInputRequestTypeDef,
     DeleteInsightRulesInputRequestTypeDef,
     PartialFailureTypeDef,
+    ResponseMetadataTypeDef,
     DeleteMetricStreamInputRequestTypeDef,
-    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
-    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
-    DescribeAlarmHistoryInputRequestTypeDef,
+    TimestampTypeDef,
+    PaginatorConfigTypeDef,
     WaiterConfigTypeDef,
-    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
     DescribeAlarmsInputRequestTypeDef,
     DescribeInsightRulesInputRequestTypeDef,
     InsightRuleTypeDef,
     DimensionFilterTypeDef,
     DisableAlarmActionsInputRequestTypeDef,
     DisableInsightRulesInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     EnableAlarmActionsInputRequestTypeDef,
     EnableInsightRulesInputRequestTypeDef,
     GetDashboardInputRequestTypeDef,
-    GetDashboardOutputTypeDef,
-    GetInsightRuleReportInputRequestTypeDef,
     InsightRuleMetricDatapointTypeDef,
     LabelOptionsTypeDef,
     MessageDataTypeDef,
     GetMetricStreamInputRequestTypeDef,
-    MetricStreamFilterTypeDef,
+    MetricStreamFilterOutputTypeDef,
     GetMetricWidgetImageInputRequestTypeDef,
-    GetMetricWidgetImageOutputTypeDef,
     InsightRuleContributorDatapointTypeDef,
-    ListDashboardsInputListDashboardsPaginateTypeDef,
     ListDashboardsInputRequestTypeDef,
     ListManagedInsightRulesInputRequestTypeDef,
     ListMetricStreamsInputRequestTypeDef,
     MetricStreamEntryTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     TagTypeDef,
     ManagedRuleStateTypeDef,
     StatisticSetTypeDef,
+    MetricStreamFilterTypeDef,
     MetricStreamStatisticsMetricTypeDef,
-    PaginatorConfigTypeDef,
     PutDashboardInputRequestTypeDef,
-    PutMetricStreamOutputTypeDef,
-    ResponseMetadataTypeDef,
     SetAlarmStateInputAlarmSetStateTypeDef,
     SetAlarmStateInputRequestTypeDef,
     StartMetricStreamsInputRequestTypeDef,
     StopMetricStreamsInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
-    DescribeAlarmHistoryOutputTypeDef,
-    AnomalyDetectorConfigurationTypeDef,
+    AnomalyDetectorConfigurationOutputTypeDef,
     DescribeAlarmsForMetricInputRequestTypeDef,
-    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
     DescribeAnomalyDetectorsInputRequestTypeDef,
-    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
-    GetMetricStatisticsInputRequestTypeDef,
+    MetricOutputTypeDef,
     MetricTypeDef,
+    SingleMetricAnomalyDetectorOutputTypeDef,
     SingleMetricAnomalyDetectorTypeDef,
-    ListDashboardsOutputTypeDef,
-    PutDashboardOutputTypeDef,
-    GetMetricStatisticsOutputTypeDef,
     DeleteInsightRulesOutputTypeDef,
+    DescribeAlarmHistoryOutputTypeDef,
     DisableInsightRulesOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
     EnableInsightRulesOutputTypeDef,
+    GetDashboardOutputTypeDef,
+    GetMetricStatisticsOutputTypeDef,
+    GetMetricWidgetImageOutputTypeDef,
+    ListDashboardsOutputTypeDef,
+    PutDashboardOutputTypeDef,
     PutManagedInsightRulesOutputTypeDef,
+    PutMetricStreamOutputTypeDef,
+    DescribeAlarmHistoryInputAlarmDescribeHistoryTypeDef,
+    DescribeAlarmHistoryInputRequestTypeDef,
+    GetInsightRuleReportInputRequestTypeDef,
+    GetMetricStatisticsInputMetricGetStatisticsTypeDef,
+    GetMetricStatisticsInputRequestTypeDef,
+    RangeTypeDef,
+    DescribeAlarmHistoryInputDescribeAlarmHistoryPaginateTypeDef,
+    DescribeAlarmsInputDescribeAlarmsPaginateTypeDef,
+    DescribeAnomalyDetectorsInputDescribeAnomalyDetectorsPaginateTypeDef,
+    ListDashboardsInputListDashboardsPaginateTypeDef,
     DescribeAlarmsInputAlarmExistsWaitTypeDef,
     DescribeAlarmsInputCompositeAlarmExistsWaitTypeDef,
     DescribeInsightRulesOutputTypeDef,
     ListMetricsInputListMetricsPaginateTypeDef,
     ListMetricsInputRequestTypeDef,
     MetricDataResultTypeDef,
     InsightRuleContributorTypeDef,
@@ -535,41 +539,52 @@
     ListTagsForResourceOutputTypeDef,
     ManagedRuleTypeDef,
     PutCompositeAlarmInputRequestTypeDef,
     PutInsightRuleInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
     ManagedRuleDescriptionTypeDef,
     MetricDatumTypeDef,
+    MetricStreamFilterUnionTypeDef,
+    MetricStreamStatisticsConfigurationOutputTypeDef,
     MetricStreamStatisticsConfigurationTypeDef,
     ListMetricsOutputTypeDef,
+    MetricStatOutputTypeDef,
     MetricStatTypeDef,
+    SingleMetricAnomalyDetectorUnionTypeDef,
+    AnomalyDetectorConfigurationTypeDef,
     GetMetricDataOutputTypeDef,
     GetInsightRuleReportOutputTypeDef,
     PutManagedInsightRulesInputRequestTypeDef,
     ListManagedInsightRulesOutputTypeDef,
     PutMetricDataInputRequestTypeDef,
     GetMetricStreamOutputTypeDef,
-    PutMetricStreamInputRequestTypeDef,
+    MetricStreamStatisticsConfigurationUnionTypeDef,
+    MetricDataQueryOutputTypeDef,
     MetricDataQueryTypeDef,
-    GetMetricDataInputGetMetricDataPaginateTypeDef,
-    GetMetricDataInputRequestTypeDef,
+    AnomalyDetectorConfigurationUnionTypeDef,
+    PutMetricStreamInputRequestTypeDef,
     MetricAlarmTypeDef,
+    MetricMathAnomalyDetectorOutputTypeDef,
+    MetricDataQueryUnionTypeDef,
     MetricMathAnomalyDetectorTypeDef,
     PutMetricAlarmInputMetricPutAlarmTypeDef,
-    PutMetricAlarmInputRequestTypeDef,
     DescribeAlarmsForMetricOutputTypeDef,
     DescribeAlarmsOutputTypeDef,
     AnomalyDetectorTypeDef,
+    GetMetricDataInputGetMetricDataPaginateTypeDef,
+    GetMetricDataInputRequestTypeDef,
+    PutMetricAlarmInputRequestTypeDef,
     DeleteAnomalyDetectorInputRequestTypeDef,
+    MetricMathAnomalyDetectorUnionTypeDef,
     PutAnomalyDetectorInputRequestTypeDef,
     DescribeAnomalyDetectorsOutputTypeDef,
 )
 
 
-def get_structure() -> AlarmHistoryItemTypeDef:
+def get_value() -> AlarmHistoryItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudwatch-2.5.2/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt` & `types-aiobotocore-cloudwatch-2.5.2.post1/types_aiobotocore_cloudwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*


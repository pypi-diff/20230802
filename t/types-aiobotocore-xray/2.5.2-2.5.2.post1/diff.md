# Comparing `tmp/types-aiobotocore-xray-2.5.2.tar.gz` & `tmp/types-aiobotocore-xray-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-xray-2.5.2.tar", last modified: Sat Jul  8 01:44:29 2023, max compression
+gzip compressed data, was "types-aiobotocore-xray-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:11 2023, max compression
```

## Comparing `types-aiobotocore-xray-2.5.2.tar` & `types-aiobotocore-xray-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:29.347067 types-aiobotocore-xray-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-07-08 01:44:29.347067 types-aiobotocore-xray-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17438 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:29.347067 types-aiobotocore-xray-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:29.347067 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27777 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27728 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-07-08 01:42:52.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    43365 2023-07-08 01:42:52.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    43316 2023-07-08 01:42:52.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:51.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:29.347067 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18991 2023-07-08 01:44:29.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-08 01:44:29.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:29.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:29.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:29.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-08 01:44:29.000000 types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.417424 types-aiobotocore-xray-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-08-02 14:53:11.417424 types-aiobotocore-xray-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:11.417424 types-aiobotocore-xray-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.413423 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27732 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27683 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9932 2023-08-02 14:51:30.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9930 2023-08-02 14:51:30.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12648 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    44138 2023-08-02 14:51:31.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44087 2023-08-02 14:51:30.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:51:26.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:11.413423 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19010 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-02 14:53:11.000000 types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-xray-2.5.2/LICENSE` & `types-aiobotocore-xray-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2/PKG-INFO` & `types-aiobotocore-xray-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-xray
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore xray type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore xray type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-xray"></a>
 
 # types-aiobotocore-xray
 
 [![PyPI - types-aiobotocore-xray](https://img.shields.io/pypi/v/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-xray?color=blue)](https://pypistats.org/packages/types-aiobotocore-xray)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.XRay 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [types-aiobotocore-xray docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/).
 
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
@@ -352,132 +351,135 @@
 )
 
 
 def check_value(value: BatchGetTracesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_xray.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetTracesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
-    GetInsightImpactGraphRequestRequestTypeDef,
+    TimestampTypeDef,
     GetInsightRequestRequestTypeDef,
-    GetInsightSummariesRequestRequestTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
-    SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
-    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
-    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
-    TelemetryRecordTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
-    SamplingRuleRecordTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
+    GetInsightImpactGraphRequestRequestTypeDef,
+    GetInsightSummariesRequestRequestTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    SamplingStatisticsDocumentTypeDef,
+    TelemetryRecordTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
-    GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
+    SamplingRuleRecordTypeDef,
+    SamplingRuleUnionTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
-    PutTelemetryRecordsRequestRequestTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
-    CreateSamplingRuleResultTypeDef,
-    DeleteSamplingRuleResultTypeDef,
-    GetSamplingRulesResultTypeDef,
-    UpdateSamplingRuleResultTypeDef,
     EdgeTypeDef,
     TimeSeriesServiceStatisticsTypeDef,
     ErrorRootCauseServiceTypeDef,
     FaultRootCauseServiceTypeDef,
+    GetSamplingTargetsRequestRequestTypeDef,
+    PutTelemetryRecordsRequestRequestTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
+    CreateSamplingRuleResultTypeDef,
+    DeleteSamplingRuleResultTypeDef,
+    GetSamplingRulesResultTypeDef,
+    UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
     GetInsightEventsResultTypeDef,
     GetInsightSummariesResultTypeDef,
     GetInsightResultTypeDef,
     ServiceTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     ErrorRootCauseTypeDef,
@@ -485,15 +487,15 @@
     GetServiceGraphResultTypeDef,
     GetTraceGraphResultTypeDef,
     TraceSummaryTypeDef,
     GetTraceSummariesResultTypeDef,
 )
 
 
-def get_structure() -> AliasTypeDef:
+def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-xray-2.5.2/README.md` & `types-aiobotocore-xray-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-xray"></a>
 
 # types-aiobotocore-xray
 
 [![PyPI - types-aiobotocore-xray](https://img.shields.io/pypi/v/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-xray?color=blue)](https://pypistats.org/packages/types-aiobotocore-xray)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.XRay 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [types-aiobotocore-xray docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/).
 
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
@@ -319,132 +319,135 @@
 )
 
 
 def check_value(value: BatchGetTracesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_xray.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetTracesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
-    GetInsightImpactGraphRequestRequestTypeDef,
+    TimestampTypeDef,
     GetInsightRequestRequestTypeDef,
-    GetInsightSummariesRequestRequestTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
-    SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
-    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
-    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
-    TelemetryRecordTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
-    SamplingRuleRecordTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
+    GetInsightImpactGraphRequestRequestTypeDef,
+    GetInsightSummariesRequestRequestTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    SamplingStatisticsDocumentTypeDef,
+    TelemetryRecordTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
-    GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
+    SamplingRuleRecordTypeDef,
+    SamplingRuleUnionTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
-    PutTelemetryRecordsRequestRequestTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
-    CreateSamplingRuleResultTypeDef,
-    DeleteSamplingRuleResultTypeDef,
-    GetSamplingRulesResultTypeDef,
-    UpdateSamplingRuleResultTypeDef,
     EdgeTypeDef,
     TimeSeriesServiceStatisticsTypeDef,
     ErrorRootCauseServiceTypeDef,
     FaultRootCauseServiceTypeDef,
+    GetSamplingTargetsRequestRequestTypeDef,
+    PutTelemetryRecordsRequestRequestTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
+    CreateSamplingRuleResultTypeDef,
+    DeleteSamplingRuleResultTypeDef,
+    GetSamplingRulesResultTypeDef,
+    UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
     GetInsightEventsResultTypeDef,
     GetInsightSummariesResultTypeDef,
     GetInsightResultTypeDef,
     ServiceTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     ErrorRootCauseTypeDef,
@@ -452,15 +455,15 @@
     GetServiceGraphResultTypeDef,
     GetTraceGraphResultTypeDef,
     TraceSummaryTypeDef,
     GetTraceSummariesResultTypeDef,
 )
 
 
-def get_structure() -> AliasTypeDef:
+def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-xray-2.5.2/setup.py` & `types-aiobotocore-xray-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-xray",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_xray"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder"
-        " 7.14.5"
+        " 7.17.1"
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
-    keywords="aiobotocore xray type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore xray type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_xray": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/__init__.py` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/__init__.pyi` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/__main__.py` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.XRay 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.XRay 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay\nOther"
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

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/client.py` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("xray") as client:
         client: XRayClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EncryptionTypeType, InsightStateType, TimeRangeTypeType
 from .paginator import (
     BatchGetTracesPaginator,
@@ -55,20 +54,21 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
-    SamplingRuleTypeDef,
+    SamplingRuleUnionTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
+    TimestampTypeDef,
     UpdateGroupResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -155,15 +155,15 @@
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_group)
         """
 
     async def create_sampling_rule(
-        self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, SamplingRule: SamplingRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_sampling_rule)
         """
@@ -255,30 +255,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_insight_events)
         """
 
     async def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_insight_impact_graph)
         """
 
     async def get_insight_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
         GroupName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetInsightSummariesResultTypeDef:
         """
@@ -317,16 +317,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_sampling_targets)
         """
 
     async def get_service_graph(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         NextToken: str = ...
     ) -> GetServiceGraphResultTypeDef:
         """
         Retrieves a document that describes services that process incoming requests, and
         downstream services that they call as a result.
@@ -334,16 +334,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_service_graph)
         """
 
     async def get_time_series_service_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
         NextToken: str = ...
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
@@ -363,16 +363,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_trace_graph)
         """
 
     async def get_trace_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
         NextToken: str = ...
     ) -> GetTraceSummariesResultTypeDef:
         """
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/client.pyi` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("xray") as client:
         client: XRayClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import EncryptionTypeType, InsightStateType, TimeRangeTypeType
 from .paginator import (
     BatchGetTracesPaginator,
@@ -55,20 +54,21 @@
     GetTraceSummariesResultTypeDef,
     InsightsConfigurationTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutEncryptionConfigResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
-    SamplingRuleTypeDef,
+    SamplingRuleUnionTypeDef,
     SamplingRuleUpdateTypeDef,
     SamplingStatisticsDocumentTypeDef,
     SamplingStrategyTypeDef,
     TagTypeDef,
     TelemetryRecordTypeDef,
+    TimestampTypeDef,
     UpdateGroupResultTypeDef,
     UpdateSamplingRuleResultTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -146,15 +146,15 @@
         """
         Creates a group resource with a name and a filter expression.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_group)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_group)
         """
     async def create_sampling_rule(
-        self, *, SamplingRule: SamplingRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, SamplingRule: SamplingRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> CreateSamplingRuleResultTypeDef:
         """
         Creates a rule to control sampling behavior for instrumented applications.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.create_sampling_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#create_sampling_rule)
         """
@@ -236,29 +236,29 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_events)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_insight_events)
         """
     async def get_insight_impact_graph(
         self,
         *,
         InsightId: str,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         NextToken: str = ...
     ) -> GetInsightImpactGraphResultTypeDef:
         """
         Retrieves a service graph structure filtered by the specified insight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_insight_impact_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_insight_impact_graph)
         """
     async def get_insight_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         States: Sequence[InsightStateType] = ...,
         GroupARN: str = ...,
         GroupName: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> GetInsightSummariesResultTypeDef:
         """
@@ -293,32 +293,32 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_sampling_targets)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_sampling_targets)
         """
     async def get_service_graph(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         NextToken: str = ...
     ) -> GetServiceGraphResultTypeDef:
         """
         Retrieves a document that describes services that process incoming requests, and
         downstream services that they call as a result.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_service_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_service_graph)
         """
     async def get_time_series_service_statistics(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
         NextToken: str = ...
     ) -> GetTimeSeriesServiceStatisticsResultTypeDef:
@@ -336,16 +336,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Client.get_trace_graph)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/client/#get_trace_graph)
         """
     async def get_trace_summaries(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
         NextToken: str = ...
     ) -> GetTraceSummariesResultTypeDef:
         """
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/literals.py` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/literals.pyi` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/paginator.py` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
         get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
         get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
         list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
         list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import TimeRangeTypeType
 from .type_defs import (
     BatchGetTracesResultTypeDef,
@@ -54,14 +53,15 @@
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     SamplingStrategyTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "BatchGetTracesPaginator",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
@@ -87,60 +87,60 @@
 class BatchGetTracesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#batchgettracespaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[BatchGetTracesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#batchgettracespaginator)
         """
 
 
 class GetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getgroupspaginator)
         """
 
 
 class GetSamplingRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSamplingRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingrulespaginator)
         """
 
 
 class GetSamplingStatisticSummariesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingstatisticsummariespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSamplingStatisticSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingstatisticsummariespaginator)
         """
 
 
@@ -149,19 +149,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getservicegraphpaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getservicegraphpaginator)
         """
 
 
@@ -170,37 +170,37 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettimeseriesservicestatisticspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 
 class GetTraceGraphPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracegraphpaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTraceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracegraphpaginator)
         """
 
 
@@ -209,49 +209,49 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracesummariespaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracesummariespaginator)
         """
 
 
 class ListResourcePoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcePoliciesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listresourcepoliciespaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/paginator.pyi` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         get_time_series_service_statistics_paginator: GetTimeSeriesServiceStatisticsPaginator = client.get_paginator("get_time_series_service_statistics")
         get_trace_graph_paginator: GetTraceGraphPaginator = client.get_paginator("get_trace_graph")
         get_trace_summaries_paginator: GetTraceSummariesPaginator = client.get_paginator("get_trace_summaries")
         list_resource_policies_paginator: ListResourcePoliciesPaginator = client.get_paginator("list_resource_policies")
         list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import TimeRangeTypeType
 from .type_defs import (
     BatchGetTracesResultTypeDef,
@@ -54,14 +53,15 @@
     GetTimeSeriesServiceStatisticsResultTypeDef,
     GetTraceGraphResultTypeDef,
     GetTraceSummariesResultTypeDef,
     ListResourcePoliciesResultTypeDef,
     ListTagsForResourceResponseTypeDef,
     PaginatorConfigTypeDef,
     SamplingStrategyTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "BatchGetTracesPaginator",
     "GetGroupsPaginator",
     "GetSamplingRulesPaginator",
     "GetSamplingStatisticSummariesPaginator",
@@ -84,57 +84,57 @@
 class BatchGetTracesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#batchgettracespaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[BatchGetTracesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.BatchGetTraces.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#batchgettracespaginator)
         """
 
 class GetGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getgroupspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetGroupsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getgroupspaginator)
         """
 
 class GetSamplingRulesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingrulespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSamplingRulesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingrulespaginator)
         """
 
 class GetSamplingStatisticSummariesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingstatisticsummariespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSamplingStatisticSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetSamplingStatisticSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getsamplingstatisticsummariespaginator)
         """
 
 class GetServiceGraphPaginator(AioPaginator):
@@ -142,19 +142,19 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getservicegraphpaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetServiceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetServiceGraph.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#getservicegraphpaginator)
         """
 
 class GetTimeSeriesServiceStatisticsPaginator(AioPaginator):
@@ -162,36 +162,36 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettimeseriesservicestatisticspaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         GroupName: str = ...,
         GroupARN: str = ...,
         EntitySelectorExpression: str = ...,
         Period: int = ...,
         ForecastStatistics: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTimeSeriesServiceStatisticsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTimeSeriesServiceStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettimeseriesservicestatisticspaginator)
         """
 
 class GetTraceGraphPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracegraphpaginator)
     """
 
     def paginate(
-        self, *, TraceIds: Sequence[str], PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, TraceIds: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTraceGraphResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceGraph.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracegraphpaginator)
         """
 
 class GetTraceSummariesPaginator(AioPaginator):
@@ -199,47 +199,47 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracesummariespaginator)
     """
 
     def paginate(
         self,
         *,
-        StartTime: Union[datetime, str],
-        EndTime: Union[datetime, str],
+        StartTime: TimestampTypeDef,
+        EndTime: TimestampTypeDef,
         TimeRangeType: TimeRangeTypeType = ...,
         Sampling: bool = ...,
         SamplingStrategy: SamplingStrategyTypeDef = ...,
         FilterExpression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTraceSummariesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.GetTraceSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#gettracesummariespaginator)
         """
 
 class ListResourcePoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listresourcepoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcePoliciesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListResourcePolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listresourcepoliciespaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/type_defs.py` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_xray.type_defs import AliasTypeDef
 
-    data: AliasTypeDef = {...}
+    data: AliasTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -28,125 +28,127 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
-    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "BatchGetTracesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "InsightsConfigurationTypeDef",
     "TagTypeDef",
     "SamplingRuleTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSamplingRuleRequestRequestTypeDef",
     "ErrorStatisticsTypeDef",
     "FaultStatisticsTypeDef",
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
-    "GetInsightImpactGraphRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetInsightRequestRequestTypeDef",
-    "GetInsightSummariesRequestRequestTypeDef",
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
-    "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    "GetServiceGraphRequestRequestTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
+    "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
-    "TelemetryRecordTypeDef",
+    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
-    "SamplingRuleRecordTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
+    "GetInsightImpactGraphRequestRequestTypeDef",
+    "GetInsightSummariesRequestRequestTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    "GetServiceGraphRequestRequestTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    "SamplingStatisticsDocumentTypeDef",
+    "TelemetryRecordTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
-    "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
+    "SamplingRuleRecordTypeDef",
+    "SamplingRuleUnionTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
-    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
-    "CreateSamplingRuleResultTypeDef",
-    "DeleteSamplingRuleResultTypeDef",
-    "GetSamplingRulesResultTypeDef",
-    "UpdateSamplingRuleResultTypeDef",
     "EdgeTypeDef",
     "TimeSeriesServiceStatisticsTypeDef",
     "ErrorRootCauseServiceTypeDef",
     "FaultRootCauseServiceTypeDef",
+    "GetSamplingTargetsRequestRequestTypeDef",
+    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
+    "CreateSamplingRuleResultTypeDef",
+    "DeleteSamplingRuleResultTypeDef",
+    "GetSamplingRulesResultTypeDef",
+    "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
     "GetInsightEventsResultTypeDef",
     "GetInsightSummariesResultTypeDef",
     "GetInsightResultTypeDef",
     "ServiceTypeDef",
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     "ErrorRootCauseTypeDef",
@@ -205,56 +207,53 @@
         "HTTPCode5XXCount": int,
         "UnknownHostCount": int,
         "OtherCount": int,
     },
     total=False,
 )
 
-_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
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
 
-
-class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
-    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGetTracesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
 ):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
 
 InsightsConfigurationTypeDef = TypedDict(
     "InsightsConfigurationTypeDef",
     {
         "InsightsEnabled": bool,
         "NotificationsEnabled": bool,
     },
@@ -290,19 +289,17 @@
         "RuleName": str,
         "RuleARN": str,
         "Attributes": Mapping[str, str],
     },
     total=False,
 )
 
-
 class SamplingRuleTypeDef(_RequiredSamplingRuleTypeDef, _OptionalSamplingRuleTypeDef):
     pass
 
-
 DeleteGroupRequestRequestTypeDef = TypedDict(
     "DeleteGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
@@ -318,22 +315,20 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
-
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
-
 DeleteSamplingRuleRequestRequestTypeDef = TypedDict(
     "DeleteSamplingRuleRequestRequestTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
     },
     total=False,
@@ -400,22 +395,14 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
-GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetGroupsRequestRequestTypeDef = TypedDict(
     "GetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -431,103 +418,35 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetInsightEventsRequestRequestTypeDef(
     _RequiredGetInsightEventsRequestRequestTypeDef, _OptionalGetInsightEventsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "InsightId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetInsightImpactGraphRequestRequestTypeDef(
-    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
-    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 GetInsightRequestRequestTypeDef = TypedDict(
     "GetInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 
-_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightSummariesRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightSummariesRequestRequestTypeDef",
-    {
-        "States": Sequence[InsightStateType],
-        "GroupARN": str,
-        "GroupName": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetInsightSummariesRequestRequestTypeDef(
-    _RequiredGetInsightSummariesRequestRequestTypeDef,
-    _OptionalGetInsightSummariesRequestRequestTypeDef,
-):
-    pass
-
-
-GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingStatisticSummariesRequestRequestTypeDef = TypedDict(
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -540,39 +459,14 @@
         "RequestCount": int,
         "BorrowCount": int,
         "SampledCount": int,
     },
     total=False,
 )
 
-_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_RequiredSamplingStatisticsDocumentTypeDef",
-    {
-        "RuleName": str,
-        "ClientID": str,
-        "Timestamp": Union[datetime, str],
-        "RequestCount": int,
-        "SampledCount": int,
-    },
-)
-_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_OptionalSamplingStatisticsDocumentTypeDef",
-    {
-        "BorrowCount": int,
-    },
-    total=False,
-)
-
-
-class SamplingStatisticsDocumentTypeDef(
-    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
-):
-    pass
-
-
 SamplingTargetDocumentTypeDef = TypedDict(
     "SamplingTargetDocumentTypeDef",
     {
         "RuleName": str,
         "FixedRate": float,
         "ReservoirQuota": int,
         "ReservoirQuotaTTL": datetime,
@@ -587,162 +481,33 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetServiceGraphRequestRequestTypeDef(
-    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
-    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_OptionalGetTraceGraphRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTraceGraphRequestRequestTypeDef(
     _RequiredGetTraceGraphRequestRequestTypeDef, _OptionalGetTraceGraphRequestRequestTypeDef
 ):
     pass
 
-
 SamplingStrategyTypeDef = TypedDict(
     "SamplingStrategyTypeDef",
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
@@ -782,22 +547,14 @@
     "InstanceIdDetailTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourcePoliciesRequestRequestTypeDef = TypedDict(
     "ListResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -809,90 +566,54 @@
         "PolicyDocument": str,
         "PolicyRevisionId": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
 _OptionalPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_OptionalPutEncryptionConfigRequestRequestTypeDef",
     {
         "KeyId": str,
     },
     total=False,
 )
 
-
 class PutEncryptionConfigRequestRequestTypeDef(
     _RequiredPutEncryptionConfigRequestRequestTypeDef,
     _OptionalPutEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -901,21 +622,19 @@
     {
         "PolicyRevisionId": str,
         "BypassPolicyLockoutCheck": bool,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
 PutTraceSegmentsRequestRequestTypeDef = TypedDict(
     "PutTraceSegmentsRequestRequestTypeDef",
     {
         "TraceSegmentDocuments": Sequence[str],
     },
 )
 
@@ -933,35 +652,54 @@
     "ResourceARNDetailTypeDef",
     {
         "ARN": str,
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
 ResponseTimeRootCauseEntityTypeDef = TypedDict(
     "ResponseTimeRootCauseEntityTypeDef",
     {
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
     total=False,
 )
 
+_RequiredSamplingRuleOutputTypeDef = TypedDict(
+    "_RequiredSamplingRuleOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Priority": int,
+        "FixedRate": float,
+        "ReservoirSize": int,
+        "ServiceName": str,
+        "ServiceType": str,
+        "Host": str,
+        "HTTPMethod": str,
+        "URLPath": str,
+        "Version": int,
+    },
+)
+_OptionalSamplingRuleOutputTypeDef = TypedDict(
+    "_OptionalSamplingRuleOutputTypeDef",
+    {
+        "RuleName": str,
+        "RuleARN": str,
+        "Attributes": Dict[str, str],
+    },
+    total=False,
+)
+
+class SamplingRuleOutputTypeDef(
+    _RequiredSamplingRuleOutputTypeDef, _OptionalSamplingRuleOutputTypeDef
+):
+    pass
+
 SamplingRuleUpdateTypeDef = TypedDict(
     "SamplingRuleUpdateTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
         "ResourceARN": str,
         "Priority": int,
@@ -1016,36 +754,105 @@
     {
         "AnnotationValue": AnnotationValueTypeDef,
         "ServiceIds": List[ServiceIdTypeDef],
     },
     total=False,
 )
 
-_RequiredTelemetryRecordTypeDef = TypedDict(
-    "_RequiredTelemetryRecordTypeDef",
+_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
-        "Timestamp": Union[datetime, str],
+        "TraceIds": Sequence[str],
     },
 )
-_OptionalTelemetryRecordTypeDef = TypedDict(
-    "_OptionalTelemetryRecordTypeDef",
+_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
-        "SegmentsReceivedCount": int,
-        "SegmentsSentCount": int,
-        "SegmentsSpilloverCount": int,
-        "SegmentsRejectedCount": int,
-        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
+    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+):
+    pass
 
-class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
+GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
+    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+):
     pass
 
+ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
 
 GroupSummaryTypeDef = TypedDict(
     "GroupSummaryTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
@@ -1088,27 +895,25 @@
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1126,32 +931,20 @@
     "_OptionalCreateSamplingRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSamplingRuleRequestRequestTypeDef(
     _RequiredCreateSamplingRuleRequestRequestTypeDef,
     _OptionalCreateSamplingRuleRequestRequestTypeDef,
 ):
     pass
 
-
-SamplingRuleRecordTypeDef = TypedDict(
-    "SamplingRuleRecordTypeDef",
-    {
-        "SamplingRule": SamplingRuleTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-    },
-    total=False,
-)
-
 EdgeStatisticsTypeDef = TypedDict(
     "EdgeStatisticsTypeDef",
     {
         "OkCount": int,
         "ErrorStatistics": ErrorStatisticsTypeDef,
         "FaultStatistics": FaultStatisticsTypeDef,
         "TotalCount": int,
@@ -1172,23 +965,23 @@
     total=False,
 )
 
 GetEncryptionConfigResultTypeDef = TypedDict(
     "GetEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEncryptionConfigResultTypeDef = TypedDict(
     "PutEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseEntityTypeDef = TypedDict(
     "ErrorRootCauseEntityTypeDef",
     {
         "Name": str,
@@ -1204,93 +997,270 @@
         "Name": str,
         "Exceptions": List[RootCauseExceptionTypeDef],
         "Remote": bool,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesResultTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesResultTypeDef",
+_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
+    {
+        "InsightId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
     {
-        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-GetSamplingTargetsRequestRequestTypeDef = TypedDict(
-    "GetSamplingTargetsRequestRequestTypeDef",
+class GetInsightImpactGraphRequestRequestTypeDef(
+    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
+    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightSummariesRequestRequestTypeDef",
     {
-        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightSummariesRequestRequestTypeDef",
+    {
+        "States": Sequence[InsightStateType],
+        "GroupARN": str,
+        "GroupName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class GetInsightSummariesRequestRequestTypeDef(
+    _RequiredGetInsightSummariesRequestRequestTypeDef,
+    _OptionalGetInsightSummariesRequestRequestTypeDef,
+):
+    pass
+
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class GetServiceGraphRequestRequestTypeDef(
+    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
+):
+    pass
+
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+):
+    pass
+
+_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_RequiredSamplingStatisticsDocumentTypeDef",
+    {
+        "RuleName": str,
+        "ClientID": str,
+        "Timestamp": TimestampTypeDef,
+        "RequestCount": int,
+        "SampledCount": int,
+    },
+)
+_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_OptionalSamplingStatisticsDocumentTypeDef",
+    {
+        "BorrowCount": int,
+    },
+    total=False,
+)
+
+class SamplingStatisticsDocumentTypeDef(
+    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
+):
+    pass
+
+_RequiredTelemetryRecordTypeDef = TypedDict(
+    "_RequiredTelemetryRecordTypeDef",
+    {
+        "Timestamp": TimestampTypeDef,
+    },
+)
+_OptionalTelemetryRecordTypeDef = TypedDict(
+    "_OptionalTelemetryRecordTypeDef",
+    {
+        "SegmentsReceivedCount": int,
+        "SegmentsSentCount": int,
+        "SegmentsSpilloverCount": int,
+        "SegmentsRejectedCount": int,
+        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
+    },
+    total=False,
+)
+
+class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
+    pass
+
+GetSamplingStatisticSummariesResultTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesResultTypeDef",
+    {
+        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
         "LastRuleModification": datetime,
         "UnprocessedStatistics": List[UnprocessedStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestRequestTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
-
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1301,31 +1271,31 @@
 )
 
 ListResourcePoliciesResultTypeDef = TypedDict(
     "ListResourcePoliciesResultTypeDef",
     {
         "ResourcePolicies": List[ResourcePolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResultTypeDef = TypedDict(
     "PutResourcePolicyResultTypeDef",
     {
         "ResourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseServiceTypeDef = TypedDict(
     "ResponseTimeRootCauseServiceTypeDef",
     {
         "Name": str,
@@ -1334,14 +1304,25 @@
         "AccountId": str,
         "EntityPath": List[ResponseTimeRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+SamplingRuleRecordTypeDef = TypedDict(
+    "SamplingRuleRecordTypeDef",
+    {
+        "SamplingRule": SamplingRuleOutputTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+    },
+    total=False,
+)
+
+SamplingRuleUnionTypeDef = Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef]
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1403,101 +1384,44 @@
         "ClientRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "RootCauseServiceRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "TopAnomalousServices": List[AnomalousServiceTypeDef],
     },
     total=False,
 )
 
-_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
-    },
-)
-_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "EC2InstanceId": str,
-        "Hostname": str,
-        "ResourceARN": str,
-    },
-    total=False,
-)
-
-
-class PutTelemetryRecordsRequestRequestTypeDef(
-    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
-    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
-):
-    pass
-
-
 GetGroupsResultTypeDef = TypedDict(
     "GetGroupsResultTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupResultTypeDef = TypedDict(
     "CreateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResultTypeDef = TypedDict(
     "GetGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupResultTypeDef = TypedDict(
     "UpdateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSamplingRuleResultTypeDef = TypedDict(
-    "CreateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSamplingRuleResultTypeDef = TypedDict(
-    "DeleteSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSamplingRulesResultTypeDef = TypedDict(
-    "GetSamplingRulesResultTypeDef",
-    {
-        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSamplingRuleResultTypeDef = TypedDict(
-    "UpdateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
@@ -1546,70 +1470,132 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+GetSamplingTargetsRequestRequestTypeDef = TypedDict(
+    "GetSamplingTargetsRequestRequestTypeDef",
+    {
+        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+    },
+)
+
+_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
+    },
+)
+_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "EC2InstanceId": str,
+        "Hostname": str,
+        "ResourceARN": str,
+    },
+    total=False,
+)
+
+class PutTelemetryRecordsRequestRequestTypeDef(
+    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
+    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
+):
+    pass
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
         "ServiceGraphEndTime": datetime,
         "Services": List[InsightImpactGraphServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseTypeDef = TypedDict(
     "ResponseTimeRootCauseTypeDef",
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
         "ClientImpacting": bool,
     },
     total=False,
 )
 
+CreateSamplingRuleResultTypeDef = TypedDict(
+    "CreateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSamplingRuleResultTypeDef = TypedDict(
+    "DeleteSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSamplingRulesResultTypeDef = TypedDict(
+    "GetSamplingRulesResultTypeDef",
+    {
+        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSamplingRuleResultTypeDef = TypedDict(
+    "UpdateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightEventsResultTypeDef = TypedDict(
     "GetInsightEventsResultTypeDef",
     {
         "InsightEvents": List[InsightEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightSummariesResultTypeDef = TypedDict(
     "GetInsightSummariesResultTypeDef",
     {
         "InsightSummaries": List[InsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightResultTypeDef = TypedDict(
     "GetInsightResultTypeDef",
     {
         "Insight": InsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "ReferenceId": int,
@@ -1631,15 +1617,15 @@
 
 GetTimeSeriesServiceStatisticsResultTypeDef = TypedDict(
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     {
         "TimeSeriesServiceStatistics": List[TimeSeriesServiceStatisticsTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseTypeDef = TypedDict(
     "ErrorRootCauseTypeDef",
     {
         "Services": List[ErrorRootCauseServiceTypeDef],
@@ -1661,24 +1647,24 @@
     "GetServiceGraphResultTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
         "Services": List[ServiceTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTraceGraphResultTypeDef = TypedDict(
     "GetTraceGraphResultTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TraceSummaryTypeDef = TypedDict(
     "TraceSummaryTypeDef",
     {
         "Id": str,
@@ -1708,10 +1694,10 @@
 GetTraceSummariesResultTypeDef = TypedDict(
     "GetTraceSummariesResultTypeDef",
     {
         "TraceSummaries": List[TraceSummaryTypeDef],
         "ApproximateTime": datetime,
         "TracesProcessedCount": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray/type_defs.pyi` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_xray.type_defs import AliasTypeDef
 
-    data: AliasTypeDef = {...}
+    data: AliasTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -28,124 +28,128 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AliasTypeDef",
     "AnnotationValueTypeDef",
     "ServiceIdTypeDef",
     "AvailabilityZoneDetailTypeDef",
     "BackendConnectionErrorsTypeDef",
-    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "BatchGetTracesRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "InsightsConfigurationTypeDef",
     "TagTypeDef",
     "SamplingRuleTypeDef",
     "DeleteGroupRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSamplingRuleRequestRequestTypeDef",
     "ErrorStatisticsTypeDef",
     "FaultStatisticsTypeDef",
     "HistogramEntryTypeDef",
     "EncryptionConfigTypeDef",
     "RootCauseExceptionTypeDef",
     "ForecastStatisticsTypeDef",
     "GetGroupRequestRequestTypeDef",
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
     "GetGroupsRequestRequestTypeDef",
     "GetInsightEventsRequestRequestTypeDef",
-    "GetInsightImpactGraphRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetInsightRequestRequestTypeDef",
-    "GetInsightSummariesRequestRequestTypeDef",
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
     "GetSamplingRulesRequestRequestTypeDef",
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     "SamplingStatisticSummaryTypeDef",
-    "SamplingStatisticsDocumentTypeDef",
     "SamplingTargetDocumentTypeDef",
     "UnprocessedStatisticsTypeDef",
-    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    "GetServiceGraphRequestRequestTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
     "GetTraceGraphRequestRequestTypeDef",
     "SamplingStrategyTypeDef",
     "HttpTypeDef",
     "RequestImpactStatisticsTypeDef",
     "InsightImpactGraphEdgeTypeDef",
     "InstanceIdDetailTypeDef",
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
     "ListResourcePoliciesRequestRequestTypeDef",
     "ResourcePolicyTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutEncryptionConfigRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "PutTraceSegmentsRequestRequestTypeDef",
     "UnprocessedTraceSegmentTypeDef",
     "ResourceARNDetailTypeDef",
-    "ResponseMetadataTypeDef",
     "ResponseTimeRootCauseEntityTypeDef",
+    "SamplingRuleOutputTypeDef",
     "SamplingRuleUpdateTypeDef",
     "SegmentTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AnomalousServiceTypeDef",
     "TraceUserTypeDef",
     "ValueWithServiceIdsTypeDef",
-    "TelemetryRecordTypeDef",
+    "BatchGetTracesRequestBatchGetTracesPaginateTypeDef",
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    "GetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "GroupSummaryTypeDef",
     "GroupTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSamplingRuleRequestRequestTypeDef",
-    "SamplingRuleRecordTypeDef",
     "EdgeStatisticsTypeDef",
     "ServiceStatisticsTypeDef",
     "GetEncryptionConfigResultTypeDef",
     "PutEncryptionConfigResultTypeDef",
     "ErrorRootCauseEntityTypeDef",
     "FaultRootCauseEntityTypeDef",
+    "GetInsightImpactGraphRequestRequestTypeDef",
+    "GetInsightSummariesRequestRequestTypeDef",
+    "GetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    "GetServiceGraphRequestRequestTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    "GetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    "SamplingStatisticsDocumentTypeDef",
+    "TelemetryRecordTypeDef",
     "GetSamplingStatisticSummariesResultTypeDef",
-    "GetSamplingTargetsRequestRequestTypeDef",
     "GetSamplingTargetsResultTypeDef",
     "GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     "GetTraceSummariesRequestRequestTypeDef",
     "InsightImpactGraphServiceTypeDef",
     "ListResourcePoliciesResultTypeDef",
     "PutResourcePolicyResultTypeDef",
     "PutTraceSegmentsResultTypeDef",
     "ResponseTimeRootCauseServiceTypeDef",
+    "SamplingRuleRecordTypeDef",
+    "SamplingRuleUnionTypeDef",
     "UpdateSamplingRuleRequestRequestTypeDef",
     "TraceTypeDef",
     "InsightEventTypeDef",
     "InsightSummaryTypeDef",
     "InsightTypeDef",
-    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetGroupsResultTypeDef",
     "CreateGroupResultTypeDef",
     "GetGroupResultTypeDef",
     "UpdateGroupResultTypeDef",
-    "CreateSamplingRuleResultTypeDef",
-    "DeleteSamplingRuleResultTypeDef",
-    "GetSamplingRulesResultTypeDef",
-    "UpdateSamplingRuleResultTypeDef",
     "EdgeTypeDef",
     "TimeSeriesServiceStatisticsTypeDef",
     "ErrorRootCauseServiceTypeDef",
     "FaultRootCauseServiceTypeDef",
+    "GetSamplingTargetsRequestRequestTypeDef",
+    "PutTelemetryRecordsRequestRequestTypeDef",
     "GetInsightImpactGraphResultTypeDef",
     "ResponseTimeRootCauseTypeDef",
+    "CreateSamplingRuleResultTypeDef",
+    "DeleteSamplingRuleResultTypeDef",
+    "GetSamplingRulesResultTypeDef",
+    "UpdateSamplingRuleResultTypeDef",
     "BatchGetTracesResultTypeDef",
     "GetInsightEventsResultTypeDef",
     "GetInsightSummariesResultTypeDef",
     "GetInsightResultTypeDef",
     "ServiceTypeDef",
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     "ErrorRootCauseTypeDef",
@@ -204,53 +208,56 @@
         "HTTPCode5XXCount": int,
         "UnknownHostCount": int,
         "OtherCount": int,
     },
     total=False,
 )
 
-_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
-    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
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
 
-class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
-    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
-):
-    pass
-
 _RequiredBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_RequiredBatchGetTracesRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalBatchGetTracesRequestRequestTypeDef = TypedDict(
     "_OptionalBatchGetTracesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class BatchGetTracesRequestRequestTypeDef(
     _RequiredBatchGetTracesRequestRequestTypeDef, _OptionalBatchGetTracesRequestRequestTypeDef
 ):
     pass
 
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 InsightsConfigurationTypeDef = TypedDict(
     "InsightsConfigurationTypeDef",
     {
         "InsightsEnabled": bool,
         "NotificationsEnabled": bool,
     },
     total=False,
@@ -285,17 +292,19 @@
         "RuleName": str,
         "RuleARN": str,
         "Attributes": Mapping[str, str],
     },
     total=False,
 )
 
+
 class SamplingRuleTypeDef(_RequiredSamplingRuleTypeDef, _OptionalSamplingRuleTypeDef):
     pass
 
+
 DeleteGroupRequestRequestTypeDef = TypedDict(
     "DeleteGroupRequestRequestTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
@@ -311,20 +320,22 @@
     "_OptionalDeleteResourcePolicyRequestRequestTypeDef",
     {
         "PolicyRevisionId": str,
     },
     total=False,
 )
 
+
 class DeleteResourcePolicyRequestRequestTypeDef(
     _RequiredDeleteResourcePolicyRequestRequestTypeDef,
     _OptionalDeleteResourcePolicyRequestRequestTypeDef,
 ):
     pass
 
+
 DeleteSamplingRuleRequestRequestTypeDef = TypedDict(
     "DeleteSamplingRuleRequestRequestTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
     },
     total=False,
@@ -391,22 +402,14 @@
     {
         "GroupName": str,
         "GroupARN": str,
     },
     total=False,
 )
 
-GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
-    "GetGroupsRequestGetGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetGroupsRequestRequestTypeDef = TypedDict(
     "GetGroupsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -422,97 +425,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetInsightEventsRequestRequestTypeDef(
     _RequiredGetInsightEventsRequestRequestTypeDef, _OptionalGetInsightEventsRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "InsightId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
-    {
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetInsightImpactGraphRequestRequestTypeDef(
-    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
-    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
-):
-    pass
 
+TimestampTypeDef = Union[datetime, str]
 GetInsightRequestRequestTypeDef = TypedDict(
     "GetInsightRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 
-_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetInsightSummariesRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetInsightSummariesRequestRequestTypeDef",
-    {
-        "States": Sequence[InsightStateType],
-        "GroupARN": str,
-        "GroupName": str,
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetInsightSummariesRequestRequestTypeDef(
-    _RequiredGetInsightSummariesRequestRequestTypeDef,
-    _OptionalGetInsightSummariesRequestRequestTypeDef,
-):
-    pass
-
-GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
-    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingRulesRequestRequestTypeDef = TypedDict(
     "GetSamplingRulesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetSamplingStatisticSummariesRequestRequestTypeDef = TypedDict(
     "GetSamplingStatisticSummariesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -525,37 +468,14 @@
         "RequestCount": int,
         "BorrowCount": int,
         "SampledCount": int,
     },
     total=False,
 )
 
-_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_RequiredSamplingStatisticsDocumentTypeDef",
-    {
-        "RuleName": str,
-        "ClientID": str,
-        "Timestamp": Union[datetime, str],
-        "RequestCount": int,
-        "SampledCount": int,
-    },
-)
-_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
-    "_OptionalSamplingStatisticsDocumentTypeDef",
-    {
-        "BorrowCount": int,
-    },
-    total=False,
-)
-
-class SamplingStatisticsDocumentTypeDef(
-    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
-):
-    pass
-
 SamplingTargetDocumentTypeDef = TypedDict(
     "SamplingTargetDocumentTypeDef",
     {
         "RuleName": str,
         "FixedRate": float,
         "ReservoirQuota": int,
         "ReservoirQuotaTTL": datetime,
@@ -570,150 +490,35 @@
         "RuleName": str,
         "ErrorCode": str,
         "Message": str,
     },
     total=False,
 )
 
-_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
-    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-):
-    pass
-
-_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_RequiredGetServiceGraphRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
-    "_OptionalGetServiceGraphRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetServiceGraphRequestRequestTypeDef(
-    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
-):
-    pass
-
-_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-):
-    pass
-
-_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-)
-_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
-    {
-        "GroupName": str,
-        "GroupARN": str,
-        "EntitySelectorExpression": str,
-        "Period": int,
-        "ForecastStatistics": bool,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
-    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-):
-    pass
-
-_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "TraceIds": Sequence[str],
-    },
-)
-_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
-    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
-    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceGraphRequestRequestTypeDef",
     {
         "TraceIds": Sequence[str],
     },
 )
 _OptionalGetTraceGraphRequestRequestTypeDef = TypedDict(
     "_OptionalGetTraceGraphRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTraceGraphRequestRequestTypeDef(
     _RequiredGetTraceGraphRequestRequestTypeDef, _OptionalGetTraceGraphRequestRequestTypeDef
 ):
     pass
 
+
 SamplingStrategyTypeDef = TypedDict(
     "SamplingStrategyTypeDef",
     {
         "Name": SamplingStrategyNameType,
         "Value": float,
     },
     total=False,
@@ -753,22 +558,14 @@
     "InstanceIdDetailTypeDef",
     {
         "Id": str,
     },
     total=False,
 )
 
-ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
-    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListResourcePoliciesRequestRequestTypeDef = TypedDict(
     "ListResourcePoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -780,63 +577,35 @@
         "PolicyDocument": str,
         "PolicyRevisionId": str,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_OptionalListTagsForResourceRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 
 _RequiredPutEncryptionConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutEncryptionConfigRequestRequestTypeDef",
     {
         "Type": EncryptionTypeType,
     },
 )
@@ -844,20 +613,22 @@
     "_OptionalPutEncryptionConfigRequestRequestTypeDef",
     {
         "KeyId": str,
     },
     total=False,
 )
 
+
 class PutEncryptionConfigRequestRequestTypeDef(
     _RequiredPutEncryptionConfigRequestRequestTypeDef,
     _OptionalPutEncryptionConfigRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyName": str,
         "PolicyDocument": str,
     },
 )
@@ -866,19 +637,21 @@
     {
         "PolicyRevisionId": str,
         "BypassPolicyLockoutCheck": bool,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
+
 PutTraceSegmentsRequestRequestTypeDef = TypedDict(
     "PutTraceSegmentsRequestRequestTypeDef",
     {
         "TraceSegmentDocuments": Sequence[str],
     },
 )
 
@@ -896,35 +669,56 @@
     "ResourceARNDetailTypeDef",
     {
         "ARN": str,
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
 ResponseTimeRootCauseEntityTypeDef = TypedDict(
     "ResponseTimeRootCauseEntityTypeDef",
     {
         "Name": str,
         "Coverage": float,
         "Remote": bool,
     },
     total=False,
 )
 
+_RequiredSamplingRuleOutputTypeDef = TypedDict(
+    "_RequiredSamplingRuleOutputTypeDef",
+    {
+        "ResourceARN": str,
+        "Priority": int,
+        "FixedRate": float,
+        "ReservoirSize": int,
+        "ServiceName": str,
+        "ServiceType": str,
+        "Host": str,
+        "HTTPMethod": str,
+        "URLPath": str,
+        "Version": int,
+    },
+)
+_OptionalSamplingRuleOutputTypeDef = TypedDict(
+    "_OptionalSamplingRuleOutputTypeDef",
+    {
+        "RuleName": str,
+        "RuleARN": str,
+        "Attributes": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class SamplingRuleOutputTypeDef(
+    _RequiredSamplingRuleOutputTypeDef, _OptionalSamplingRuleOutputTypeDef
+):
+    pass
+
+
 SamplingRuleUpdateTypeDef = TypedDict(
     "SamplingRuleUpdateTypeDef",
     {
         "RuleName": str,
         "RuleARN": str,
         "ResourceARN": str,
         "Priority": int,
@@ -979,35 +773,112 @@
     {
         "AnnotationValue": AnnotationValueTypeDef,
         "ServiceIds": List[ServiceIdTypeDef],
     },
     total=False,
 )
 
-_RequiredTelemetryRecordTypeDef = TypedDict(
-    "_RequiredTelemetryRecordTypeDef",
+_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
-        "Timestamp": Union[datetime, str],
+        "TraceIds": Sequence[str],
     },
 )
-_OptionalTelemetryRecordTypeDef = TypedDict(
-    "_OptionalTelemetryRecordTypeDef",
+_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef = TypedDict(
+    "_OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef",
     {
-        "SegmentsReceivedCount": int,
-        "SegmentsSentCount": int,
-        "SegmentsSpilloverCount": int,
-        "SegmentsRejectedCount": int,
-        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
+
+class BatchGetTracesRequestBatchGetTracesPaginateTypeDef(
+    _RequiredBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    _OptionalBatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+):
     pass
 
+
+GetGroupsRequestGetGroupsPaginateTypeDef = TypedDict(
+    "GetGroupsRequestGetGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef = TypedDict(
+    "GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "TraceIds": Sequence[str],
+    },
+)
+_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTraceGraphRequestGetTraceGraphPaginateTypeDef(
+    _RequiredGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    _OptionalGetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+):
+    pass
+
+
+ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef = TypedDict(
+    "ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 GroupSummaryTypeDef = TypedDict(
     "GroupSummaryTypeDef",
     {
         "GroupName": str,
         "GroupARN": str,
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
@@ -1049,25 +920,27 @@
         "FilterExpression": str,
         "InsightsConfiguration": InsightsConfigurationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateGroupRequestRequestTypeDef(
     _RequiredCreateGroupRequestRequestTypeDef, _OptionalCreateGroupRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1085,29 +958,21 @@
     "_OptionalCreateSamplingRuleRequestRequestTypeDef",
     {
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSamplingRuleRequestRequestTypeDef(
     _RequiredCreateSamplingRuleRequestRequestTypeDef,
     _OptionalCreateSamplingRuleRequestRequestTypeDef,
 ):
     pass
 
-SamplingRuleRecordTypeDef = TypedDict(
-    "SamplingRuleRecordTypeDef",
-    {
-        "SamplingRule": SamplingRuleTypeDef,
-        "CreatedAt": datetime,
-        "ModifiedAt": datetime,
-    },
-    total=False,
-)
 
 EdgeStatisticsTypeDef = TypedDict(
     "EdgeStatisticsTypeDef",
     {
         "OkCount": int,
         "ErrorStatistics": ErrorStatisticsTypeDef,
         "FaultStatistics": FaultStatisticsTypeDef,
@@ -1129,23 +994,23 @@
     total=False,
 )
 
 GetEncryptionConfigResultTypeDef = TypedDict(
     "GetEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutEncryptionConfigResultTypeDef = TypedDict(
     "PutEncryptionConfigResultTypeDef",
     {
         "EncryptionConfig": EncryptionConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseEntityTypeDef = TypedDict(
     "ErrorRootCauseEntityTypeDef",
     {
         "Name": str,
@@ -1161,89 +1026,290 @@
         "Name": str,
         "Exceptions": List[RootCauseExceptionTypeDef],
         "Remote": bool,
     },
     total=False,
 )
 
-GetSamplingStatisticSummariesResultTypeDef = TypedDict(
-    "GetSamplingStatisticSummariesResultTypeDef",
+_RequiredGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightImpactGraphRequestRequestTypeDef",
+    {
+        "InsightId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightImpactGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightImpactGraphRequestRequestTypeDef",
     {
-        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
     },
+    total=False,
 )
 
-GetSamplingTargetsRequestRequestTypeDef = TypedDict(
-    "GetSamplingTargetsRequestRequestTypeDef",
+
+class GetInsightImpactGraphRequestRequestTypeDef(
+    _RequiredGetInsightImpactGraphRequestRequestTypeDef,
+    _OptionalGetInsightImpactGraphRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetInsightSummariesRequestRequestTypeDef",
     {
-        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetInsightSummariesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetInsightSummariesRequestRequestTypeDef",
+    {
+        "States": Sequence[InsightStateType],
+        "GroupARN": str,
+        "GroupName": str,
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class GetInsightSummariesRequestRequestTypeDef(
+    _RequiredGetInsightSummariesRequestRequestTypeDef,
+    _OptionalGetInsightSummariesRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetServiceGraphRequestGetServiceGraphPaginateTypeDef(
+    _RequiredGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    _OptionalGetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_RequiredGetServiceGraphRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetServiceGraphRequestRequestTypeDef = TypedDict(
+    "_OptionalGetServiceGraphRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class GetServiceGraphRequestRequestTypeDef(
+    _RequiredGetServiceGraphRequestRequestTypeDef, _OptionalGetServiceGraphRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+)
+_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef",
+    {
+        "GroupName": str,
+        "GroupARN": str,
+        "EntitySelectorExpression": str,
+        "Period": int,
+        "ForecastStatistics": bool,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class GetTimeSeriesServiceStatisticsRequestRequestTypeDef(
+    _RequiredGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    _OptionalGetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_RequiredSamplingStatisticsDocumentTypeDef",
+    {
+        "RuleName": str,
+        "ClientID": str,
+        "Timestamp": TimestampTypeDef,
+        "RequestCount": int,
+        "SampledCount": int,
+    },
+)
+_OptionalSamplingStatisticsDocumentTypeDef = TypedDict(
+    "_OptionalSamplingStatisticsDocumentTypeDef",
+    {
+        "BorrowCount": int,
+    },
+    total=False,
+)
+
+
+class SamplingStatisticsDocumentTypeDef(
+    _RequiredSamplingStatisticsDocumentTypeDef, _OptionalSamplingStatisticsDocumentTypeDef
+):
+    pass
+
+
+_RequiredTelemetryRecordTypeDef = TypedDict(
+    "_RequiredTelemetryRecordTypeDef",
+    {
+        "Timestamp": TimestampTypeDef,
+    },
+)
+_OptionalTelemetryRecordTypeDef = TypedDict(
+    "_OptionalTelemetryRecordTypeDef",
+    {
+        "SegmentsReceivedCount": int,
+        "SegmentsSentCount": int,
+        "SegmentsSpilloverCount": int,
+        "SegmentsRejectedCount": int,
+        "BackendConnectionErrors": BackendConnectionErrorsTypeDef,
+    },
+    total=False,
+)
+
+
+class TelemetryRecordTypeDef(_RequiredTelemetryRecordTypeDef, _OptionalTelemetryRecordTypeDef):
+    pass
+
+
+GetSamplingStatisticSummariesResultTypeDef = TypedDict(
+    "GetSamplingStatisticSummariesResultTypeDef",
+    {
+        "SamplingStatisticSummaries": List[SamplingStatisticSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSamplingTargetsResultTypeDef = TypedDict(
     "GetSamplingTargetsResultTypeDef",
     {
         "SamplingTargetDocuments": List[SamplingTargetDocumentTypeDef],
         "LastRuleModification": datetime,
         "UnprocessedStatistics": List[UnprocessedStatisticsTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef(
     _RequiredGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     _OptionalGetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_RequiredGetTraceSummariesRequestRequestTypeDef",
     {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
 )
 _OptionalGetTraceSummariesRequestRequestTypeDef = TypedDict(
     "_OptionalGetTraceSummariesRequestRequestTypeDef",
     {
         "TimeRangeType": TimeRangeTypeType,
         "Sampling": bool,
         "SamplingStrategy": SamplingStrategyTypeDef,
         "FilterExpression": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTraceSummariesRequestRequestTypeDef(
     _RequiredGetTraceSummariesRequestRequestTypeDef, _OptionalGetTraceSummariesRequestRequestTypeDef
 ):
     pass
 
+
 InsightImpactGraphServiceTypeDef = TypedDict(
     "InsightImpactGraphServiceTypeDef",
     {
         "ReferenceId": int,
         "Type": str,
         "Name": str,
         "Names": List[str],
@@ -1254,31 +1320,31 @@
 )
 
 ListResourcePoliciesResultTypeDef = TypedDict(
     "ListResourcePoliciesResultTypeDef",
     {
         "ResourcePolicies": List[ResourcePolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourcePolicyResultTypeDef = TypedDict(
     "PutResourcePolicyResultTypeDef",
     {
         "ResourcePolicy": ResourcePolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutTraceSegmentsResultTypeDef = TypedDict(
     "PutTraceSegmentsResultTypeDef",
     {
         "UnprocessedTraceSegments": List[UnprocessedTraceSegmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseServiceTypeDef = TypedDict(
     "ResponseTimeRootCauseServiceTypeDef",
     {
         "Name": str,
@@ -1287,14 +1353,25 @@
         "AccountId": str,
         "EntityPath": List[ResponseTimeRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+SamplingRuleRecordTypeDef = TypedDict(
+    "SamplingRuleRecordTypeDef",
+    {
+        "SamplingRule": SamplingRuleOutputTypeDef,
+        "CreatedAt": datetime,
+        "ModifiedAt": datetime,
+    },
+    total=False,
+)
+
+SamplingRuleUnionTypeDef = Union[SamplingRuleTypeDef, SamplingRuleOutputTypeDef]
 UpdateSamplingRuleRequestRequestTypeDef = TypedDict(
     "UpdateSamplingRuleRequestRequestTypeDef",
     {
         "SamplingRuleUpdate": SamplingRuleUpdateTypeDef,
     },
 )
 
@@ -1356,99 +1433,44 @@
         "ClientRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "RootCauseServiceRequestImpactStatistics": RequestImpactStatisticsTypeDef,
         "TopAnomalousServices": List[AnomalousServiceTypeDef],
     },
     total=False,
 )
 
-_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
-    },
-)
-_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
-    {
-        "EC2InstanceId": str,
-        "Hostname": str,
-        "ResourceARN": str,
-    },
-    total=False,
-)
-
-class PutTelemetryRecordsRequestRequestTypeDef(
-    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
-    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
-):
-    pass
-
 GetGroupsResultTypeDef = TypedDict(
     "GetGroupsResultTypeDef",
     {
         "Groups": List[GroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupResultTypeDef = TypedDict(
     "CreateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResultTypeDef = TypedDict(
     "GetGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupResultTypeDef = TypedDict(
     "UpdateGroupResultTypeDef",
     {
         "Group": GroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSamplingRuleResultTypeDef = TypedDict(
-    "CreateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DeleteSamplingRuleResultTypeDef = TypedDict(
-    "DeleteSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetSamplingRulesResultTypeDef = TypedDict(
-    "GetSamplingRulesResultTypeDef",
-    {
-        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateSamplingRuleResultTypeDef = TypedDict(
-    "UpdateSamplingRuleResultTypeDef",
-    {
-        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EdgeTypeDef = TypedDict(
     "EdgeTypeDef",
     {
         "ReferenceId": int,
@@ -1497,70 +1519,134 @@
         "AccountId": str,
         "EntityPath": List[FaultRootCauseEntityTypeDef],
         "Inferred": bool,
     },
     total=False,
 )
 
+GetSamplingTargetsRequestRequestTypeDef = TypedDict(
+    "GetSamplingTargetsRequestRequestTypeDef",
+    {
+        "SamplingStatisticsDocuments": Sequence[SamplingStatisticsDocumentTypeDef],
+    },
+)
+
+_RequiredPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "TelemetryRecords": Sequence[TelemetryRecordTypeDef],
+    },
+)
+_OptionalPutTelemetryRecordsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutTelemetryRecordsRequestRequestTypeDef",
+    {
+        "EC2InstanceId": str,
+        "Hostname": str,
+        "ResourceARN": str,
+    },
+    total=False,
+)
+
+
+class PutTelemetryRecordsRequestRequestTypeDef(
+    _RequiredPutTelemetryRecordsRequestRequestTypeDef,
+    _OptionalPutTelemetryRecordsRequestRequestTypeDef,
+):
+    pass
+
+
 GetInsightImpactGraphResultTypeDef = TypedDict(
     "GetInsightImpactGraphResultTypeDef",
     {
         "InsightId": str,
         "StartTime": datetime,
         "EndTime": datetime,
         "ServiceGraphStartTime": datetime,
         "ServiceGraphEndTime": datetime,
         "Services": List[InsightImpactGraphServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResponseTimeRootCauseTypeDef = TypedDict(
     "ResponseTimeRootCauseTypeDef",
     {
         "Services": List[ResponseTimeRootCauseServiceTypeDef],
         "ClientImpacting": bool,
     },
     total=False,
 )
 
+CreateSamplingRuleResultTypeDef = TypedDict(
+    "CreateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteSamplingRuleResultTypeDef = TypedDict(
+    "DeleteSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSamplingRulesResultTypeDef = TypedDict(
+    "GetSamplingRulesResultTypeDef",
+    {
+        "SamplingRuleRecords": List[SamplingRuleRecordTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSamplingRuleResultTypeDef = TypedDict(
+    "UpdateSamplingRuleResultTypeDef",
+    {
+        "SamplingRuleRecord": SamplingRuleRecordTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 BatchGetTracesResultTypeDef = TypedDict(
     "BatchGetTracesResultTypeDef",
     {
         "Traces": List[TraceTypeDef],
         "UnprocessedTraceIds": List[str],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightEventsResultTypeDef = TypedDict(
     "GetInsightEventsResultTypeDef",
     {
         "InsightEvents": List[InsightEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightSummariesResultTypeDef = TypedDict(
     "GetInsightSummariesResultTypeDef",
     {
         "InsightSummaries": List[InsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetInsightResultTypeDef = TypedDict(
     "GetInsightResultTypeDef",
     {
         "Insight": InsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "ReferenceId": int,
@@ -1582,15 +1668,15 @@
 
 GetTimeSeriesServiceStatisticsResultTypeDef = TypedDict(
     "GetTimeSeriesServiceStatisticsResultTypeDef",
     {
         "TimeSeriesServiceStatistics": List[TimeSeriesServiceStatisticsTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorRootCauseTypeDef = TypedDict(
     "ErrorRootCauseTypeDef",
     {
         "Services": List[ErrorRootCauseServiceTypeDef],
@@ -1612,24 +1698,24 @@
     "GetServiceGraphResultTypeDef",
     {
         "StartTime": datetime,
         "EndTime": datetime,
         "Services": List[ServiceTypeDef],
         "ContainsOldGroupVersions": bool,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTraceGraphResultTypeDef = TypedDict(
     "GetTraceGraphResultTypeDef",
     {
         "Services": List[ServiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TraceSummaryTypeDef = TypedDict(
     "TraceSummaryTypeDef",
     {
         "Id": str,
@@ -1659,10 +1745,10 @@
 GetTraceSummariesResultTypeDef = TypedDict(
     "GetTraceSummariesResultTypeDef",
     {
         "TraceSummaries": List[TraceSummaryTypeDef],
         "ApproximateTime": datetime,
         "TracesProcessedCount": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/PKG-INFO` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-xray
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.XRay 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore xray type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore xray type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-xray"></a>
 
 # types-aiobotocore-xray
 
 [![PyPI - types-aiobotocore-xray](https://img.shields.io/pypi/v/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-xray.svg?color=blue)](https://pypi.org/project/types-aiobotocore-xray)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-xray?color=blue)](https://pypistats.org/packages/types-aiobotocore-xray)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-xray)](https://pepy.tech/project/types-aiobotocore-xray)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.XRay 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/xray.html#XRay)
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
 [types-aiobotocore-xray docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_xray/).
 
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
@@ -352,132 +351,135 @@
 )
 
 
 def check_value(value: BatchGetTracesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_xray.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_xray.type_defs import (
     AliasTypeDef,
     AnnotationValueTypeDef,
     ServiceIdTypeDef,
     AvailabilityZoneDetailTypeDef,
     BackendConnectionErrorsTypeDef,
-    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     BatchGetTracesRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     InsightsConfigurationTypeDef,
     TagTypeDef,
     SamplingRuleTypeDef,
     DeleteGroupRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSamplingRuleRequestRequestTypeDef,
     ErrorStatisticsTypeDef,
     FaultStatisticsTypeDef,
     HistogramEntryTypeDef,
     EncryptionConfigTypeDef,
     RootCauseExceptionTypeDef,
     ForecastStatisticsTypeDef,
     GetGroupRequestRequestTypeDef,
-    GetGroupsRequestGetGroupsPaginateTypeDef,
     GetGroupsRequestRequestTypeDef,
     GetInsightEventsRequestRequestTypeDef,
-    GetInsightImpactGraphRequestRequestTypeDef,
+    TimestampTypeDef,
     GetInsightRequestRequestTypeDef,
-    GetInsightSummariesRequestRequestTypeDef,
-    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
     GetSamplingRulesRequestRequestTypeDef,
-    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
     GetSamplingStatisticSummariesRequestRequestTypeDef,
     SamplingStatisticSummaryTypeDef,
-    SamplingStatisticsDocumentTypeDef,
     SamplingTargetDocumentTypeDef,
     UnprocessedStatisticsTypeDef,
-    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
-    GetServiceGraphRequestRequestTypeDef,
-    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
-    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
-    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
     GetTraceGraphRequestRequestTypeDef,
     SamplingStrategyTypeDef,
     HttpTypeDef,
     RequestImpactStatisticsTypeDef,
     InsightImpactGraphEdgeTypeDef,
     InstanceIdDetailTypeDef,
-    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
     ListResourcePoliciesRequestRequestTypeDef,
     ResourcePolicyTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutEncryptionConfigRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     PutTraceSegmentsRequestRequestTypeDef,
     UnprocessedTraceSegmentTypeDef,
     ResourceARNDetailTypeDef,
-    ResponseMetadataTypeDef,
     ResponseTimeRootCauseEntityTypeDef,
+    SamplingRuleOutputTypeDef,
     SamplingRuleUpdateTypeDef,
     SegmentTypeDef,
     UntagResourceRequestRequestTypeDef,
     AnomalousServiceTypeDef,
     TraceUserTypeDef,
     ValueWithServiceIdsTypeDef,
-    TelemetryRecordTypeDef,
+    BatchGetTracesRequestBatchGetTracesPaginateTypeDef,
+    GetGroupsRequestGetGroupsPaginateTypeDef,
+    GetSamplingRulesRequestGetSamplingRulesPaginateTypeDef,
+    GetSamplingStatisticSummariesRequestGetSamplingStatisticSummariesPaginateTypeDef,
+    GetTraceGraphRequestGetTraceGraphPaginateTypeDef,
+    ListResourcePoliciesRequestListResourcePoliciesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     GroupSummaryTypeDef,
     GroupTypeDef,
     UpdateGroupRequestRequestTypeDef,
     CreateGroupRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSamplingRuleRequestRequestTypeDef,
-    SamplingRuleRecordTypeDef,
     EdgeStatisticsTypeDef,
     ServiceStatisticsTypeDef,
     GetEncryptionConfigResultTypeDef,
     PutEncryptionConfigResultTypeDef,
     ErrorRootCauseEntityTypeDef,
     FaultRootCauseEntityTypeDef,
+    GetInsightImpactGraphRequestRequestTypeDef,
+    GetInsightSummariesRequestRequestTypeDef,
+    GetServiceGraphRequestGetServiceGraphPaginateTypeDef,
+    GetServiceGraphRequestRequestTypeDef,
+    GetTimeSeriesServiceStatisticsRequestGetTimeSeriesServiceStatisticsPaginateTypeDef,
+    GetTimeSeriesServiceStatisticsRequestRequestTypeDef,
+    SamplingStatisticsDocumentTypeDef,
+    TelemetryRecordTypeDef,
     GetSamplingStatisticSummariesResultTypeDef,
-    GetSamplingTargetsRequestRequestTypeDef,
     GetSamplingTargetsResultTypeDef,
     GetTraceSummariesRequestGetTraceSummariesPaginateTypeDef,
     GetTraceSummariesRequestRequestTypeDef,
     InsightImpactGraphServiceTypeDef,
     ListResourcePoliciesResultTypeDef,
     PutResourcePolicyResultTypeDef,
     PutTraceSegmentsResultTypeDef,
     ResponseTimeRootCauseServiceTypeDef,
+    SamplingRuleRecordTypeDef,
+    SamplingRuleUnionTypeDef,
     UpdateSamplingRuleRequestRequestTypeDef,
     TraceTypeDef,
     InsightEventTypeDef,
     InsightSummaryTypeDef,
     InsightTypeDef,
-    PutTelemetryRecordsRequestRequestTypeDef,
     GetGroupsResultTypeDef,
     CreateGroupResultTypeDef,
     GetGroupResultTypeDef,
     UpdateGroupResultTypeDef,
-    CreateSamplingRuleResultTypeDef,
-    DeleteSamplingRuleResultTypeDef,
-    GetSamplingRulesResultTypeDef,
-    UpdateSamplingRuleResultTypeDef,
     EdgeTypeDef,
     TimeSeriesServiceStatisticsTypeDef,
     ErrorRootCauseServiceTypeDef,
     FaultRootCauseServiceTypeDef,
+    GetSamplingTargetsRequestRequestTypeDef,
+    PutTelemetryRecordsRequestRequestTypeDef,
     GetInsightImpactGraphResultTypeDef,
     ResponseTimeRootCauseTypeDef,
+    CreateSamplingRuleResultTypeDef,
+    DeleteSamplingRuleResultTypeDef,
+    GetSamplingRulesResultTypeDef,
+    UpdateSamplingRuleResultTypeDef,
     BatchGetTracesResultTypeDef,
     GetInsightEventsResultTypeDef,
     GetInsightSummariesResultTypeDef,
     GetInsightResultTypeDef,
     ServiceTypeDef,
     GetTimeSeriesServiceStatisticsResultTypeDef,
     ErrorRootCauseTypeDef,
@@ -485,15 +487,15 @@
     GetServiceGraphResultTypeDef,
     GetTraceGraphResultTypeDef,
     TraceSummaryTypeDef,
     GetTraceSummariesResultTypeDef,
 )
 
 
-def get_structure() -> AliasTypeDef:
+def get_value() -> AliasTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-xray-2.5.2/types_aiobotocore_xray.egg-info/SOURCES.txt` & `types-aiobotocore-xray-2.5.2.post1/types_aiobotocore_xray.egg-info/SOURCES.txt`

 * *Files identical despite different names*


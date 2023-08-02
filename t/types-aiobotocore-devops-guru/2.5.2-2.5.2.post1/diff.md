# Comparing `tmp/types-aiobotocore-devops-guru-2.5.2.tar.gz` & `tmp/types-aiobotocore-devops-guru-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-devops-guru-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-devops-guru-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:09 2023, max compression
```

## Comparing `types-aiobotocore-devops-guru-2.5.2.tar` & `types-aiobotocore-devops-guru-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/
--rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33212 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33158 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    19343 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-08 01:28:42.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62107 2023-07-08 01:28:43.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62042 2023-07-08 01:28:43.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:41.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.726001 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23414 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:30.000000 types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.813607 types-aiobotocore-devops-guru-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-08-02 14:52:09.809607 types-aiobotocore-devops-guru-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22361 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:09.813607 types-aiobotocore-devops-guru-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.805607 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/
+-rw-r--r--   0 runner    (1001) docker     (123)     3882 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33201 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33147 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-08-02 14:36:21.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-08-02 14:36:21.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    19315 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19299 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    65266 2023-08-02 14:36:23.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65199 2023-08-02 14:36:21.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:20.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:09.809607 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:09.000000 types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/LICENSE` & `types-aiobotocore-devops-guru-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2/PKG-INFO` & `types-aiobotocore-devops-guru-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devops-guru
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore devops-guru type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore devops-guru type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-devops-guru"></a>
 
 # types-aiobotocore-devops-guru
 
 [![PyPI - types-aiobotocore-devops-guru](https://img.shields.io/pypi/v/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devops-guru?color=blue)](https://pypistats.org/packages/types-aiobotocore-devops-guru)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devops-guru)](https://pepy.tech/project/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DevOpsGuru 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [types-aiobotocore-devops-guru docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/).
 
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
@@ -393,186 +392,198 @@
 )
 
 
 def check_value(value: AnomalySeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_devops_guru.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
+    ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
+    CloudFormationCollectionOutputTypeDef,
     CloudFormationCollectionTypeDef,
+    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
+    TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountHealthResponseTypeDef,
-    DescribeAccountOverviewRequestRequestTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
+    TimestampTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
-    DescribeOrganizationOverviewRequestRequestTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
-    EndTimeRangeTypeDef,
     EventResourceTypeDef,
-    EventTimeRangeTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
-    StartTimeRangeTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
-    NotificationFilterConfigTypeDef,
+    NotificationFilterConfigOutputTypeDef,
     SnsChannelConfigTypeDef,
+    NotificationFilterConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
-    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
+    ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
+    TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
-    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
+    AddNotificationChannelResponseTypeDef,
+    DescribeAccountHealthResponseTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
+    DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeOrganizationOverviewRequestRequestTypeDef,
+    EndTimeRangeTypeDef,
+    EventTimeRangeTypeDef,
+    StartTimeRangeTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
-    ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
     PerformanceInsightsMetricQueryTypeDef,
     RecommendationRelatedAnomalySourceDetailTypeDef,
     RecommendationRelatedEventTypeDef,
     ResourceCollectionFilterTypeDef,
+    ResourceCollectionOutputTypeDef,
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     StartCostEstimationRequestRequestTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
+    ListInsightsAnyStatusFilterTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
-    ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
-    AddNotificationChannelRequestRequestTypeDef,
     NotificationChannelTypeDef,
+    AddNotificationChannelRequestRequestTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
-    ListEventsFiltersTypeDef,
     MonitoredResourceIdentifierTypeDef,
     ProactiveInsightSummaryTypeDef,
     ProactiveInsightTypeDef,
     ProactiveOrganizationInsightSummaryTypeDef,
     ReactiveInsightSummaryTypeDef,
     ReactiveInsightTypeDef,
     ReactiveOrganizationInsightSummaryTypeDef,
+    ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
-    ListInsightsRequestListInsightsPaginateTypeDef,
-    ListInsightsRequestRequestTypeDef,
-    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    ListOrganizationInsightsRequestRequestTypeDef,
+    ListInsightsStatusFilterTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
-    ListEventsRequestListEventsPaginateTypeDef,
-    ListEventsRequestRequestTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     DescribeInsightResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
+    ListEventsRequestListEventsPaginateTypeDef,
+    ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
+    ListInsightsRequestListInsightsPaginateTypeDef,
+    ListInsightsRequestRequestTypeDef,
+    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    ListOrganizationInsightsRequestRequestTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
     AnomalySourceDetailsTypeDef,
     ProactiveAnomalySummaryTypeDef,
     ProactiveAnomalyTypeDef,
     ReactiveAnomalySummaryTypeDef,
     ReactiveAnomalyTypeDef,
     ListAnomaliesForInsightResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInsightHealthTypeDef:
+def get_value() -> AccountInsightHealthTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/README.md` & `types-aiobotocore-devops-guru-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-devops-guru"></a>
 
 # types-aiobotocore-devops-guru
 
 [![PyPI - types-aiobotocore-devops-guru](https://img.shields.io/pypi/v/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devops-guru?color=blue)](https://pypistats.org/packages/types-aiobotocore-devops-guru)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devops-guru)](https://pepy.tech/project/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DevOpsGuru 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [types-aiobotocore-devops-guru docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/).
 
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
@@ -360,186 +360,198 @@
 )
 
 
 def check_value(value: AnomalySeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_devops_guru.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
+    ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
+    CloudFormationCollectionOutputTypeDef,
     CloudFormationCollectionTypeDef,
+    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
+    TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountHealthResponseTypeDef,
-    DescribeAccountOverviewRequestRequestTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
+    TimestampTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
-    DescribeOrganizationOverviewRequestRequestTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
-    EndTimeRangeTypeDef,
     EventResourceTypeDef,
-    EventTimeRangeTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
-    StartTimeRangeTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
-    NotificationFilterConfigTypeDef,
+    NotificationFilterConfigOutputTypeDef,
     SnsChannelConfigTypeDef,
+    NotificationFilterConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
-    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
+    ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
+    TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
-    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
+    AddNotificationChannelResponseTypeDef,
+    DescribeAccountHealthResponseTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
+    DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeOrganizationOverviewRequestRequestTypeDef,
+    EndTimeRangeTypeDef,
+    EventTimeRangeTypeDef,
+    StartTimeRangeTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
-    ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
     PerformanceInsightsMetricQueryTypeDef,
     RecommendationRelatedAnomalySourceDetailTypeDef,
     RecommendationRelatedEventTypeDef,
     ResourceCollectionFilterTypeDef,
+    ResourceCollectionOutputTypeDef,
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     StartCostEstimationRequestRequestTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
+    ListInsightsAnyStatusFilterTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
-    ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
-    AddNotificationChannelRequestRequestTypeDef,
     NotificationChannelTypeDef,
+    AddNotificationChannelRequestRequestTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
-    ListEventsFiltersTypeDef,
     MonitoredResourceIdentifierTypeDef,
     ProactiveInsightSummaryTypeDef,
     ProactiveInsightTypeDef,
     ProactiveOrganizationInsightSummaryTypeDef,
     ReactiveInsightSummaryTypeDef,
     ReactiveInsightTypeDef,
     ReactiveOrganizationInsightSummaryTypeDef,
+    ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
-    ListInsightsRequestListInsightsPaginateTypeDef,
-    ListInsightsRequestRequestTypeDef,
-    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    ListOrganizationInsightsRequestRequestTypeDef,
+    ListInsightsStatusFilterTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
-    ListEventsRequestListEventsPaginateTypeDef,
-    ListEventsRequestRequestTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     DescribeInsightResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
+    ListEventsRequestListEventsPaginateTypeDef,
+    ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
+    ListInsightsRequestListInsightsPaginateTypeDef,
+    ListInsightsRequestRequestTypeDef,
+    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    ListOrganizationInsightsRequestRequestTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
     AnomalySourceDetailsTypeDef,
     ProactiveAnomalySummaryTypeDef,
     ProactiveAnomalyTypeDef,
     ReactiveAnomalySummaryTypeDef,
     ReactiveAnomalyTypeDef,
     ListAnomaliesForInsightResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInsightHealthTypeDef:
+def get_value() -> AccountInsightHealthTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/setup.py` & `types-aiobotocore-devops-guru-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-devops-guru",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_devops_guru"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with"
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
-    keywords="aiobotocore devops-guru type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore devops-guru type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_devops_guru": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/"
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.py` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__init__.pyi` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/__main__.py` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DevOpsGuru 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DevOpsGuru 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru\nOther"
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

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.py` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("devops-guru") as client:
         client: DevOpsGuruClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     InsightTypeType,
     LocaleType,
@@ -42,15 +41,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
-    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
@@ -70,20 +69,21 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
-    NotificationChannelConfigTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
+    TimestampTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -126,15 +126,15 @@
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#exceptions)
         """
 
     async def add_notification_channel(
-        self, *, Config: NotificationChannelConfigTypeDef
+        self, *, Config: NotificationChannelConfigUnionTypeDef
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#add_notification_channel)
         """
@@ -171,15 +171,15 @@
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_account_health)
         """
 
     async def describe_account_overview(
-        self, *, FromTime: Union[datetime, str], ToTime: Union[datetime, str] = ...
+        self, *, FromTime: TimestampTypeDef, ToTime: TimestampTypeDef = ...
     ) -> DescribeAccountOverviewResponseTypeDef:
         """
         For the time range passed in, returns the number of open reactive insight that
         were created, the number of open proactive insights that were created, and the
         Mean Time to Recover (MTTR) for all closed reactive insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_overview)
@@ -234,16 +234,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_organization_health)
         """
 
     async def describe_organization_overview(
         self,
         *,
-        FromTime: Union[datetime, str],
-        ToTime: Union[datetime, str] = ...,
+        FromTime: TimestampTypeDef,
+        ToTime: TimestampTypeDef = ...,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...
     ) -> DescribeOrganizationOverviewResponseTypeDef:
         """
         Returns an overview of your organization's history based on the specified time
         range.
 
@@ -487,15 +487,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_organization_insights)
         """
 
     async def start_cost_estimation(
         self,
         *,
-        ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
+        ResourceCollection: CostEstimationResourceCollectionFilterUnionTypeDef,
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/client.pyi` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("devops-guru") as client:
         client: DevOpsGuruClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     InsightTypeType,
     LocaleType,
@@ -42,15 +41,15 @@
     ListOrganizationInsightsPaginator,
     ListRecommendationsPaginator,
     SearchInsightsPaginator,
     SearchOrganizationInsightsPaginator,
 )
 from .type_defs import (
     AddNotificationChannelResponseTypeDef,
-    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     DescribeAccountHealthResponseTypeDef,
     DescribeAccountOverviewResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     DescribeFeedbackResponseTypeDef,
     DescribeInsightResponseTypeDef,
     DescribeOrganizationHealthResponseTypeDef,
@@ -70,20 +69,21 @@
     ListInsightsResponseTypeDef,
     ListInsightsStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
     ListRecommendationsResponseTypeDef,
-    NotificationChannelConfigTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     StartTimeRangeTypeDef,
+    TimestampTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -121,15 +121,15 @@
         """
         DevOpsGuruClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#exceptions)
         """
     async def add_notification_channel(
-        self, *, Config: NotificationChannelConfigTypeDef
+        self, *, Config: NotificationChannelConfigUnionTypeDef
     ) -> AddNotificationChannelResponseTypeDef:
         """
         Adds a notification channel to DevOps Guru.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.add_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#add_notification_channel)
         """
@@ -161,15 +161,15 @@
         insights, and the number of metrics analyzed in your Amazon Web Services
         account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_account_health)
         """
     async def describe_account_overview(
-        self, *, FromTime: Union[datetime, str], ToTime: Union[datetime, str] = ...
+        self, *, FromTime: TimestampTypeDef, ToTime: TimestampTypeDef = ...
     ) -> DescribeAccountOverviewResponseTypeDef:
         """
         For the time range passed in, returns the number of open reactive insight that
         were created, the number of open proactive insights that were created, and the
         Mean Time to Recover (MTTR) for all closed reactive insights.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_account_overview)
@@ -218,16 +218,16 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.describe_organization_health)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#describe_organization_health)
         """
     async def describe_organization_overview(
         self,
         *,
-        FromTime: Union[datetime, str],
-        ToTime: Union[datetime, str] = ...,
+        FromTime: TimestampTypeDef,
+        ToTime: TimestampTypeDef = ...,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...
     ) -> DescribeOrganizationOverviewResponseTypeDef:
         """
         Returns an overview of your organization's history based on the specified time
         range.
 
@@ -452,15 +452,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.search_organization_insights)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/client/#search_organization_insights)
         """
     async def start_cost_estimation(
         self,
         *,
-        ResourceCollection: CostEstimationResourceCollectionFilterTypeDef,
+        ResourceCollection: CostEstimationResourceCollectionFilterUnionTypeDef,
         ClientToken: str = ...
     ) -> Dict[str, Any]:
         """
         Starts the creation of an estimate of the monthly cost to analyze your Amazon
         Web Services resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Client.start_cost_estimation)
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.py` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/literals.pyi` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.py` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
 
@@ -137,30 +137,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
 
 class GetCostEstimationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getcostestimationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCostEstimationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getcostestimationpaginator)
         """
 
 
@@ -170,15 +170,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
 
@@ -191,30 +191,30 @@
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
 
 class ListAnomalousLogGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomalousloggroupspaginator)
     """
 
     def paginate(
-        self, *, InsightId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnomalousLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomalousloggroupspaginator)
         """
 
 
@@ -225,15 +225,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listeventspaginator)
         """
 
 
@@ -243,15 +243,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
         """
 
 
@@ -261,30 +261,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
 
 class ListNotificationChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listnotificationchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNotificationChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listnotificationchannelspaginator)
         """
 
 
@@ -296,15 +296,15 @@
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
 
@@ -316,15 +316,15 @@
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listrecommendationspaginator)
         """
 
 
@@ -336,15 +336,15 @@
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchinsightspaginator)
         """
 
 
@@ -357,13 +357,13 @@
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/paginator.pyi` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     def paginate(
         self,
         *,
         OrganizationResourceCollectionType: OrganizationResourceCollectionTypeType,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeOrganizationResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeorganizationresourcecollectionhealthpaginator)
         """
 
 class DescribeResourceCollectionHealthPaginator(AioPaginator):
@@ -133,29 +133,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeResourceCollectionHealthResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.DescribeResourceCollectionHealth.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#describeresourcecollectionhealthpaginator)
         """
 
 class GetCostEstimationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getcostestimationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCostEstimationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetCostEstimation.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getcostestimationpaginator)
         """
 
 class GetResourceCollectionPaginator(AioPaginator):
@@ -164,15 +164,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceCollectionType: ResourceCollectionTypeType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourceCollectionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.GetResourceCollection.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#getresourcecollectionpaginator)
         """
 
 class ListAnomaliesForInsightPaginator(AioPaginator):
@@ -184,29 +184,29 @@
     def paginate(
         self,
         *,
         InsightId: str,
         StartTimeRange: StartTimeRangeTypeDef = ...,
         AccountId: str = ...,
         Filters: ListAnomaliesForInsightFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnomaliesForInsightResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomaliesForInsight.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomaliesforinsightpaginator)
         """
 
 class ListAnomalousLogGroupsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomalousloggroupspaginator)
     """
 
     def paginate(
-        self, *, InsightId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, InsightId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAnomalousLogGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListAnomalousLogGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listanomalousloggroupspaginator)
         """
 
 class ListEventsPaginator(AioPaginator):
@@ -216,15 +216,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: ListEventsFiltersTypeDef,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listeventspaginator)
         """
 
 class ListInsightsPaginator(AioPaginator):
@@ -233,15 +233,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
     """
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listinsightspaginator)
         """
 
 class ListMonitoredResourcesPaginator(AioPaginator):
@@ -250,29 +250,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ListMonitoredResourcesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMonitoredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListMonitoredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listmonitoredresourcespaginator)
         """
 
 class ListNotificationChannelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listnotificationchannelspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNotificationChannelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListNotificationChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listnotificationchannelspaginator)
         """
 
 class ListOrganizationInsightsPaginator(AioPaginator):
@@ -283,15 +283,15 @@
 
     def paginate(
         self,
         *,
         StatusFilter: ListInsightsStatusFilterTypeDef,
         AccountIds: Sequence[str] = ...,
         OrganizationalUnitIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listorganizationinsightspaginator)
         """
 
 class ListRecommendationsPaginator(AioPaginator):
@@ -302,15 +302,15 @@
 
     def paginate(
         self,
         *,
         InsightId: str,
         Locale: LocaleType = ...,
         AccountId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.ListRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#listrecommendationspaginator)
         """
 
 class SearchInsightsPaginator(AioPaginator):
@@ -321,15 +321,15 @@
 
     def paginate(
         self,
         *,
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchinsightspaginator)
         """
 
 class SearchOrganizationInsightsPaginator(AioPaginator):
@@ -341,13 +341,13 @@
     def paginate(
         self,
         *,
         AccountIds: Sequence[str],
         StartTimeRange: StartTimeRangeTypeDef,
         Type: InsightTypeType,
         Filters: SearchOrganizationInsightsFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchOrganizationInsightsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru.Paginator.SearchOrganizationInsights.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/paginators/#searchorganizationinsightspaginator)
         """
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.py` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_devops_guru.type_defs import AccountInsightHealthTypeDef
 
-    data: AccountInsightHealthTypeDef = {...}
+    data: AccountInsightHealthTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -47,162 +47,174 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountInsightHealthTypeDef",
-    "AddNotificationChannelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
+    "CloudFormationCollectionOutputTypeDef",
     "CloudFormationCollectionTypeDef",
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DescribeAccountHealthResponseTypeDef",
-    "DescribeAccountOverviewRequestRequestTypeDef",
-    "DescribeAccountOverviewResponseTypeDef",
+    "TimestampTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
-    "DescribeOrganizationHealthResponseTypeDef",
-    "DescribeOrganizationOverviewRequestRequestTypeDef",
-    "DescribeOrganizationOverviewResponseTypeDef",
-    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
-    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
-    "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
-    "EventTimeRangeTypeDef",
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
-    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
-    "StartTimeRangeTypeDef",
-    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
-    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
-    "NotificationFilterConfigTypeDef",
+    "NotificationFilterConfigOutputTypeDef",
     "SnsChannelConfigTypeDef",
+    "NotificationFilterConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
-    "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
+    "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
+    "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
-    "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
+    "AddNotificationChannelResponseTypeDef",
+    "DescribeAccountHealthResponseTypeDef",
+    "DescribeAccountOverviewResponseTypeDef",
+    "DescribeOrganizationHealthResponseTypeDef",
+    "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
+    "DescribeAccountOverviewRequestRequestTypeDef",
+    "DescribeOrganizationOverviewRequestRequestTypeDef",
+    "EndTimeRangeTypeDef",
+    "EventTimeRangeTypeDef",
+    "StartTimeRangeTypeDef",
     "DescribeFeedbackResponseTypeDef",
     "PutFeedbackRequestRequestTypeDef",
-    "ListInsightsClosedStatusFilterTypeDef",
+    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
-    "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
+    "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "RecommendationRelatedAnomalySourceDetailTypeDef",
     "RecommendationRelatedEventTypeDef",
     "ResourceCollectionFilterTypeDef",
+    "ResourceCollectionOutputTypeDef",
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
+    "CostEstimationResourceCollectionFilterUnionTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
+    "ListInsightsClosedStatusFilterTypeDef",
+    "ListInsightsAnyStatusFilterTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
-    "ListInsightsStatusFilterTypeDef",
     "AnomalousLogGroupTypeDef",
-    "AddNotificationChannelRequestRequestTypeDef",
     "NotificationChannelTypeDef",
+    "AddNotificationChannelRequestRequestTypeDef",
+    "NotificationChannelConfigUnionTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
-    "ListEventsFiltersTypeDef",
     "MonitoredResourceIdentifierTypeDef",
     "ProactiveInsightSummaryTypeDef",
     "ProactiveInsightTypeDef",
     "ProactiveOrganizationInsightSummaryTypeDef",
     "ReactiveInsightSummaryTypeDef",
     "ReactiveInsightTypeDef",
     "ReactiveOrganizationInsightSummaryTypeDef",
+    "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
-    "ListInsightsRequestListInsightsPaginateTypeDef",
-    "ListInsightsRequestRequestTypeDef",
-    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    "ListOrganizationInsightsRequestRequestTypeDef",
+    "ListInsightsStatusFilterTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
-    "ListEventsRequestListEventsPaginateTypeDef",
-    "ListEventsRequestRequestTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
     "SearchInsightsResponseTypeDef",
     "SearchOrganizationInsightsResponseTypeDef",
     "DescribeInsightResponseTypeDef",
     "ListOrganizationInsightsResponseTypeDef",
+    "ListEventsRequestListEventsPaginateTypeDef",
+    "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
+    "ListInsightsRequestListInsightsPaginateTypeDef",
+    "ListInsightsRequestRequestTypeDef",
+    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    "ListOrganizationInsightsRequestRequestTypeDef",
     "PerformanceInsightsReferenceDataTypeDef",
     "ListRecommendationsResponseTypeDef",
     "PerformanceInsightsMetricsDetailTypeDef",
     "AnomalySourceDetailsTypeDef",
     "ProactiveAnomalySummaryTypeDef",
     "ProactiveAnomalyTypeDef",
     "ReactiveAnomalySummaryTypeDef",
@@ -216,19 +228,22 @@
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
 )
 
-AddNotificationChannelResponseTypeDef = TypedDict(
-    "AddNotificationChannelResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
@@ -299,26 +314,42 @@
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
 
+CloudFormationCollectionOutputTypeDef = TypedDict(
+    "CloudFormationCollectionOutputTypeDef",
+    {
+        "StackNames": List[str],
+    },
+    total=False,
+)
+
 CloudFormationCollectionTypeDef = TypedDict(
     "CloudFormationCollectionTypeDef",
     {
+        "StackNames": Sequence[str],
+    },
+    total=False,
+)
+
+CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
         "StackNames": List[str],
     },
     total=False,
 )
 
 CloudFormationCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     {
-        "StackNames": List[str],
+        "StackNames": Sequence[str],
     },
     total=False,
 )
 
 InsightHealthTypeDef = TypedDict(
     "InsightHealthTypeDef",
     {
@@ -343,19 +374,27 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+TagCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "AppBoundaryKey": str,
+        "TagValues": List[str],
+    },
+)
+
 TagCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "TagCostEstimationResourceCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": List[str],
+        "TagValues": Sequence[str],
     },
 )
 
 CostEstimationTimeRangeTypeDef = TypedDict(
     "CostEstimationTimeRangeTypeDef",
     {
         "StartTime": datetime,
@@ -367,58 +406,15 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DescribeAccountHealthResponseTypeDef = TypedDict(
-    "DescribeAccountHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "AnalyzedResourceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-
-class DescribeAccountOverviewRequestRequestTypeDef(
-    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
-    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
-):
-    pass
-
-
-DescribeAccountOverviewResponseTypeDef = TypedDict(
-    "DescribeAccountOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "MeanTimeToRecoverInMilliseconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
@@ -479,83 +475,24 @@
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationHealthResponseTypeDef = TypedDict(
-    "DescribeOrganizationHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-    },
-    total=False,
-)
-
-
-class DescribeOrganizationOverviewRequestRequestTypeDef(
-    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
-    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
-):
-    pass
-
-
-DescribeOrganizationOverviewResponseTypeDef = TypedDict(
-    "DescribeOrganizationOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "MaxResults": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -573,36 +510,14 @@
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -617,49 +532,24 @@
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
 
-EndTimeRangeTypeDef = TypedDict(
-    "EndTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 EventResourceTypeDef = TypedDict(
     "EventResourceTypeDef",
     {
         "Type": str,
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-EventTimeRangeTypeDef = TypedDict(
-    "EventTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-)
-
-GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -672,36 +562,14 @@
         "Count": int,
         "UnitCost": float,
         "Cost": float,
     },
     total=False,
 )
 
-_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
-    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
@@ -763,45 +631,14 @@
     "ServiceCollectionTypeDef",
     {
         "ServiceNames": Sequence[ServiceNameType],
     },
     total=False,
 )
 
-StartTimeRangeTypeDef = TypedDict(
-    "StartTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
-    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -832,54 +669,22 @@
     "ListMonitoredResourcesFiltersTypeDef",
     {
         "ResourcePermission": ResourcePermissionType,
         "ResourceTypeFilters": Sequence[ResourceTypeFilterType],
     },
 )
 
-ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNotificationChannelsRequestRequestTypeDef = TypedDict(
     "ListNotificationChannelsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "Locale": LocaleType,
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
-    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -926,53 +731,52 @@
     "LogsAnomalyDetectionIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
-NotificationFilterConfigTypeDef = TypedDict(
-    "NotificationFilterConfigTypeDef",
+NotificationFilterConfigOutputTypeDef = TypedDict(
+    "NotificationFilterConfigOutputTypeDef",
     {
-        "Severities": Sequence[InsightSeverityType],
-        "MessageTypes": Sequence[NotificationMessageTypeType],
+        "Severities": List[InsightSeverityType],
+        "MessageTypes": List[NotificationMessageTypeType],
     },
     total=False,
 )
 
 SnsChannelConfigTypeDef = TypedDict(
     "SnsChannelConfigTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-OpsCenterIntegrationConfigTypeDef = TypedDict(
-    "OpsCenterIntegrationConfigTypeDef",
+NotificationFilterConfigTypeDef = TypedDict(
+    "NotificationFilterConfigTypeDef",
     {
-        "OptInStatus": OptInStatusType,
+        "Severities": Sequence[InsightSeverityType],
+        "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
 )
 
-OpsCenterIntegrationTypeDef = TypedDict(
-    "OpsCenterIntegrationTypeDef",
+OpsCenterIntegrationConfigTypeDef = TypedDict(
+    "OpsCenterIntegrationConfigTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+OpsCenterIntegrationTypeDef = TypedDict(
+    "OpsCenterIntegrationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
 PerformanceInsightsMetricDimensionGroupTypeDef = TypedDict(
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     {
@@ -1017,14 +821,22 @@
 
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
 
+ServiceCollectionOutputTypeDef = TypedDict(
+    "ServiceCollectionOutputTypeDef",
+    {
+        "ServiceNames": List[ServiceNameType],
+    },
+    total=False,
+)
+
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -1059,30 +871,27 @@
     "TagCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
-TagCollectionTypeDef = TypedDict(
-    "TagCollectionTypeDef",
+TagCollectionOutputTypeDef = TypedDict(
+    "TagCollectionOutputTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagCollectionTypeDef = TypedDict(
+    "TagCollectionTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AppBoundaryKey": str,
+        "TagValues": Sequence[str],
     },
 )
 
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
@@ -1112,14 +921,64 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
+AddNotificationChannelResponseTypeDef = TypedDict(
+    "AddNotificationChannelResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountHealthResponseTypeDef = TypedDict(
+    "DescribeAccountHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "AnalyzedResourceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountOverviewResponseTypeDef = TypedDict(
+    "DescribeAccountOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "MeanTimeToRecoverInMilliseconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationHealthResponseTypeDef = TypedDict(
+    "DescribeOrganizationHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationOverviewResponseTypeDef = TypedDict(
+    "DescribeOrganizationOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
     total=False,
 )
@@ -1150,68 +1009,264 @@
     {
         "TimestampMetricValuePairList": List[TimestampMetricValuePairTypeDef],
         "StatusCode": CloudWatchMetricDataStatusCodeType,
     },
     total=False,
 )
 
+CostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
+        "Tags": List[TagCostEstimationResourceCollectionFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 CostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CostEstimationResourceCollectionFilterTypeDef",
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
-        "Tags": List[TagCostEstimationResourceCollectionFilterTypeDef],
+        "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAccountOverviewRequestRequestTypeDef(
+    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
+    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+    },
+    total=False,
+)
+
+
+class DescribeOrganizationOverviewRequestRequestTypeDef(
+    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
+    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
+):
+    pass
+
+
+EndTimeRangeTypeDef = TypedDict(
+    "EndTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventTimeRangeTypeDef = TypedDict(
+    "EventTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+)
+
+StartTimeRangeTypeDef = TypedDict(
+    "StartTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
     },
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
     },
     total=False,
 )
 
-ListInsightsClosedStatusFilterTypeDef = TypedDict(
-    "ListInsightsClosedStatusFilterTypeDef",
+_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     {
-        "Type": InsightTypeType,
-        "EndTimeRange": EndTimeRangeTypeDef,
+        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListAnomaliesForInsightFiltersTypeDef = TypedDict(
-    "ListAnomaliesForInsightFiltersTypeDef",
+
+class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListInsightsAnyStatusFilterTypeDef = TypedDict(
-    "ListInsightsAnyStatusFilterTypeDef",
+
+class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+
+GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     {
-        "Type": InsightTypeType,
-        "StartTimeRange": StartTimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
+    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+
+class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
+    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+):
+    pass
+
+
+ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "Locale": LocaleType,
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
+    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
+):
+    pass
+
+
+ListAnomaliesForInsightFiltersTypeDef = TypedDict(
+    "ListAnomaliesForInsightFiltersTypeDef",
+    {
+        "ServiceCollection": ServiceCollectionTypeDef,
+    },
+    total=False,
 )
 
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitoredResourcesRequestRequestTypeDef = TypedDict(
     "ListMonitoredResourcesRequestRequestTypeDef",
     {
@@ -1226,14 +1281,35 @@
     "LogAnomalyShowcaseTypeDef",
     {
         "LogAnomalyClasses": List[LogAnomalyClassTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_RequiredNotificationChannelConfigOutputTypeDef",
+    {
+        "Sns": SnsChannelConfigTypeDef,
+    },
+)
+_OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_OptionalNotificationChannelConfigOutputTypeDef",
+    {
+        "Filters": NotificationFilterConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class NotificationChannelConfigOutputTypeDef(
+    _RequiredNotificationChannelConfigOutputTypeDef, _OptionalNotificationChannelConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredNotificationChannelConfigTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigTypeDef",
     {
         "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigTypeDef = TypedDict(
@@ -1303,19 +1379,28 @@
     {
         "CloudFormation": CloudFormationCollectionFilterTypeDef,
         "Tags": List[TagCollectionFilterTypeDef],
     },
     total=False,
 )
 
+ResourceCollectionOutputTypeDef = TypedDict(
+    "ResourceCollectionOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCollectionOutputTypeDef,
+        "Tags": List[TagCollectionOutputTypeDef],
+    },
+    total=False,
+)
+
 ResourceCollectionTypeDef = TypedDict(
     "ResourceCollectionTypeDef",
     {
         "CloudFormation": CloudFormationCollectionTypeDef,
-        "Tags": List[TagCollectionTypeDef],
+        "Tags": Sequence[TagCollectionTypeDef],
     },
     total=False,
 )
 
 ServiceHealthTypeDef = TypedDict(
     "ServiceHealthTypeDef",
     {
@@ -1335,15 +1420,15 @@
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
@@ -1364,24 +1449,28 @@
     },
     total=False,
 )
 
 GetCostEstimationResponseTypeDef = TypedDict(
     "GetCostEstimationResponseTypeDef",
     {
-        "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
+        "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CostEstimationResourceCollectionFilterUnionTypeDef = Union[
+    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
+]
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
     },
 )
 _OptionalStartCostEstimationRequestRequestTypeDef = TypedDict(
@@ -1396,27 +1485,43 @@
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
 
+ListInsightsClosedStatusFilterTypeDef = TypedDict(
+    "ListInsightsClosedStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "EndTimeRange": EndTimeRangeTypeDef,
+    },
+)
+
+ListInsightsAnyStatusFilterTypeDef = TypedDict(
+    "ListInsightsAnyStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "StartTimeRange": StartTimeRangeTypeDef,
+    },
+)
+
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
@@ -1447,64 +1552,57 @@
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
 
-ListInsightsStatusFilterTypeDef = TypedDict(
-    "ListInsightsStatusFilterTypeDef",
-    {
-        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
-        "Closed": ListInsightsClosedStatusFilterTypeDef,
-        "Any": ListInsightsAnyStatusFilterTypeDef,
-    },
-    total=False,
-)
-
 AnomalousLogGroupTypeDef = TypedDict(
     "AnomalousLogGroupTypeDef",
     {
         "LogGroupName": str,
         "ImpactStartTime": datetime,
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
         "LogAnomalyShowcases": List[LogAnomalyShowcaseTypeDef],
     },
     total=False,
 )
 
-AddNotificationChannelRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelRequestRequestTypeDef",
+NotificationChannelTypeDef = TypedDict(
+    "NotificationChannelTypeDef",
     {
-        "Config": NotificationChannelConfigTypeDef,
+        "Id": str,
+        "Config": NotificationChannelConfigOutputTypeDef,
     },
+    total=False,
 )
 
-NotificationChannelTypeDef = TypedDict(
-    "NotificationChannelTypeDef",
+AddNotificationChannelRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelRequestRequestTypeDef",
     {
-        "Id": str,
         "Config": NotificationChannelConfigTypeDef,
     },
-    total=False,
 )
 
+NotificationChannelConfigUnionTypeDef = Union[
+    NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef
+]
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
 )
 
 DescribeServiceIntegrationResponseTypeDef = TypedDict(
     "DescribeServiceIntegrationResponseTypeDef",
     {
         "ServiceIntegration": ServiceIntegrationConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceMetricTypeDef = TypedDict(
     "PerformanceInsightsReferenceMetricTypeDef",
     {
         "MetricQuery": PerformanceInsightsMetricQueryTypeDef,
@@ -1523,84 +1621,71 @@
 )
 
 GetResourceCollectionResponseTypeDef = TypedDict(
     "GetResourceCollectionResponseTypeDef",
     {
         "ResourceCollection": ResourceCollectionFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Id": str,
         "Time": datetime,
         "EventSource": str,
         "Name": str,
         "DataSource": EventDataSourceType,
         "EventClass": EventClassType,
         "Resources": List[EventResourceTypeDef],
     },
     total=False,
 )
 
-ListEventsFiltersTypeDef = TypedDict(
-    "ListEventsFiltersTypeDef",
-    {
-        "InsightId": str,
-        "EventTimeRange": EventTimeRangeTypeDef,
-        "EventClass": EventClassType,
-        "EventSource": str,
-        "DataSource": EventDataSourceType,
-        "ResourceCollection": ResourceCollectionTypeDef,
-    },
-    total=False,
-)
-
 MonitoredResourceIdentifierTypeDef = TypedDict(
     "MonitoredResourceIdentifierTypeDef",
     {
         "MonitoredResourceName": str,
         "Type": str,
         "ResourcePermission": ResourcePermissionType,
         "LastUpdated": datetime,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ProactiveInsightSummaryTypeDef = TypedDict(
     "ProactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ProactiveInsightTypeDef = TypedDict(
     "ProactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ProactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1610,44 +1695,44 @@
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ReactiveInsightSummaryTypeDef = TypedDict(
     "ReactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ReactiveInsightTypeDef = TypedDict(
     "ReactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ReactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1656,16 +1741,29 @@
         "Id": str,
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
+    },
+    total=False,
+)
+
+ListEventsFiltersTypeDef = TypedDict(
+    "ListEventsFiltersTypeDef",
+    {
+        "InsightId": str,
+        "EventTimeRange": EventTimeRangeTypeDef,
+        "EventClass": EventClassType,
+        "EventSource": str,
+        "DataSource": EventDataSourceType,
         "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 SearchInsightsFiltersTypeDef = TypedDict(
     "SearchInsightsFiltersTypeDef",
     {
@@ -1692,146 +1790,63 @@
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "Account": List[AccountHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceCollectionHealthResponseTypeDef = TypedDict(
     "DescribeResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceCollectionRequestRequestTypeDef = TypedDict(
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
         "ResourceCollection": UpdateResourceCollectionFilterTypeDef,
     },
 )
 
-_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListInsightsRequestListInsightsPaginateTypeDef(
-    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
-    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListInsightsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-
-class ListInsightsRequestRequestTypeDef(
-    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
-    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+ListInsightsStatusFilterTypeDef = TypedDict(
+    "ListInsightsStatusFilterTypeDef",
     {
-        "MaxResults": int,
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "NextToken": str,
+        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
+        "Closed": ListInsightsClosedStatusFilterTypeDef,
+        "Any": ListInsightsAnyStatusFilterTypeDef,
     },
     total=False,
 )
 
-
-class ListOrganizationInsightsRequestRequestTypeDef(
-    _RequiredListOrganizationInsightsRequestRequestTypeDef,
-    _OptionalListOrganizationInsightsRequestRequestTypeDef,
-):
-    pass
-
-
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationChannelsResponseTypeDef = TypedDict(
     "ListNotificationChannelsResponseTypeDef",
     {
         "Channels": List[NotificationChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceComparisonValuesTypeDef = TypedDict(
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     {
         "ReferenceScalar": PerformanceInsightsReferenceScalarTypeDef,
@@ -1855,121 +1870,121 @@
 )
 
 ListEventsResponseTypeDef = TypedDict(
     "ListEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_RequiredListEventsRequestListEventsPaginateTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_OptionalListEventsRequestListEventsPaginateTypeDef",
-    {
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListEventsRequestListEventsPaginateTypeDef(
-    _RequiredListEventsRequestListEventsPaginateTypeDef,
-    _OptionalListEventsRequestListEventsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventsRequestRequestTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class ListEventsRequestRequestTypeDef(
-    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
-):
-    pass
-
-
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInsightsResponseTypeDef = TypedDict(
     "ListInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchInsightsResponseTypeDef = TypedDict(
     "SearchInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchOrganizationInsightsResponseTypeDef = TypedDict(
     "SearchOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInsightResponseTypeDef = TypedDict(
     "DescribeInsightResponseTypeDef",
     {
         "ProactiveInsight": ProactiveInsightTypeDef,
         "ReactiveInsight": ReactiveInsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrganizationInsightsResponseTypeDef = TypedDict(
     "ListOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_RequiredListEventsRequestListEventsPaginateTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
     },
 )
+_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_OptionalListEventsRequestListEventsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEventsRequestListEventsPaginateTypeDef(
+    _RequiredListEventsRequestListEventsPaginateTypeDef,
+    _OptionalListEventsRequestListEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventsRequestRequestTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+
+class ListEventsRequestRequestTypeDef(
+    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
@@ -1998,15 +2013,15 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "Filters": SearchInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
@@ -2049,42 +2064,135 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
 
+_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListInsightsRequestListInsightsPaginateTypeDef(
+    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
+    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListInsightsRequestRequestTypeDef(
+    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
+    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+
+class ListOrganizationInsightsRequestRequestTypeDef(
+    _RequiredListOrganizationInsightsRequestRequestTypeDef,
+    _OptionalListOrganizationInsightsRequestRequestTypeDef,
+):
+    pass
+
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsMetricsDetailTypeDef = TypedDict(
     "PerformanceInsightsMetricsDetailTypeDef",
     {
         "MetricDisplayName": str,
@@ -2114,15 +2222,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2135,15 +2243,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2154,15 +2262,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2174,15 +2282,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2190,19 +2298,19 @@
 
 ListAnomaliesForInsightResponseTypeDef = TypedDict(
     "ListAnomaliesForInsightResponseTypeDef",
     {
         "ProactiveAnomalies": List[ProactiveAnomalySummaryTypeDef],
         "ReactiveAnomalies": List[ReactiveAnomalySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnomalyResponseTypeDef = TypedDict(
     "DescribeAnomalyResponseTypeDef",
     {
         "ProactiveAnomaly": ProactiveAnomalyTypeDef,
         "ReactiveAnomaly": ReactiveAnomalyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru/type_defs.pyi` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_devops_guru.type_defs import AccountInsightHealthTypeDef
 
-    data: AccountInsightHealthTypeDef = {...}
+    data: AccountInsightHealthTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -46,162 +46,174 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountInsightHealthTypeDef",
-    "AddNotificationChannelResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     "AnomalyReportedTimeRangeTypeDef",
     "AnomalyResourceTypeDef",
     "AnomalySourceMetadataTypeDef",
     "AnomalyTimeRangeTypeDef",
     "CloudFormationCollectionFilterTypeDef",
+    "CloudFormationCollectionOutputTypeDef",
     "CloudFormationCollectionTypeDef",
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     "InsightHealthTypeDef",
     "TimestampMetricValuePairTypeDef",
     "CloudWatchMetricsDimensionTypeDef",
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
     "TagCostEstimationResourceCollectionFilterTypeDef",
     "CostEstimationTimeRangeTypeDef",
     "DeleteInsightRequestRequestTypeDef",
-    "DescribeAccountHealthResponseTypeDef",
-    "DescribeAccountOverviewRequestRequestTypeDef",
-    "DescribeAccountOverviewResponseTypeDef",
+    "TimestampTypeDef",
     "DescribeAnomalyRequestRequestTypeDef",
     "DescribeFeedbackRequestRequestTypeDef",
     "InsightFeedbackTypeDef",
     "DescribeInsightRequestRequestTypeDef",
     "DescribeOrganizationHealthRequestRequestTypeDef",
-    "DescribeOrganizationHealthResponseTypeDef",
-    "DescribeOrganizationOverviewRequestRequestTypeDef",
-    "DescribeOrganizationOverviewResponseTypeDef",
-    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
-    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     "DescribeResourceCollectionHealthRequestRequestTypeDef",
-    "EndTimeRangeTypeDef",
     "EventResourceTypeDef",
-    "EventTimeRangeTypeDef",
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     "GetCostEstimationRequestRequestTypeDef",
     "ServiceResourceCostTypeDef",
-    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
     "GetResourceCollectionRequestRequestTypeDef",
     "InsightTimeRangeTypeDef",
     "KMSServerSideEncryptionIntegrationConfigTypeDef",
     "KMSServerSideEncryptionIntegrationTypeDef",
     "ServiceCollectionTypeDef",
-    "StartTimeRangeTypeDef",
-    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
     "ListAnomalousLogGroupsRequestRequestTypeDef",
     "ListInsightsOngoingStatusFilterTypeDef",
     "ListMonitoredResourcesFiltersTypeDef",
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
     "ListNotificationChannelsRequestRequestTypeDef",
-    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListRecommendationsRequestRequestTypeDef",
     "LogAnomalyClassTypeDef",
     "LogsAnomalyDetectionIntegrationConfigTypeDef",
     "LogsAnomalyDetectionIntegrationTypeDef",
-    "NotificationFilterConfigTypeDef",
+    "NotificationFilterConfigOutputTypeDef",
     "SnsChannelConfigTypeDef",
+    "NotificationFilterConfigTypeDef",
     "OpsCenterIntegrationConfigTypeDef",
     "OpsCenterIntegrationTypeDef",
-    "PaginatorConfigTypeDef",
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     "PerformanceInsightsStatTypeDef",
     "PerformanceInsightsReferenceScalarTypeDef",
     "PredictionTimeRangeTypeDef",
+    "ServiceCollectionOutputTypeDef",
     "RecommendationRelatedAnomalyResourceTypeDef",
     "RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef",
     "RecommendationRelatedEventResourceTypeDef",
     "RemoveNotificationChannelRequestRequestTypeDef",
     "TagCollectionFilterTypeDef",
+    "TagCollectionOutputTypeDef",
     "TagCollectionTypeDef",
-    "ResponseMetadataTypeDef",
     "ServiceInsightHealthTypeDef",
     "UpdateCloudFormationCollectionFilterTypeDef",
     "UpdateTagCollectionFilterTypeDef",
     "AccountHealthTypeDef",
+    "AddNotificationChannelResponseTypeDef",
+    "DescribeAccountHealthResponseTypeDef",
+    "DescribeAccountOverviewResponseTypeDef",
+    "DescribeOrganizationHealthResponseTypeDef",
+    "DescribeOrganizationOverviewResponseTypeDef",
     "EventSourcesConfigTypeDef",
     "CloudFormationHealthTypeDef",
     "TagHealthTypeDef",
     "CloudWatchMetricsDataSummaryTypeDef",
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
     "CostEstimationResourceCollectionFilterTypeDef",
+    "DescribeAccountOverviewRequestRequestTypeDef",
+    "DescribeOrganizationOverviewRequestRequestTypeDef",
+    "EndTimeRangeTypeDef",
+    "EventTimeRangeTypeDef",
+    "StartTimeRangeTypeDef",
     "DescribeFeedbackResponseTypeDef",
     "PutFeedbackRequestRequestTypeDef",
-    "ListInsightsClosedStatusFilterTypeDef",
+    "DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    "DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
+    "GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    "ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    "ListRecommendationsRequestListRecommendationsPaginateTypeDef",
     "ListAnomaliesForInsightFiltersTypeDef",
-    "ListInsightsAnyStatusFilterTypeDef",
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     "ListMonitoredResourcesRequestRequestTypeDef",
     "LogAnomalyShowcaseTypeDef",
+    "NotificationChannelConfigOutputTypeDef",
     "NotificationChannelConfigTypeDef",
     "UpdateServiceIntegrationConfigTypeDef",
     "ServiceIntegrationConfigTypeDef",
     "PerformanceInsightsMetricQueryTypeDef",
     "RecommendationRelatedAnomalySourceDetailTypeDef",
     "RecommendationRelatedEventTypeDef",
     "ResourceCollectionFilterTypeDef",
+    "ResourceCollectionOutputTypeDef",
     "ResourceCollectionTypeDef",
     "ServiceHealthTypeDef",
     "UpdateResourceCollectionFilterTypeDef",
     "DescribeEventSourcesConfigResponseTypeDef",
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     "CloudWatchMetricsDetailTypeDef",
     "GetCostEstimationResponseTypeDef",
+    "CostEstimationResourceCollectionFilterUnionTypeDef",
     "StartCostEstimationRequestRequestTypeDef",
+    "ListInsightsClosedStatusFilterTypeDef",
+    "ListInsightsAnyStatusFilterTypeDef",
     "ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     "ListAnomaliesForInsightRequestRequestTypeDef",
-    "ListInsightsStatusFilterTypeDef",
     "AnomalousLogGroupTypeDef",
-    "AddNotificationChannelRequestRequestTypeDef",
     "NotificationChannelTypeDef",
+    "AddNotificationChannelRequestRequestTypeDef",
+    "NotificationChannelConfigUnionTypeDef",
     "UpdateServiceIntegrationRequestRequestTypeDef",
     "DescribeServiceIntegrationResponseTypeDef",
     "PerformanceInsightsReferenceMetricTypeDef",
     "RecommendationRelatedAnomalyTypeDef",
     "GetResourceCollectionResponseTypeDef",
     "EventTypeDef",
-    "ListEventsFiltersTypeDef",
     "MonitoredResourceIdentifierTypeDef",
     "ProactiveInsightSummaryTypeDef",
     "ProactiveInsightTypeDef",
     "ProactiveOrganizationInsightSummaryTypeDef",
     "ReactiveInsightSummaryTypeDef",
     "ReactiveInsightTypeDef",
     "ReactiveOrganizationInsightSummaryTypeDef",
+    "ListEventsFiltersTypeDef",
     "SearchInsightsFiltersTypeDef",
     "SearchOrganizationInsightsFiltersTypeDef",
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     "DescribeResourceCollectionHealthResponseTypeDef",
     "UpdateResourceCollectionRequestRequestTypeDef",
-    "ListInsightsRequestListInsightsPaginateTypeDef",
-    "ListInsightsRequestRequestTypeDef",
-    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    "ListOrganizationInsightsRequestRequestTypeDef",
+    "ListInsightsStatusFilterTypeDef",
     "ListAnomalousLogGroupsResponseTypeDef",
     "ListNotificationChannelsResponseTypeDef",
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     "RecommendationTypeDef",
     "ListEventsResponseTypeDef",
-    "ListEventsRequestListEventsPaginateTypeDef",
-    "ListEventsRequestRequestTypeDef",
     "ListMonitoredResourcesResponseTypeDef",
     "ListInsightsResponseTypeDef",
     "SearchInsightsResponseTypeDef",
     "SearchOrganizationInsightsResponseTypeDef",
     "DescribeInsightResponseTypeDef",
     "ListOrganizationInsightsResponseTypeDef",
+    "ListEventsRequestListEventsPaginateTypeDef",
+    "ListEventsRequestRequestTypeDef",
     "SearchInsightsRequestRequestTypeDef",
     "SearchInsightsRequestSearchInsightsPaginateTypeDef",
     "SearchOrganizationInsightsRequestRequestTypeDef",
     "SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
+    "ListInsightsRequestListInsightsPaginateTypeDef",
+    "ListInsightsRequestRequestTypeDef",
+    "ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    "ListOrganizationInsightsRequestRequestTypeDef",
     "PerformanceInsightsReferenceDataTypeDef",
     "ListRecommendationsResponseTypeDef",
     "PerformanceInsightsMetricsDetailTypeDef",
     "AnomalySourceDetailsTypeDef",
     "ProactiveAnomalySummaryTypeDef",
     "ProactiveAnomalyTypeDef",
     "ReactiveAnomalySummaryTypeDef",
@@ -215,19 +227,22 @@
     {
         "OpenProactiveInsights": int,
         "OpenReactiveInsights": int,
     },
     total=False,
 )
 
-AddNotificationChannelResponseTypeDef = TypedDict(
-    "AddNotificationChannelResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AmazonCodeGuruProfilerIntegrationTypeDef = TypedDict(
     "AmazonCodeGuruProfilerIntegrationTypeDef",
     {
         "Status": EventSourceOptInStatusType,
@@ -294,26 +309,42 @@
     "CloudFormationCollectionFilterTypeDef",
     {
         "StackNames": List[str],
     },
     total=False,
 )
 
+CloudFormationCollectionOutputTypeDef = TypedDict(
+    "CloudFormationCollectionOutputTypeDef",
+    {
+        "StackNames": List[str],
+    },
+    total=False,
+)
+
 CloudFormationCollectionTypeDef = TypedDict(
     "CloudFormationCollectionTypeDef",
     {
+        "StackNames": Sequence[str],
+    },
+    total=False,
+)
+
+CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
         "StackNames": List[str],
     },
     total=False,
 )
 
 CloudFormationCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CloudFormationCostEstimationResourceCollectionFilterTypeDef",
     {
-        "StackNames": List[str],
+        "StackNames": Sequence[str],
     },
     total=False,
 )
 
 InsightHealthTypeDef = TypedDict(
     "InsightHealthTypeDef",
     {
@@ -338,19 +369,27 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
+TagCostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "TagCostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "AppBoundaryKey": str,
+        "TagValues": List[str],
+    },
+)
+
 TagCostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "TagCostEstimationResourceCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
-        "TagValues": List[str],
+        "TagValues": Sequence[str],
     },
 )
 
 CostEstimationTimeRangeTypeDef = TypedDict(
     "CostEstimationTimeRangeTypeDef",
     {
         "StartTime": datetime,
@@ -362,56 +401,15 @@
 DeleteInsightRequestRequestTypeDef = TypedDict(
     "DeleteInsightRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-DescribeAccountHealthResponseTypeDef = TypedDict(
-    "DescribeAccountHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "AnalyzedResourceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-class DescribeAccountOverviewRequestRequestTypeDef(
-    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
-    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
-):
-    pass
-
-DescribeAccountOverviewResponseTypeDef = TypedDict(
-    "DescribeAccountOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "MeanTimeToRecoverInMilliseconds": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredDescribeAnomalyRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAnomalyRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalDescribeAnomalyRequestRequestTypeDef = TypedDict(
@@ -468,79 +466,24 @@
     {
         "AccountIds": Sequence[str],
         "OrganizationalUnitIds": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationHealthResponseTypeDef = TypedDict(
-    "DescribeOrganizationHealthResponseTypeDef",
-    {
-        "OpenReactiveInsights": int,
-        "OpenProactiveInsights": int,
-        "MetricsAnalyzed": int,
-        "ResourceHours": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-    },
-)
-_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
-    {
-        "ToTime": Union[datetime, str],
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-    },
-    total=False,
-)
-
-class DescribeOrganizationOverviewRequestRequestTypeDef(
-    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
-    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
-):
-    pass
-
-DescribeOrganizationOverviewResponseTypeDef = TypedDict(
-    "DescribeOrganizationOverviewResponseTypeDef",
-    {
-        "ReactiveInsights": int,
-        "ProactiveInsights": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
-    {
-        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "MaxResults": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef",
     {
         "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
 _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -556,34 +499,14 @@
 
 class DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
-    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
-    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeResourceCollectionHealthRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef = TypedDict(
@@ -596,49 +519,24 @@
 
 class DescribeResourceCollectionHealthRequestRequestTypeDef(
     _RequiredDescribeResourceCollectionHealthRequestRequestTypeDef,
     _OptionalDescribeResourceCollectionHealthRequestRequestTypeDef,
 ):
     pass
 
-EndTimeRangeTypeDef = TypedDict(
-    "EndTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
 EventResourceTypeDef = TypedDict(
     "EventResourceTypeDef",
     {
         "Type": str,
         "Name": str,
         "Arn": str,
     },
     total=False,
 )
 
-EventTimeRangeTypeDef = TypedDict(
-    "EventTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-)
-
-GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
-    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetCostEstimationRequestRequestTypeDef = TypedDict(
     "GetCostEstimationRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
@@ -651,34 +549,14 @@
         "Count": int,
         "UnitCost": float,
         "Cost": float,
     },
     total=False,
 )
 
-_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "ResourceCollectionType": ResourceCollectionTypeType,
-    },
-)
-_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
-    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
-):
-    pass
-
 _RequiredGetResourceCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredGetResourceCollectionRequestRequestTypeDef",
     {
         "ResourceCollectionType": ResourceCollectionTypeType,
     },
 )
 _OptionalGetResourceCollectionRequestRequestTypeDef = TypedDict(
@@ -736,43 +614,14 @@
     "ServiceCollectionTypeDef",
     {
         "ServiceNames": Sequence[ServiceNameType],
     },
     total=False,
 )
 
-StartTimeRangeTypeDef = TypedDict(
-    "StartTimeRangeTypeDef",
-    {
-        "FromTime": Union[datetime, str],
-        "ToTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
-    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListAnomalousLogGroupsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomalousLogGroupsRequestRequestTypeDef = TypedDict(
@@ -801,52 +650,22 @@
     "ListMonitoredResourcesFiltersTypeDef",
     {
         "ResourcePermission": ResourcePermissionType,
         "ResourceTypeFilters": Sequence[ResourceTypeFilterType],
     },
 )
 
-ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
-    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNotificationChannelsRequestRequestTypeDef = TypedDict(
     "ListNotificationChannelsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "InsightId": str,
-    },
-)
-_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
-    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
-    {
-        "Locale": LocaleType,
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
-    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
-    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredListRecommendationsRequestRequestTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListRecommendationsRequestRequestTypeDef = TypedDict(
@@ -891,53 +710,52 @@
     "LogsAnomalyDetectionIntegrationTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
-NotificationFilterConfigTypeDef = TypedDict(
-    "NotificationFilterConfigTypeDef",
+NotificationFilterConfigOutputTypeDef = TypedDict(
+    "NotificationFilterConfigOutputTypeDef",
     {
-        "Severities": Sequence[InsightSeverityType],
-        "MessageTypes": Sequence[NotificationMessageTypeType],
+        "Severities": List[InsightSeverityType],
+        "MessageTypes": List[NotificationMessageTypeType],
     },
     total=False,
 )
 
 SnsChannelConfigTypeDef = TypedDict(
     "SnsChannelConfigTypeDef",
     {
         "TopicArn": str,
     },
     total=False,
 )
 
-OpsCenterIntegrationConfigTypeDef = TypedDict(
-    "OpsCenterIntegrationConfigTypeDef",
+NotificationFilterConfigTypeDef = TypedDict(
+    "NotificationFilterConfigTypeDef",
     {
-        "OptInStatus": OptInStatusType,
+        "Severities": Sequence[InsightSeverityType],
+        "MessageTypes": Sequence[NotificationMessageTypeType],
     },
     total=False,
 )
 
-OpsCenterIntegrationTypeDef = TypedDict(
-    "OpsCenterIntegrationTypeDef",
+OpsCenterIntegrationConfigTypeDef = TypedDict(
+    "OpsCenterIntegrationConfigTypeDef",
     {
         "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+OpsCenterIntegrationTypeDef = TypedDict(
+    "OpsCenterIntegrationTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "OptInStatus": OptInStatusType,
     },
     total=False,
 )
 
 PerformanceInsightsMetricDimensionGroupTypeDef = TypedDict(
     "PerformanceInsightsMetricDimensionGroupTypeDef",
     {
@@ -980,14 +798,22 @@
 )
 
 class PredictionTimeRangeTypeDef(
     _RequiredPredictionTimeRangeTypeDef, _OptionalPredictionTimeRangeTypeDef
 ):
     pass
 
+ServiceCollectionOutputTypeDef = TypedDict(
+    "ServiceCollectionOutputTypeDef",
+    {
+        "ServiceNames": List[ServiceNameType],
+    },
+    total=False,
+)
+
 RecommendationRelatedAnomalyResourceTypeDef = TypedDict(
     "RecommendationRelatedAnomalyResourceTypeDef",
     {
         "Name": str,
         "Type": str,
     },
     total=False,
@@ -1022,30 +848,27 @@
     "TagCollectionFilterTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
-TagCollectionTypeDef = TypedDict(
-    "TagCollectionTypeDef",
+TagCollectionOutputTypeDef = TypedDict(
+    "TagCollectionOutputTypeDef",
     {
         "AppBoundaryKey": str,
         "TagValues": List[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+TagCollectionTypeDef = TypedDict(
+    "TagCollectionTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "AppBoundaryKey": str,
+        "TagValues": Sequence[str],
     },
 )
 
 ServiceInsightHealthTypeDef = TypedDict(
     "ServiceInsightHealthTypeDef",
     {
         "OpenProactiveInsights": int,
@@ -1075,14 +898,64 @@
     {
         "AccountId": str,
         "Insight": AccountInsightHealthTypeDef,
     },
     total=False,
 )
 
+AddNotificationChannelResponseTypeDef = TypedDict(
+    "AddNotificationChannelResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountHealthResponseTypeDef = TypedDict(
+    "DescribeAccountHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "AnalyzedResourceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountOverviewResponseTypeDef = TypedDict(
+    "DescribeAccountOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "MeanTimeToRecoverInMilliseconds": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationHealthResponseTypeDef = TypedDict(
+    "DescribeOrganizationHealthResponseTypeDef",
+    {
+        "OpenReactiveInsights": int,
+        "OpenProactiveInsights": int,
+        "MetricsAnalyzed": int,
+        "ResourceHours": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationOverviewResponseTypeDef = TypedDict(
+    "DescribeOrganizationOverviewResponseTypeDef",
+    {
+        "ReactiveInsights": int,
+        "ProactiveInsights": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 EventSourcesConfigTypeDef = TypedDict(
     "EventSourcesConfigTypeDef",
     {
         "AmazonCodeGuruProfiler": AmazonCodeGuruProfilerIntegrationTypeDef,
     },
     total=False,
 )
@@ -1113,68 +986,250 @@
     {
         "TimestampMetricValuePairList": List[TimestampMetricValuePairTypeDef],
         "StatusCode": CloudWatchMetricDataStatusCodeType,
     },
     total=False,
 )
 
+CostEstimationResourceCollectionFilterOutputTypeDef = TypedDict(
+    "CostEstimationResourceCollectionFilterOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
+        "Tags": List[TagCostEstimationResourceCollectionFilterOutputTypeDef],
+    },
+    total=False,
+)
+
 CostEstimationResourceCollectionFilterTypeDef = TypedDict(
     "CostEstimationResourceCollectionFilterTypeDef",
     {
         "CloudFormation": CloudFormationCostEstimationResourceCollectionFilterTypeDef,
-        "Tags": List[TagCostEstimationResourceCollectionFilterTypeDef],
+        "Tags": Sequence[TagCostEstimationResourceCollectionFilterTypeDef],
+    },
+    total=False,
+)
+
+_RequiredDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeAccountOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeAccountOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAccountOverviewRequestRequestTypeDef(
+    _RequiredDescribeAccountOverviewRequestRequestTypeDef,
+    _OptionalDescribeAccountOverviewRequestRequestTypeDef,
+):
+    pass
+
+_RequiredDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+    },
+)
+_OptionalDescribeOrganizationOverviewRequestRequestTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationOverviewRequestRequestTypeDef",
+    {
+        "ToTime": TimestampTypeDef,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+    },
+    total=False,
+)
+
+class DescribeOrganizationOverviewRequestRequestTypeDef(
+    _RequiredDescribeOrganizationOverviewRequestRequestTypeDef,
+    _OptionalDescribeOrganizationOverviewRequestRequestTypeDef,
+):
+    pass
+
+EndTimeRangeTypeDef = TypedDict(
+    "EndTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+EventTimeRangeTypeDef = TypedDict(
+    "EventTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
+    },
+)
+
+StartTimeRangeTypeDef = TypedDict(
+    "StartTimeRangeTypeDef",
+    {
+        "FromTime": TimestampTypeDef,
+        "ToTime": TimestampTypeDef,
     },
     total=False,
 )
 
 DescribeFeedbackResponseTypeDef = TypedDict(
     "DescribeFeedbackResponseTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutFeedbackRequestRequestTypeDef = TypedDict(
     "PutFeedbackRequestRequestTypeDef",
     {
         "InsightFeedback": InsightFeedbackTypeDef,
     },
     total=False,
 )
 
-ListInsightsClosedStatusFilterTypeDef = TypedDict(
-    "ListInsightsClosedStatusFilterTypeDef",
+_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
     {
-        "Type": InsightTypeType,
-        "EndTimeRange": EndTimeRangeTypeDef,
+        "OrganizationResourceCollectionType": OrganizationResourceCollectionTypeType,
     },
 )
+_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "MaxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListAnomaliesForInsightFiltersTypeDef = TypedDict(
-    "ListAnomaliesForInsightFiltersTypeDef",
+class DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
     {
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef = TypedDict(
+    "_OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ListInsightsAnyStatusFilterTypeDef = TypedDict(
-    "ListInsightsAnyStatusFilterTypeDef",
+class DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef(
+    _RequiredDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    _OptionalDescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+):
+    pass
+
+GetCostEstimationRequestGetCostEstimationPaginateTypeDef = TypedDict(
+    "GetCostEstimationRequestGetCostEstimationPaginateTypeDef",
     {
-        "Type": InsightTypeType,
-        "StartTimeRange": StartTimeRangeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "ResourceCollectionType": ResourceCollectionTypeType,
+    },
+)
+_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef(
+    _RequiredGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    _OptionalGetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+):
+    pass
+
+_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef(
+    _RequiredListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    _OptionalListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+):
+    pass
+
+ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef = TypedDict(
+    "ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "InsightId": str,
+    },
+)
+_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef = TypedDict(
+    "_OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef",
+    {
+        "Locale": LocaleType,
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRecommendationsRequestListRecommendationsPaginateTypeDef(
+    _RequiredListRecommendationsRequestListRecommendationsPaginateTypeDef,
+    _OptionalListRecommendationsRequestListRecommendationsPaginateTypeDef,
+):
+    pass
+
+ListAnomaliesForInsightFiltersTypeDef = TypedDict(
+    "ListAnomaliesForInsightFiltersTypeDef",
+    {
+        "ServiceCollection": ServiceCollectionTypeDef,
+    },
+    total=False,
 )
 
 ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef = TypedDict(
     "ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef",
     {
         "Filters": ListMonitoredResourcesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListMonitoredResourcesRequestRequestTypeDef = TypedDict(
     "ListMonitoredResourcesRequestRequestTypeDef",
     {
@@ -1189,14 +1244,33 @@
     "LogAnomalyShowcaseTypeDef",
     {
         "LogAnomalyClasses": List[LogAnomalyClassTypeDef],
     },
     total=False,
 )
 
+_RequiredNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_RequiredNotificationChannelConfigOutputTypeDef",
+    {
+        "Sns": SnsChannelConfigTypeDef,
+    },
+)
+_OptionalNotificationChannelConfigOutputTypeDef = TypedDict(
+    "_OptionalNotificationChannelConfigOutputTypeDef",
+    {
+        "Filters": NotificationFilterConfigOutputTypeDef,
+    },
+    total=False,
+)
+
+class NotificationChannelConfigOutputTypeDef(
+    _RequiredNotificationChannelConfigOutputTypeDef, _OptionalNotificationChannelConfigOutputTypeDef
+):
+    pass
+
 _RequiredNotificationChannelConfigTypeDef = TypedDict(
     "_RequiredNotificationChannelConfigTypeDef",
     {
         "Sns": SnsChannelConfigTypeDef,
     },
 )
 _OptionalNotificationChannelConfigTypeDef = TypedDict(
@@ -1264,19 +1338,28 @@
     {
         "CloudFormation": CloudFormationCollectionFilterTypeDef,
         "Tags": List[TagCollectionFilterTypeDef],
     },
     total=False,
 )
 
+ResourceCollectionOutputTypeDef = TypedDict(
+    "ResourceCollectionOutputTypeDef",
+    {
+        "CloudFormation": CloudFormationCollectionOutputTypeDef,
+        "Tags": List[TagCollectionOutputTypeDef],
+    },
+    total=False,
+)
+
 ResourceCollectionTypeDef = TypedDict(
     "ResourceCollectionTypeDef",
     {
         "CloudFormation": CloudFormationCollectionTypeDef,
-        "Tags": List[TagCollectionTypeDef],
+        "Tags": Sequence[TagCollectionTypeDef],
     },
     total=False,
 )
 
 ServiceHealthTypeDef = TypedDict(
     "ServiceHealthTypeDef",
     {
@@ -1296,15 +1379,15 @@
     total=False,
 )
 
 DescribeEventSourcesConfigResponseTypeDef = TypedDict(
     "DescribeEventSourcesConfigResponseTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEventSourcesConfigRequestRequestTypeDef = TypedDict(
     "UpdateEventSourcesConfigRequestRequestTypeDef",
     {
         "EventSources": EventSourcesConfigTypeDef,
@@ -1325,24 +1408,28 @@
     },
     total=False,
 )
 
 GetCostEstimationResponseTypeDef = TypedDict(
     "GetCostEstimationResponseTypeDef",
     {
-        "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
+        "ResourceCollection": CostEstimationResourceCollectionFilterOutputTypeDef,
         "Status": CostEstimationStatusType,
         "Costs": List[ServiceResourceCostTypeDef],
         "TimeRange": CostEstimationTimeRangeTypeDef,
         "TotalCost": float,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+CostEstimationResourceCollectionFilterUnionTypeDef = Union[
+    CostEstimationResourceCollectionFilterTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
+]
 _RequiredStartCostEstimationRequestRequestTypeDef = TypedDict(
     "_RequiredStartCostEstimationRequestRequestTypeDef",
     {
         "ResourceCollection": CostEstimationResourceCollectionFilterTypeDef,
     },
 )
 _OptionalStartCostEstimationRequestRequestTypeDef = TypedDict(
@@ -1355,27 +1442,43 @@
 
 class StartCostEstimationRequestRequestTypeDef(
     _RequiredStartCostEstimationRequestRequestTypeDef,
     _OptionalStartCostEstimationRequestRequestTypeDef,
 ):
     pass
 
+ListInsightsClosedStatusFilterTypeDef = TypedDict(
+    "ListInsightsClosedStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "EndTimeRange": EndTimeRangeTypeDef,
+    },
+)
+
+ListInsightsAnyStatusFilterTypeDef = TypedDict(
+    "ListInsightsAnyStatusFilterTypeDef",
+    {
+        "Type": InsightTypeType,
+        "StartTimeRange": StartTimeRangeTypeDef,
+    },
+)
+
 _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "InsightId": str,
     },
 )
 _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef = TypedDict(
     "_OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "AccountId": str,
         "Filters": ListAnomaliesForInsightFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef(
     _RequiredListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     _OptionalListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
@@ -1402,64 +1505,57 @@
 
 class ListAnomaliesForInsightRequestRequestTypeDef(
     _RequiredListAnomaliesForInsightRequestRequestTypeDef,
     _OptionalListAnomaliesForInsightRequestRequestTypeDef,
 ):
     pass
 
-ListInsightsStatusFilterTypeDef = TypedDict(
-    "ListInsightsStatusFilterTypeDef",
-    {
-        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
-        "Closed": ListInsightsClosedStatusFilterTypeDef,
-        "Any": ListInsightsAnyStatusFilterTypeDef,
-    },
-    total=False,
-)
-
 AnomalousLogGroupTypeDef = TypedDict(
     "AnomalousLogGroupTypeDef",
     {
         "LogGroupName": str,
         "ImpactStartTime": datetime,
         "ImpactEndTime": datetime,
         "NumberOfLogLinesScanned": int,
         "LogAnomalyShowcases": List[LogAnomalyShowcaseTypeDef],
     },
     total=False,
 )
 
-AddNotificationChannelRequestRequestTypeDef = TypedDict(
-    "AddNotificationChannelRequestRequestTypeDef",
+NotificationChannelTypeDef = TypedDict(
+    "NotificationChannelTypeDef",
     {
-        "Config": NotificationChannelConfigTypeDef,
+        "Id": str,
+        "Config": NotificationChannelConfigOutputTypeDef,
     },
+    total=False,
 )
 
-NotificationChannelTypeDef = TypedDict(
-    "NotificationChannelTypeDef",
+AddNotificationChannelRequestRequestTypeDef = TypedDict(
+    "AddNotificationChannelRequestRequestTypeDef",
     {
-        "Id": str,
         "Config": NotificationChannelConfigTypeDef,
     },
-    total=False,
 )
 
+NotificationChannelConfigUnionTypeDef = Union[
+    NotificationChannelConfigTypeDef, NotificationChannelConfigOutputTypeDef
+]
 UpdateServiceIntegrationRequestRequestTypeDef = TypedDict(
     "UpdateServiceIntegrationRequestRequestTypeDef",
     {
         "ServiceIntegration": UpdateServiceIntegrationConfigTypeDef,
     },
 )
 
 DescribeServiceIntegrationResponseTypeDef = TypedDict(
     "DescribeServiceIntegrationResponseTypeDef",
     {
         "ServiceIntegration": ServiceIntegrationConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceMetricTypeDef = TypedDict(
     "PerformanceInsightsReferenceMetricTypeDef",
     {
         "MetricQuery": PerformanceInsightsMetricQueryTypeDef,
@@ -1478,84 +1574,71 @@
 )
 
 GetResourceCollectionResponseTypeDef = TypedDict(
     "GetResourceCollectionResponseTypeDef",
     {
         "ResourceCollection": ResourceCollectionFilterTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EventTypeDef = TypedDict(
     "EventTypeDef",
     {
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Id": str,
         "Time": datetime,
         "EventSource": str,
         "Name": str,
         "DataSource": EventDataSourceType,
         "EventClass": EventClassType,
         "Resources": List[EventResourceTypeDef],
     },
     total=False,
 )
 
-ListEventsFiltersTypeDef = TypedDict(
-    "ListEventsFiltersTypeDef",
-    {
-        "InsightId": str,
-        "EventTimeRange": EventTimeRangeTypeDef,
-        "EventClass": EventClassType,
-        "EventSource": str,
-        "DataSource": EventDataSourceType,
-        "ResourceCollection": ResourceCollectionTypeDef,
-    },
-    total=False,
-)
-
 MonitoredResourceIdentifierTypeDef = TypedDict(
     "MonitoredResourceIdentifierTypeDef",
     {
         "MonitoredResourceName": str,
         "Type": str,
         "ResourcePermission": ResourcePermissionType,
         "LastUpdated": datetime,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ProactiveInsightSummaryTypeDef = TypedDict(
     "ProactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ProactiveInsightTypeDef = TypedDict(
     "ProactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ProactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1565,44 +1648,44 @@
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
     },
     total=False,
 )
 
 ReactiveInsightSummaryTypeDef = TypedDict(
     "ReactiveInsightSummaryTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
         "AssociatedResourceArns": List[str],
     },
     total=False,
 )
 
 ReactiveInsightTypeDef = TypedDict(
     "ReactiveInsightTypeDef",
     {
         "Id": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "SsmOpsItemId": str,
         "Description": str,
     },
     total=False,
 )
 
 ReactiveOrganizationInsightSummaryTypeDef = TypedDict(
@@ -1611,16 +1694,29 @@
         "Id": str,
         "AccountId": str,
         "OrganizationalUnitId": str,
         "Name": str,
         "Severity": InsightSeverityType,
         "Status": InsightStatusType,
         "InsightTimeRange": InsightTimeRangeTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
+        "ServiceCollection": ServiceCollectionOutputTypeDef,
+    },
+    total=False,
+)
+
+ListEventsFiltersTypeDef = TypedDict(
+    "ListEventsFiltersTypeDef",
+    {
+        "InsightId": str,
+        "EventTimeRange": EventTimeRangeTypeDef,
+        "EventClass": EventClassType,
+        "EventSource": str,
+        "DataSource": EventDataSourceType,
         "ResourceCollection": ResourceCollectionTypeDef,
-        "ServiceCollection": ServiceCollectionTypeDef,
     },
     total=False,
 )
 
 SearchInsightsFiltersTypeDef = TypedDict(
     "SearchInsightsFiltersTypeDef",
     {
@@ -1647,138 +1743,63 @@
     "DescribeOrganizationResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "Account": List[AccountHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceCollectionHealthResponseTypeDef = TypedDict(
     "DescribeResourceCollectionHealthResponseTypeDef",
     {
         "CloudFormation": List[CloudFormationHealthTypeDef],
         "Service": List[ServiceHealthTypeDef],
         "NextToken": str,
         "Tags": List[TagHealthTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceCollectionRequestRequestTypeDef = TypedDict(
     "UpdateResourceCollectionRequestRequestTypeDef",
     {
         "Action": UpdateResourceCollectionActionType,
         "ResourceCollection": UpdateResourceCollectionFilterTypeDef,
     },
 )
 
-_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListInsightsRequestListInsightsPaginateTypeDef(
-    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
-    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
-):
-    pass
-
-_RequiredListInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListInsightsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-    },
-    total=False,
-)
-
-class ListInsightsRequestRequestTypeDef(
-    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
-):
-    pass
-
-_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
-    {
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
-    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-):
-    pass
-
-_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
-    {
-        "StatusFilter": ListInsightsStatusFilterTypeDef,
-    },
-)
-_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
-    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+ListInsightsStatusFilterTypeDef = TypedDict(
+    "ListInsightsStatusFilterTypeDef",
     {
-        "MaxResults": int,
-        "AccountIds": Sequence[str],
-        "OrganizationalUnitIds": Sequence[str],
-        "NextToken": str,
+        "Ongoing": ListInsightsOngoingStatusFilterTypeDef,
+        "Closed": ListInsightsClosedStatusFilterTypeDef,
+        "Any": ListInsightsAnyStatusFilterTypeDef,
     },
     total=False,
 )
 
-class ListOrganizationInsightsRequestRequestTypeDef(
-    _RequiredListOrganizationInsightsRequestRequestTypeDef,
-    _OptionalListOrganizationInsightsRequestRequestTypeDef,
-):
-    pass
-
 ListAnomalousLogGroupsResponseTypeDef = TypedDict(
     "ListAnomalousLogGroupsResponseTypeDef",
     {
         "InsightId": str,
         "AnomalousLogGroups": List[AnomalousLogGroupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotificationChannelsResponseTypeDef = TypedDict(
     "ListNotificationChannelsResponseTypeDef",
     {
         "Channels": List[NotificationChannelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsReferenceComparisonValuesTypeDef = TypedDict(
     "PerformanceInsightsReferenceComparisonValuesTypeDef",
     {
         "ReferenceScalar": PerformanceInsightsReferenceScalarTypeDef,
@@ -1802,118 +1823,118 @@
 )
 
 ListEventsResponseTypeDef = TypedDict(
     "ListEventsResponseTypeDef",
     {
         "Events": List[EventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_RequiredListEventsRequestListEventsPaginateTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
-    "_OptionalListEventsRequestListEventsPaginateTypeDef",
-    {
-        "AccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListEventsRequestListEventsPaginateTypeDef(
-    _RequiredListEventsRequestListEventsPaginateTypeDef,
-    _OptionalListEventsRequestListEventsPaginateTypeDef,
-):
-    pass
-
-_RequiredListEventsRequestRequestTypeDef = TypedDict(
-    "_RequiredListEventsRequestRequestTypeDef",
-    {
-        "Filters": ListEventsFiltersTypeDef,
-    },
-)
-_OptionalListEventsRequestRequestTypeDef = TypedDict(
-    "_OptionalListEventsRequestRequestTypeDef",
-    {
-        "MaxResults": int,
-        "NextToken": str,
-        "AccountId": str,
-    },
-    total=False,
-)
-
-class ListEventsRequestRequestTypeDef(
-    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
-):
-    pass
-
 ListMonitoredResourcesResponseTypeDef = TypedDict(
     "ListMonitoredResourcesResponseTypeDef",
     {
         "MonitoredResourceIdentifiers": List[MonitoredResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInsightsResponseTypeDef = TypedDict(
     "ListInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchInsightsResponseTypeDef = TypedDict(
     "SearchInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchOrganizationInsightsResponseTypeDef = TypedDict(
     "SearchOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInsightResponseTypeDef = TypedDict(
     "DescribeInsightResponseTypeDef",
     {
         "ProactiveInsight": ProactiveInsightTypeDef,
         "ReactiveInsight": ReactiveInsightTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListOrganizationInsightsResponseTypeDef = TypedDict(
     "ListOrganizationInsightsResponseTypeDef",
     {
         "ProactiveInsights": List[ProactiveOrganizationInsightSummaryTypeDef],
         "ReactiveInsights": List[ReactiveOrganizationInsightSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_RequiredListEventsRequestListEventsPaginateTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestListEventsPaginateTypeDef = TypedDict(
+    "_OptionalListEventsRequestListEventsPaginateTypeDef",
+    {
+        "AccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEventsRequestListEventsPaginateTypeDef(
+    _RequiredListEventsRequestListEventsPaginateTypeDef,
+    _OptionalListEventsRequestListEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListEventsRequestRequestTypeDef = TypedDict(
+    "_RequiredListEventsRequestRequestTypeDef",
+    {
+        "Filters": ListEventsFiltersTypeDef,
+    },
+)
+_OptionalListEventsRequestRequestTypeDef = TypedDict(
+    "_OptionalListEventsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+        "AccountId": str,
+    },
+    total=False,
+)
+
+class ListEventsRequestRequestTypeDef(
+    _RequiredListEventsRequestRequestTypeDef, _OptionalListEventsRequestRequestTypeDef
+):
+    pass
+
 _RequiredSearchInsightsRequestRequestTypeDef = TypedDict(
     "_RequiredSearchInsightsRequestRequestTypeDef",
     {
         "StartTimeRange": StartTimeRangeTypeDef,
         "Type": InsightTypeType,
     },
 )
@@ -1939,15 +1960,15 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef",
     {
         "Filters": SearchInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchInsightsRequestSearchInsightsPaginateTypeDef(
     _RequiredSearchInsightsRequestSearchInsightsPaginateTypeDef,
     _OptionalSearchInsightsRequestSearchInsightsPaginateTypeDef,
@@ -1986,40 +2007,125 @@
         "Type": InsightTypeType,
     },
 )
 _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef = TypedDict(
     "_OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef",
     {
         "Filters": SearchOrganizationInsightsFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef(
     _RequiredSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
     _OptionalSearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
 ):
     pass
 
+_RequiredListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestListInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListInsightsRequestListInsightsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListInsightsRequestListInsightsPaginateTypeDef(
+    _RequiredListInsightsRequestListInsightsPaginateTypeDef,
+    _OptionalListInsightsRequestListInsightsPaginateTypeDef,
+):
+    pass
+
+_RequiredListInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListInsightsRequestRequestTypeDef(
+    _RequiredListInsightsRequestRequestTypeDef, _OptionalListInsightsRequestRequestTypeDef
+):
+    pass
+
+_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef",
+    {
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef(
+    _RequiredListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    _OptionalListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+):
+    pass
+
+_RequiredListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_RequiredListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "StatusFilter": ListInsightsStatusFilterTypeDef,
+    },
+)
+_OptionalListOrganizationInsightsRequestRequestTypeDef = TypedDict(
+    "_OptionalListOrganizationInsightsRequestRequestTypeDef",
+    {
+        "MaxResults": int,
+        "AccountIds": Sequence[str],
+        "OrganizationalUnitIds": Sequence[str],
+        "NextToken": str,
+    },
+    total=False,
+)
+
+class ListOrganizationInsightsRequestRequestTypeDef(
+    _RequiredListOrganizationInsightsRequestRequestTypeDef,
+    _OptionalListOrganizationInsightsRequestRequestTypeDef,
+):
+    pass
+
 PerformanceInsightsReferenceDataTypeDef = TypedDict(
     "PerformanceInsightsReferenceDataTypeDef",
     {
         "Name": str,
         "ComparisonValues": PerformanceInsightsReferenceComparisonValuesTypeDef,
     },
     total=False,
 )
 
 ListRecommendationsResponseTypeDef = TypedDict(
     "ListRecommendationsResponseTypeDef",
     {
         "Recommendations": List[RecommendationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PerformanceInsightsMetricsDetailTypeDef = TypedDict(
     "PerformanceInsightsMetricsDetailTypeDef",
     {
         "MetricDisplayName": str,
@@ -2049,15 +2155,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2070,15 +2176,15 @@
         "Status": AnomalyStatusType,
         "UpdateTime": datetime,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "PredictionTimeRange": PredictionTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Limit": float,
         "SourceMetadata": AnomalySourceMetadataTypeDef,
         "AnomalyResources": List[AnomalyResourceTypeDef],
         "Description": str,
     },
     total=False,
 )
@@ -2089,15 +2195,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2109,15 +2215,15 @@
         "Id": str,
         "Severity": AnomalySeverityType,
         "Status": AnomalyStatusType,
         "AnomalyTimeRange": AnomalyTimeRangeTypeDef,
         "AnomalyReportedTimeRange": AnomalyReportedTimeRangeTypeDef,
         "SourceDetails": AnomalySourceDetailsTypeDef,
         "AssociatedInsightId": str,
-        "ResourceCollection": ResourceCollectionTypeDef,
+        "ResourceCollection": ResourceCollectionOutputTypeDef,
         "Type": AnomalyTypeType,
         "Name": str,
         "Description": str,
         "CausalAnomalyId": str,
         "AnomalyResources": List[AnomalyResourceTypeDef],
     },
     total=False,
@@ -2125,19 +2231,19 @@
 
 ListAnomaliesForInsightResponseTypeDef = TypedDict(
     "ListAnomaliesForInsightResponseTypeDef",
     {
         "ProactiveAnomalies": List[ProactiveAnomalySummaryTypeDef],
         "ReactiveAnomalies": List[ReactiveAnomalySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAnomalyResponseTypeDef = TypedDict(
     "DescribeAnomalyResponseTypeDef",
     {
         "ProactiveAnomaly": ProactiveAnomalyTypeDef,
         "ReactiveAnomaly": ReactiveAnomalyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/PKG-INFO` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-devops-guru
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DevOpsGuru 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore devops-guru type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore devops-guru type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-devops-guru"></a>
 
 # types-aiobotocore-devops-guru
 
 [![PyPI - types-aiobotocore-devops-guru](https://img.shields.io/pypi/v/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-devops-guru.svg?color=blue)](https://pypi.org/project/types-aiobotocore-devops-guru)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-devops-guru?color=blue)](https://pypistats.org/packages/types-aiobotocore-devops-guru)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-devops-guru)](https://pepy.tech/project/types-aiobotocore-devops-guru)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DevOpsGuru 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/devops-guru.html#DevOpsGuru)
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
 [types-aiobotocore-devops-guru docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_devops_guru/).
 
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
@@ -393,186 +392,198 @@
 )
 
 
 def check_value(value: AnomalySeverityType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_devops_guru.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_devops_guru.type_defs import (
     AccountInsightHealthTypeDef,
-    AddNotificationChannelResponseTypeDef,
+    ResponseMetadataTypeDef,
     AmazonCodeGuruProfilerIntegrationTypeDef,
     AnomalyReportedTimeRangeTypeDef,
     AnomalyResourceTypeDef,
     AnomalySourceMetadataTypeDef,
     AnomalyTimeRangeTypeDef,
     CloudFormationCollectionFilterTypeDef,
+    CloudFormationCollectionOutputTypeDef,
     CloudFormationCollectionTypeDef,
+    CloudFormationCostEstimationResourceCollectionFilterOutputTypeDef,
     CloudFormationCostEstimationResourceCollectionFilterTypeDef,
     InsightHealthTypeDef,
     TimestampMetricValuePairTypeDef,
     CloudWatchMetricsDimensionTypeDef,
+    TagCostEstimationResourceCollectionFilterOutputTypeDef,
     TagCostEstimationResourceCollectionFilterTypeDef,
     CostEstimationTimeRangeTypeDef,
     DeleteInsightRequestRequestTypeDef,
-    DescribeAccountHealthResponseTypeDef,
-    DescribeAccountOverviewRequestRequestTypeDef,
-    DescribeAccountOverviewResponseTypeDef,
+    TimestampTypeDef,
     DescribeAnomalyRequestRequestTypeDef,
     DescribeFeedbackRequestRequestTypeDef,
     InsightFeedbackTypeDef,
     DescribeInsightRequestRequestTypeDef,
     DescribeOrganizationHealthRequestRequestTypeDef,
-    DescribeOrganizationHealthResponseTypeDef,
-    DescribeOrganizationOverviewRequestRequestTypeDef,
-    DescribeOrganizationOverviewResponseTypeDef,
-    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeOrganizationResourceCollectionHealthRequestRequestTypeDef,
-    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
     DescribeResourceCollectionHealthRequestRequestTypeDef,
-    EndTimeRangeTypeDef,
     EventResourceTypeDef,
-    EventTimeRangeTypeDef,
-    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
     GetCostEstimationRequestRequestTypeDef,
     ServiceResourceCostTypeDef,
-    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
     GetResourceCollectionRequestRequestTypeDef,
     InsightTimeRangeTypeDef,
     KMSServerSideEncryptionIntegrationConfigTypeDef,
     KMSServerSideEncryptionIntegrationTypeDef,
     ServiceCollectionTypeDef,
-    StartTimeRangeTypeDef,
-    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
     ListAnomalousLogGroupsRequestRequestTypeDef,
     ListInsightsOngoingStatusFilterTypeDef,
     ListMonitoredResourcesFiltersTypeDef,
-    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
     ListNotificationChannelsRequestRequestTypeDef,
-    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListRecommendationsRequestRequestTypeDef,
     LogAnomalyClassTypeDef,
     LogsAnomalyDetectionIntegrationConfigTypeDef,
     LogsAnomalyDetectionIntegrationTypeDef,
-    NotificationFilterConfigTypeDef,
+    NotificationFilterConfigOutputTypeDef,
     SnsChannelConfigTypeDef,
+    NotificationFilterConfigTypeDef,
     OpsCenterIntegrationConfigTypeDef,
     OpsCenterIntegrationTypeDef,
-    PaginatorConfigTypeDef,
     PerformanceInsightsMetricDimensionGroupTypeDef,
     PerformanceInsightsStatTypeDef,
     PerformanceInsightsReferenceScalarTypeDef,
     PredictionTimeRangeTypeDef,
+    ServiceCollectionOutputTypeDef,
     RecommendationRelatedAnomalyResourceTypeDef,
     RecommendationRelatedCloudWatchMetricsSourceDetailTypeDef,
     RecommendationRelatedEventResourceTypeDef,
     RemoveNotificationChannelRequestRequestTypeDef,
     TagCollectionFilterTypeDef,
+    TagCollectionOutputTypeDef,
     TagCollectionTypeDef,
-    ResponseMetadataTypeDef,
     ServiceInsightHealthTypeDef,
     UpdateCloudFormationCollectionFilterTypeDef,
     UpdateTagCollectionFilterTypeDef,
     AccountHealthTypeDef,
+    AddNotificationChannelResponseTypeDef,
+    DescribeAccountHealthResponseTypeDef,
+    DescribeAccountOverviewResponseTypeDef,
+    DescribeOrganizationHealthResponseTypeDef,
+    DescribeOrganizationOverviewResponseTypeDef,
     EventSourcesConfigTypeDef,
     CloudFormationHealthTypeDef,
     TagHealthTypeDef,
     CloudWatchMetricsDataSummaryTypeDef,
+    CostEstimationResourceCollectionFilterOutputTypeDef,
     CostEstimationResourceCollectionFilterTypeDef,
+    DescribeAccountOverviewRequestRequestTypeDef,
+    DescribeOrganizationOverviewRequestRequestTypeDef,
+    EndTimeRangeTypeDef,
+    EventTimeRangeTypeDef,
+    StartTimeRangeTypeDef,
     DescribeFeedbackResponseTypeDef,
     PutFeedbackRequestRequestTypeDef,
-    ListInsightsClosedStatusFilterTypeDef,
+    DescribeOrganizationResourceCollectionHealthRequestDescribeOrganizationResourceCollectionHealthPaginateTypeDef,
+    DescribeResourceCollectionHealthRequestDescribeResourceCollectionHealthPaginateTypeDef,
+    GetCostEstimationRequestGetCostEstimationPaginateTypeDef,
+    GetResourceCollectionRequestGetResourceCollectionPaginateTypeDef,
+    ListAnomalousLogGroupsRequestListAnomalousLogGroupsPaginateTypeDef,
+    ListNotificationChannelsRequestListNotificationChannelsPaginateTypeDef,
+    ListRecommendationsRequestListRecommendationsPaginateTypeDef,
     ListAnomaliesForInsightFiltersTypeDef,
-    ListInsightsAnyStatusFilterTypeDef,
     ListMonitoredResourcesRequestListMonitoredResourcesPaginateTypeDef,
     ListMonitoredResourcesRequestRequestTypeDef,
     LogAnomalyShowcaseTypeDef,
+    NotificationChannelConfigOutputTypeDef,
     NotificationChannelConfigTypeDef,
     UpdateServiceIntegrationConfigTypeDef,
     ServiceIntegrationConfigTypeDef,
     PerformanceInsightsMetricQueryTypeDef,
     RecommendationRelatedAnomalySourceDetailTypeDef,
     RecommendationRelatedEventTypeDef,
     ResourceCollectionFilterTypeDef,
+    ResourceCollectionOutputTypeDef,
     ResourceCollectionTypeDef,
     ServiceHealthTypeDef,
     UpdateResourceCollectionFilterTypeDef,
     DescribeEventSourcesConfigResponseTypeDef,
     UpdateEventSourcesConfigRequestRequestTypeDef,
     CloudWatchMetricsDetailTypeDef,
     GetCostEstimationResponseTypeDef,
+    CostEstimationResourceCollectionFilterUnionTypeDef,
     StartCostEstimationRequestRequestTypeDef,
+    ListInsightsClosedStatusFilterTypeDef,
+    ListInsightsAnyStatusFilterTypeDef,
     ListAnomaliesForInsightRequestListAnomaliesForInsightPaginateTypeDef,
     ListAnomaliesForInsightRequestRequestTypeDef,
-    ListInsightsStatusFilterTypeDef,
     AnomalousLogGroupTypeDef,
-    AddNotificationChannelRequestRequestTypeDef,
     NotificationChannelTypeDef,
+    AddNotificationChannelRequestRequestTypeDef,
+    NotificationChannelConfigUnionTypeDef,
     UpdateServiceIntegrationRequestRequestTypeDef,
     DescribeServiceIntegrationResponseTypeDef,
     PerformanceInsightsReferenceMetricTypeDef,
     RecommendationRelatedAnomalyTypeDef,
     GetResourceCollectionResponseTypeDef,
     EventTypeDef,
-    ListEventsFiltersTypeDef,
     MonitoredResourceIdentifierTypeDef,
     ProactiveInsightSummaryTypeDef,
     ProactiveInsightTypeDef,
     ProactiveOrganizationInsightSummaryTypeDef,
     ReactiveInsightSummaryTypeDef,
     ReactiveInsightTypeDef,
     ReactiveOrganizationInsightSummaryTypeDef,
+    ListEventsFiltersTypeDef,
     SearchInsightsFiltersTypeDef,
     SearchOrganizationInsightsFiltersTypeDef,
     DescribeOrganizationResourceCollectionHealthResponseTypeDef,
     DescribeResourceCollectionHealthResponseTypeDef,
     UpdateResourceCollectionRequestRequestTypeDef,
-    ListInsightsRequestListInsightsPaginateTypeDef,
-    ListInsightsRequestRequestTypeDef,
-    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
-    ListOrganizationInsightsRequestRequestTypeDef,
+    ListInsightsStatusFilterTypeDef,
     ListAnomalousLogGroupsResponseTypeDef,
     ListNotificationChannelsResponseTypeDef,
     PerformanceInsightsReferenceComparisonValuesTypeDef,
     RecommendationTypeDef,
     ListEventsResponseTypeDef,
-    ListEventsRequestListEventsPaginateTypeDef,
-    ListEventsRequestRequestTypeDef,
     ListMonitoredResourcesResponseTypeDef,
     ListInsightsResponseTypeDef,
     SearchInsightsResponseTypeDef,
     SearchOrganizationInsightsResponseTypeDef,
     DescribeInsightResponseTypeDef,
     ListOrganizationInsightsResponseTypeDef,
+    ListEventsRequestListEventsPaginateTypeDef,
+    ListEventsRequestRequestTypeDef,
     SearchInsightsRequestRequestTypeDef,
     SearchInsightsRequestSearchInsightsPaginateTypeDef,
     SearchOrganizationInsightsRequestRequestTypeDef,
     SearchOrganizationInsightsRequestSearchOrganizationInsightsPaginateTypeDef,
+    ListInsightsRequestListInsightsPaginateTypeDef,
+    ListInsightsRequestRequestTypeDef,
+    ListOrganizationInsightsRequestListOrganizationInsightsPaginateTypeDef,
+    ListOrganizationInsightsRequestRequestTypeDef,
     PerformanceInsightsReferenceDataTypeDef,
     ListRecommendationsResponseTypeDef,
     PerformanceInsightsMetricsDetailTypeDef,
     AnomalySourceDetailsTypeDef,
     ProactiveAnomalySummaryTypeDef,
     ProactiveAnomalyTypeDef,
     ReactiveAnomalySummaryTypeDef,
     ReactiveAnomalyTypeDef,
     ListAnomaliesForInsightResponseTypeDef,
     DescribeAnomalyResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInsightHealthTypeDef:
+def get_value() -> AccountInsightHealthTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-devops-guru-2.5.2/types_aiobotocore_devops_guru.egg-info/SOURCES.txt` & `types-aiobotocore-devops-guru-2.5.2.post1/types_aiobotocore_devops_guru.egg-info/SOURCES.txt`

 * *Files identical despite different names*


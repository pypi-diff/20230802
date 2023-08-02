# Comparing `tmp/types-aiobotocore-compute-optimizer-2.5.2.tar.gz` & `tmp/types-aiobotocore-compute-optimizer-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-compute-optimizer-2.5.2.tar", last modified: Sat Jul  8 01:43:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-compute-optimizer-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:06 2023, max compression
```

## Comparing `types-aiobotocore-compute-optimizer-2.5.2.tar` & `types-aiobotocore-compute-optimizer-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:27.193933 types-aiobotocore-compute-optimizer-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20616 2023-07-08 01:43:27.181933 types-aiobotocore-compute-optimizer-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:27.193933 types-aiobotocore-compute-optimizer-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-08 01:27:57.000000 types-aiobotocore-compute-optimizer-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:27.181933 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26351 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    26316 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8267 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    42053 2023-07-08 01:27:59.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    42030 2023-07-08 01:27:59.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:58.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:27.181933 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20616 2023-07-08 01:43:27.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-08 01:43:27.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:27.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:27.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:27.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:27.000000 types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:06.853614 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26320 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26285 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23914 2023-08-02 14:35:33.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23912 2023-08-02 14:35:33.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    42051 2023-08-02 14:35:34.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42028 2023-08-02 14:35:33.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:32.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:06.857614 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:06.000000 types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/LICENSE` & `types-aiobotocore-compute-optimizer-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/PKG-INFO` & `types-aiobotocore-compute-optimizer-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-compute-optimizer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore compute-optimizer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore compute-optimizer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-compute-optimizer"></a>
 
 # types-aiobotocore-compute-optimizer
 
 [![PyPI - types-aiobotocore-compute-optimizer](https://img.shields.io/pypi/v/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-compute-optimizer?color=blue)](https://pypistats.org/packages/types-aiobotocore-compute-optimizer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-compute-optimizer)](https://pepy.tech/project/types-aiobotocore-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ComputeOptimizer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [types-aiobotocore-compute-optimizer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/).
 
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
@@ -377,30 +376,32 @@
 )
 
 
 def check_value(value: AutoScalingConfigurationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_compute_optimizer.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_compute_optimizer.type_defs import (
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
@@ -410,64 +411,63 @@
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
-    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
-    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
+    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
     PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
-    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
     ExportECSServiceRecommendationsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsResponseTypeDef,
     ExportDestinationTypeDef,
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
     GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
@@ -488,15 +488,15 @@
     GetECSServiceRecommendationsResponseTypeDef,
     GetEC2InstanceRecommendationsResponseTypeDef,
     GetLambdaFunctionRecommendationsResponseTypeDef,
     GetEBSVolumeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountEnrollmentStatusTypeDef:
+def get_value() -> AccountEnrollmentStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/README.md` & `types-aiobotocore-compute-optimizer-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-compute-optimizer"></a>
 
 # types-aiobotocore-compute-optimizer
 
 [![PyPI - types-aiobotocore-compute-optimizer](https://img.shields.io/pypi/v/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-compute-optimizer?color=blue)](https://pypistats.org/packages/types-aiobotocore-compute-optimizer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-compute-optimizer)](https://pepy.tech/project/types-aiobotocore-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ComputeOptimizer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [types-aiobotocore-compute-optimizer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/).
 
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
@@ -344,30 +344,32 @@
 )
 
 
 def check_value(value: AutoScalingConfigurationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_compute_optimizer.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_compute_optimizer.type_defs import (
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
@@ -377,64 +379,63 @@
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
-    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
-    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
+    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
     PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
-    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
     ExportECSServiceRecommendationsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsResponseTypeDef,
     ExportDestinationTypeDef,
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
     GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
@@ -455,15 +456,15 @@
     GetECSServiceRecommendationsResponseTypeDef,
     GetEC2InstanceRecommendationsResponseTypeDef,
     GetLambdaFunctionRecommendationsResponseTypeDef,
     GetEBSVolumeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountEnrollmentStatusTypeDef:
+def get_value() -> AccountEnrollmentStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/setup.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-compute-optimizer",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_compute_optimizer"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore compute-optimizer type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore compute-optimizer type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_compute_optimizer": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/"
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/__init__.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/__init__.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/__main__.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ComputeOptimizer 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ComputeOptimizer 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer\nOther"
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

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/client.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("compute-optimizer") as client:
         client: ComputeOptimizerClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     EnhancedInfrastructureMetricsType,
     ExportableAutoScalingGroupFieldType,
@@ -66,47 +65,44 @@
     GetRecommendationPreferencesResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
     JobFilterTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     ScopeTypeDef,
+    TimestampTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("ComputeOptimizerClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidParameterValueException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MissingAuthenticationToken: Type[BotocoreClientError]
     OptInRequiredException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
-
 class ComputeOptimizerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/)
     """
 
     meta: ClientMeta
@@ -115,60 +111,55 @@
     def exceptions(self) -> Exceptions:
         """
         ComputeOptimizerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#close)
         """
-
     async def delete_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],
         scope: ScopeTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes a recommendation preference, such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.delete_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#delete_recommendation_preferences)
         """
-
     async def describe_recommendation_export_jobs(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> DescribeRecommendationExportJobsResponseTypeDef:
         """
         Describes recommendation export jobs created in the last seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.describe_recommendation_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#describe_recommendation_export_jobs)
         """
-
     async def export_auto_scaling_group_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableAutoScalingGroupFieldType] = ...,
@@ -178,15 +169,14 @@
     ) -> ExportAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Auto Scaling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_auto_scaling_group_recommendations)
         """
-
     async def export_ebs_volume_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableVolumeFieldType] = ...,
@@ -195,15 +185,14 @@
     ) -> ExportEBSVolumeRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ebs_volume_recommendations)
         """
-
     async def export_ec2_instance_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableInstanceFieldType] = ...,
@@ -213,15 +202,14 @@
     ) -> ExportEC2InstanceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ec2_instance_recommendations)
         """
-
     async def export_ecs_service_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableECSServiceFieldType] = ...,
@@ -230,15 +218,14 @@
     ) -> ExportECSServiceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon ECS services on Fargate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ecs_service_recommendations)
         """
-
     async def export_lambda_function_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableLambdaFunctionFieldType] = ...,
@@ -247,29 +234,27 @@
     ) -> ExportLambdaFunctionRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Lambda functions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_lambda_function_recommendations)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#generate_presigned_url)
         """
-
     async def get_auto_scaling_group_recommendations(
         self,
         *,
         accountIds: Sequence[str] = ...,
         autoScalingGroupArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
@@ -278,15 +263,14 @@
     ) -> GetAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Returns Auto Scaling group recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_auto_scaling_group_recommendations)
         """
-
     async def get_ebs_volume_recommendations(
         self,
         *,
         volumeArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
@@ -294,15 +278,14 @@
     ) -> GetEBSVolumeRecommendationsResponseTypeDef:
         """
         Returns Amazon Elastic Block Store (Amazon EBS) volume recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ebs_volume_recommendations)
         """
-
     async def get_ec2_instance_recommendations(
         self,
         *,
         instanceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[FilterTypeDef] = ...,
@@ -311,49 +294,46 @@
     ) -> GetEC2InstanceRecommendationsResponseTypeDef:
         """
         Returns Amazon EC2 instance recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_instance_recommendations)
         """
-
     async def get_ec2_recommendation_projected_metrics(
         self,
         *,
         instanceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         recommendationPreferences: RecommendationPreferencesTypeDef = ...
     ) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected utilization metrics of Amazon EC2 instance
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_recommendation_projected_metrics)
         """
-
     async def get_ecs_service_recommendation_projected_metrics(
         self,
         *,
         serviceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str]
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef
     ) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected metrics of Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendation_projected_metrics)
         """
-
     async def get_ecs_service_recommendations(
         self,
         *,
         serviceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
@@ -361,50 +341,46 @@
     ) -> GetECSServiceRecommendationsResponseTypeDef:
         """
         Returns Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendations)
         """
-
     async def get_effective_recommendation_preferences(
         self, *, resourceArn: str
     ) -> GetEffectiveRecommendationPreferencesResponseTypeDef:
         """
         Returns the recommendation preferences that are in effect for a given resource,
         such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_effective_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_effective_recommendation_preferences)
         """
-
     async def get_enrollment_status(self) -> GetEnrollmentStatusResponseTypeDef:
         """
         Returns the enrollment (opt in) status of an account to the Compute Optimizer
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_enrollment_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_enrollment_status)
         """
-
     async def get_enrollment_statuses_for_organization(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetEnrollmentStatusesForOrganizationResponseTypeDef:
         """
         Returns the Compute Optimizer enrollment (opt-in) status of organization member
         accounts, if your account is an organization management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_enrollment_statuses_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_enrollment_statuses_for_organization)
         """
-
     async def get_lambda_function_recommendations(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         nextToken: str = ...,
@@ -412,15 +388,14 @@
     ) -> GetLambdaFunctionRecommendationsResponseTypeDef:
         """
         Returns Lambda function recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_lambda_function_recommendations)
         """
-
     async def get_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -428,25 +403,23 @@
         """
         Returns existing recommendation preferences, such as enhanced infrastructure
         metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_recommendation_preferences)
         """
-
     async def get_recommendation_summaries(
         self, *, accountIds: Sequence[str] = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetRecommendationSummariesResponseTypeDef:
         """
         Returns the optimization findings for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_recommendation_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_recommendation_summaries)
         """
-
     async def put_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
         enhancedInfrastructureMetrics: EnhancedInfrastructureMetricsType = ...,
         inferredWorkloadTypes: InferredWorkloadTypesPreferenceType = ...,
@@ -455,75 +428,67 @@
         """
         Creates a new recommendation preference or updates an existing recommendation
         preference, such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.put_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#put_recommendation_preferences)
         """
-
     async def update_enrollment_status(
         self, *, status: StatusType, includeMemberAccounts: bool = ...
     ) -> UpdateEnrollmentStatusResponseTypeDef:
         """
         Updates the enrollment (opt in and opt out) status of an account to the Compute
         Optimizer service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.update_enrollment_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#update_enrollment_status)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_recommendation_export_jobs"]
     ) -> DescribeRecommendationExportJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_enrollment_statuses_for_organization"]
     ) -> GetEnrollmentStatusesForOrganizationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_lambda_function_recommendations"]
     ) -> GetLambdaFunctionRecommendationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_recommendation_preferences"]
     ) -> GetRecommendationPreferencesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["get_recommendation_summaries"]
     ) -> GetRecommendationSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "ComputeOptimizerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/)
         """
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/client.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("compute-optimizer") as client:
         client: ComputeOptimizerClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     EnhancedInfrastructureMetricsType,
     ExportableAutoScalingGroupFieldType,
@@ -66,43 +65,48 @@
     GetRecommendationPreferencesResponseTypeDef,
     GetRecommendationSummariesResponseTypeDef,
     JobFilterTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     ScopeTypeDef,
+    TimestampTypeDef,
     UpdateEnrollmentStatusResponseTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("ComputeOptimizerClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     InvalidParameterValueException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     MissingAuthenticationToken: Type[BotocoreClientError]
     OptInRequiredException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
+
 class ComputeOptimizerClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/)
     """
 
     meta: ClientMeta
@@ -111,55 +115,60 @@
     def exceptions(self) -> Exceptions:
         """
         ComputeOptimizerClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#close)
         """
+
     async def delete_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         recommendationPreferenceNames: Sequence[RecommendationPreferenceNameType],
         scope: ScopeTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Deletes a recommendation preference, such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.delete_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#delete_recommendation_preferences)
         """
+
     async def describe_recommendation_export_jobs(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> DescribeRecommendationExportJobsResponseTypeDef:
         """
         Describes recommendation export jobs created in the last seven days.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.describe_recommendation_export_jobs)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#describe_recommendation_export_jobs)
         """
+
     async def export_auto_scaling_group_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableAutoScalingGroupFieldType] = ...,
@@ -169,14 +178,15 @@
     ) -> ExportAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Auto Scaling groups.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_auto_scaling_group_recommendations)
         """
+
     async def export_ebs_volume_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableVolumeFieldType] = ...,
@@ -185,14 +195,15 @@
     ) -> ExportEBSVolumeRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EBS volumes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ebs_volume_recommendations)
         """
+
     async def export_ec2_instance_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[FilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableInstanceFieldType] = ...,
@@ -202,14 +213,15 @@
     ) -> ExportEC2InstanceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon EC2 instances.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ec2_instance_recommendations)
         """
+
     async def export_ecs_service_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableECSServiceFieldType] = ...,
@@ -218,14 +230,15 @@
     ) -> ExportECSServiceRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Amazon ECS services on Fargate.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_ecs_service_recommendations)
         """
+
     async def export_lambda_function_recommendations(
         self,
         *,
         s3DestinationConfig: S3DestinationConfigTypeDef,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         fieldsToExport: Sequence[ExportableLambdaFunctionFieldType] = ...,
@@ -234,27 +247,29 @@
     ) -> ExportLambdaFunctionRecommendationsResponseTypeDef:
         """
         Exports optimization recommendations for Lambda functions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.export_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#export_lambda_function_recommendations)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#generate_presigned_url)
         """
+
     async def get_auto_scaling_group_recommendations(
         self,
         *,
         accountIds: Sequence[str] = ...,
         autoScalingGroupArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
@@ -263,14 +278,15 @@
     ) -> GetAutoScalingGroupRecommendationsResponseTypeDef:
         """
         Returns Auto Scaling group recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_auto_scaling_group_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_auto_scaling_group_recommendations)
         """
+
     async def get_ebs_volume_recommendations(
         self,
         *,
         volumeArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[EBSFilterTypeDef] = ...,
@@ -278,14 +294,15 @@
     ) -> GetEBSVolumeRecommendationsResponseTypeDef:
         """
         Returns Amazon Elastic Block Store (Amazon EBS) volume recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ebs_volume_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ebs_volume_recommendations)
         """
+
     async def get_ec2_instance_recommendations(
         self,
         *,
         instanceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[FilterTypeDef] = ...,
@@ -294,46 +311,49 @@
     ) -> GetEC2InstanceRecommendationsResponseTypeDef:
         """
         Returns Amazon EC2 instance recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_instance_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_instance_recommendations)
         """
+
     async def get_ec2_recommendation_projected_metrics(
         self,
         *,
         instanceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str],
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef,
         recommendationPreferences: RecommendationPreferencesTypeDef = ...
     ) -> GetEC2RecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected utilization metrics of Amazon EC2 instance
         recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ec2_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ec2_recommendation_projected_metrics)
         """
+
     async def get_ecs_service_recommendation_projected_metrics(
         self,
         *,
         serviceArn: str,
         stat: MetricStatisticType,
         period: int,
-        startTime: Union[datetime, str],
-        endTime: Union[datetime, str]
+        startTime: TimestampTypeDef,
+        endTime: TimestampTypeDef
     ) -> GetECSServiceRecommendationProjectedMetricsResponseTypeDef:
         """
         Returns the projected metrics of Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendation_projected_metrics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendation_projected_metrics)
         """
+
     async def get_ecs_service_recommendations(
         self,
         *,
         serviceArns: Sequence[str] = ...,
         nextToken: str = ...,
         maxResults: int = ...,
         filters: Sequence[ECSServiceRecommendationFilterTypeDef] = ...,
@@ -341,46 +361,50 @@
     ) -> GetECSServiceRecommendationsResponseTypeDef:
         """
         Returns Amazon ECS service recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_ecs_service_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_ecs_service_recommendations)
         """
+
     async def get_effective_recommendation_preferences(
         self, *, resourceArn: str
     ) -> GetEffectiveRecommendationPreferencesResponseTypeDef:
         """
         Returns the recommendation preferences that are in effect for a given resource,
         such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_effective_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_effective_recommendation_preferences)
         """
+
     async def get_enrollment_status(self) -> GetEnrollmentStatusResponseTypeDef:
         """
         Returns the enrollment (opt in) status of an account to the Compute Optimizer
         service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_enrollment_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_enrollment_status)
         """
+
     async def get_enrollment_statuses_for_organization(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
         nextToken: str = ...,
         maxResults: int = ...
     ) -> GetEnrollmentStatusesForOrganizationResponseTypeDef:
         """
         Returns the Compute Optimizer enrollment (opt-in) status of organization member
         accounts, if your account is an organization management account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_enrollment_statuses_for_organization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_enrollment_statuses_for_organization)
         """
+
     async def get_lambda_function_recommendations(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
         nextToken: str = ...,
@@ -388,14 +412,15 @@
     ) -> GetLambdaFunctionRecommendationsResponseTypeDef:
         """
         Returns Lambda function recommendations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_lambda_function_recommendations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_lambda_function_recommendations)
         """
+
     async def get_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
         nextToken: str = ...,
         maxResults: int = ...
@@ -403,23 +428,25 @@
         """
         Returns existing recommendation preferences, such as enhanced infrastructure
         metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_recommendation_preferences)
         """
+
     async def get_recommendation_summaries(
         self, *, accountIds: Sequence[str] = ..., nextToken: str = ..., maxResults: int = ...
     ) -> GetRecommendationSummariesResponseTypeDef:
         """
         Returns the optimization findings for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_recommendation_summaries)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_recommendation_summaries)
         """
+
     async def put_recommendation_preferences(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
         enhancedInfrastructureMetrics: EnhancedInfrastructureMetricsType = ...,
         inferredWorkloadTypes: InferredWorkloadTypesPreferenceType = ...,
@@ -428,67 +455,75 @@
         """
         Creates a new recommendation preference or updates an existing recommendation
         preference, such as enhanced infrastructure metrics.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.put_recommendation_preferences)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#put_recommendation_preferences)
         """
+
     async def update_enrollment_status(
         self, *, status: StatusType, includeMemberAccounts: bool = ...
     ) -> UpdateEnrollmentStatusResponseTypeDef:
         """
         Updates the enrollment (opt in and opt out) status of an account to the Compute
         Optimizer service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.update_enrollment_status)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#update_enrollment_status)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_recommendation_export_jobs"]
     ) -> DescribeRecommendationExportJobsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_enrollment_statuses_for_organization"]
     ) -> GetEnrollmentStatusesForOrganizationPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_lambda_function_recommendations"]
     ) -> GetLambdaFunctionRecommendationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_recommendation_preferences"]
     ) -> GetRecommendationPreferencesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["get_recommendation_summaries"]
     ) -> GetRecommendationSummariesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "ComputeOptimizerClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/client/)
         """
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/literals.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/literals.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/paginator.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
 
@@ -91,15 +91,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
 
@@ -111,15 +111,15 @@
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
 
@@ -130,28 +130,28 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
 
 class GetRecommendationSummariesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationsummariespaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationsummariespaginator)
         """
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/paginator.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     """
 
     def paginate(
         self,
         *,
         jobIds: Sequence[str] = ...,
         filters: Sequence[JobFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRecommendationExportJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.DescribeRecommendationExportJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#describerecommendationexportjobspaginator)
         """
 
 class GetEnrollmentStatusesForOrganizationPaginator(AioPaginator):
@@ -87,15 +87,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
     """
 
     def paginate(
         self,
         *,
         filters: Sequence[EnrollmentFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetEnrollmentStatusesForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetEnrollmentStatusesForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getenrollmentstatusesfororganizationpaginator)
         """
 
 class GetLambdaFunctionRecommendationsPaginator(AioPaginator):
@@ -106,15 +106,15 @@
 
     def paginate(
         self,
         *,
         functionArns: Sequence[str] = ...,
         accountIds: Sequence[str] = ...,
         filters: Sequence[LambdaFunctionRecommendationFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLambdaFunctionRecommendationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetLambdaFunctionRecommendations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getlambdafunctionrecommendationspaginator)
         """
 
 class GetRecommendationPreferencesPaginator(AioPaginator):
@@ -124,27 +124,27 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         scope: ScopeTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRecommendationPreferencesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationPreferences.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationpreferencespaginator)
         """
 
 class GetRecommendationSummariesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationsummariespaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRecommendationSummariesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer.Paginator.GetRecommendationSummaries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/paginators/#getrecommendationsummariespaginator)
         """
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/type_defs.py` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_compute_optimizer.type_defs import AccountEnrollmentStatusTypeDef
 
-    data: AccountEnrollmentStatusTypeDef = {...}
+    data: AccountEnrollmentStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -76,14 +76,16 @@
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
     "ScopeTypeDef",
     "JobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
     "TagTypeDef",
@@ -93,64 +95,63 @@
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
     "GetRecommendationErrorTypeDef",
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
-    "GetEnrollmentStatusResponseTypeDef",
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
-    "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
     "DeleteRecommendationPreferencesRequestRequestTypeDef",
-    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     "GetRecommendationPreferencesRequestRequestTypeDef",
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     "DescribeRecommendationExportJobsRequestRequestTypeDef",
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    "GetEnrollmentStatusResponseTypeDef",
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    "UpdateEnrollmentStatusResponseTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
-    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "ExportEBSVolumeRecommendationsRequestRequestTypeDef",
     "ExportEC2InstanceRecommendationsRequestRequestTypeDef",
     "ExportECSServiceRecommendationsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     "ExportDestinationTypeDef",
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
+    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
@@ -240,14 +241,35 @@
     {
         "name": JobFilterNameType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
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
 EBSFilterTypeDef = TypedDict(
     "EBSFilterTypeDef",
     {
         "name": Literal["Finding"],
         "values": Sequence[str],
     },
     total=False,
@@ -399,53 +421,22 @@
         "identifier": str,
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "serviceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetEnrollmentStatusResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "memberAccountsEnrolled": bool,
-        "lastUpdatedTimestamp": datetime,
-        "numberOfMemberAccountsOptedIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRecommendationSummariesRequestRequestTypeDef = TypedDict(
     "GetRecommendationSummariesRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -477,24 +468,14 @@
         "name": LambdaFunctionMetricNameType,
         "statistic": LambdaFunctionMetricStatisticType,
         "value": float,
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
 ProjectedMetricTypeDef = TypedDict(
     "ProjectedMetricTypeDef",
     {
         "name": MetricNameType,
         "timestamps": List[datetime],
         "values": List[float],
     },
@@ -506,25 +487,14 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
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
 _RequiredUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnrollmentStatusRequestRequestTypeDef",
     {
         "status": StatusType,
     },
 )
 _OptionalUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
@@ -539,46 +509,28 @@
 class UpdateEnrollmentStatusRequestRequestTypeDef(
     _RequiredUpdateEnrollmentStatusRequestRequestTypeDef,
     _OptionalUpdateEnrollmentStatusRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateEnrollmentStatusResponseTypeDef = TypedDict(
-    "UpdateEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VolumeConfigurationTypeDef = TypedDict(
     "VolumeConfigurationTypeDef",
     {
         "volumeType": str,
         "volumeSize": int,
         "volumeBaselineIOPS": int,
         "volumeBurstIOPS": int,
         "volumeBaselineThroughput": int,
         "volumeBurstThroughput": int,
         "rootVolume": bool,
     },
     total=False,
 )
 
-GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
-    {
-        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ContainerConfigurationTypeDef = TypedDict(
     "ContainerConfigurationTypeDef",
     {
         "containerName": str,
         "memorySizeConfiguration": MemorySizeConfigurationTypeDef,
         "cpu": int,
     },
@@ -614,80 +566,119 @@
 class DeleteRecommendationPreferencesRequestRequestTypeDef(
     _RequiredDeleteRecommendationPreferencesRequestRequestTypeDef,
     _OptionalDeleteRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "scope": ScopeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
 
-class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
-    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+class GetRecommendationPreferencesRequestRequestTypeDef(
+    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
+    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
+DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
+    {
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
+        "nextToken": str,
+        "maxResults": int,
+    },
+    total=False,
+)
+
+DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+    {
+        "jobIds": Sequence[str],
+        "filters": Sequence[JobFilterTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
-_OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestRequestTypeDef",
+_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     {
         "scope": ScopeTypeDef,
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class GetRecommendationPreferencesRequestRequestTypeDef(
-    _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
-    _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
+class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
+    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
 ):
     pass
 
 
-DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
+GetEnrollmentStatusResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusResponseTypeDef",
     {
-        "jobIds": Sequence[str],
-        "filters": Sequence[JobFilterTypeDef],
+        "status": StatusType,
+        "statusReason": str,
+        "memberAccountsEnrolled": bool,
+        "lastUpdatedTimestamp": datetime,
+        "numberOfMemberAccountsOptedIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    {
+        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
         "nextToken": str,
-        "maxResults": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEnrollmentStatusResponseTypeDef = TypedDict(
+    "UpdateEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 GetEBSVolumeRecommendationsRequestRequestTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     {
         "volumeArns": Sequence[str],
         "nextToken": str,
@@ -732,15 +723,15 @@
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
@@ -777,15 +768,15 @@
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     {
@@ -836,40 +827,14 @@
         "filters": Sequence[FilterTypeDef],
         "accountIds": Sequence[str],
         "recommendationPreferences": RecommendationPreferencesTypeDef,
     },
     total=False,
 )
 
-_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "instanceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "recommendationPreferences": RecommendationPreferencesTypeDef,
-    },
-    total=False,
-)
-
-
-class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
-    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
     },
 )
 _OptionalExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
@@ -973,15 +938,15 @@
 
 
 ExportAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportDestinationTypeDef = TypedDict(
     "ExportDestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
@@ -990,42 +955,42 @@
 )
 
 ExportEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportECSServiceRecommendationsResponseTypeDef = TypedDict(
     "ExportECSServiceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
@@ -1053,15 +1018,15 @@
 
 GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     {
         "functionArns": Sequence[str],
         "accountIds": Sequence[str],
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
@@ -1070,14 +1035,51 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "instanceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "recommendationPreferences": RecommendationPreferencesTypeDef,
+    },
+    total=False,
+)
+
+
+class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
+    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+):
+    pass
+
+
+GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "serviceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
@@ -1108,24 +1110,24 @@
 
 GetECSServiceRecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetRecommendationPreferencesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
@@ -1200,15 +1202,15 @@
     total=False,
 )
 
 GetEC2RecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[RecommendedOptionProjectedMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "summaries": List[SummaryTypeDef],
@@ -1321,68 +1323,68 @@
 )
 
 DescribeRecommendationExportJobsResponseTypeDef = TypedDict(
     "DescribeRecommendationExportJobsResponseTypeDef",
     {
         "recommendationExportJobs": List[RecommendationExportJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationSummariesResponseTypeDef = TypedDict(
     "GetRecommendationSummariesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationSummaries": List[RecommendationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "GetAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "autoScalingGroupRecommendations": List[AutoScalingGroupRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetECSServiceRecommendationsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "ecsServiceRecommendations": List[ECSServiceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "GetEC2InstanceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "instanceRecommendations": List[InstanceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "lambdaFunctionRecommendations": List[LambdaFunctionRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "volumeRecommendations": List[VolumeRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer/type_defs.pyi` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_compute_optimizer.type_defs import AccountEnrollmentStatusTypeDef
 
-    data: AccountEnrollmentStatusTypeDef = {...}
+    data: AccountEnrollmentStatusTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import (
@@ -75,14 +75,16 @@
     "AccountEnrollmentStatusTypeDef",
     "AutoScalingGroupConfigurationTypeDef",
     "UtilizationMetricTypeDef",
     "MemorySizeConfigurationTypeDef",
     "CurrentPerformanceRiskRatingsTypeDef",
     "ScopeTypeDef",
     "JobFilterTypeDef",
+    "PaginatorConfigTypeDef",
+    "ResponseMetadataTypeDef",
     "EBSFilterTypeDef",
     "EBSUtilizationMetricTypeDef",
     "ECSServiceProjectedMetricTypeDef",
     "ECSServiceProjectedUtilizationMetricTypeDef",
     "ECSServiceRecommendationFilterTypeDef",
     "ECSServiceUtilizationMetricTypeDef",
     "TagTypeDef",
@@ -92,64 +94,63 @@
     "FilterTypeDef",
     "RecommendationPreferencesTypeDef",
     "S3DestinationConfigTypeDef",
     "S3DestinationTypeDef",
     "LambdaFunctionRecommendationFilterTypeDef",
     "ExternalMetricStatusTypeDef",
     "GetRecommendationErrorTypeDef",
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    "TimestampTypeDef",
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
-    "GetEnrollmentStatusResponseTypeDef",
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
     "GetRecommendationSummariesRequestRequestTypeDef",
     "RecommendationSourceTypeDef",
     "LambdaFunctionMemoryProjectedMetricTypeDef",
     "LambdaFunctionUtilizationMetricTypeDef",
-    "PaginatorConfigTypeDef",
     "ProjectedMetricTypeDef",
     "ReasonCodeSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateEnrollmentStatusRequestRequestTypeDef",
-    "UpdateEnrollmentStatusResponseTypeDef",
     "VolumeConfigurationTypeDef",
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
     "ContainerConfigurationTypeDef",
     "ContainerRecommendationTypeDef",
     "DeleteRecommendationPreferencesRequestRequestTypeDef",
-    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
     "GetRecommendationPreferencesRequestRequestTypeDef",
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     "DescribeRecommendationExportJobsRequestRequestTypeDef",
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+    "GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    "GetEnrollmentStatusResponseTypeDef",
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    "UpdateEnrollmentStatusResponseTypeDef",
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     "ECSServiceRecommendedOptionProjectedMetricTypeDef",
     "GetECSServiceRecommendationsRequestRequestTypeDef",
     "EffectiveRecommendationPreferencesTypeDef",
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     "PutRecommendationPreferencesRequestRequestTypeDef",
     "RecommendationPreferencesDetailTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     "InferredWorkloadSavingTypeDef",
     "SavingsOpportunityTypeDef",
     "GetAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "GetEC2InstanceRecommendationsRequestRequestTypeDef",
-    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     "ExportEBSVolumeRecommendationsRequestRequestTypeDef",
     "ExportEC2InstanceRecommendationsRequestRequestTypeDef",
     "ExportECSServiceRecommendationsRequestRequestTypeDef",
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     "ExportDestinationTypeDef",
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     "ExportECSServiceRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     "ExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
+    "GetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
     "RecommendedOptionProjectedMetricTypeDef",
     "SummaryTypeDef",
     "ServiceConfigurationTypeDef",
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     "GetRecommendationPreferencesResponseTypeDef",
     "AutoScalingGroupRecommendationOptionTypeDef",
     "ECSServiceRecommendationOptionTypeDef",
@@ -239,14 +240,35 @@
     {
         "name": JobFilterNameType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
+    {
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
+    },
+    total=False,
+)
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
 EBSFilterTypeDef = TypedDict(
     "EBSFilterTypeDef",
     {
         "name": Literal["Finding"],
         "values": Sequence[str],
     },
     total=False,
@@ -398,53 +420,22 @@
         "identifier": str,
         "code": str,
         "message": str,
     },
     total=False,
 )
 
-GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "serviceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 GetEffectiveRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetEnrollmentStatusResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "memberAccountsEnrolled": bool,
-        "lastUpdatedTimestamp": datetime,
-        "numberOfMemberAccountsOptedIn": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
-    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetRecommendationSummariesRequestRequestTypeDef = TypedDict(
     "GetRecommendationSummariesRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "nextToken": str,
         "maxResults": int,
     },
@@ -476,24 +467,14 @@
         "name": LambdaFunctionMetricNameType,
         "statistic": LambdaFunctionMetricStatisticType,
         "value": float,
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
 ProjectedMetricTypeDef = TypedDict(
     "ProjectedMetricTypeDef",
     {
         "name": MetricNameType,
         "timestamps": List[datetime],
         "values": List[float],
     },
@@ -505,25 +486,14 @@
     {
         "name": FindingReasonCodeType,
         "value": float,
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
 _RequiredUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateEnrollmentStatusRequestRequestTypeDef",
     {
         "status": StatusType,
     },
 )
 _OptionalUpdateEnrollmentStatusRequestRequestTypeDef = TypedDict(
@@ -536,46 +506,28 @@
 
 class UpdateEnrollmentStatusRequestRequestTypeDef(
     _RequiredUpdateEnrollmentStatusRequestRequestTypeDef,
     _OptionalUpdateEnrollmentStatusRequestRequestTypeDef,
 ):
     pass
 
-UpdateEnrollmentStatusResponseTypeDef = TypedDict(
-    "UpdateEnrollmentStatusResponseTypeDef",
-    {
-        "status": StatusType,
-        "statusReason": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VolumeConfigurationTypeDef = TypedDict(
     "VolumeConfigurationTypeDef",
     {
         "volumeType": str,
         "volumeSize": int,
         "volumeBaselineIOPS": int,
         "volumeBurstIOPS": int,
         "volumeBaselineThroughput": int,
         "volumeBurstThroughput": int,
         "rootVolume": bool,
     },
     total=False,
 )
 
-GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
-    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
-    {
-        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ContainerConfigurationTypeDef = TypedDict(
     "ContainerConfigurationTypeDef",
     {
         "containerName": str,
         "memorySizeConfiguration": MemorySizeConfigurationTypeDef,
         "cpu": int,
     },
@@ -609,35 +561,14 @@
 
 class DeleteRecommendationPreferencesRequestRequestTypeDef(
     _RequiredDeleteRecommendationPreferencesRequestRequestTypeDef,
     _OptionalDeleteRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
-    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
-    {
-        "scope": ScopeTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
-    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalGetRecommendationPreferencesRequestRequestTypeDef = TypedDict(
@@ -652,35 +583,95 @@
 
 class GetRecommendationPreferencesRequestRequestTypeDef(
     _RequiredGetRecommendationPreferencesRequestRequestTypeDef,
     _OptionalGetRecommendationPreferencesRequestRequestTypeDef,
 ):
     pass
 
-DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
+DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestRequestTypeDef",
     {
         "jobIds": Sequence[str],
         "filters": Sequence[JobFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "nextToken": str,
+        "maxResults": int,
     },
     total=False,
 )
 
-DescribeRecommendationExportJobsRequestRequestTypeDef = TypedDict(
-    "DescribeRecommendationExportJobsRequestRequestTypeDef",
+DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef = TypedDict(
+    "DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef",
     {
         "jobIds": Sequence[str],
         "filters": Sequence[JobFilterTypeDef],
-        "nextToken": str,
-        "maxResults": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef = TypedDict(
+    "_OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef",
+    {
+        "scope": ScopeTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef(
+    _RequiredGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    _OptionalGetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+):
+    pass
+
+GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef = TypedDict(
+    "GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+GetEnrollmentStatusResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "memberAccountsEnrolled": bool,
+        "lastUpdatedTimestamp": datetime,
+        "numberOfMemberAccountsOptedIn": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEnrollmentStatusesForOrganizationResponseTypeDef = TypedDict(
+    "GetEnrollmentStatusesForOrganizationResponseTypeDef",
+    {
+        "accountEnrollmentStatuses": List[AccountEnrollmentStatusTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEnrollmentStatusResponseTypeDef = TypedDict(
+    "UpdateEnrollmentStatusResponseTypeDef",
+    {
+        "status": StatusType,
+        "statusReason": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetEBSVolumeRecommendationsRequestRequestTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsRequestRequestTypeDef",
     {
         "volumeArns": Sequence[str],
         "nextToken": str,
         "maxResults": int,
         "filters": Sequence[EBSFilterTypeDef],
@@ -723,15 +714,15 @@
 )
 
 GetEffectiveRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetEffectiveRecommendationPreferencesResponseTypeDef",
     {
         "enhancedInfrastructureMetrics": EnhancedInfrastructureMetricsType,
         "externalMetricsPreference": ExternalMetricsPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutRecommendationPreferencesRequestRequestTypeDef = TypedDict(
     "_RequiredPutRecommendationPreferencesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
@@ -766,15 +757,15 @@
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef",
     {
         "filters": Sequence[EnrollmentFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetEnrollmentStatusesForOrganizationRequestRequestTypeDef = TypedDict(
     "GetEnrollmentStatusesForOrganizationRequestRequestTypeDef",
     {
@@ -825,38 +816,14 @@
         "filters": Sequence[FilterTypeDef],
         "accountIds": Sequence[str],
         "recommendationPreferences": RecommendationPreferencesTypeDef,
     },
     total=False,
 )
 
-_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "instanceArn": str,
-        "stat": MetricStatisticType,
-        "period": int,
-        "startTime": Union[datetime, str],
-        "endTime": Union[datetime, str],
-    },
-)
-_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
-    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
-    {
-        "recommendationPreferences": RecommendationPreferencesTypeDef,
-    },
-    total=False,
-)
-
-class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
-    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
-):
-    pass
-
 _RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportAutoScalingGroupRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
     },
 )
 _OptionalExportAutoScalingGroupRecommendationsRequestRequestTypeDef = TypedDict(
@@ -952,15 +919,15 @@
     pass
 
 ExportAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "ExportAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportDestinationTypeDef = TypedDict(
     "ExportDestinationTypeDef",
     {
         "s3": S3DestinationTypeDef,
@@ -969,42 +936,42 @@
 )
 
 ExportEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "ExportEBSVolumeRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "ExportEC2InstanceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportECSServiceRecommendationsResponseTypeDef = TypedDict(
     "ExportECSServiceRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "ExportLambdaFunctionRecommendationsResponseTypeDef",
     {
         "jobId": str,
         "s3Destination": S3DestinationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "_RequiredExportLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
         "s3DestinationConfig": S3DestinationConfigTypeDef,
@@ -1030,15 +997,15 @@
 
 GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef",
     {
         "functionArns": Sequence[str],
         "accountIds": Sequence[str],
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetLambdaFunctionRecommendationsRequestRequestTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsRequestRequestTypeDef",
     {
@@ -1047,14 +1014,49 @@
         "filters": Sequence[LambdaFunctionRecommendationFilterTypeDef],
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
+_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "instanceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "_OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "recommendationPreferences": RecommendationPreferencesTypeDef,
+    },
+    total=False,
+)
+
+class GetEC2RecommendationProjectedMetricsRequestRequestTypeDef(
+    _RequiredGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    _OptionalGetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+):
+    pass
+
+GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef = TypedDict(
+    "GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef",
+    {
+        "serviceArn": str,
+        "stat": MetricStatisticType,
+        "period": int,
+        "startTime": TimestampTypeDef,
+        "endTime": TimestampTypeDef,
+    },
+)
+
 RecommendedOptionProjectedMetricTypeDef = TypedDict(
     "RecommendedOptionProjectedMetricTypeDef",
     {
         "recommendedInstanceType": str,
         "rank": int,
         "projectedMetrics": List[ProjectedMetricTypeDef],
     },
@@ -1085,24 +1087,24 @@
 
 GetECSServiceRecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[
             ECSServiceRecommendedOptionProjectedMetricTypeDef
         ],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationPreferencesResponseTypeDef = TypedDict(
     "GetRecommendationPreferencesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationPreferencesDetails": List[RecommendationPreferencesDetailTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AutoScalingGroupRecommendationOptionTypeDef = TypedDict(
     "AutoScalingGroupRecommendationOptionTypeDef",
     {
         "configuration": AutoScalingGroupConfigurationTypeDef,
@@ -1177,15 +1179,15 @@
     total=False,
 )
 
 GetEC2RecommendationProjectedMetricsResponseTypeDef = TypedDict(
     "GetEC2RecommendationProjectedMetricsResponseTypeDef",
     {
         "recommendedOptionProjectedMetrics": List[RecommendedOptionProjectedMetricTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecommendationSummaryTypeDef = TypedDict(
     "RecommendationSummaryTypeDef",
     {
         "summaries": List[SummaryTypeDef],
@@ -1298,68 +1300,68 @@
 )
 
 DescribeRecommendationExportJobsResponseTypeDef = TypedDict(
     "DescribeRecommendationExportJobsResponseTypeDef",
     {
         "recommendationExportJobs": List[RecommendationExportJobTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRecommendationSummariesResponseTypeDef = TypedDict(
     "GetRecommendationSummariesResponseTypeDef",
     {
         "nextToken": str,
         "recommendationSummaries": List[RecommendationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAutoScalingGroupRecommendationsResponseTypeDef = TypedDict(
     "GetAutoScalingGroupRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "autoScalingGroupRecommendations": List[AutoScalingGroupRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetECSServiceRecommendationsResponseTypeDef = TypedDict(
     "GetECSServiceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "ecsServiceRecommendations": List[ECSServiceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEC2InstanceRecommendationsResponseTypeDef = TypedDict(
     "GetEC2InstanceRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "instanceRecommendations": List[InstanceRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLambdaFunctionRecommendationsResponseTypeDef = TypedDict(
     "GetLambdaFunctionRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "lambdaFunctionRecommendations": List[LambdaFunctionRecommendationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetEBSVolumeRecommendationsResponseTypeDef = TypedDict(
     "GetEBSVolumeRecommendationsResponseTypeDef",
     {
         "nextToken": str,
         "volumeRecommendations": List[VolumeRecommendationTypeDef],
         "errors": List[GetRecommendationErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-compute-optimizer
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ComputeOptimizer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore compute-optimizer type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore compute-optimizer type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-compute-optimizer"></a>
 
 # types-aiobotocore-compute-optimizer
 
 [![PyPI - types-aiobotocore-compute-optimizer](https://img.shields.io/pypi/v/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-compute-optimizer.svg?color=blue)](https://pypi.org/project/types-aiobotocore-compute-optimizer)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-compute-optimizer?color=blue)](https://pypistats.org/packages/types-aiobotocore-compute-optimizer)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-compute-optimizer)](https://pepy.tech/project/types-aiobotocore-compute-optimizer)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ComputeOptimizer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/compute-optimizer.html#ComputeOptimizer)
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
 [types-aiobotocore-compute-optimizer docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_compute_optimizer/).
 
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
@@ -377,30 +376,32 @@
 )
 
 
 def check_value(value: AutoScalingConfigurationType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_compute_optimizer.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_compute_optimizer.type_defs import (
     AccountEnrollmentStatusTypeDef,
     AutoScalingGroupConfigurationTypeDef,
     UtilizationMetricTypeDef,
     MemorySizeConfigurationTypeDef,
     CurrentPerformanceRiskRatingsTypeDef,
     ScopeTypeDef,
     JobFilterTypeDef,
+    PaginatorConfigTypeDef,
+    ResponseMetadataTypeDef,
     EBSFilterTypeDef,
     EBSUtilizationMetricTypeDef,
     ECSServiceProjectedMetricTypeDef,
     ECSServiceProjectedUtilizationMetricTypeDef,
     ECSServiceRecommendationFilterTypeDef,
     ECSServiceUtilizationMetricTypeDef,
     TagTypeDef,
@@ -410,64 +411,63 @@
     FilterTypeDef,
     RecommendationPreferencesTypeDef,
     S3DestinationConfigTypeDef,
     S3DestinationTypeDef,
     LambdaFunctionRecommendationFilterTypeDef,
     ExternalMetricStatusTypeDef,
     GetRecommendationErrorTypeDef,
-    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
+    TimestampTypeDef,
     GetEffectiveRecommendationPreferencesRequestRequestTypeDef,
-    GetEnrollmentStatusResponseTypeDef,
-    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
     GetRecommendationSummariesRequestRequestTypeDef,
     RecommendationSourceTypeDef,
     LambdaFunctionMemoryProjectedMetricTypeDef,
     LambdaFunctionUtilizationMetricTypeDef,
-    PaginatorConfigTypeDef,
     ProjectedMetricTypeDef,
     ReasonCodeSummaryTypeDef,
-    ResponseMetadataTypeDef,
     UpdateEnrollmentStatusRequestRequestTypeDef,
-    UpdateEnrollmentStatusResponseTypeDef,
     VolumeConfigurationTypeDef,
-    GetEnrollmentStatusesForOrganizationResponseTypeDef,
     ContainerConfigurationTypeDef,
     ContainerRecommendationTypeDef,
     DeleteRecommendationPreferencesRequestRequestTypeDef,
-    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
     GetRecommendationPreferencesRequestRequestTypeDef,
-    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
     DescribeRecommendationExportJobsRequestRequestTypeDef,
+    DescribeRecommendationExportJobsRequestDescribeRecommendationExportJobsPaginateTypeDef,
+    GetRecommendationPreferencesRequestGetRecommendationPreferencesPaginateTypeDef,
+    GetRecommendationSummariesRequestGetRecommendationSummariesPaginateTypeDef,
+    GetEnrollmentStatusResponseTypeDef,
+    GetEnrollmentStatusesForOrganizationResponseTypeDef,
+    UpdateEnrollmentStatusResponseTypeDef,
     GetEBSVolumeRecommendationsRequestRequestTypeDef,
     ECSServiceRecommendedOptionProjectedMetricTypeDef,
     GetECSServiceRecommendationsRequestRequestTypeDef,
     EffectiveRecommendationPreferencesTypeDef,
     GetEffectiveRecommendationPreferencesResponseTypeDef,
     PutRecommendationPreferencesRequestRequestTypeDef,
     RecommendationPreferencesDetailTypeDef,
     GetEnrollmentStatusesForOrganizationRequestGetEnrollmentStatusesForOrganizationPaginateTypeDef,
     GetEnrollmentStatusesForOrganizationRequestRequestTypeDef,
     InferredWorkloadSavingTypeDef,
     SavingsOpportunityTypeDef,
     GetAutoScalingGroupRecommendationsRequestRequestTypeDef,
     GetEC2InstanceRecommendationsRequestRequestTypeDef,
-    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsRequestRequestTypeDef,
     ExportEBSVolumeRecommendationsRequestRequestTypeDef,
     ExportEC2InstanceRecommendationsRequestRequestTypeDef,
     ExportECSServiceRecommendationsRequestRequestTypeDef,
     ExportAutoScalingGroupRecommendationsResponseTypeDef,
     ExportDestinationTypeDef,
     ExportEBSVolumeRecommendationsResponseTypeDef,
     ExportEC2InstanceRecommendationsResponseTypeDef,
     ExportECSServiceRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsResponseTypeDef,
     ExportLambdaFunctionRecommendationsRequestRequestTypeDef,
     GetLambdaFunctionRecommendationsRequestGetLambdaFunctionRecommendationsPaginateTypeDef,
     GetLambdaFunctionRecommendationsRequestRequestTypeDef,
+    GetEC2RecommendationProjectedMetricsRequestRequestTypeDef,
+    GetECSServiceRecommendationProjectedMetricsRequestRequestTypeDef,
     RecommendedOptionProjectedMetricTypeDef,
     SummaryTypeDef,
     ServiceConfigurationTypeDef,
     GetECSServiceRecommendationProjectedMetricsResponseTypeDef,
     GetRecommendationPreferencesResponseTypeDef,
     AutoScalingGroupRecommendationOptionTypeDef,
     ECSServiceRecommendationOptionTypeDef,
@@ -488,15 +488,15 @@
     GetECSServiceRecommendationsResponseTypeDef,
     GetEC2InstanceRecommendationsResponseTypeDef,
     GetLambdaFunctionRecommendationsResponseTypeDef,
     GetEBSVolumeRecommendationsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountEnrollmentStatusTypeDef:
+def get_value() -> AccountEnrollmentStatusTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-compute-optimizer-2.5.2/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt` & `types-aiobotocore-compute-optimizer-2.5.2.post1/types_aiobotocore_compute_optimizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*


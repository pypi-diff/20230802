# Comparing `tmp/types-aiobotocore-ce-2.5.2.tar.gz` & `tmp/types-aiobotocore-ce-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-ce-2.5.2.tar", last modified: Sat Jul  8 01:43:19 2023, max compression
+gzip compressed data, was "types-aiobotocore-ce-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:57 2023, max compression
```

## Comparing `types-aiobotocore-ce-2.5.2.tar` & `types-aiobotocore-ce-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33821 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    33775 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    63460 2023-07-08 01:26:30.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63391 2023-07-08 01:26:30.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:29.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:18.993777 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18996 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-08 01:43:18.000000 types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17801 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33899 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33853 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    66703 2023-08-02 14:33:58.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66630 2023-08-02 14:33:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:56.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:57.509643 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19309 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-02 14:51:57.000000 types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-ce-2.5.2/LICENSE` & `types-aiobotocore-ce-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2/PKG-INFO` & `types-aiobotocore-ce-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ce type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ce type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ce"></a>
 
 # types-aiobotocore-ce
 
 [![PyPI - types-aiobotocore-ce](https://img.shields.io/pypi/v/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ce?color=blue)](https://pypistats.org/packages/types-aiobotocore-ce)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [types-aiobotocore-ce docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/).
 
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
@@ -312,120 +311,128 @@
 )
 
 
 def check_value(value: AccountScopeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ce.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
+    CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
+    CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    TagValuesTypeDef,
+    ResponseMetadataTypeDef,
+    TagValuesOutputTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
+    DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
+    TagValuesTypeDef,
+    ExpressionUnionTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExpressionTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationTypeDef,
+    ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
     GetDimensionValuesRequestRequestTypeDef,
     GetReservationCoverageRequestRequestTypeDef,
@@ -440,34 +447,36 @@
     InstanceDetailsTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
-    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    AnomalySubscriptionUnionTypeDef,
+    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
-    CreateCostCategoryDefinitionRequestRequestTypeDef,
-    UpdateCostCategoryDefinitionRequestRequestTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    CreateCostCategoryDefinitionRequestRequestTypeDef,
+    UpdateCostCategoryDefinitionRequestRequestTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
     TargetInstanceTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     ReservationPurchaseRecommendationTypeDef,
@@ -476,15 +485,15 @@
     ModifyRecommendationDetailTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     RightsizingRecommendationTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
 )
 
 
-def get_structure() -> AnomalyDateIntervalTypeDef:
+def get_value() -> AnomalyDateIntervalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ce-2.5.2/README.md` & `types-aiobotocore-ce-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-ce"></a>
 
 # types-aiobotocore-ce
 
 [![PyPI - types-aiobotocore-ce](https://img.shields.io/pypi/v/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ce?color=blue)](https://pypistats.org/packages/types-aiobotocore-ce)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [types-aiobotocore-ce docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/).
 
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
@@ -279,120 +279,128 @@
 )
 
 
 def check_value(value: AccountScopeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ce.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
+    CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
+    CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    TagValuesTypeDef,
+    ResponseMetadataTypeDef,
+    TagValuesOutputTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
+    DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
+    TagValuesTypeDef,
+    ExpressionUnionTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExpressionTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationTypeDef,
+    ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
     GetDimensionValuesRequestRequestTypeDef,
     GetReservationCoverageRequestRequestTypeDef,
@@ -407,34 +415,36 @@
     InstanceDetailsTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
-    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    AnomalySubscriptionUnionTypeDef,
+    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
-    CreateCostCategoryDefinitionRequestRequestTypeDef,
-    UpdateCostCategoryDefinitionRequestRequestTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    CreateCostCategoryDefinitionRequestRequestTypeDef,
+    UpdateCostCategoryDefinitionRequestRequestTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
     TargetInstanceTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     ReservationPurchaseRecommendationTypeDef,
@@ -443,15 +453,15 @@
     ModifyRecommendationDetailTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     RightsizingRecommendationTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
 )
 
 
-def get_structure() -> AnomalyDateIntervalTypeDef:
+def get_value() -> AnomalyDateIntervalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ce-2.5.2/setup.py` & `types-aiobotocore-ce-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-ce",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_ce"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with"
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
-    keywords="aiobotocore ce type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore ce type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_ce": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/__main__.py` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CostExplorer 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CostExplorer 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer\nOther"
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

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.py` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
-    AnomalySubscriptionTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
-    CostCategorySplitChargeRuleTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
-    ExpressionTypeDef,
+    ExpressionUnionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
@@ -167,15 +167,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_monitor)
         """
 
     async def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: AnomalySubscriptionTypeDef,
+        AnomalySubscription: AnomalySubscriptionUnionTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_subscription)
@@ -185,15 +185,15 @@
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_cost_category_definition)
@@ -299,15 +299,15 @@
 
     async def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
@@ -315,15 +315,15 @@
         """
 
     async def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef",
+        Filter: ExpressionUnionTypeDef,
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
@@ -333,15 +333,15 @@
 
     async def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
@@ -351,15 +351,15 @@
 
     async def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -369,15 +369,15 @@
     async def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
@@ -388,15 +388,15 @@
 
     async def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
@@ -409,15 +409,15 @@
         """
 
     async def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -431,15 +431,15 @@
 
     async def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
@@ -447,15 +447,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_utilization)
         """
 
     async def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
@@ -466,15 +466,15 @@
 
     async def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
@@ -489,44 +489,44 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: "ExpressionTypeDef" = ...
+        Filter: ExpressionUnionTypeDef = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_purchase_recommendation)
         """
 
     async def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_utilization)
         """
 
     async def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
@@ -538,15 +538,15 @@
 
     async def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
@@ -556,15 +556,15 @@
 
     async def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -680,15 +680,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: "ExpressionTypeDef" = ...
+        ThresholdExpression: ExpressionUnionTypeDef = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly monitor subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
@@ -707,15 +707,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_cost_category_definition)
         """
```

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/client.pyi` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -36,25 +36,25 @@
     SavingsPlansDataTypeType,
     SupportedSavingsPlansTypeType,
     TermInYearsType,
 )
 from .type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
-    AnomalySubscriptionTypeDef,
+    AnomalySubscriptionUnionTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostCategoryRuleTypeDef,
-    CostCategorySplitChargeRuleTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     CreateAnomalyMonitorResponseTypeDef,
     CreateAnomalySubscriptionResponseTypeDef,
     CreateCostCategoryDefinitionResponseTypeDef,
     DateIntervalTypeDef,
     DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
-    ExpressionTypeDef,
+    ExpressionUnionTypeDef,
     GetAnomaliesResponseTypeDef,
     GetAnomalyMonitorsResponseTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetCostCategoriesResponseTypeDef,
     GetCostForecastResponseTypeDef,
@@ -159,15 +159,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_monitor)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_monitor)
         """
     async def create_anomaly_subscription(
         self,
         *,
-        AnomalySubscription: AnomalySubscriptionTypeDef,
+        AnomalySubscription: AnomalySubscriptionUnionTypeDef,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateAnomalySubscriptionResponseTypeDef:
         """
         Adds an alert subscription to a cost anomaly detection monitor.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_anomaly_subscription)
@@ -176,15 +176,15 @@
         self,
         *,
         Name: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...,
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...,
         ResourceTags: Sequence[ResourceTagTypeDef] = ...
     ) -> CreateCostCategoryDefinitionResponseTypeDef:
         """
         Creates a new Cost Category with the requested name and rules.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.create_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#create_cost_category_definition)
@@ -281,30 +281,30 @@
         """
     async def get_cost_and_usage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
         Metrics: Sequence[str],
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageResponseTypeDef:
         """
         Retrieves cost and usage metrics for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_and_usage)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_cost_and_usage)
         """
     async def get_cost_and_usage_with_resources(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef",
+        Filter: ExpressionUnionTypeDef,
         Metrics: Sequence[str] = ...,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         NextPageToken: str = ...
     ) -> GetCostAndUsageWithResourcesResponseTypeDef:
         """
         Retrieves cost and usage metrics with resources for your account.
 
@@ -313,15 +313,15 @@
         """
     async def get_cost_categories(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         CostCategoryName: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetCostCategoriesResponseTypeDef:
         """
         Retrieves an array of Cost Category names and values incurred cost.
 
@@ -330,15 +330,15 @@
         """
     async def get_cost_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetCostForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will
         spend over the forecast time period that you select, based on your past costs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_cost_forecast)
@@ -347,15 +347,15 @@
     async def get_dimension_values(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Dimension: DimensionType,
         SearchString: str = ...,
         Context: ContextType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetDimensionValuesResponseTypeDef:
         """
         Retrieves all available filter values for a specified filter over a period of
         time.
@@ -365,15 +365,15 @@
         """
     async def get_reservation_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextPageToken: str = ...,
         SortBy: SortDefinitionTypeDef = ...,
         MaxResults: int = ...
     ) -> GetReservationCoverageResponseTypeDef:
         """
         Retrieves the reservation coverage for your account, which you can use to see
@@ -385,15 +385,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_coverage)
         """
     async def get_reservation_purchase_recommendation(
         self,
         *,
         Service: str,
         AccountId: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         AccountScope: AccountScopeType = ...,
         LookbackPeriodInDays: LookbackPeriodInDaysType = ...,
         TermInYears: TermInYearsType = ...,
         PaymentOption: PaymentOptionType = ...,
         ServiceSpecification: ServiceSpecificationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
@@ -406,30 +406,30 @@
         """
     async def get_reservation_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...,
         NextPageToken: str = ...,
         MaxResults: int = ...
     ) -> GetReservationUtilizationResponseTypeDef:
         """
         Retrieves the reservation utilization for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_reservation_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_reservation_utilization)
         """
     async def get_rightsizing_recommendation(
         self,
         *,
         Service: str,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Configuration: RightsizingRecommendationConfigurationTypeDef = ...,
         PageSize: int = ...,
         NextPageToken: str = ...
     ) -> GetRightsizingRecommendationResponseTypeDef:
         """
         Creates recommendations that help you save cost by identifying idle and
         underutilized Amazon EC2 instances.
@@ -439,15 +439,15 @@
         """
     async def get_savings_plans_coverage(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         GroupBy: Sequence[GroupDefinitionTypeDef] = ...,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         Metrics: Sequence[str] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansCoverageResponseTypeDef:
         """
         Retrieves the Savings Plans covered for your account.
@@ -461,42 +461,42 @@
         SavingsPlansType: SupportedSavingsPlansTypeType,
         TermInYears: TermInYearsType,
         PaymentOption: PaymentOptionType,
         LookbackPeriodInDays: LookbackPeriodInDaysType,
         AccountScope: AccountScopeType = ...,
         NextPageToken: str = ...,
         PageSize: int = ...,
-        Filter: "ExpressionTypeDef" = ...
+        Filter: ExpressionUnionTypeDef = ...
     ) -> GetSavingsPlansPurchaseRecommendationResponseTypeDef:
         """
         Retrieves the Savings Plans recommendations for your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_purchase_recommendation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_purchase_recommendation)
         """
     async def get_savings_plans_utilization(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Granularity: GranularityType = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationResponseTypeDef:
         """
         Retrieves the Savings Plans utilization for your account across date ranges with
         daily or monthly granularity.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_savings_plans_utilization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#get_savings_plans_utilization)
         """
     async def get_savings_plans_utilization_details(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         DataType: Sequence[SavingsPlansDataTypeType] = ...,
         NextToken: str = ...,
         MaxResults: int = ...,
         SortBy: SortDefinitionTypeDef = ...
     ) -> GetSavingsPlansUtilizationDetailsResponseTypeDef:
         """
         Retrieves attribute data along with aggregate utilization and savings data for a
@@ -507,15 +507,15 @@
         """
     async def get_tags(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         SearchString: str = ...,
         TagKey: str = ...,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         SortBy: Sequence[SortDefinitionTypeDef] = ...,
         MaxResults: int = ...,
         NextPageToken: str = ...
     ) -> GetTagsResponseTypeDef:
         """
         Queries for available tag keys and tag values for a specified period.
 
@@ -524,15 +524,15 @@
         """
     async def get_usage_forecast(
         self,
         *,
         TimePeriod: DateIntervalTypeDef,
         Metric: MetricType,
         Granularity: GranularityType,
-        Filter: "ExpressionTypeDef" = ...,
+        Filter: ExpressionUnionTypeDef = ...,
         PredictionIntervalLevel: int = ...
     ) -> GetUsageForecastResponseTypeDef:
         """
         Retrieves a forecast for how much Amazon Web Services predicts that you will use
         over the forecast time period that you select, based on your past usage.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.get_usage_forecast)
@@ -638,15 +638,15 @@
         *,
         SubscriptionArn: str,
         Threshold: float = ...,
         Frequency: AnomalySubscriptionFrequencyType = ...,
         MonitorArnList: Sequence[str] = ...,
         Subscribers: Sequence[SubscriberTypeDef] = ...,
         SubscriptionName: str = ...,
-        ThresholdExpression: "ExpressionTypeDef" = ...
+        ThresholdExpression: ExpressionUnionTypeDef = ...
     ) -> UpdateAnomalySubscriptionResponseTypeDef:
         """
         Updates an existing cost anomaly monitor subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_anomaly_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_anomaly_subscription)
         """
@@ -663,15 +663,15 @@
         self,
         *,
         CostCategoryArn: str,
         RuleVersion: Literal["CostCategoryExpression.v1"],
         Rules: Sequence[CostCategoryRuleTypeDef],
         EffectiveStart: str = ...,
         DefaultValue: str = ...,
-        SplitChargeRules: Sequence[CostCategorySplitChargeRuleTypeDef] = ...
+        SplitChargeRules: Sequence[CostCategorySplitChargeRuleUnionTypeDef] = ...
     ) -> UpdateCostCategoryDefinitionResponseTypeDef:
         """
         Updates an existing Cost Category.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer.Client.update_cost_category_definition)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/client/#update_cost_category_definition)
         """
```

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.py` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/literals.pyi` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.py` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ce.type_defs import AnomalyDateIntervalTypeDef
 
-    data: AnomalyDateIntervalTypeDef = {...}
+    data: AnomalyDateIntervalTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
     ContextType,
     CostAllocationTagStatusType,
@@ -53,113 +53,120 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AnomalyDateIntervalTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
+    "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "TagValuesTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagValuesOutputTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
+    "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
+    "TagValuesTypeDef",
+    "ExpressionUnionTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
-    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
-    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
+    "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
+    "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ExpressionTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
+    "GetCostCategoriesResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationTypeDef",
+    "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
     "GetDimensionValuesRequestRequestTypeDef",
     "GetReservationCoverageRequestRequestTypeDef",
@@ -174,34 +181,36 @@
     "InstanceDetailsTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
-    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomalySubscriptionsResponseTypeDef",
+    "AnomalySubscriptionUnionTypeDef",
+    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
-    "CreateCostCategoryDefinitionRequestRequestTypeDef",
-    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
+    "CostCategorySplitChargeRuleUnionTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
+    "CreateCostCategoryDefinitionRequestRequestTypeDef",
+    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
     "TargetInstanceTypeDef",
     "GetCostAndUsageResponseTypeDef",
     "GetCostAndUsageWithResourcesResponseTypeDef",
     "GetReservationUtilizationResponseTypeDef",
     "ReservationPurchaseRecommendationTypeDef",
@@ -223,21 +232,19 @@
     "_OptionalAnomalyDateIntervalTypeDef",
     {
         "EndDate": str,
     },
     total=False,
 )
 
-
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
-
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -251,19 +258,17 @@
         "MonitorDimension": Literal["SERVICE"],
         "MonitorSpecification": "ExpressionTypeDef",
         "DimensionalValueCount": int,
     },
     total=False,
 )
 
-
 class AnomalyMonitorTypeDef(_RequiredAnomalyMonitorTypeDef, _OptionalAnomalyMonitorTypeDef):
     pass
 
-
 AnomalyScoreTypeDef = TypedDict(
     "AnomalyScoreTypeDef",
     {
         "MaxScore": float,
         "CurrentScore": float,
     },
 )
@@ -291,19 +296,17 @@
         "TotalActualSpend": float,
         "TotalExpectedSpend": float,
         "TotalImpactPercentage": float,
     },
     total=False,
 )
 
-
 class ImpactTypeDef(_RequiredImpactTypeDef, _OptionalImpactTypeDef):
     pass
 
-
 RootCauseTypeDef = TypedDict(
     "RootCauseTypeDef",
     {
         "Service": str,
         "Region": str,
         "LinkedAccount": str,
         "UsageType": str,
@@ -343,22 +346,40 @@
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
     total=False,
 )
 
+CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
+    {
+        "Type": Literal["ALLOCATION_PERCENTAGES"],
+        "Values": List[str],
+    },
+)
+
 CostCategorySplitChargeRuleParameterTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": Sequence[str],
     },
 )
 
+CostCategoryValuesOutputTypeDef = TypedDict(
+    "CostCategoryValuesOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+    total=False,
+)
+
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -407,45 +428,31 @@
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-TagValuesTypeDef = TypedDict(
-    "TagValuesTypeDef",
+TagValuesOutputTypeDef = TypedDict(
+    "TagValuesOutputTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
-        "MatchOptions": Sequence[MatchOptionType],
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
     },
     total=False,
 )
 
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
@@ -463,44 +470,43 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveOn": str,
     },
     total=False,
 )
 
-
 class DescribeCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+DimensionValuesOutputTypeDef = TypedDict(
+    "DimensionValuesOutputTypeDef",
+    {
+        "Key": DimensionType,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+    total=False,
+)
 
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
@@ -610,14 +616,25 @@
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
     total=False,
 )
 
+TagValuesTypeDef = TypedDict(
+    "TagValuesTypeDef",
+    {
+        "Key": str,
+        "Values": Sequence[str],
+        "MatchOptions": Sequence[MatchOptionType],
+    },
+    total=False,
+)
+
+ExpressionUnionTypeDef = Union["ExpressionTypeDef", "ExpressionOutputTypeDef"]
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
@@ -637,21 +654,19 @@
     "_OptionalTotalImpactFilterTypeDef",
     {
         "EndValue": float,
     },
     total=False,
 )
 
-
 class TotalImpactFilterTypeDef(
     _RequiredTotalImpactFilterTypeDef, _OptionalTotalImpactFilterTypeDef
 ):
     pass
 
-
 GetAnomalyMonitorsRequestRequestTypeDef = TypedDict(
     "GetAnomalyMonitorsRequestRequestTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "NextPageToken": str,
         "MaxResults": int,
     },
@@ -688,31 +703,17 @@
     "_OptionalSortDefinitionTypeDef",
     {
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
-
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
-
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
     total=False,
@@ -797,43 +798,30 @@
         "NextPageToken": str,
         "PageSize": int,
         "Filter": "ExpressionTypeDef",
     },
     total=False,
 )
 
-
 class GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
-
 SavingsPlansPurchaseRecommendationMetadataTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
     total=False,
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "DatabaseEngine": str,
@@ -902,43 +890,24 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
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
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
     total=False,
@@ -1009,24 +978,14 @@
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
     total=False,
 )
 
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
     },
 )
@@ -1041,66 +1000,55 @@
     "_OptionalUpdateAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
     },
     total=False,
 )
 
-
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+_RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_RequiredAnomalySubscriptionOutputTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MonitorArnList": List[str],
+        "Subscribers": List[SubscriberTypeDef],
+        "Frequency": AnomalySubscriptionFrequencyType,
+        "SubscriptionName": str,
     },
 )
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
+_OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_OptionalAnomalySubscriptionOutputTypeDef",
     {
-        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubscriptionArn": str,
+        "AccountId": str,
+        "Threshold": float,
+        "ThresholdExpression": "ExpressionOutputTypeDef",
     },
+    total=False,
 )
 
+class AnomalySubscriptionOutputTypeDef(
+    _RequiredAnomalySubscriptionOutputTypeDef, _OptionalAnomalySubscriptionOutputTypeDef
+):
+    pass
+
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1113,21 +1061,19 @@
         "AccountId": str,
         "Threshold": float,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
-
 class AnomalySubscriptionTypeDef(
     _RequiredAnomalySubscriptionTypeDef, _OptionalAnomalySubscriptionTypeDef
 ):
     pass
 
-
 _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalySubscriptionRequestRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -1139,22 +1085,20 @@
         "Subscribers": Sequence[SubscriberTypeDef],
         "SubscriptionName": str,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
-
 class UpdateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredAnomalyTypeDef = TypedDict(
     "_RequiredAnomalyTypeDef",
     {
         "AnomalyId": str,
         "AnomalyScore": AnomalyScoreTypeDef,
         "Impact": ImpactTypeDef,
         "MonitorArn": str,
@@ -1168,35 +1112,24 @@
         "DimensionValue": str,
         "RootCauses": List[RootCauseTypeDef],
         "Feedback": AnomalyFeedbackTypeType,
     },
     total=False,
 )
 
-
 class AnomalyTypeDef(_RequiredAnomalyTypeDef, _OptionalAnomalyTypeDef):
     pass
 
-
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionTypeDef,
         "Type": CostCategoryRuleTypeType,
@@ -1215,14 +1148,36 @@
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
     total=False,
 )
 
+_RequiredCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_RequiredCostCategorySplitChargeRuleOutputTypeDef",
+    {
+        "Source": str,
+        "Targets": List[str],
+        "Method": CostCategorySplitChargeMethodType,
+    },
+)
+_OptionalCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_OptionalCostCategorySplitChargeRuleOutputTypeDef",
+    {
+        "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+class CostCategorySplitChargeRuleOutputTypeDef(
+    _RequiredCostCategorySplitChargeRuleOutputTypeDef,
+    _OptionalCostCategorySplitChargeRuleOutputTypeDef,
+):
+    pass
+
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
         "Method": CostCategorySplitChargeMethodType,
     },
@@ -1231,21 +1186,19 @@
     "_OptionalCostCategorySplitChargeRuleTypeDef",
     {
         "Parameters": Sequence[CostCategorySplitChargeRuleParameterTypeDef],
     },
     total=False,
 )
 
-
 class CostCategorySplitChargeRuleTypeDef(
     _RequiredCostCategorySplitChargeRuleTypeDef, _OptionalCostCategorySplitChargeRuleTypeDef
 ):
     pass
 
-
 ForecastResultTypeDef = TypedDict(
     "ForecastResultTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
@@ -1266,21 +1219,19 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
-
 class GetCostForecastRequestRequestTypeDef(
     _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1290,21 +1241,19 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
-
 class GetUsageForecastRequestRequestTypeDef(
     _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
 ):
     pass
 
-
 CoverageTypeDef = TypedDict(
     "CoverageTypeDef",
     {
         "CoverageHours": CoverageHoursTypeDef,
         "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
         "CoverageCost": CoverageCostTypeDef,
     },
@@ -1321,59 +1270,175 @@
     "_OptionalCreateAnomalyMonitorRequestRequestTypeDef",
     {
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class CreateAnomalyMonitorRequestRequestTypeDef(
     _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
     _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+)
+
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
     {
-        "ResourceArn": str,
-        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "AnomalyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExpressionTypeDef = TypedDict(
-    "ExpressionTypeDef",
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
-        "Or": Sequence[Dict[str, Any]],
-        "And": Sequence[Dict[str, Any]],
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExpressionOutputTypeDef = TypedDict(
+    "ExpressionOutputTypeDef",
+    {
+        "Or": List[Dict[str, Any]],
+        "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesTypeDef,
-        "Tags": TagValuesTypeDef,
-        "CostCategories": CostCategoryValuesTypeDef,
+        "Dimensions": DimensionValuesOutputTypeDef,
+        "Tags": TagValuesOutputTypeDef,
+        "CostCategories": CostCategoryValuesOutputTypeDef,
     },
     total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
@@ -1398,20 +1463,33 @@
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
 
+ExpressionTypeDef = TypedDict(
+    "ExpressionTypeDef",
+    {
+        "Or": Sequence[Dict[str, Any]],
+        "And": Sequence[Dict[str, Any]],
+        "Not": Dict[str, Any],
+        "Dimensions": DimensionValuesTypeDef,
+        "Tags": TagValuesTypeDef,
+        "CostCategories": CostCategoryValuesTypeDef,
+    },
+    total=False,
+)
+
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1425,21 +1503,19 @@
         "TotalImpact": TotalImpactFilterTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetAnomaliesRequestRequestTypeDef(
     _RequiredGetAnomaliesRequestRequestTypeDef, _OptionalGetAnomaliesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetCostAndUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Metrics": Sequence[str],
     },
@@ -1450,21 +1526,19 @@
         "Filter": "ExpressionTypeDef",
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetCostAndUsageRequestRequestTypeDef(
     _RequiredGetCostAndUsageRequestRequestTypeDef, _OptionalGetCostAndUsageRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
     },
@@ -1475,22 +1549,20 @@
         "Metrics": Sequence[str],
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetCostAndUsageWithResourcesRequestRequestTypeDef(
     _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef,
     _OptionalGetCostAndUsageWithResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCostCategoriesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostCategoriesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetCostCategoriesRequestRequestTypeDef = TypedDict(
@@ -1502,21 +1574,19 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetCostCategoriesRequestRequestTypeDef(
     _RequiredGetCostCategoriesRequestRequestTypeDef, _OptionalGetCostCategoriesRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredGetDimensionValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetDimensionValuesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Dimension": DimensionType,
     },
 )
@@ -1529,22 +1599,20 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetDimensionValuesRequestRequestTypeDef(
     _RequiredGetDimensionValuesRequestRequestTypeDef,
     _OptionalGetDimensionValuesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetReservationCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationCoverageRequestRequestTypeDef = TypedDict(
@@ -1557,22 +1625,20 @@
         "NextPageToken": str,
         "SortBy": SortDefinitionTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetReservationCoverageRequestRequestTypeDef(
     _RequiredGetReservationCoverageRequestRequestTypeDef,
     _OptionalGetReservationCoverageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetReservationUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationUtilizationRequestRequestTypeDef = TypedDict(
@@ -1584,22 +1650,20 @@
         "SortBy": SortDefinitionTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class GetReservationUtilizationRequestRequestTypeDef(
     _RequiredGetReservationUtilizationRequestRequestTypeDef,
     _OptionalGetReservationUtilizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
@@ -1612,22 +1676,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class GetSavingsPlansCoverageRequestRequestTypeDef(
     _RequiredGetSavingsPlansCoverageRequestRequestTypeDef,
     _OptionalGetSavingsPlansCoverageRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
@@ -1638,22 +1700,20 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class GetSavingsPlansUtilizationDetailsRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
@@ -1662,22 +1722,20 @@
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
-
 class GetSavingsPlansUtilizationRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetTagsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTagsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetTagsRequestRequestTypeDef = TypedDict(
@@ -1689,21 +1747,19 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetTagsRequestRequestTypeDef(
     _RequiredGetTagsRequestRequestTypeDef, _OptionalGetTagsRequestRequestTypeDef
 ):
     pass
 
-
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Keys": List[str],
         "Metrics": Dict[str, MetricValueTypeDef],
     },
     total=False,
@@ -1733,22 +1789,20 @@
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetRightsizingRecommendationRequestRequestTypeDef(
     _RequiredGetRightsizingRecommendationRequestRequestTypeDef,
     _OptionalGetRightsizingRecommendationRequestRequestTypeDef,
 ):
     pass
 
-
 InstanceDetailsTypeDef = TypedDict(
     "InstanceDetailsTypeDef",
     {
         "EC2InstanceDetails": EC2InstanceDetailsTypeDef,
         "RDSInstanceDetails": RDSInstanceDetailsTypeDef,
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
@@ -1801,22 +1855,20 @@
     {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
     total=False,
 )
 
-
 class SavingsPlansUtilizationAggregatesTypeDef(
     _RequiredSavingsPlansUtilizationAggregatesTypeDef,
     _OptionalSavingsPlansUtilizationAggregatesTypeDef,
 ):
     pass
 
-
 _RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
     "_RequiredSavingsPlansUtilizationByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
     },
 )
@@ -1825,21 +1877,19 @@
     {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
     total=False,
 )
 
-
 class SavingsPlansUtilizationByTimeTypeDef(
     _RequiredSavingsPlansUtilizationByTimeTypeDef, _OptionalSavingsPlansUtilizationByTimeTypeDef
 ):
     pass
 
-
 SavingsPlansUtilizationDetailTypeDef = TypedDict(
     "SavingsPlansUtilizationDetailTypeDef",
     {
         "SavingsPlanArn": str,
         "Attributes": Dict[str, str],
         "Utilization": SavingsPlansUtilizationTypeDef,
         "Savings": SavingsPlansSavingsTypeDef,
@@ -1848,64 +1898,65 @@
     total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalySubscriptionsResponseTypeDef = TypedDict(
+    "GetAnomalySubscriptionsResponseTypeDef",
+    {
+        "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AnomalySubscriptionUnionTypeDef = Union[
+    AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef
+]
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
     },
 )
 _OptionalCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
-
 class CreateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredCreateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalCreateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-
-GetAnomalySubscriptionsResponseTypeDef = TypedDict(
-    "GetAnomalySubscriptionsResponseTypeDef",
-    {
-        "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCostCategoryTypeDef = TypedDict(
     "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
@@ -1915,94 +1966,42 @@
         "Rules": List[CostCategoryRuleTypeDef],
     },
 )
 _OptionalCostCategoryTypeDef = TypedDict(
     "_OptionalCostCategoryTypeDef",
     {
         "EffectiveEnd": str,
-        "SplitChargeRules": List[CostCategorySplitChargeRuleTypeDef],
+        "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
     total=False,
 )
 
-
 class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
     pass
 
-
-_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
-
-
-class CreateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
-_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "CostCategoryArn": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
-    },
-    total=False,
-)
-
-
-class UpdateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
-
-
+CostCategorySplitChargeRuleUnionTypeDef = Union[
+    CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef
+]
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
@@ -2037,22 +2036,20 @@
         "ServiceSpecification": ServiceSpecificationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
-
 class GetReservationPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetReservationPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
-
 ResultByTimeTypeDef = TypedDict(
     "ResultByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
@@ -2097,15 +2094,15 @@
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2124,37 +2121,86 @@
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
         "TimePeriod": DateIntervalTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+    total=False,
+)
+
+class CreateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "CostCategoryArn": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
     },
+    total=False,
 )
 
+class UpdateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
     },
@@ -2162,15 +2208,15 @@
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
-        "Tags": List[TagValuesTypeDef],
+        "Tags": List[TagValuesOutputTypeDef],
         "ResourceDetails": ResourceDetailsTypeDef,
         "ResourceUtilization": ResourceUtilizationTypeDef,
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
@@ -2196,36 +2242,36 @@
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2241,25 +2287,25 @@
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
@@ -2269,15 +2315,15 @@
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
@@ -2294,10 +2340,10 @@
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce/type_defs.pyi` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_ce.type_defs import AnomalyDateIntervalTypeDef
 
-    data: AnomalyDateIntervalTypeDef = {...}
+    data: AnomalyDateIntervalTypeDef = ...
     ```
 """
 import sys
-from typing import Any, Dict, List, Sequence
+from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
     AccountScopeType,
     AnomalyFeedbackTypeType,
     AnomalySubscriptionFrequencyType,
     ContextType,
     CostAllocationTagStatusType,
@@ -53,112 +53,121 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AnomalyDateIntervalTypeDef",
     "AnomalyMonitorTypeDef",
     "AnomalyScoreTypeDef",
     "SubscriberTypeDef",
     "ImpactTypeDef",
     "RootCauseTypeDef",
     "CostAllocationTagStatusEntryTypeDef",
     "CostAllocationTagTypeDef",
     "CostCategoryInheritedValueDimensionTypeDef",
     "CostCategoryProcessingStatusTypeDef",
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
     "CostCategorySplitChargeRuleParameterTypeDef",
+    "CostCategoryValuesOutputTypeDef",
     "CostCategoryValuesTypeDef",
     "DateIntervalTypeDef",
     "CoverageCostTypeDef",
     "CoverageHoursTypeDef",
     "CoverageNormalizedUnitsTypeDef",
     "ResourceTagTypeDef",
-    "CreateAnomalyMonitorResponseTypeDef",
-    "CreateAnomalySubscriptionResponseTypeDef",
-    "CreateCostCategoryDefinitionResponseTypeDef",
-    "TagValuesTypeDef",
+    "ResponseMetadataTypeDef",
+    "TagValuesOutputTypeDef",
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     "DeleteAnomalySubscriptionRequestRequestTypeDef",
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
-    "DeleteCostCategoryDefinitionResponseTypeDef",
     "DescribeCostCategoryDefinitionRequestRequestTypeDef",
+    "DimensionValuesOutputTypeDef",
     "DimensionValuesTypeDef",
     "DimensionValuesWithAttributesTypeDef",
     "DiskResourceUtilizationTypeDef",
     "EBSResourceUtilizationTypeDef",
     "EC2InstanceDetailsTypeDef",
     "EC2ResourceDetailsTypeDef",
     "NetworkResourceUtilizationTypeDef",
     "EC2SpecificationTypeDef",
     "ESInstanceDetailsTypeDef",
     "ElastiCacheInstanceDetailsTypeDef",
+    "TagValuesTypeDef",
+    "ExpressionUnionTypeDef",
     "GenerationSummaryTypeDef",
     "TotalImpactFilterTypeDef",
     "GetAnomalyMonitorsRequestRequestTypeDef",
     "GetAnomalySubscriptionsRequestRequestTypeDef",
     "GroupDefinitionTypeDef",
     "SortDefinitionTypeDef",
-    "GetCostCategoriesResponseTypeDef",
     "MetricValueTypeDef",
     "ReservationPurchaseRecommendationMetadataTypeDef",
     "ReservationAggregatesTypeDef",
     "RightsizingRecommendationConfigurationTypeDef",
     "RightsizingRecommendationMetadataTypeDef",
     "RightsizingRecommendationSummaryTypeDef",
     "GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef",
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
-    "GetTagsResponseTypeDef",
     "RDSInstanceDetailsTypeDef",
     "RedshiftInstanceDetailsTypeDef",
     "ListCostAllocationTagsRequestRequestTypeDef",
     "ListCostCategoryDefinitionsRequestRequestTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
-    "ProvideAnomalyFeedbackResponseTypeDef",
     "ReservationPurchaseRecommendationSummaryTypeDef",
-    "ResponseMetadataTypeDef",
     "TerminateRecommendationDetailTypeDef",
     "SavingsPlansAmortizedCommitmentTypeDef",
     "SavingsPlansCoverageDataTypeDef",
     "SavingsPlansDetailsTypeDef",
     "SavingsPlansPurchaseRecommendationSummaryTypeDef",
     "SavingsPlansSavingsTypeDef",
     "SavingsPlansUtilizationTypeDef",
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAnomalyMonitorRequestRequestTypeDef",
-    "UpdateAnomalyMonitorResponseTypeDef",
-    "UpdateAnomalySubscriptionResponseTypeDef",
     "UpdateCostAllocationTagsStatusErrorTypeDef",
-    "UpdateCostCategoryDefinitionResponseTypeDef",
-    "GetAnomalyMonitorsResponseTypeDef",
+    "AnomalySubscriptionOutputTypeDef",
     "AnomalySubscriptionTypeDef",
     "UpdateAnomalySubscriptionRequestRequestTypeDef",
     "AnomalyTypeDef",
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
-    "ListCostAllocationTagsResponseTypeDef",
     "CostCategoryRuleTypeDef",
     "CostCategoryReferenceTypeDef",
+    "CostCategorySplitChargeRuleOutputTypeDef",
     "CostCategorySplitChargeRuleTypeDef",
     "ForecastResultTypeDef",
     "GetCostForecastRequestRequestTypeDef",
     "GetUsageForecastRequestRequestTypeDef",
     "CoverageTypeDef",
     "CreateAnomalyMonitorRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
-    "ExpressionTypeDef",
+    "CreateAnomalyMonitorResponseTypeDef",
+    "CreateAnomalySubscriptionResponseTypeDef",
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    "GetAnomalyMonitorsResponseTypeDef",
+    "GetCostCategoriesResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "ListCostAllocationTagsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ProvideAnomalyFeedbackResponseTypeDef",
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
+    "UpdateAnomalyMonitorResponseTypeDef",
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    "ExpressionOutputTypeDef",
     "GetDimensionValuesResponseTypeDef",
     "ResourceDetailsTypeDef",
     "EC2ResourceUtilizationTypeDef",
     "ServiceSpecificationTypeDef",
+    "ExpressionTypeDef",
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     "GetAnomaliesRequestRequestTypeDef",
     "GetCostAndUsageRequestRequestTypeDef",
     "GetCostAndUsageWithResourcesRequestRequestTypeDef",
     "GetCostCategoriesRequestRequestTypeDef",
     "GetDimensionValuesRequestRequestTypeDef",
     "GetReservationCoverageRequestRequestTypeDef",
@@ -173,34 +182,36 @@
     "InstanceDetailsTypeDef",
     "SavingsPlansCoverageTypeDef",
     "SavingsPlansPurchaseRecommendationDetailTypeDef",
     "SavingsPlansUtilizationAggregatesTypeDef",
     "SavingsPlansUtilizationByTimeTypeDef",
     "SavingsPlansUtilizationDetailTypeDef",
     "UpdateCostAllocationTagsStatusResponseTypeDef",
-    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomalySubscriptionsResponseTypeDef",
+    "AnomalySubscriptionUnionTypeDef",
+    "CreateAnomalySubscriptionRequestRequestTypeDef",
     "GetAnomaliesResponseTypeDef",
     "ListCostCategoryDefinitionsResponseTypeDef",
     "CostCategoryTypeDef",
-    "CreateCostCategoryDefinitionRequestRequestTypeDef",
-    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
+    "CostCategorySplitChargeRuleUnionTypeDef",
     "GetCostForecastResponseTypeDef",
     "GetUsageForecastResponseTypeDef",
     "ReservationCoverageGroupTypeDef",
     "ResourceUtilizationTypeDef",
     "GetReservationPurchaseRecommendationRequestRequestTypeDef",
     "ResultByTimeTypeDef",
     "UtilizationByTimeTypeDef",
     "ReservationPurchaseRecommendationDetailTypeDef",
     "GetSavingsPlansCoverageResponseTypeDef",
     "SavingsPlansPurchaseRecommendationTypeDef",
     "GetSavingsPlansUtilizationResponseTypeDef",
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     "DescribeCostCategoryDefinitionResponseTypeDef",
+    "CreateCostCategoryDefinitionRequestRequestTypeDef",
+    "UpdateCostCategoryDefinitionRequestRequestTypeDef",
     "CoverageByTimeTypeDef",
     "CurrentInstanceTypeDef",
     "TargetInstanceTypeDef",
     "GetCostAndUsageResponseTypeDef",
     "GetCostAndUsageWithResourcesResponseTypeDef",
     "GetReservationUtilizationResponseTypeDef",
     "ReservationPurchaseRecommendationTypeDef",
@@ -222,19 +233,21 @@
     "_OptionalAnomalyDateIntervalTypeDef",
     {
         "EndDate": str,
     },
     total=False,
 )
 
+
 class AnomalyDateIntervalTypeDef(
     _RequiredAnomalyDateIntervalTypeDef, _OptionalAnomalyDateIntervalTypeDef
 ):
     pass
 
+
 _RequiredAnomalyMonitorTypeDef = TypedDict(
     "_RequiredAnomalyMonitorTypeDef",
     {
         "MonitorName": str,
         "MonitorType": MonitorTypeType,
     },
 )
@@ -248,17 +261,19 @@
         "MonitorDimension": Literal["SERVICE"],
         "MonitorSpecification": "ExpressionTypeDef",
         "DimensionalValueCount": int,
     },
     total=False,
 )
 
+
 class AnomalyMonitorTypeDef(_RequiredAnomalyMonitorTypeDef, _OptionalAnomalyMonitorTypeDef):
     pass
 
+
 AnomalyScoreTypeDef = TypedDict(
     "AnomalyScoreTypeDef",
     {
         "MaxScore": float,
         "CurrentScore": float,
     },
 )
@@ -286,17 +301,19 @@
         "TotalActualSpend": float,
         "TotalExpectedSpend": float,
         "TotalImpactPercentage": float,
     },
     total=False,
 )
 
+
 class ImpactTypeDef(_RequiredImpactTypeDef, _OptionalImpactTypeDef):
     pass
 
+
 RootCauseTypeDef = TypedDict(
     "RootCauseTypeDef",
     {
         "Service": str,
         "Region": str,
         "LinkedAccount": str,
         "UsageType": str,
@@ -336,22 +353,40 @@
     {
         "Component": Literal["COST_EXPLORER"],
         "Status": CostCategoryStatusType,
     },
     total=False,
 )
 
+CostCategorySplitChargeRuleParameterOutputTypeDef = TypedDict(
+    "CostCategorySplitChargeRuleParameterOutputTypeDef",
+    {
+        "Type": Literal["ALLOCATION_PERCENTAGES"],
+        "Values": List[str],
+    },
+)
+
 CostCategorySplitChargeRuleParameterTypeDef = TypedDict(
     "CostCategorySplitChargeRuleParameterTypeDef",
     {
         "Type": Literal["ALLOCATION_PERCENTAGES"],
         "Values": Sequence[str],
     },
 )
 
+CostCategoryValuesOutputTypeDef = TypedDict(
+    "CostCategoryValuesOutputTypeDef",
+    {
+        "Key": str,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+    total=False,
+)
+
 CostCategoryValuesTypeDef = TypedDict(
     "CostCategoryValuesTypeDef",
     {
         "Key": str,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -400,45 +435,31 @@
     "ResourceTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateAnomalyMonitorResponseTypeDef = TypedDict(
-    "CreateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "CreateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "CreateCostCategoryDefinitionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-TagValuesTypeDef = TypedDict(
-    "TagValuesTypeDef",
+TagValuesOutputTypeDef = TypedDict(
+    "TagValuesOutputTypeDef",
     {
         "Key": str,
-        "Values": Sequence[str],
-        "MatchOptions": Sequence[MatchOptionType],
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
     },
     total=False,
 )
 
 DeleteAnomalyMonitorRequestRequestTypeDef = TypedDict(
     "DeleteAnomalyMonitorRequestRequestTypeDef",
     {
@@ -456,43 +477,46 @@
 DeleteCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 
-DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "DeleteCostCategoryDefinitionResponseTypeDef",
-    {
-        "CostCategoryArn": str,
-        "EffectiveEnd": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "CostCategoryArn": str,
     },
 )
 _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
     "_OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef",
     {
         "EffectiveOn": str,
     },
     total=False,
 )
 
+
 class DescribeCostCategoryDefinitionRequestRequestTypeDef(
     _RequiredDescribeCostCategoryDefinitionRequestRequestTypeDef,
     _OptionalDescribeCostCategoryDefinitionRequestRequestTypeDef,
 ):
     pass
 
+
+DimensionValuesOutputTypeDef = TypedDict(
+    "DimensionValuesOutputTypeDef",
+    {
+        "Key": DimensionType,
+        "Values": List[str],
+        "MatchOptions": List[MatchOptionType],
+    },
+    total=False,
+)
+
 DimensionValuesTypeDef = TypedDict(
     "DimensionValuesTypeDef",
     {
         "Key": DimensionType,
         "Values": Sequence[str],
         "MatchOptions": Sequence[MatchOptionType],
     },
@@ -601,14 +625,25 @@
         "ProductDescription": str,
         "CurrentGeneration": bool,
         "SizeFlexEligible": bool,
     },
     total=False,
 )
 
+TagValuesTypeDef = TypedDict(
+    "TagValuesTypeDef",
+    {
+        "Key": str,
+        "Values": Sequence[str],
+        "MatchOptions": Sequence[MatchOptionType],
+    },
+    total=False,
+)
+
+ExpressionUnionTypeDef = Union["ExpressionTypeDef", "ExpressionOutputTypeDef"]
 GenerationSummaryTypeDef = TypedDict(
     "GenerationSummaryTypeDef",
     {
         "RecommendationId": str,
         "GenerationStatus": GenerationStatusType,
         "GenerationStartedTime": str,
         "GenerationCompletionTime": str,
@@ -628,19 +663,21 @@
     "_OptionalTotalImpactFilterTypeDef",
     {
         "EndValue": float,
     },
     total=False,
 )
 
+
 class TotalImpactFilterTypeDef(
     _RequiredTotalImpactFilterTypeDef, _OptionalTotalImpactFilterTypeDef
 ):
     pass
 
+
 GetAnomalyMonitorsRequestRequestTypeDef = TypedDict(
     "GetAnomalyMonitorsRequestRequestTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "NextPageToken": str,
         "MaxResults": int,
     },
@@ -677,28 +714,18 @@
     "_OptionalSortDefinitionTypeDef",
     {
         "SortOrder": SortOrderType,
     },
     total=False,
 )
 
+
 class SortDefinitionTypeDef(_RequiredSortDefinitionTypeDef, _OptionalSortDefinitionTypeDef):
     pass
 
-GetCostCategoriesResponseTypeDef = TypedDict(
-    "GetCostCategoriesResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "CostCategoryNames": List[str],
-        "CostCategoryValues": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 MetricValueTypeDef = TypedDict(
     "MetricValueTypeDef",
     {
         "Amount": str,
         "Unit": str,
     },
@@ -784,41 +811,32 @@
         "NextPageToken": str,
         "PageSize": int,
         "Filter": "ExpressionTypeDef",
     },
     total=False,
 )
 
+
 class GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
+
 SavingsPlansPurchaseRecommendationMetadataTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationMetadataTypeDef",
     {
         "RecommendationId": str,
         "GenerationTimestamp": str,
         "AdditionalMetadata": str,
     },
     total=False,
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "NextPageToken": str,
-        "Tags": List[str],
-        "ReturnSize": int,
-        "TotalSize": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RDSInstanceDetailsTypeDef = TypedDict(
     "RDSInstanceDetailsTypeDef",
     {
         "Family": str,
         "InstanceType": str,
         "Region": str,
         "DatabaseEngine": str,
@@ -887,43 +905,24 @@
     "ProvideAnomalyFeedbackRequestRequestTypeDef",
     {
         "AnomalyId": str,
         "Feedback": AnomalyFeedbackTypeType,
     },
 )
 
-ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
-    "ProvideAnomalyFeedbackResponseTypeDef",
-    {
-        "AnomalyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ReservationPurchaseRecommendationSummaryTypeDef = TypedDict(
     "ReservationPurchaseRecommendationSummaryTypeDef",
     {
         "TotalEstimatedMonthlySavingsAmount": str,
         "TotalEstimatedMonthlySavingsPercentage": str,
         "CurrencyCode": str,
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
 TerminateRecommendationDetailTypeDef = TypedDict(
     "TerminateRecommendationDetailTypeDef",
     {
         "EstimatedMonthlySavings": str,
         "CurrencyCode": str,
     },
     total=False,
@@ -994,24 +993,14 @@
         "UsedCommitment": str,
         "UnusedCommitment": str,
         "UtilizationPercentage": str,
     },
     total=False,
 )
 
-StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
-    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
-    {
-        "RecommendationId": str,
-        "GenerationStartedTime": str,
-        "EstimatedCompletionTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "ResourceTagKeys": Sequence[str],
     },
 )
@@ -1026,64 +1015,59 @@
     "_OptionalUpdateAnomalyMonitorRequestRequestTypeDef",
     {
         "MonitorName": str,
     },
     total=False,
 )
 
+
 class UpdateAnomalyMonitorRequestRequestTypeDef(
     _RequiredUpdateAnomalyMonitorRequestRequestTypeDef,
     _OptionalUpdateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
-UpdateAnomalyMonitorResponseTypeDef = TypedDict(
-    "UpdateAnomalyMonitorResponseTypeDef",
-    {
-        "MonitorArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
-    "UpdateAnomalySubscriptionResponseTypeDef",
-    {
-        "SubscriptionArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 UpdateCostAllocationTagsStatusErrorTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusErrorTypeDef",
     {
         "TagKey": str,
         "Code": str,
         "Message": str,
     },
     total=False,
 )
 
-UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
-    "UpdateCostCategoryDefinitionResponseTypeDef",
+_RequiredAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_RequiredAnomalySubscriptionOutputTypeDef",
     {
-        "CostCategoryArn": str,
-        "EffectiveStart": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MonitorArnList": List[str],
+        "Subscribers": List[SubscriberTypeDef],
+        "Frequency": AnomalySubscriptionFrequencyType,
+        "SubscriptionName": str,
     },
 )
-
-GetAnomalyMonitorsResponseTypeDef = TypedDict(
-    "GetAnomalyMonitorsResponseTypeDef",
+_OptionalAnomalySubscriptionOutputTypeDef = TypedDict(
+    "_OptionalAnomalySubscriptionOutputTypeDef",
     {
-        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SubscriptionArn": str,
+        "AccountId": str,
+        "Threshold": float,
+        "ThresholdExpression": "ExpressionOutputTypeDef",
     },
+    total=False,
 )
 
+
+class AnomalySubscriptionOutputTypeDef(
+    _RequiredAnomalySubscriptionOutputTypeDef, _OptionalAnomalySubscriptionOutputTypeDef
+):
+    pass
+
+
 _RequiredAnomalySubscriptionTypeDef = TypedDict(
     "_RequiredAnomalySubscriptionTypeDef",
     {
         "MonitorArnList": Sequence[str],
         "Subscribers": Sequence[SubscriberTypeDef],
         "Frequency": AnomalySubscriptionFrequencyType,
         "SubscriptionName": str,
@@ -1096,19 +1080,21 @@
         "AccountId": str,
         "Threshold": float,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
+
 class AnomalySubscriptionTypeDef(
     _RequiredAnomalySubscriptionTypeDef, _OptionalAnomalySubscriptionTypeDef
 ):
     pass
 
+
 _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAnomalySubscriptionRequestRequestTypeDef",
     {
         "SubscriptionArn": str,
     },
 )
 _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
@@ -1120,20 +1106,22 @@
         "Subscribers": Sequence[SubscriberTypeDef],
         "SubscriptionName": str,
         "ThresholdExpression": "ExpressionTypeDef",
     },
     total=False,
 )
 
+
 class UpdateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredUpdateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalUpdateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredAnomalyTypeDef = TypedDict(
     "_RequiredAnomalyTypeDef",
     {
         "AnomalyId": str,
         "AnomalyScore": AnomalyScoreTypeDef,
         "Impact": ImpactTypeDef,
         "MonitorArn": str,
@@ -1147,33 +1135,26 @@
         "DimensionValue": str,
         "RootCauses": List[RootCauseTypeDef],
         "Feedback": AnomalyFeedbackTypeType,
     },
     total=False,
 )
 
+
 class AnomalyTypeDef(_RequiredAnomalyTypeDef, _OptionalAnomalyTypeDef):
     pass
 
+
 UpdateCostAllocationTagsStatusRequestRequestTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusRequestRequestTypeDef",
     {
         "CostAllocationTagsStatus": Sequence[CostAllocationTagStatusEntryTypeDef],
     },
 )
 
-ListCostAllocationTagsResponseTypeDef = TypedDict(
-    "ListCostAllocationTagsResponseTypeDef",
-    {
-        "CostAllocationTags": List[CostAllocationTagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CostCategoryRuleTypeDef = TypedDict(
     "CostCategoryRuleTypeDef",
     {
         "Value": str,
         "Rule": "ExpressionTypeDef",
         "InheritedValue": CostCategoryInheritedValueDimensionTypeDef,
         "Type": CostCategoryRuleTypeType,
@@ -1192,14 +1173,38 @@
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "Values": List[str],
         "DefaultValue": str,
     },
     total=False,
 )
 
+_RequiredCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_RequiredCostCategorySplitChargeRuleOutputTypeDef",
+    {
+        "Source": str,
+        "Targets": List[str],
+        "Method": CostCategorySplitChargeMethodType,
+    },
+)
+_OptionalCostCategorySplitChargeRuleOutputTypeDef = TypedDict(
+    "_OptionalCostCategorySplitChargeRuleOutputTypeDef",
+    {
+        "Parameters": List[CostCategorySplitChargeRuleParameterOutputTypeDef],
+    },
+    total=False,
+)
+
+
+class CostCategorySplitChargeRuleOutputTypeDef(
+    _RequiredCostCategorySplitChargeRuleOutputTypeDef,
+    _OptionalCostCategorySplitChargeRuleOutputTypeDef,
+):
+    pass
+
+
 _RequiredCostCategorySplitChargeRuleTypeDef = TypedDict(
     "_RequiredCostCategorySplitChargeRuleTypeDef",
     {
         "Source": str,
         "Targets": Sequence[str],
         "Method": CostCategorySplitChargeMethodType,
     },
@@ -1208,19 +1213,21 @@
     "_OptionalCostCategorySplitChargeRuleTypeDef",
     {
         "Parameters": Sequence[CostCategorySplitChargeRuleParameterTypeDef],
     },
     total=False,
 )
 
+
 class CostCategorySplitChargeRuleTypeDef(
     _RequiredCostCategorySplitChargeRuleTypeDef, _OptionalCostCategorySplitChargeRuleTypeDef
 ):
     pass
 
+
 ForecastResultTypeDef = TypedDict(
     "ForecastResultTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "MeanValue": str,
         "PredictionIntervalLowerBound": str,
         "PredictionIntervalUpperBound": str,
@@ -1241,19 +1248,21 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
+
 class GetCostForecastRequestRequestTypeDef(
     _RequiredGetCostForecastRequestRequestTypeDef, _OptionalGetCostForecastRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetUsageForecastRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageForecastRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Metric": MetricType,
         "Granularity": GranularityType,
     },
@@ -1263,19 +1272,21 @@
     {
         "Filter": "ExpressionTypeDef",
         "PredictionIntervalLevel": int,
     },
     total=False,
 )
 
+
 class GetUsageForecastRequestRequestTypeDef(
     _RequiredGetUsageForecastRequestRequestTypeDef, _OptionalGetUsageForecastRequestRequestTypeDef
 ):
     pass
 
+
 CoverageTypeDef = TypedDict(
     "CoverageTypeDef",
     {
         "CoverageHours": CoverageHoursTypeDef,
         "CoverageNormalizedUnits": CoverageNormalizedUnitsTypeDef,
         "CoverageCost": CoverageCostTypeDef,
     },
@@ -1292,57 +1303,177 @@
     "_OptionalCreateAnomalyMonitorRequestRequestTypeDef",
     {
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class CreateAnomalyMonitorRequestRequestTypeDef(
     _RequiredCreateAnomalyMonitorRequestRequestTypeDef,
     _OptionalCreateAnomalyMonitorRequestRequestTypeDef,
 ):
     pass
 
+
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+)
+
+CreateAnomalyMonitorResponseTypeDef = TypedDict(
+    "CreateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "CreateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "CreateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "DeleteCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveEnd": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalyMonitorsResponseTypeDef = TypedDict(
+    "GetAnomalyMonitorsResponseTypeDef",
+    {
+        "AnomalyMonitors": List[AnomalyMonitorTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCostCategoriesResponseTypeDef = TypedDict(
+    "GetCostCategoriesResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "CostCategoryNames": List[str],
+        "CostCategoryValues": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "NextPageToken": str,
+        "Tags": List[str],
+        "ReturnSize": int,
+        "TotalSize": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListCostAllocationTagsResponseTypeDef = TypedDict(
+    "ListCostAllocationTagsResponseTypeDef",
+    {
+        "CostAllocationTags": List[CostAllocationTagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+ProvideAnomalyFeedbackResponseTypeDef = TypedDict(
+    "ProvideAnomalyFeedbackResponseTypeDef",
     {
-        "ResourceArn": str,
-        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "AnomalyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ExpressionTypeDef = TypedDict(
-    "ExpressionTypeDef",
+StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
+    "StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
-        "Or": Sequence[Dict[str, Any]],
-        "And": Sequence[Dict[str, Any]],
+        "RecommendationId": str,
+        "GenerationStartedTime": str,
+        "EstimatedCompletionTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalyMonitorResponseTypeDef = TypedDict(
+    "UpdateAnomalyMonitorResponseTypeDef",
+    {
+        "MonitorArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAnomalySubscriptionResponseTypeDef = TypedDict(
+    "UpdateAnomalySubscriptionResponseTypeDef",
+    {
+        "SubscriptionArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateCostCategoryDefinitionResponseTypeDef = TypedDict(
+    "UpdateCostCategoryDefinitionResponseTypeDef",
+    {
+        "CostCategoryArn": str,
+        "EffectiveStart": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExpressionOutputTypeDef = TypedDict(
+    "ExpressionOutputTypeDef",
+    {
+        "Or": List[Dict[str, Any]],
+        "And": List[Dict[str, Any]],
         "Not": Dict[str, Any],
-        "Dimensions": DimensionValuesTypeDef,
-        "Tags": TagValuesTypeDef,
-        "CostCategories": CostCategoryValuesTypeDef,
+        "Dimensions": DimensionValuesOutputTypeDef,
+        "Tags": TagValuesOutputTypeDef,
+        "CostCategories": CostCategoryValuesOutputTypeDef,
     },
     total=False,
 )
 
 GetDimensionValuesResponseTypeDef = TypedDict(
     "GetDimensionValuesResponseTypeDef",
     {
         "DimensionValues": List[DimensionValuesWithAttributesTypeDef],
         "ReturnSize": int,
         "TotalSize": int,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "EC2ResourceDetails": EC2ResourceDetailsTypeDef,
@@ -1367,20 +1498,33 @@
     "ServiceSpecificationTypeDef",
     {
         "EC2Specification": EC2SpecificationTypeDef,
     },
     total=False,
 )
 
+ExpressionTypeDef = TypedDict(
+    "ExpressionTypeDef",
+    {
+        "Or": Sequence[Dict[str, Any]],
+        "And": Sequence[Dict[str, Any]],
+        "Not": Dict[str, Any],
+        "Dimensions": DimensionValuesTypeDef,
+        "Tags": TagValuesTypeDef,
+        "CostCategories": CostCategoryValuesTypeDef,
+    },
+    total=False,
+)
+
 ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef = TypedDict(
     "ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef",
     {
         "GenerationSummaryList": List[GenerationSummaryTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetAnomaliesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAnomaliesRequestRequestTypeDef",
     {
         "DateInterval": AnomalyDateIntervalTypeDef,
@@ -1394,19 +1538,21 @@
         "TotalImpact": TotalImpactFilterTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetAnomaliesRequestRequestTypeDef(
     _RequiredGetAnomaliesRequestRequestTypeDef, _OptionalGetAnomaliesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetCostAndUsageRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Metrics": Sequence[str],
     },
@@ -1417,19 +1563,21 @@
         "Filter": "ExpressionTypeDef",
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetCostAndUsageRequestRequestTypeDef(
     _RequiredGetCostAndUsageRequestRequestTypeDef, _OptionalGetCostAndUsageRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
     },
@@ -1440,20 +1588,22 @@
         "Metrics": Sequence[str],
         "GroupBy": Sequence[GroupDefinitionTypeDef],
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetCostAndUsageWithResourcesRequestRequestTypeDef(
     _RequiredGetCostAndUsageWithResourcesRequestRequestTypeDef,
     _OptionalGetCostAndUsageWithResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCostCategoriesRequestRequestTypeDef = TypedDict(
     "_RequiredGetCostCategoriesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetCostCategoriesRequestRequestTypeDef = TypedDict(
@@ -1465,19 +1615,21 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetCostCategoriesRequestRequestTypeDef(
     _RequiredGetCostCategoriesRequestRequestTypeDef, _OptionalGetCostCategoriesRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredGetDimensionValuesRequestRequestTypeDef = TypedDict(
     "_RequiredGetDimensionValuesRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Dimension": DimensionType,
     },
 )
@@ -1490,20 +1642,22 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetDimensionValuesRequestRequestTypeDef(
     _RequiredGetDimensionValuesRequestRequestTypeDef,
     _OptionalGetDimensionValuesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetReservationCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationCoverageRequestRequestTypeDef = TypedDict(
@@ -1516,20 +1670,22 @@
         "NextPageToken": str,
         "SortBy": SortDefinitionTypeDef,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetReservationCoverageRequestRequestTypeDef(
     _RequiredGetReservationCoverageRequestRequestTypeDef,
     _OptionalGetReservationCoverageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetReservationUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetReservationUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetReservationUtilizationRequestRequestTypeDef = TypedDict(
@@ -1541,20 +1697,22 @@
         "SortBy": SortDefinitionTypeDef,
         "NextPageToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class GetReservationUtilizationRequestRequestTypeDef(
     _RequiredGetReservationUtilizationRequestRequestTypeDef,
     _OptionalGetReservationUtilizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansCoverageRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansCoverageRequestRequestTypeDef = TypedDict(
@@ -1567,20 +1725,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class GetSavingsPlansCoverageRequestRequestTypeDef(
     _RequiredGetSavingsPlansCoverageRequestRequestTypeDef,
     _OptionalGetSavingsPlansCoverageRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef = TypedDict(
@@ -1591,20 +1751,22 @@
         "NextToken": str,
         "MaxResults": int,
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class GetSavingsPlansUtilizationDetailsRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationDetailsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetSavingsPlansUtilizationRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef = TypedDict(
@@ -1613,20 +1775,22 @@
         "Granularity": GranularityType,
         "Filter": "ExpressionTypeDef",
         "SortBy": SortDefinitionTypeDef,
     },
     total=False,
 )
 
+
 class GetSavingsPlansUtilizationRequestRequestTypeDef(
     _RequiredGetSavingsPlansUtilizationRequestRequestTypeDef,
     _OptionalGetSavingsPlansUtilizationRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetTagsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTagsRequestRequestTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
     },
 )
 _OptionalGetTagsRequestRequestTypeDef = TypedDict(
@@ -1638,19 +1802,21 @@
         "SortBy": Sequence[SortDefinitionTypeDef],
         "MaxResults": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetTagsRequestRequestTypeDef(
     _RequiredGetTagsRequestRequestTypeDef, _OptionalGetTagsRequestRequestTypeDef
 ):
     pass
 
+
 GroupTypeDef = TypedDict(
     "GroupTypeDef",
     {
         "Keys": List[str],
         "Metrics": Dict[str, MetricValueTypeDef],
     },
     total=False,
@@ -1680,20 +1846,22 @@
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetRightsizingRecommendationRequestRequestTypeDef(
     _RequiredGetRightsizingRecommendationRequestRequestTypeDef,
     _OptionalGetRightsizingRecommendationRequestRequestTypeDef,
 ):
     pass
 
+
 InstanceDetailsTypeDef = TypedDict(
     "InstanceDetailsTypeDef",
     {
         "EC2InstanceDetails": EC2InstanceDetailsTypeDef,
         "RDSInstanceDetails": RDSInstanceDetailsTypeDef,
         "RedshiftInstanceDetails": RedshiftInstanceDetailsTypeDef,
         "ElastiCacheInstanceDetails": ElastiCacheInstanceDetailsTypeDef,
@@ -1746,20 +1914,22 @@
     {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
     total=False,
 )
 
+
 class SavingsPlansUtilizationAggregatesTypeDef(
     _RequiredSavingsPlansUtilizationAggregatesTypeDef,
     _OptionalSavingsPlansUtilizationAggregatesTypeDef,
 ):
     pass
 
+
 _RequiredSavingsPlansUtilizationByTimeTypeDef = TypedDict(
     "_RequiredSavingsPlansUtilizationByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Utilization": SavingsPlansUtilizationTypeDef,
     },
 )
@@ -1768,19 +1938,21 @@
     {
         "Savings": SavingsPlansSavingsTypeDef,
         "AmortizedCommitment": SavingsPlansAmortizedCommitmentTypeDef,
     },
     total=False,
 )
 
+
 class SavingsPlansUtilizationByTimeTypeDef(
     _RequiredSavingsPlansUtilizationByTimeTypeDef, _OptionalSavingsPlansUtilizationByTimeTypeDef
 ):
     pass
 
+
 SavingsPlansUtilizationDetailTypeDef = TypedDict(
     "SavingsPlansUtilizationDetailTypeDef",
     {
         "SavingsPlanArn": str,
         "Attributes": Dict[str, str],
         "Utilization": SavingsPlansUtilizationTypeDef,
         "Savings": SavingsPlansSavingsTypeDef,
@@ -1789,62 +1961,67 @@
     total=False,
 )
 
 UpdateCostAllocationTagsStatusResponseTypeDef = TypedDict(
     "UpdateCostAllocationTagsStatusResponseTypeDef",
     {
         "Errors": List[UpdateCostAllocationTagsStatusErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAnomalySubscriptionsResponseTypeDef = TypedDict(
+    "GetAnomalySubscriptionsResponseTypeDef",
+    {
+        "AnomalySubscriptions": List[AnomalySubscriptionOutputTypeDef],
+        "NextPageToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AnomalySubscriptionUnionTypeDef = Union[
+    AnomalySubscriptionTypeDef, AnomalySubscriptionOutputTypeDef
+]
 _RequiredCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "AnomalySubscription": AnomalySubscriptionTypeDef,
     },
 )
 _OptionalCreateAnomalySubscriptionRequestRequestTypeDef = TypedDict(
     "_OptionalCreateAnomalySubscriptionRequestRequestTypeDef",
     {
         "ResourceTags": Sequence[ResourceTagTypeDef],
     },
     total=False,
 )
 
+
 class CreateAnomalySubscriptionRequestRequestTypeDef(
     _RequiredCreateAnomalySubscriptionRequestRequestTypeDef,
     _OptionalCreateAnomalySubscriptionRequestRequestTypeDef,
 ):
     pass
 
-GetAnomalySubscriptionsResponseTypeDef = TypedDict(
-    "GetAnomalySubscriptionsResponseTypeDef",
-    {
-        "AnomalySubscriptions": List[AnomalySubscriptionTypeDef],
-        "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetAnomaliesResponseTypeDef = TypedDict(
     "GetAnomaliesResponseTypeDef",
     {
         "Anomalies": List[AnomalyTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCostCategoryDefinitionsResponseTypeDef = TypedDict(
     "ListCostCategoryDefinitionsResponseTypeDef",
     {
         "CostCategoryReferences": List[CostCategoryReferenceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCostCategoryTypeDef = TypedDict(
     "_RequiredCostCategoryTypeDef",
     {
         "CostCategoryArn": str,
@@ -1854,88 +2031,44 @@
         "Rules": List[CostCategoryRuleTypeDef],
     },
 )
 _OptionalCostCategoryTypeDef = TypedDict(
     "_OptionalCostCategoryTypeDef",
     {
         "EffectiveEnd": str,
-        "SplitChargeRules": List[CostCategorySplitChargeRuleTypeDef],
+        "SplitChargeRules": List[CostCategorySplitChargeRuleOutputTypeDef],
         "ProcessingStatus": List[CostCategoryProcessingStatusTypeDef],
         "DefaultValue": str,
     },
     total=False,
 )
 
-class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
-    pass
-
-_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "Name": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
-        "ResourceTags": Sequence[ResourceTagTypeDef],
-    },
-    total=False,
-)
 
-class CreateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
-):
+class CostCategoryTypeDef(_RequiredCostCategoryTypeDef, _OptionalCostCategoryTypeDef):
     pass
 
-_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "CostCategoryArn": str,
-        "RuleVersion": Literal["CostCategoryExpression.v1"],
-        "Rules": Sequence[CostCategoryRuleTypeDef],
-    },
-)
-_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
-    {
-        "EffectiveStart": str,
-        "DefaultValue": str,
-        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleTypeDef],
-    },
-    total=False,
-)
-
-class UpdateCostCategoryDefinitionRequestRequestTypeDef(
-    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
-    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
-):
-    pass
 
+CostCategorySplitChargeRuleUnionTypeDef = Union[
+    CostCategorySplitChargeRuleTypeDef, CostCategorySplitChargeRuleOutputTypeDef
+]
 GetCostForecastResponseTypeDef = TypedDict(
     "GetCostForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUsageForecastResponseTypeDef = TypedDict(
     "GetUsageForecastResponseTypeDef",
     {
         "Total": MetricValueTypeDef,
         "ForecastResultsByTime": List[ForecastResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationCoverageGroupTypeDef = TypedDict(
     "ReservationCoverageGroupTypeDef",
     {
         "Attributes": Dict[str, str],
@@ -1970,20 +2103,22 @@
         "ServiceSpecification": ServiceSpecificationTypeDef,
         "PageSize": int,
         "NextPageToken": str,
     },
     total=False,
 )
 
+
 class GetReservationPurchaseRecommendationRequestRequestTypeDef(
     _RequiredGetReservationPurchaseRecommendationRequestRequestTypeDef,
     _OptionalGetReservationPurchaseRecommendationRequestRequestTypeDef,
 ):
     pass
 
+
 ResultByTimeTypeDef = TypedDict(
     "ResultByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Total": Dict[str, MetricValueTypeDef],
         "Groups": List[GroupTypeDef],
         "Estimated": bool,
@@ -2028,15 +2163,15 @@
 )
 
 GetSavingsPlansCoverageResponseTypeDef = TypedDict(
     "GetSavingsPlansCoverageResponseTypeDef",
     {
         "SavingsPlansCoverages": List[SavingsPlansCoverageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SavingsPlansPurchaseRecommendationTypeDef = TypedDict(
     "SavingsPlansPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2055,36 +2190,89 @@
 )
 
 GetSavingsPlansUtilizationResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationResponseTypeDef",
     {
         "SavingsPlansUtilizationsByTime": List[SavingsPlansUtilizationByTimeTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSavingsPlansUtilizationDetailsResponseTypeDef = TypedDict(
     "GetSavingsPlansUtilizationDetailsResponseTypeDef",
     {
         "SavingsPlansUtilizationDetails": List[SavingsPlansUtilizationDetailTypeDef],
         "Total": SavingsPlansUtilizationAggregatesTypeDef,
         "TimePeriod": DateIntervalTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCostCategoryDefinitionResponseTypeDef = TypedDict(
     "DescribeCostCategoryDefinitionResponseTypeDef",
     {
         "CostCategory": CostCategoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "Name": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
+    },
+)
+_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+    },
+    total=False,
+)
+
+
+class CreateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredCreateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalCreateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "CostCategoryArn": str,
+        "RuleVersion": Literal["CostCategoryExpression.v1"],
+        "Rules": Sequence[CostCategoryRuleTypeDef],
     },
 )
+_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef",
+    {
+        "EffectiveStart": str,
+        "DefaultValue": str,
+        "SplitChargeRules": Sequence[CostCategorySplitChargeRuleUnionTypeDef],
+    },
+    total=False,
+)
+
+
+class UpdateCostCategoryDefinitionRequestRequestTypeDef(
+    _RequiredUpdateCostCategoryDefinitionRequestRequestTypeDef,
+    _OptionalUpdateCostCategoryDefinitionRequestRequestTypeDef,
+):
+    pass
+
 
 CoverageByTimeTypeDef = TypedDict(
     "CoverageByTimeTypeDef",
     {
         "TimePeriod": DateIntervalTypeDef,
         "Groups": List[ReservationCoverageGroupTypeDef],
         "Total": CoverageTypeDef,
@@ -2093,15 +2281,15 @@
 )
 
 CurrentInstanceTypeDef = TypedDict(
     "CurrentInstanceTypeDef",
     {
         "ResourceId": str,
         "InstanceName": str,
-        "Tags": List[TagValuesTypeDef],
+        "Tags": List[TagValuesOutputTypeDef],
         "ResourceDetails": ResourceDetailsTypeDef,
         "ResourceUtilization": ResourceUtilizationTypeDef,
         "ReservationCoveredHoursInLookbackPeriod": str,
         "SavingsPlansCoveredHoursInLookbackPeriod": str,
         "OnDemandHoursInLookbackPeriod": str,
         "TotalRunningHoursInLookbackPeriod": str,
         "MonthlyCost": str,
@@ -2127,36 +2315,36 @@
 GetCostAndUsageResponseTypeDef = TypedDict(
     "GetCostAndUsageResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCostAndUsageWithResourcesResponseTypeDef = TypedDict(
     "GetCostAndUsageWithResourcesResponseTypeDef",
     {
         "NextPageToken": str,
         "GroupDefinitions": List[GroupDefinitionTypeDef],
         "ResultsByTime": List[ResultByTimeTypeDef],
         "DimensionValueAttributes": List[DimensionValuesWithAttributesTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationUtilizationResponseTypeDef = TypedDict(
     "GetReservationUtilizationResponseTypeDef",
     {
         "UtilizationsByTime": List[UtilizationByTimeTypeDef],
         "Total": ReservationAggregatesTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReservationPurchaseRecommendationTypeDef = TypedDict(
     "ReservationPurchaseRecommendationTypeDef",
     {
         "AccountScope": AccountScopeType,
@@ -2172,25 +2360,25 @@
 
 GetSavingsPlansPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetSavingsPlansPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": SavingsPlansPurchaseRecommendationMetadataTypeDef,
         "SavingsPlansPurchaseRecommendation": SavingsPlansPurchaseRecommendationTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReservationCoverageResponseTypeDef = TypedDict(
     "GetReservationCoverageResponseTypeDef",
     {
         "CoveragesByTime": List[CoverageByTimeTypeDef],
         "Total": CoverageTypeDef,
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyRecommendationDetailTypeDef = TypedDict(
     "ModifyRecommendationDetailTypeDef",
     {
         "TargetInstances": List[TargetInstanceTypeDef],
@@ -2200,15 +2388,15 @@
 
 GetReservationPurchaseRecommendationResponseTypeDef = TypedDict(
     "GetReservationPurchaseRecommendationResponseTypeDef",
     {
         "Metadata": ReservationPurchaseRecommendationMetadataTypeDef,
         "Recommendations": List[ReservationPurchaseRecommendationTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RightsizingRecommendationTypeDef = TypedDict(
     "RightsizingRecommendationTypeDef",
     {
         "AccountId": str,
@@ -2225,10 +2413,10 @@
     "GetRightsizingRecommendationResponseTypeDef",
     {
         "Metadata": RightsizingRecommendationMetadataTypeDef,
         "Summary": RightsizingRecommendationSummaryTypeDef,
         "RightsizingRecommendations": List[RightsizingRecommendationTypeDef],
         "NextPageToken": str,
         "Configuration": RightsizingRecommendationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/PKG-INFO` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-ce
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CostExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore ce type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore ce type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-ce"></a>
 
 # types-aiobotocore-ce
 
 [![PyPI - types-aiobotocore-ce](https://img.shields.io/pypi/v/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-ce.svg?color=blue)](https://pypi.org/project/types-aiobotocore-ce)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-ce?color=blue)](https://pypistats.org/packages/types-aiobotocore-ce)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-ce)](https://pepy.tech/project/types-aiobotocore-ce)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CostExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ce.html#CostExplorer)
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
 [types-aiobotocore-ce docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_ce/).
 
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
@@ -312,120 +311,128 @@
 )
 
 
 def check_value(value: AccountScopeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_ce.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_ce.type_defs import (
     AnomalyDateIntervalTypeDef,
     AnomalyMonitorTypeDef,
     AnomalyScoreTypeDef,
     SubscriberTypeDef,
     ImpactTypeDef,
     RootCauseTypeDef,
     CostAllocationTagStatusEntryTypeDef,
     CostAllocationTagTypeDef,
     CostCategoryInheritedValueDimensionTypeDef,
     CostCategoryProcessingStatusTypeDef,
+    CostCategorySplitChargeRuleParameterOutputTypeDef,
     CostCategorySplitChargeRuleParameterTypeDef,
+    CostCategoryValuesOutputTypeDef,
     CostCategoryValuesTypeDef,
     DateIntervalTypeDef,
     CoverageCostTypeDef,
     CoverageHoursTypeDef,
     CoverageNormalizedUnitsTypeDef,
     ResourceTagTypeDef,
-    CreateAnomalyMonitorResponseTypeDef,
-    CreateAnomalySubscriptionResponseTypeDef,
-    CreateCostCategoryDefinitionResponseTypeDef,
-    TagValuesTypeDef,
+    ResponseMetadataTypeDef,
+    TagValuesOutputTypeDef,
     DeleteAnomalyMonitorRequestRequestTypeDef,
     DeleteAnomalySubscriptionRequestRequestTypeDef,
     DeleteCostCategoryDefinitionRequestRequestTypeDef,
-    DeleteCostCategoryDefinitionResponseTypeDef,
     DescribeCostCategoryDefinitionRequestRequestTypeDef,
+    DimensionValuesOutputTypeDef,
     DimensionValuesTypeDef,
     DimensionValuesWithAttributesTypeDef,
     DiskResourceUtilizationTypeDef,
     EBSResourceUtilizationTypeDef,
     EC2InstanceDetailsTypeDef,
     EC2ResourceDetailsTypeDef,
     NetworkResourceUtilizationTypeDef,
     EC2SpecificationTypeDef,
     ESInstanceDetailsTypeDef,
     ElastiCacheInstanceDetailsTypeDef,
+    TagValuesTypeDef,
+    ExpressionUnionTypeDef,
     GenerationSummaryTypeDef,
     TotalImpactFilterTypeDef,
     GetAnomalyMonitorsRequestRequestTypeDef,
     GetAnomalySubscriptionsRequestRequestTypeDef,
     GroupDefinitionTypeDef,
     SortDefinitionTypeDef,
-    GetCostCategoriesResponseTypeDef,
     MetricValueTypeDef,
     ReservationPurchaseRecommendationMetadataTypeDef,
     ReservationAggregatesTypeDef,
     RightsizingRecommendationConfigurationTypeDef,
     RightsizingRecommendationMetadataTypeDef,
     RightsizingRecommendationSummaryTypeDef,
     GetSavingsPlansPurchaseRecommendationRequestRequestTypeDef,
     SavingsPlansPurchaseRecommendationMetadataTypeDef,
-    GetTagsResponseTypeDef,
     RDSInstanceDetailsTypeDef,
     RedshiftInstanceDetailsTypeDef,
     ListCostAllocationTagsRequestRequestTypeDef,
     ListCostCategoryDefinitionsRequestRequestTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ProvideAnomalyFeedbackRequestRequestTypeDef,
-    ProvideAnomalyFeedbackResponseTypeDef,
     ReservationPurchaseRecommendationSummaryTypeDef,
-    ResponseMetadataTypeDef,
     TerminateRecommendationDetailTypeDef,
     SavingsPlansAmortizedCommitmentTypeDef,
     SavingsPlansCoverageDataTypeDef,
     SavingsPlansDetailsTypeDef,
     SavingsPlansPurchaseRecommendationSummaryTypeDef,
     SavingsPlansSavingsTypeDef,
     SavingsPlansUtilizationTypeDef,
-    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAnomalyMonitorRequestRequestTypeDef,
-    UpdateAnomalyMonitorResponseTypeDef,
-    UpdateAnomalySubscriptionResponseTypeDef,
     UpdateCostAllocationTagsStatusErrorTypeDef,
-    UpdateCostCategoryDefinitionResponseTypeDef,
-    GetAnomalyMonitorsResponseTypeDef,
+    AnomalySubscriptionOutputTypeDef,
     AnomalySubscriptionTypeDef,
     UpdateAnomalySubscriptionRequestRequestTypeDef,
     AnomalyTypeDef,
     UpdateCostAllocationTagsStatusRequestRequestTypeDef,
-    ListCostAllocationTagsResponseTypeDef,
     CostCategoryRuleTypeDef,
     CostCategoryReferenceTypeDef,
+    CostCategorySplitChargeRuleOutputTypeDef,
     CostCategorySplitChargeRuleTypeDef,
     ForecastResultTypeDef,
     GetCostForecastRequestRequestTypeDef,
     GetUsageForecastRequestRequestTypeDef,
     CoverageTypeDef,
     CreateAnomalyMonitorRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
-    ExpressionTypeDef,
+    CreateAnomalyMonitorResponseTypeDef,
+    CreateAnomalySubscriptionResponseTypeDef,
+    CreateCostCategoryDefinitionResponseTypeDef,
+    DeleteCostCategoryDefinitionResponseTypeDef,
+    GetAnomalyMonitorsResponseTypeDef,
+    GetCostCategoriesResponseTypeDef,
+    GetTagsResponseTypeDef,
+    ListCostAllocationTagsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ProvideAnomalyFeedbackResponseTypeDef,
+    StartSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
+    UpdateAnomalyMonitorResponseTypeDef,
+    UpdateAnomalySubscriptionResponseTypeDef,
+    UpdateCostCategoryDefinitionResponseTypeDef,
+    ExpressionOutputTypeDef,
     GetDimensionValuesResponseTypeDef,
     ResourceDetailsTypeDef,
     EC2ResourceUtilizationTypeDef,
     ServiceSpecificationTypeDef,
+    ExpressionTypeDef,
     ListSavingsPlansPurchaseRecommendationGenerationResponseTypeDef,
     GetAnomaliesRequestRequestTypeDef,
     GetCostAndUsageRequestRequestTypeDef,
     GetCostAndUsageWithResourcesRequestRequestTypeDef,
     GetCostCategoriesRequestRequestTypeDef,
     GetDimensionValuesRequestRequestTypeDef,
     GetReservationCoverageRequestRequestTypeDef,
@@ -440,34 +447,36 @@
     InstanceDetailsTypeDef,
     SavingsPlansCoverageTypeDef,
     SavingsPlansPurchaseRecommendationDetailTypeDef,
     SavingsPlansUtilizationAggregatesTypeDef,
     SavingsPlansUtilizationByTimeTypeDef,
     SavingsPlansUtilizationDetailTypeDef,
     UpdateCostAllocationTagsStatusResponseTypeDef,
-    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomalySubscriptionsResponseTypeDef,
+    AnomalySubscriptionUnionTypeDef,
+    CreateAnomalySubscriptionRequestRequestTypeDef,
     GetAnomaliesResponseTypeDef,
     ListCostCategoryDefinitionsResponseTypeDef,
     CostCategoryTypeDef,
-    CreateCostCategoryDefinitionRequestRequestTypeDef,
-    UpdateCostCategoryDefinitionRequestRequestTypeDef,
+    CostCategorySplitChargeRuleUnionTypeDef,
     GetCostForecastResponseTypeDef,
     GetUsageForecastResponseTypeDef,
     ReservationCoverageGroupTypeDef,
     ResourceUtilizationTypeDef,
     GetReservationPurchaseRecommendationRequestRequestTypeDef,
     ResultByTimeTypeDef,
     UtilizationByTimeTypeDef,
     ReservationPurchaseRecommendationDetailTypeDef,
     GetSavingsPlansCoverageResponseTypeDef,
     SavingsPlansPurchaseRecommendationTypeDef,
     GetSavingsPlansUtilizationResponseTypeDef,
     GetSavingsPlansUtilizationDetailsResponseTypeDef,
     DescribeCostCategoryDefinitionResponseTypeDef,
+    CreateCostCategoryDefinitionRequestRequestTypeDef,
+    UpdateCostCategoryDefinitionRequestRequestTypeDef,
     CoverageByTimeTypeDef,
     CurrentInstanceTypeDef,
     TargetInstanceTypeDef,
     GetCostAndUsageResponseTypeDef,
     GetCostAndUsageWithResourcesResponseTypeDef,
     GetReservationUtilizationResponseTypeDef,
     ReservationPurchaseRecommendationTypeDef,
@@ -476,15 +485,15 @@
     ModifyRecommendationDetailTypeDef,
     GetReservationPurchaseRecommendationResponseTypeDef,
     RightsizingRecommendationTypeDef,
     GetRightsizingRecommendationResponseTypeDef,
 )
 
 
-def get_structure() -> AnomalyDateIntervalTypeDef:
+def get_value() -> AnomalyDateIntervalTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-ce-2.5.2/types_aiobotocore_ce.egg-info/SOURCES.txt` & `types-aiobotocore-ce-2.5.2.post1/types_aiobotocore_ce.egg-info/SOURCES.txt`

 * *Files identical despite different names*


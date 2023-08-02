# Comparing `tmp/types-aiobotocore-config-2.5.2.tar.gz` & `tmp/types-aiobotocore-config-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-config-2.5.2.tar", last modified: Sat Jul  8 01:43:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-config-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
```

## Comparing `types-aiobotocore-config-2.5.2.tar` & `types-aiobotocore-config-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:27.377937 types-aiobotocore-config-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    37260 2023-07-08 01:43:27.377937 types-aiobotocore-config-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    35692 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:27.377937 types-aiobotocore-config-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:27.377937 types-aiobotocore-config-2.5.2/types_aiobotocore_config/
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    92719 2023-07-08 01:28:01.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    92587 2023-07-08 01:28:01.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-07-08 01:28:02.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-07-08 01:28:02.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    44508 2023-07-08 01:28:01.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    44475 2023-07-08 01:28:01.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   128192 2023-07-08 01:28:05.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   128041 2023-07-08 01:28:03.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:00.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:27.377937 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    37260 2023-07-08 01:43:27.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:43:27.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:27.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:27.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:27.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:27.000000 types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.061613 types-aiobotocore-config-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    38077 2023-08-02 14:52:07.053614 types-aiobotocore-config-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    36556 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.061613 types-aiobotocore-config-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:35:35.000000 types-aiobotocore-config-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.053614 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/
+-rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9917 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92772 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92640 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    30075 2023-08-02 14:35:37.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30073 2023-08-02 14:35:37.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    44399 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44366 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   136691 2023-08-02 14:35:40.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136524 2023-08-02 14:35:39.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:36.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.053614 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    38077 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:06.000000 types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-config-2.5.2/LICENSE` & `types-aiobotocore-config-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2/PKG-INFO` & `types-aiobotocore-config-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-config
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConfigService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConfigService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-config"></a>
 
 # types-aiobotocore-config
 
 [![PyPI - types-aiobotocore-config](https://img.shields.io/pypi/v/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-config)](https://pepy.tech/project/types-aiobotocore-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConfigService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [types-aiobotocore-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/).
 
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
@@ -493,43 +492,46 @@
 )
 
 
 def check_value(value: AggregateConformancePackComplianceSummaryGroupKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_config.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_config.type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
+    ResponseMetadataTypeDef,
     ResourceKeyTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
     EvaluationModeConfigurationTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
     ConformancePackInputParameterTypeDef,
@@ -550,148 +552,125 @@
     DeletePendingAggregationRequestRequestRequestTypeDef,
     DeleteRemediationConfigurationRequestRequestTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     DeleteResourceConfigRequestRequestTypeDef,
     DeleteRetentionConfigurationRequestRequestTypeDef,
     DeleteStoredQueryRequestRequestTypeDef,
     DeliverConfigSnapshotRequestRequestTypeDef,
-    DeliverConfigSnapshotResponseTypeDef,
-    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAggregationAuthorizationsRequestRequestTypeDef,
-    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByConfigRuleRequestRequestTypeDef,
-    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeComplianceByResourceRequestRequestTypeDef,
-    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestRequestTypeDef,
     DescribeConfigRulesFiltersTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
-    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
     DescribeConfigurationAggregatorsRequestRequestTypeDef,
     DescribeConfigurationRecorderStatusRequestRequestTypeDef,
     DescribeConfigurationRecordersRequestRequestTypeDef,
-    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
     DescribeConformancePackStatusRequestRequestTypeDef,
-    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
     DescribeConformancePacksRequestRequestTypeDef,
     DescribeDeliveryChannelStatusRequestRequestTypeDef,
     DescribeDeliveryChannelsRequestRequestTypeDef,
-    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
     DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef,
     OrganizationConfigRuleStatusTypeDef,
-    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
     DescribeOrganizationConfigRulesRequestRequestTypeDef,
-    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
     DescribeOrganizationConformancePackStatusesRequestRequestTypeDef,
     OrganizationConformancePackStatusTypeDef,
-    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
     DescribeOrganizationConformancePacksRequestRequestTypeDef,
-    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribePendingAggregationRequestsRequestRequestTypeDef,
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
-    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
-    EvaluationTypeDef,
+    TimestampTypeDef,
+    ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
     SsmControlsTypeDef,
-    ExternalEvaluationTypeDef,
     FieldInfoTypeDef,
-    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
-    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
-    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
-    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     GetConformancePackComplianceSummaryRequestRequestTypeDef,
     GetCustomRulePolicyRequestRequestTypeDef,
-    GetCustomRulePolicyResponseTypeDef,
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetOrganizationCustomRulePolicyResponseTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
     StoredQueryTypeDef,
     ResourceFiltersTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
+    OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    OrganizationCustomPolicyRuleMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    PutConformancePackResponseTypeDef,
-    PutOrganizationConfigRuleResponseTypeDef,
-    PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
-    PutStoredQueryResponseTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
     ResourceValueTypeDef,
+    StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    TimeWindowTypeDef,
-    ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
-    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
-    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
-    StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
-    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    BatchGetAggregateResourceConfigResponseTypeDef,
+    DeliverConfigSnapshotResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCustomRulePolicyResponseTypeDef,
+    GetOrganizationCustomRulePolicyResponseTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
-    BatchGetAggregateResourceConfigResponseTypeDef,
+    PutConformancePackResponseTypeDef,
+    PutOrganizationConfigRuleResponseTypeDef,
+    PutOrganizationConformancePackResponseTypeDef,
+    PutStoredQueryResponseTypeDef,
+    StartResourceEvaluationResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
     BatchGetResourceConfigResponseTypeDef,
-    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
-    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
@@ -706,29 +685,57 @@
     PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
     FailedDeleteRemediationExceptionsBatchTypeDef,
-    PutRemediationExceptionsRequestRequestTypeDef,
+    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
+    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
+    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
+    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
+    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
+    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
+    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
+    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
+    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
+    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
+    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
+    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
+    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
-    EvaluationResultIdentifierTypeDef,
-    PutEvaluationsRequestRequestTypeDef,
     PutEvaluationsResponseTypeDef,
+    EvaluationResultIdentifierTypeDef,
+    EvaluationTypeDef,
+    ExternalEvaluationTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    GetResourceConfigHistoryRequestRequestTypeDef,
+    PutRemediationExceptionsRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ExecutionControlsTypeDef,
-    PutExternalEvaluationRequestRequestTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
@@ -741,24 +748,29 @@
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationConfigRuleTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     PutOrganizationConfigRuleRequestRequestTypeDef,
+    RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
+    RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    ResourceEvaluationFiltersTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
     ComplianceByConfigRuleTypeDef,
@@ -773,44 +785,54 @@
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    EvaluationUnionTypeDef,
+    PutExternalEvaluationRequestRequestTypeDef,
+    ResourceEvaluationFiltersTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
-    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
-    ListResourceEvaluationsRequestRequestTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetConformancePackComplianceDetailsResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
     GetComplianceDetailsByResourceResponseTypeDef,
+    PutEvaluationsRequestRequestTypeDef,
+    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
+    ListResourceEvaluationsRequestRequestTypeDef,
     DescribeConfigurationRecordersResponseTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     PutConfigurationRecorderRequestRequestTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     FailedRemediationBatchTypeDef,
-    PutRemediationConfigurationsRequestRequestTypeDef,
+    RemediationConfigurationUnionTypeDef,
     DescribeConfigRulesResponseTypeDef,
+    ConfigRuleUnionTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
+    PutRemediationConfigurationsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceTypeDef:
+def get_value() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-config-2.5.2/README.md` & `types-aiobotocore-config-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-config"></a>
 
 # types-aiobotocore-config
 
 [![PyPI - types-aiobotocore-config](https://img.shields.io/pypi/v/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-config)](https://pepy.tech/project/types-aiobotocore-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConfigService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [types-aiobotocore-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/).
 
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
@@ -460,43 +460,46 @@
 )
 
 
 def check_value(value: AggregateConformancePackComplianceSummaryGroupKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_config.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_config.type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
+    ResponseMetadataTypeDef,
     ResourceKeyTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
     EvaluationModeConfigurationTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
     ConformancePackInputParameterTypeDef,
@@ -517,148 +520,125 @@
     DeletePendingAggregationRequestRequestRequestTypeDef,
     DeleteRemediationConfigurationRequestRequestTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     DeleteResourceConfigRequestRequestTypeDef,
     DeleteRetentionConfigurationRequestRequestTypeDef,
     DeleteStoredQueryRequestRequestTypeDef,
     DeliverConfigSnapshotRequestRequestTypeDef,
-    DeliverConfigSnapshotResponseTypeDef,
-    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAggregationAuthorizationsRequestRequestTypeDef,
-    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByConfigRuleRequestRequestTypeDef,
-    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeComplianceByResourceRequestRequestTypeDef,
-    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestRequestTypeDef,
     DescribeConfigRulesFiltersTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
-    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
     DescribeConfigurationAggregatorsRequestRequestTypeDef,
     DescribeConfigurationRecorderStatusRequestRequestTypeDef,
     DescribeConfigurationRecordersRequestRequestTypeDef,
-    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
     DescribeConformancePackStatusRequestRequestTypeDef,
-    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
     DescribeConformancePacksRequestRequestTypeDef,
     DescribeDeliveryChannelStatusRequestRequestTypeDef,
     DescribeDeliveryChannelsRequestRequestTypeDef,
-    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
     DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef,
     OrganizationConfigRuleStatusTypeDef,
-    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
     DescribeOrganizationConfigRulesRequestRequestTypeDef,
-    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
     DescribeOrganizationConformancePackStatusesRequestRequestTypeDef,
     OrganizationConformancePackStatusTypeDef,
-    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
     DescribeOrganizationConformancePacksRequestRequestTypeDef,
-    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribePendingAggregationRequestsRequestRequestTypeDef,
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
-    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
-    EvaluationTypeDef,
+    TimestampTypeDef,
+    ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
     SsmControlsTypeDef,
-    ExternalEvaluationTypeDef,
     FieldInfoTypeDef,
-    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
-    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
-    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
-    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     GetConformancePackComplianceSummaryRequestRequestTypeDef,
     GetCustomRulePolicyRequestRequestTypeDef,
-    GetCustomRulePolicyResponseTypeDef,
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetOrganizationCustomRulePolicyResponseTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
     StoredQueryTypeDef,
     ResourceFiltersTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
+    OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    OrganizationCustomPolicyRuleMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    PutConformancePackResponseTypeDef,
-    PutOrganizationConfigRuleResponseTypeDef,
-    PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
-    PutStoredQueryResponseTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
     ResourceValueTypeDef,
+    StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    TimeWindowTypeDef,
-    ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
-    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
-    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
-    StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
-    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    BatchGetAggregateResourceConfigResponseTypeDef,
+    DeliverConfigSnapshotResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCustomRulePolicyResponseTypeDef,
+    GetOrganizationCustomRulePolicyResponseTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
-    BatchGetAggregateResourceConfigResponseTypeDef,
+    PutConformancePackResponseTypeDef,
+    PutOrganizationConfigRuleResponseTypeDef,
+    PutOrganizationConformancePackResponseTypeDef,
+    PutStoredQueryResponseTypeDef,
+    StartResourceEvaluationResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
     BatchGetResourceConfigResponseTypeDef,
-    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
-    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
@@ -673,29 +653,57 @@
     PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
     FailedDeleteRemediationExceptionsBatchTypeDef,
-    PutRemediationExceptionsRequestRequestTypeDef,
+    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
+    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
+    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
+    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
+    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
+    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
+    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
+    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
+    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
+    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
+    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
+    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
+    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
-    EvaluationResultIdentifierTypeDef,
-    PutEvaluationsRequestRequestTypeDef,
     PutEvaluationsResponseTypeDef,
+    EvaluationResultIdentifierTypeDef,
+    EvaluationTypeDef,
+    ExternalEvaluationTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    GetResourceConfigHistoryRequestRequestTypeDef,
+    PutRemediationExceptionsRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ExecutionControlsTypeDef,
-    PutExternalEvaluationRequestRequestTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
@@ -708,24 +716,29 @@
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationConfigRuleTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     PutOrganizationConfigRuleRequestRequestTypeDef,
+    RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
+    RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    ResourceEvaluationFiltersTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
     ComplianceByConfigRuleTypeDef,
@@ -740,44 +753,54 @@
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    EvaluationUnionTypeDef,
+    PutExternalEvaluationRequestRequestTypeDef,
+    ResourceEvaluationFiltersTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
-    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
-    ListResourceEvaluationsRequestRequestTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetConformancePackComplianceDetailsResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
     GetComplianceDetailsByResourceResponseTypeDef,
+    PutEvaluationsRequestRequestTypeDef,
+    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
+    ListResourceEvaluationsRequestRequestTypeDef,
     DescribeConfigurationRecordersResponseTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     PutConfigurationRecorderRequestRequestTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     FailedRemediationBatchTypeDef,
-    PutRemediationConfigurationsRequestRequestTypeDef,
+    RemediationConfigurationUnionTypeDef,
     DescribeConfigRulesResponseTypeDef,
+    ConfigRuleUnionTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
+    PutRemediationConfigurationsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceTypeDef:
+def get_value() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-config-2.5.2/setup.py` & `types-aiobotocore-config-2.5.2.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-config",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_config"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConfigService 2.5.2 service generated with"
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
-    keywords="aiobotocore config type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore config type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_config": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/"
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/__init__.py` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/__init__.pyi` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/__main__.py` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConfigService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ConfigService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService\nOther"
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

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/client.py` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("config") as client:
         client: ConfigServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AggregateConformancePackComplianceSummaryGroupKeyType,
     AggregatedSourceStatusTypeType,
@@ -62,24 +61,24 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
-    AccountAggregationSourceTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
-    ConfigRuleTypeDef,
-    ConfigurationRecorderTypeDef,
+    ConfigRuleUnionTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
     DeliveryChannelTypeDef,
@@ -107,15 +106,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
-    EvaluationTypeDef,
+    EvaluationUnionTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
@@ -134,44 +133,45 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
-    OrganizationCustomRuleMetadataTypeDef,
-    OrganizationManagedRuleMetadataTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
-    RemediationConfigurationTypeDef,
+    RemediationConfigurationUnionTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StatusDetailFiltersTypeDef,
     StoredQueryTypeDef,
     TagTypeDef,
     TemplateSSMDocumentDetailsTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -1030,16 +1030,16 @@
         """
 
     async def get_resource_config_history(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         limit: int = ...,
         nextToken: str = ...
     ) -> GetResourceConfigHistoryResponseTypeDef:
         """
         Returns a list of `ConfigurationItems` for the specified resource.
 
@@ -1164,42 +1164,42 @@
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_aggregation_authorization)
         """
 
     async def put_config_rule(
-        self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, ConfigRule: ConfigRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_config_rule)
         """
 
     async def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
-        OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
+        AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,
+        OrganizationAggregationSource: OrganizationAggregationSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_aggregator)
         """
 
     async def put_configuration_recorder(
-        self, *, ConfigurationRecorder: ConfigurationRecorderTypeDef
+        self, *, ConfigurationRecorder: ConfigurationRecorderUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_recorder)
@@ -1234,15 +1234,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_delivery_channel)
         """
 
     async def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[EvaluationTypeDef] = ...,
+        Evaluations: Sequence[EvaluationUnionTypeDef] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_evaluations)
@@ -1258,16 +1258,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_external_evaluation)
         """
 
     async def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
-        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
+        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataUnionTypeDef = ...,
+        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataUnionTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1291,15 +1291,15 @@
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_organization_conformance_pack)
         """
 
     async def put_remediation_configurations(
-        self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
+        self, *, RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_remediation_configurations)
@@ -1307,15 +1307,15 @@
 
     async def put_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
-        ExpirationTime: Union[datetime, str] = ...
+        ExpirationTime: TimestampTypeDef = ...
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
         A remediation exception is when a specified resource is no longer considered for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_remediation_exceptions)
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/client.pyi` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("config") as client:
         client: ConfigServiceClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     AggregateConformancePackComplianceSummaryGroupKeyType,
     AggregatedSourceStatusTypeType,
@@ -62,24 +61,24 @@
     ListDiscoveredResourcesPaginator,
     ListResourceEvaluationsPaginator,
     ListTagsForResourcePaginator,
     SelectAggregateResourceConfigPaginator,
     SelectResourceConfigPaginator,
 )
 from .type_defs import (
-    AccountAggregationSourceTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     BatchGetAggregateResourceConfigResponseTypeDef,
     BatchGetResourceConfigResponseTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
-    ConfigRuleTypeDef,
-    ConfigurationRecorderTypeDef,
+    ConfigRuleUnionTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackEvaluationFiltersTypeDef,
     ConformancePackInputParameterTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     DeliverConfigSnapshotResponseTypeDef,
     DeliveryChannelTypeDef,
@@ -107,15 +106,15 @@
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
-    EvaluationTypeDef,
+    EvaluationUnionTypeDef,
     ExternalEvaluationTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetAggregateResourceConfigResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
@@ -134,44 +133,45 @@
     GetStoredQueryResponseTypeDef,
     ListAggregateDiscoveredResourcesResponseTypeDef,
     ListConformancePackComplianceScoresResponseTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationCustomPolicyRuleMetadataTypeDef,
-    OrganizationCustomRuleMetadataTypeDef,
-    OrganizationManagedRuleMetadataTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
     PutConfigurationAggregatorResponseTypeDef,
     PutConformancePackResponseTypeDef,
     PutEvaluationsResponseTypeDef,
     PutOrganizationConfigRuleResponseTypeDef,
     PutOrganizationConformancePackResponseTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
     PutStoredQueryResponseTypeDef,
-    RemediationConfigurationTypeDef,
+    RemediationConfigurationUnionTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     ResourceCountFiltersTypeDef,
     ResourceDetailsTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StartRemediationExecutionResponseTypeDef,
     StartResourceEvaluationResponseTypeDef,
     StatusDetailFiltersTypeDef,
     StoredQueryTypeDef,
     TagTypeDef,
     TemplateSSMDocumentDetailsTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -963,16 +963,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#get_organization_custom_rule_policy)
         """
     async def get_resource_config_history(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
         limit: int = ...,
         nextToken: str = ...
     ) -> GetResourceConfigHistoryResponseTypeDef:
         """
         Returns a list of `ConfigurationItems` for the specified resource.
 
@@ -1087,40 +1087,40 @@
         Authorizes the aggregator account and region to collect data from the source
         account and region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_aggregation_authorization)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_aggregation_authorization)
         """
     async def put_config_rule(
-        self, *, ConfigRule: ConfigRuleTypeDef, Tags: Sequence[TagTypeDef] = ...
+        self, *, ConfigRule: ConfigRuleUnionTypeDef, Tags: Sequence[TagTypeDef] = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Adds or updates an Config rule to evaluate if your Amazon Web Services resources
         comply with your desired configurations.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_config_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_config_rule)
         """
     async def put_configuration_aggregator(
         self,
         *,
         ConfigurationAggregatorName: str,
-        AccountAggregationSources: Sequence[AccountAggregationSourceTypeDef] = ...,
-        OrganizationAggregationSource: OrganizationAggregationSourceTypeDef = ...,
+        AccountAggregationSources: Sequence[AccountAggregationSourceUnionTypeDef] = ...,
+        OrganizationAggregationSource: OrganizationAggregationSourceUnionTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...
     ) -> PutConfigurationAggregatorResponseTypeDef:
         """
         Creates and updates the configuration aggregator with the selected source
         accounts and regions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_aggregator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_aggregator)
         """
     async def put_configuration_recorder(
-        self, *, ConfigurationRecorder: ConfigurationRecorderTypeDef
+        self, *, ConfigurationRecorder: ConfigurationRecorderUnionTypeDef
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates a new configuration recorder to record configuration changes for
         specified resource types.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_configuration_recorder)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_configuration_recorder)
@@ -1152,15 +1152,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_delivery_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_delivery_channel)
         """
     async def put_evaluations(
         self,
         *,
         ResultToken: str,
-        Evaluations: Sequence[EvaluationTypeDef] = ...,
+        Evaluations: Sequence[EvaluationUnionTypeDef] = ...,
         TestMode: bool = ...
     ) -> PutEvaluationsResponseTypeDef:
         """
         Used by an Lambda function to deliver evaluation results to Config.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_evaluations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_evaluations)
@@ -1174,16 +1174,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_external_evaluation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_external_evaluation)
         """
     async def put_organization_config_rule(
         self,
         *,
         OrganizationConfigRuleName: str,
-        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataTypeDef = ...,
-        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataTypeDef = ...,
+        OrganizationManagedRuleMetadata: OrganizationManagedRuleMetadataUnionTypeDef = ...,
+        OrganizationCustomRuleMetadata: OrganizationCustomRuleMetadataUnionTypeDef = ...,
         ExcludedAccounts: Sequence[str] = ...,
         OrganizationCustomPolicyRuleMetadata: OrganizationCustomPolicyRuleMetadataTypeDef = ...
     ) -> PutOrganizationConfigRuleResponseTypeDef:
         """
         Adds or updates an Config rule for your entire organization to evaluate if your
         Amazon Web Services resources comply with your desired configurations.
 
@@ -1205,30 +1205,30 @@
         Deploys conformance packs across member accounts in an Amazon Web Services
         Organization.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_organization_conformance_pack)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_organization_conformance_pack)
         """
     async def put_remediation_configurations(
-        self, *, RemediationConfigurations: Sequence[RemediationConfigurationTypeDef]
+        self, *, RemediationConfigurations: Sequence[RemediationConfigurationUnionTypeDef]
     ) -> PutRemediationConfigurationsResponseTypeDef:
         """
         Adds or updates the remediation configuration with a specific Config rule with
         the selected target or action.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_configurations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_remediation_configurations)
         """
     async def put_remediation_exceptions(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[RemediationExceptionResourceKeyTypeDef],
         Message: str = ...,
-        ExpirationTime: Union[datetime, str] = ...
+        ExpirationTime: TimestampTypeDef = ...
     ) -> PutRemediationExceptionsResponseTypeDef:
         """
         A remediation exception is when a specified resource is no longer considered for
         auto-remediation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Client.put_remediation_exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/client/#put_remediation_exceptions)
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/literals.py` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/literals.pyi` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/paginator.py` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,16 +76,15 @@
         list_discovered_resources_paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")
         list_resource_evaluations_paginator: ListResourceEvaluationsPaginator = client.get_paginator("list_resource_evaluations")
         list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
         select_aggregate_resource_config_paginator: SelectAggregateResourceConfigPaginator = client.get_paginator("select_aggregate_resource_config")
         select_resource_config_paginator: SelectResourceConfigPaginator = client.get_paginator("select_resource_config")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     AggregatedSourceStatusTypeType,
     ChronologicalOrderType,
@@ -129,14 +128,15 @@
     PaginatorConfigTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StatusDetailFiltersTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAggregateComplianceByConfigRulesPaginator",
     "DescribeAggregateComplianceByConformancePacksPaginator",
     "DescribeAggregationAuthorizationsPaginator",
     "DescribeComplianceByConfigRulePaginator",
@@ -187,15 +187,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconfigrulespaginator)
         """
 
 
@@ -206,30 +206,30 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconformancepackspaginator)
         """
 
 
 class DescribeAggregationAuthorizationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregationauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAggregationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregationauthorizationspaginator)
         """
 
 
@@ -240,15 +240,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeComplianceByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyconfigrulepaginator)
         """
 
 
@@ -260,15 +260,15 @@
 
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeComplianceByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyresourcepaginator)
         """
 
 
@@ -278,15 +278,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
         """
 
 
@@ -297,15 +297,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         Filters: DescribeConfigRulesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigrulespaginator)
         """
 
 
@@ -316,15 +316,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorsourcesstatuspaginator)
         """
 
 
@@ -334,15 +334,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigurationAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
         """
 
 
@@ -352,15 +352,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConformancePackStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
         """
 
 
@@ -370,15 +370,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
         """
 
 
@@ -388,15 +388,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
         """
 
 
@@ -406,15 +406,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
         """
 
 
@@ -424,15 +424,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
         """
 
 
@@ -442,30 +442,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
         """
 
 
 class DescribePendingAggregationRequestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describependingaggregationrequestspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePendingAggregationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describependingaggregationrequestspaginator)
         """
 
 
@@ -476,15 +476,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRemediationExecutionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeremediationexecutionstatuspaginator)
         """
 
 
@@ -494,15 +494,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         RetentionConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRetentionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
         """
 
 
@@ -516,15 +516,15 @@
         self,
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getaggregatecompliancedetailsbyconfigrulepaginator)
         """
 
 
@@ -535,15 +535,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyconfigrulepaginator)
         """
 
 
@@ -556,33 +556,30 @@
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         ResourceEvaluationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetComplianceDetailsByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyresourcepaginator)
         """
 
 
 class GetConformancePackComplianceSummaryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getconformancepackcompliancesummarypaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ConformancePackNames: Sequence[str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ConformancePackNames: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConformancePackComplianceSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getconformancepackcompliancesummarypaginator)
         """
 
 
@@ -593,15 +590,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconfigruledetailedstatuspaginator)
         """
 
 
@@ -612,15 +609,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconformancepackdetailedstatuspaginator)
         """
 
 
@@ -631,18 +628,18 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getresourceconfighistorypaginator)
         """
 
 
@@ -654,15 +651,15 @@
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listaggregatediscoveredresourcespaginator)
         """
 
 
@@ -675,15 +672,15 @@
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         includeDeletedResources: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listdiscoveredresourcespaginator)
         """
 
 
@@ -693,30 +690,30 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListResourceEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -728,28 +725,28 @@
 
     def paginate(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SelectAggregateResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectaggregateresourceconfigpaginator)
         """
 
 
 class SelectResourceConfigPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectresourceconfigpaginator)
     """
 
     def paginate(
-        self, *, Expression: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Expression: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SelectResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectresourceconfigpaginator)
         """
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/paginator.pyi` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -76,16 +76,15 @@
         list_discovered_resources_paginator: ListDiscoveredResourcesPaginator = client.get_paginator("list_discovered_resources")
         list_resource_evaluations_paginator: ListResourceEvaluationsPaginator = client.get_paginator("list_resource_evaluations")
         list_tags_for_resource_paginator: ListTagsForResourcePaginator = client.get_paginator("list_tags_for_resource")
         select_aggregate_resource_config_paginator: SelectAggregateResourceConfigPaginator = client.get_paginator("select_aggregate_resource_config")
         select_resource_config_paginator: SelectResourceConfigPaginator = client.get_paginator("select_resource_config")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Sequence, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import (
     AggregatedSourceStatusTypeType,
     ChronologicalOrderType,
@@ -129,14 +128,15 @@
     PaginatorConfigTypeDef,
     ResourceEvaluationFiltersTypeDef,
     ResourceFiltersTypeDef,
     ResourceKeyTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     StatusDetailFiltersTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = (
     "DescribeAggregateComplianceByConfigRulesPaginator",
     "DescribeAggregateComplianceByConformancePacksPaginator",
     "DescribeAggregationAuthorizationsPaginator",
     "DescribeComplianceByConfigRulePaginator",
@@ -184,15 +184,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: ConfigRuleComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAggregateComplianceByConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconfigrulespaginator)
         """
 
 class DescribeAggregateComplianceByConformancePacksPaginator(AioPaginator):
@@ -202,29 +202,29 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         Filters: AggregateConformancePackComplianceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAggregateComplianceByConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregateComplianceByConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregatecompliancebyconformancepackspaginator)
         """
 
 class DescribeAggregationAuthorizationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregationauthorizationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeAggregationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeAggregationAuthorizations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeaggregationauthorizationspaginator)
         """
 
 class DescribeComplianceByConfigRulePaginator(AioPaginator):
@@ -234,15 +234,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeComplianceByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyconfigrulepaginator)
         """
 
 class DescribeComplianceByResourcePaginator(AioPaginator):
@@ -253,15 +253,15 @@
 
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeComplianceByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeComplianceByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describecompliancebyresourcepaginator)
         """
 
 class DescribeConfigRuleEvaluationStatusPaginator(AioPaginator):
@@ -270,15 +270,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigRuleEvaluationStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRuleEvaluationStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigruleevaluationstatuspaginator)
         """
 
 class DescribeConfigRulesPaginator(AioPaginator):
@@ -288,15 +288,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleNames: Sequence[str] = ...,
         Filters: DescribeConfigRulesFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigrulespaginator)
         """
 
 class DescribeConfigurationAggregatorSourcesStatusPaginator(AioPaginator):
@@ -306,15 +306,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         UpdateStatus: Sequence[AggregatedSourceStatusTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigurationAggregatorSourcesStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregatorSourcesStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorsourcesstatuspaginator)
         """
 
 class DescribeConfigurationAggregatorsPaginator(AioPaginator):
@@ -323,15 +323,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
     """
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConfigurationAggregatorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConfigurationAggregators.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconfigurationaggregatorspaginator)
         """
 
 class DescribeConformancePackStatusPaginator(AioPaginator):
@@ -340,15 +340,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConformancePackStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePackStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackstatuspaginator)
         """
 
 class DescribeConformancePacksPaginator(AioPaginator):
@@ -357,15 +357,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         ConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeconformancepackspaginator)
         """
 
 class DescribeOrganizationConfigRuleStatusesPaginator(AioPaginator):
@@ -374,15 +374,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConfigRuleStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRuleStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulestatusespaginator)
         """
 
 class DescribeOrganizationConfigRulesPaginator(AioPaginator):
@@ -391,15 +391,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConfigRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConfigRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconfigrulespaginator)
         """
 
 class DescribeOrganizationConformancePackStatusesPaginator(AioPaginator):
@@ -408,15 +408,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConformancePackStatusesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePackStatuses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackstatusespaginator)
         """
 
 class DescribeOrganizationConformancePacksPaginator(AioPaginator):
@@ -425,29 +425,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeOrganizationConformancePacksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeOrganizationConformancePacks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeorganizationconformancepackspaginator)
         """
 
 class DescribePendingAggregationRequestsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describependingaggregationrequestspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribePendingAggregationRequestsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribePendingAggregationRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describependingaggregationrequestspaginator)
         """
 
 class DescribeRemediationExecutionStatusPaginator(AioPaginator):
@@ -457,15 +457,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ResourceKeys: Sequence[ResourceKeyTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRemediationExecutionStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRemediationExecutionStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeremediationexecutionstatuspaginator)
         """
 
 class DescribeRetentionConfigurationsPaginator(AioPaginator):
@@ -474,15 +474,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
     """
 
     def paginate(
         self,
         *,
         RetentionConfigurationNames: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeRetentionConfigurationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.DescribeRetentionConfigurations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#describeretentionconfigurationspaginator)
         """
 
 class GetAggregateComplianceDetailsByConfigRulePaginator(AioPaginator):
@@ -495,15 +495,15 @@
         self,
         *,
         ConfigurationAggregatorName: str,
         ConfigRuleName: str,
         AccountId: str,
         AwsRegion: str,
         ComplianceType: ComplianceTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetAggregateComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetAggregateComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getaggregatecompliancedetailsbyconfigrulepaginator)
         """
 
 class GetComplianceDetailsByConfigRulePaginator(AioPaginator):
@@ -513,15 +513,15 @@
     """
 
     def paginate(
         self,
         *,
         ConfigRuleName: str,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetComplianceDetailsByConfigRuleResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByConfigRule.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyconfigrulepaginator)
         """
 
 class GetComplianceDetailsByResourcePaginator(AioPaginator):
@@ -533,32 +533,29 @@
     def paginate(
         self,
         *,
         ResourceType: str = ...,
         ResourceId: str = ...,
         ComplianceTypes: Sequence[ComplianceTypeType] = ...,
         ResourceEvaluationId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetComplianceDetailsByResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetComplianceDetailsByResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getcompliancedetailsbyresourcepaginator)
         """
 
 class GetConformancePackComplianceSummaryPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getconformancepackcompliancesummarypaginator)
     """
 
     def paginate(
-        self,
-        *,
-        ConformancePackNames: Sequence[str],
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ConformancePackNames: Sequence[str], PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConformancePackComplianceSummaryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetConformancePackComplianceSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getconformancepackcompliancesummarypaginator)
         """
 
 class GetOrganizationConfigRuleDetailedStatusPaginator(AioPaginator):
@@ -568,15 +565,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConfigRuleName: str,
         Filters: StatusDetailFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetOrganizationConfigRuleDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConfigRuleDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconfigruledetailedstatuspaginator)
         """
 
 class GetOrganizationConformancePackDetailedStatusPaginator(AioPaginator):
@@ -586,15 +583,15 @@
     """
 
     def paginate(
         self,
         *,
         OrganizationConformancePackName: str,
         Filters: OrganizationResourceDetailedStatusFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetOrganizationConformancePackDetailedStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetOrganizationConformancePackDetailedStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getorganizationconformancepackdetailedstatuspaginator)
         """
 
 class GetResourceConfigHistoryPaginator(AioPaginator):
@@ -604,18 +601,18 @@
     """
 
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceId: str,
-        laterTime: Union[datetime, str] = ...,
-        earlierTime: Union[datetime, str] = ...,
+        laterTime: TimestampTypeDef = ...,
+        earlierTime: TimestampTypeDef = ...,
         chronologicalOrder: ChronologicalOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourceConfigHistoryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.GetResourceConfigHistory.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#getresourceconfighistorypaginator)
         """
 
 class ListAggregateDiscoveredResourcesPaginator(AioPaginator):
@@ -626,15 +623,15 @@
 
     def paginate(
         self,
         *,
         ConfigurationAggregatorName: str,
         ResourceType: ResourceTypeType,
         Filters: ResourceFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAggregateDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListAggregateDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listaggregatediscoveredresourcespaginator)
         """
 
 class ListDiscoveredResourcesPaginator(AioPaginator):
@@ -646,15 +643,15 @@
     def paginate(
         self,
         *,
         resourceType: ResourceTypeType,
         resourceIds: Sequence[str] = ...,
         resourceName: str = ...,
         includeDeletedResources: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDiscoveredResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListDiscoveredResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listdiscoveredresourcespaginator)
         """
 
 class ListResourceEvaluationsPaginator(AioPaginator):
@@ -663,29 +660,29 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: ResourceEvaluationFiltersTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceEvaluationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListResourceEvaluations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listresourceevaluationspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#listtagsforresourcepaginator)
         """
 
 class SelectAggregateResourceConfigPaginator(AioPaginator):
@@ -696,27 +693,27 @@
 
     def paginate(
         self,
         *,
         Expression: str,
         ConfigurationAggregatorName: str,
         MaxResults: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SelectAggregateResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectAggregateResourceConfig.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectaggregateresourceconfigpaginator)
         """
 
 class SelectResourceConfigPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectresourceconfigpaginator)
     """
 
     def paginate(
-        self, *, Expression: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Expression: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SelectResourceConfigResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService.Paginator.SelectResourceConfig.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/paginators/#selectresourceconfigpaginator)
         """
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/type_defs.py` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for config service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_config.type_defs import AccountAggregationSourceTypeDef
+    from types_aiobotocore_config.type_defs import AccountAggregationSourceOutputTypeDef
 
-    data: AccountAggregationSourceTypeDef = {...}
+    data: AccountAggregationSourceOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -54,34 +54,37 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
     "AggregationAuthorizationTypeDef",
     "BaseConfigurationItemTypeDef",
+    "ResponseMetadataTypeDef",
     "ResourceKeyTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
     "EvaluationModeConfigurationTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
-    "OrganizationAggregationSourceTypeDef",
+    "OrganizationAggregationSourceOutputTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
     "ConformancePackInputParameterTypeDef",
@@ -102,148 +105,125 @@
     "DeletePendingAggregationRequestRequestRequestTypeDef",
     "DeleteRemediationConfigurationRequestRequestTypeDef",
     "RemediationExceptionResourceKeyTypeDef",
     "DeleteResourceConfigRequestRequestTypeDef",
     "DeleteRetentionConfigurationRequestRequestTypeDef",
     "DeleteStoredQueryRequestRequestTypeDef",
     "DeliverConfigSnapshotRequestRequestTypeDef",
-    "DeliverConfigSnapshotResponseTypeDef",
-    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
     "DescribeComplianceByResourceRequestRequestTypeDef",
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     "DescribeConfigRulesFiltersTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     "DescribeConfigurationRecorderStatusRequestRequestTypeDef",
     "DescribeConfigurationRecordersRequestRequestTypeDef",
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
     "DescribeConformancePackStatusRequestRequestTypeDef",
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
     "DescribeConformancePacksRequestRequestTypeDef",
     "DescribeDeliveryChannelStatusRequestRequestTypeDef",
     "DescribeDeliveryChannelsRequestRequestTypeDef",
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     "OrganizationConfigRuleStatusTypeDef",
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     "OrganizationConformancePackStatusTypeDef",
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluationContextTypeDef",
+    "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
-    "EvaluationTypeDef",
+    "TimestampTypeDef",
+    "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
     "SsmControlsTypeDef",
-    "ExternalEvaluationTypeDef",
     "FieldInfoTypeDef",
-    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
-    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
-    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     "GetConformancePackComplianceSummaryRequestRequestTypeDef",
     "GetCustomRulePolicyRequestRequestTypeDef",
-    "GetCustomRulePolicyResponseTypeDef",
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     "ResourceCountTypeDef",
     "StatusDetailFiltersTypeDef",
     "MemberAccountStatusTypeDef",
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     "ResourceDetailsTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
     "StoredQueryTypeDef",
     "ResourceFiltersTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
+    "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
+    "OrganizationCustomRuleMetadataOutputTypeDef",
+    "OrganizationManagedRuleMetadataOutputTypeDef",
+    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
-    "OrganizationCustomPolicyRuleMetadataTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutConformancePackResponseTypeDef",
-    "PutOrganizationConfigRuleResponseTypeDef",
-    "PutOrganizationConformancePackResponseTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
-    "PutStoredQueryResponseTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
     "ResourceValueTypeDef",
+    "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
-    "TimeWindowTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
-    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
-    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
-    "StartResourceEvaluationResponseTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AccountAggregationSourceUnionTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
-    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "DeliverConfigSnapshotResponseTypeDef",
     "DescribeAggregationAuthorizationsResponseTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCustomRulePolicyResponseTypeDef",
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "PutAggregationAuthorizationResponseTypeDef",
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "PutConformancePackResponseTypeDef",
+    "PutOrganizationConfigRuleResponseTypeDef",
+    "PutOrganizationConformancePackResponseTypeDef",
+    "PutStoredQueryResponseTypeDef",
+    "StartResourceEvaluationResponseTypeDef",
     "BatchGetResourceConfigRequestRequestTypeDef",
     "BatchGetResourceConfigResponseTypeDef",
-    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     "DescribeRemediationExecutionStatusRequestRequestTypeDef",
     "StartRemediationExecutionRequestRequestTypeDef",
     "StartRemediationExecutionResponseTypeDef",
     "ComplianceSummaryTypeDef",
     "ComplianceTypeDef",
-    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     "GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     "DeliveryChannelTypeDef",
     "DeliveryChannelStatusTypeDef",
     "ConfigurationAggregatorTypeDef",
     "ConfigurationItemTypeDef",
@@ -258,29 +238,57 @@
     "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
     "FailedDeleteRemediationExceptionsBatchTypeDef",
-    "PutRemediationExceptionsRequestRequestTypeDef",
+    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
-    "EvaluationResultIdentifierTypeDef",
-    "PutEvaluationsRequestRequestTypeDef",
     "PutEvaluationsResponseTypeDef",
+    "EvaluationResultIdentifierTypeDef",
+    "EvaluationTypeDef",
+    "ExternalEvaluationTypeDef",
+    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    "GetResourceConfigHistoryRequestRequestTypeDef",
+    "PutRemediationExceptionsRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ExecutionControlsTypeDef",
-    "PutExternalEvaluationRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
@@ -293,24 +301,29 @@
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "OrganizationAggregationSourceUnionTypeDef",
     "OrganizationConfigRuleTypeDef",
+    "OrganizationCustomRuleMetadataUnionTypeDef",
+    "OrganizationManagedRuleMetadataUnionTypeDef",
     "PutOrganizationConfigRuleRequestRequestTypeDef",
+    "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
+    "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "ResourceEvaluationFiltersTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
     "ComplianceByConfigRuleTypeDef",
@@ -325,53 +338,85 @@
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
     "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
+    "EvaluationUnionTypeDef",
+    "PutExternalEvaluationRequestRequestTypeDef",
+    "ResourceEvaluationFiltersTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
+    "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
+    "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
-    "ListResourceEvaluationsRequestRequestTypeDef",
+    "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     "GetConformancePackComplianceDetailsResponseTypeDef",
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     "GetComplianceDetailsByResourceResponseTypeDef",
+    "PutEvaluationsRequestRequestTypeDef",
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    "ListResourceEvaluationsRequestRequestTypeDef",
     "DescribeConfigurationRecordersResponseTypeDef",
+    "ConfigurationRecorderUnionTypeDef",
     "PutConfigurationRecorderRequestRequestTypeDef",
     "DescribeRemediationConfigurationsResponseTypeDef",
     "FailedRemediationBatchTypeDef",
-    "PutRemediationConfigurationsRequestRequestTypeDef",
+    "RemediationConfigurationUnionTypeDef",
     "DescribeConfigRulesResponseTypeDef",
+    "ConfigRuleUnionTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
+    "PutRemediationConfigurationsRequestRequestTypeDef",
 )
 
+_RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredAccountAggregationSourceOutputTypeDef",
+    {
+        "AccountIds": List[str],
+    },
+)
+_OptionalAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalAccountAggregationSourceOutputTypeDef",
+    {
+        "AllAwsRegions": bool,
+        "AwsRegions": List[str],
+    },
+    total=False,
+)
+
+
+class AccountAggregationSourceOutputTypeDef(
+    _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
+):
+    pass
+
+
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
-        "AccountIds": List[str],
+        "AccountIds": Sequence[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
     "_OptionalAccountAggregationSourceTypeDef",
     {
         "AllAwsRegions": bool,
-        "AwsRegions": List[str],
+        "AwsRegions": Sequence[str],
     },
     total=False,
 )
 
 
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
@@ -485,14 +530,25 @@
         "resourceCreationTime": datetime,
         "configuration": str,
         "supplementaryConfiguration": Dict[str, str],
     },
     total=False,
 )
 
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
 ResourceKeyTypeDef = TypedDict(
     "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
@@ -565,18 +621,29 @@
     "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "ComplianceResourceTypes": List[str],
+        "TagKey": str,
+        "TagValue": str,
+        "ComplianceResourceId": str,
+    },
+    total=False,
+)
+
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
-        "ComplianceResourceTypes": List[str],
+        "ComplianceResourceTypes": Sequence[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
@@ -595,32 +662,33 @@
         "lastErrorCode": str,
         "lastErrorMessage": str,
         "lastStatusChangeTime": datetime,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceTypeDef",
+_RequiredOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceOutputTypeDef",
     {
         "RoleArn": str,
     },
 )
-_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceTypeDef",
+_OptionalOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceOutputTypeDef",
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
 
-class OrganizationAggregationSourceTypeDef(
-    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+class OrganizationAggregationSourceOutputTypeDef(
+    _RequiredOrganizationAggregationSourceOutputTypeDef,
+    _OptionalOrganizationAggregationSourceOutputTypeDef,
 ):
     pass
 
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
@@ -908,93 +976,55 @@
 DeliverConfigSnapshotRequestRequestTypeDef = TypedDict(
     "DeliverConfigSnapshotRequestRequestTypeDef",
     {
         "deliveryChannelName": str,
     },
 )
 
-DeliverConfigSnapshotResponseTypeDef = TypedDict(
-    "DeliverConfigSnapshotResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configSnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
-)
-
-DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
-    TypedDict(
-        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+    total=False,
 )
 
 DescribeAggregationAuthorizationsRequestRequestTypeDef = TypedDict(
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByConfigRuleRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByResourceRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigRuleEvaluationStatusRequestRequestTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1005,37 +1035,14 @@
     "DescribeConfigRulesFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
     },
     total=False,
 )
 
-_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
-    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
@@ -1052,23 +1059,14 @@
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
-    {
-        "ConfigurationAggregatorNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigurationAggregatorsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1087,42 +1085,24 @@
     "DescribeConfigurationRecordersRequestRequestTypeDef",
     {
         "ConfigurationRecorderNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePackStatusRequestRequestTypeDef = TypedDict(
     "DescribeConformancePackStatusRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeConformancePacksRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1141,23 +1121,14 @@
     "DescribeDeliveryChannelsRequestRequestTypeDef",
     {
         "DeliveryChannelNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1184,42 +1155,24 @@
 
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
 
-DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePackStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1247,41 +1200,24 @@
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
 
-DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePendingAggregationRequestsRequestRequestTypeDef = TypedDict(
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1323,23 +1259,14 @@
 
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
 
-DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
-    {
-        "RetentionConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRetentionConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1349,29 +1276,44 @@
     "RetentionConfigurationTypeDef",
     {
         "Name": str,
         "RetentionPeriodInDays": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EvaluationContextTypeDef = TypedDict(
+    "EvaluationContextTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EvaluationContextIdentifier": str,
     },
+    total=False,
 )
 
-EvaluationContextTypeDef = TypedDict(
-    "EvaluationContextTypeDef",
+_RequiredEvaluationOutputTypeDef = TypedDict(
+    "_RequiredEvaluationOutputTypeDef",
     {
-        "EvaluationContextIdentifier": str,
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": datetime,
+    },
+)
+_OptionalEvaluationOutputTypeDef = TypedDict(
+    "_OptionalEvaluationOutputTypeDef",
+    {
+        "Annotation": str,
     },
     total=False,
 )
 
+
+class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
+    pass
+
+
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1394,111 +1336,48 @@
 )
 
 
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
 
-_RequiredEvaluationTypeDef = TypedDict(
-    "_RequiredEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalEvaluationTypeDef = TypedDict(
-    "_OptionalEvaluationTypeDef",
+TimestampTypeDef = Union[datetime, str]
+ExclusionByResourceTypesOutputTypeDef = TypedDict(
+    "ExclusionByResourceTypesOutputTypeDef",
     {
-        "Annotation": str,
+        "resourceTypes": List[ResourceTypeType],
     },
     total=False,
 )
 
-
-class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
-    pass
-
-
 ExclusionByResourceTypesTypeDef = TypedDict(
     "ExclusionByResourceTypesTypeDef",
     {
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
     },
     total=False,
 )
 
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
         "ConcurrentExecutionRatePercentage": int,
         "ErrorPercentage": int,
     },
     total=False,
 )
 
-_RequiredExternalEvaluationTypeDef = TypedDict(
-    "_RequiredExternalEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalExternalEvaluationTypeDef = TypedDict(
-    "_OptionalExternalEvaluationTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-
-class ExternalEvaluationTypeDef(
-    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
-):
-    pass
-
-
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-        "ConfigRuleName": str,
-        "AccountId": str,
-        "AwsRegion": str,
-    },
-)
-_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceType": ComplianceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigRuleName": str,
         "AccountId": str,
         "AwsRegion": str,
@@ -1536,37 +1415,14 @@
     "GroupedResourceCountTypeDef",
     {
         "GroupName": str,
         "ResourceCount": int,
     },
 )
 
-_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleName": str,
-    },
-)
-_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
@@ -1583,26 +1439,14 @@
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
 
-GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "ResourceEvaluationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetComplianceDetailsByResourceRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
@@ -1615,36 +1459,14 @@
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
     {
         "ResourceTypes": Sequence[str],
     },
     total=False,
 )
 
-_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-    },
-)
-_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
-    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
     },
 )
 _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -1668,22 +1490,14 @@
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
 
-GetCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredResourceCountsRequestRequestTypeDef = TypedDict(
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[str],
         "limit": int,
         "nextToken": str,
     },
@@ -1771,75 +1585,14 @@
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
-GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
-    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-):
-    pass
-
-
-_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "limit": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-
-class GetResourceConfigHistoryRequestRequestTypeDef(
-    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
-    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
-):
-    pass
-
-
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
@@ -1900,39 +1653,14 @@
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
     },
     total=False,
 )
 
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceIds": Sequence[str],
-        "resourceName": str,
-        "includeDeletedResources": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
@@ -2004,36 +1732,14 @@
 
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
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
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -2058,14 +1764,36 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceTypeDef",
+    {
+        "RoleArn": str,
+    },
+)
+_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceTypeDef",
+    {
+        "AwsRegions": Sequence[str],
+        "AllAwsRegions": bool,
+    },
+    total=False,
+)
+
+
+class OrganizationAggregationSourceTypeDef(
+    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+):
+    pass
+
+
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -2075,65 +1803,67 @@
         "TagValueScope": str,
         "PolicyRuntime": str,
         "DebugLogDeliveryAccounts": List[str],
     },
     total=False,
 )
 
-_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataTypeDef",
+_RequiredOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeType],
     },
 )
-_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataTypeDef",
+_OptionalOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
 
-class OrganizationCustomRuleMetadataTypeDef(
-    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+class OrganizationCustomRuleMetadataOutputTypeDef(
+    _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
+    _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
 ):
     pass
 
 
-_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataTypeDef",
+_RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
-_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataTypeDef",
+_OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
 
-class OrganizationManagedRuleMetadataTypeDef(
-    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+class OrganizationManagedRuleMetadataOutputTypeDef(
+    _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
+    _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
 ):
     pass
 
 
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
@@ -2161,48 +1891,69 @@
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "LambdaFunctionArn": str,
+        "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
     },
-    total=False,
 )
-
-PutConformancePackResponseTypeDef = TypedDict(
-    "PutConformancePackResponseTypeDef",
+_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataTypeDef",
     {
-        "ConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
     },
+    total=False,
 )
 
-PutOrganizationConfigRuleResponseTypeDef = TypedDict(
-    "PutOrganizationConfigRuleResponseTypeDef",
+
+class OrganizationCustomRuleMetadataTypeDef(
+    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+):
+    pass
+
+
+_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataTypeDef",
     {
-        "OrganizationConfigRuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RuleIdentifier": str,
     },
 )
-
-PutOrganizationConformancePackResponseTypeDef = TypedDict(
-    "PutOrganizationConformancePackResponseTypeDef",
+_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataTypeDef",
     {
-        "OrganizationConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
     },
+    total=False,
 )
 
+
+class OrganizationManagedRuleMetadataTypeDef(
+    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+):
+    pass
+
+
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -2227,22 +1978,14 @@
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
-PutStoredQueryResponseTypeDef = TypedDict(
-    "PutStoredQueryResponseTypeDef",
-    {
-        "QueryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecordingStrategyTypeDef = TypedDict(
     "RecordingStrategyTypeDef",
     {
         "useOnly": RecordingStrategyTypeType,
     },
     total=False,
 )
@@ -2262,38 +2005,25 @@
 ResourceValueTypeDef = TypedDict(
     "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
-StaticValueTypeDef = TypedDict(
-    "StaticValueTypeDef",
+StaticValueOutputTypeDef = TypedDict(
+    "StaticValueOutputTypeDef",
     {
         "Values": List[str],
     },
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+StaticValueTypeDef = TypedDict(
+    "StaticValueTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Values": Sequence[str],
     },
 )
 
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
@@ -2314,42 +2044,14 @@
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "Expression": str,
-            "ConfigurationAggregatorName": str,
-        },
-    )
-)
-_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "MaxResults": int,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
-    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-):
-    pass
-
-
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2365,36 +2067,14 @@
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
-    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-):
-    pass
-
-
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2412,22 +2092,14 @@
 StartConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StartConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
-StartResourceEvaluationResponseTypeDef = TypedDict(
-    "StartResourceEvaluationResponseTypeDef",
-    {
-        "ResourceEvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StopConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
@@ -2435,14 +2107,17 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AccountAggregationSourceUnionTypeDef = Union[
+    AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef
+]
 AggregateComplianceByConformancePackTypeDef = TypedDict(
     "AggregateComplianceByConformancePackTypeDef",
     {
         "ConformancePackName": str,
         "Compliance": AggregateConformancePackComplianceTypeDef,
         "AccountId": str,
         "AwsRegion": str,
@@ -2455,37 +2130,14 @@
     {
         "ComplianceSummary": AggregateConformancePackComplianceCountTypeDef,
         "GroupName": str,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
@@ -2543,96 +2195,144 @@
     "GetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifier": AggregateResourceIdentifierTypeDef,
     },
 )
 
-ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
+BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetAggregateResourceConfigResponseTypeDef",
     {
-        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeliverConfigSnapshotResponseTypeDef = TypedDict(
+    "DeliverConfigSnapshotResponseTypeDef",
+    {
+        "configSnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
+    "DescribeAggregationAuthorizationsResponseTypeDef",
+    {
+        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationAggregatorSourcesStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     {
         "AggregatedSourceStatusList": List[AggregatedSourceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
-    "DescribeAggregationAuthorizationsResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
+    {
+        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAggregationAuthorizationResponseTypeDef = TypedDict(
     "PutAggregationAuthorizationResponseTypeDef",
     {
         "AggregationAuthorization": AggregationAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+PutConformancePackResponseTypeDef = TypedDict(
+    "PutConformancePackResponseTypeDef",
     {
-        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
-    "BatchGetResourceConfigRequestRequestTypeDef",
+PutOrganizationConfigRuleResponseTypeDef = TypedDict(
+    "PutOrganizationConfigRuleResponseTypeDef",
     {
-        "resourceKeys": Sequence[ResourceKeyTypeDef],
+        "OrganizationConfigRuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetResourceConfigResponseTypeDef",
+PutOrganizationConformancePackResponseTypeDef = TypedDict(
+    "PutOrganizationConformancePackResponseTypeDef",
     {
-        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OrganizationConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+PutStoredQueryResponseTypeDef = TypedDict(
+    "PutStoredQueryResponseTypeDef",
     {
-        "ConfigRuleName": str,
+        "QueryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+
+StartResourceEvaluationResponseTypeDef = TypedDict(
+    "StartResourceEvaluationResponseTypeDef",
     {
-        "ResourceKeys": Sequence[ResourceKeyTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResourceEvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
+    "BatchGetResourceConfigRequestRequestTypeDef",
+    {
+        "resourceKeys": Sequence[ResourceKeyTypeDef],
+    },
+)
 
-class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
-    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-):
-    pass
-
+BatchGetResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetResourceConfigResponseTypeDef",
+    {
+        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
@@ -2663,15 +2363,15 @@
 )
 
 StartRemediationExecutionResponseTypeDef = TypedDict(
     "StartRemediationExecutionResponseTypeDef",
     {
         "FailureMessage": str,
         "FailedItems": List[ResourceKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryTypeDef = TypedDict(
     "ComplianceSummaryTypeDef",
     {
         "CompliantResourceCount": ComplianceContributorCountTypeDef,
@@ -2686,37 +2386,14 @@
     {
         "ComplianceType": ComplianceTypeType,
         "ComplianceContributorCount": ComplianceContributorCountTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "Filters": ConfigRuleComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
@@ -2763,15 +2440,15 @@
 
 
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeliveryChannelTypeDef = TypedDict(
     "DeliveryChannelTypeDef",
     {
         "name": str,
@@ -2796,16 +2473,16 @@
 )
 
 ConfigurationAggregatorTypeDef = TypedDict(
     "ConfigurationAggregatorTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigurationAggregatorArn": str,
-        "AccountAggregationSources": List[AccountAggregationSourceTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "AccountAggregationSources": List[AccountAggregationSourceOutputTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
@@ -2834,15 +2511,15 @@
     total=False,
 )
 
 DescribeConfigurationRecorderStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     {
         "ConfigurationRecordersStatus": List[ConfigurationRecorderStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeConformancePackComplianceRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConformancePackComplianceRequestRequestTypeDef",
     {
         "ConformancePackName": str,
@@ -2867,15 +2544,15 @@
 
 
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConformancePackComplianceScoresRequestRequestTypeDef = TypedDict(
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     {
         "Filters": ConformancePackComplianceScoresFiltersTypeDef,
@@ -2888,15 +2565,15 @@
 )
 
 GetConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetConformancePackComplianceSummaryResponseTypeDef",
     {
         "ConformancePackComplianceSummaryList": List[ConformancePackComplianceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOrganizationConformancePackTypeDef = TypedDict(
     "_RequiredOrganizationConformancePackTypeDef",
     {
         "OrganizationConformancePackName": str,
@@ -3030,24 +2707,24 @@
 
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePackStatusResponseTypeDef = TypedDict(
     "DescribeConformancePackStatusResponseTypeDef",
     {
         "ConformancePackStatusDetails": List[ConformancePackStatusDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
@@ -3084,44 +2761,412 @@
     {
         "FailureMessage": str,
         "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
     },
     total=False,
 )
 
-_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
+_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "Filters": ConfigRuleComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+):
+    pass
+
+
+DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
+    TypedDict(
+        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
+    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+):
+    pass
+
+
+DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    {
+        "ConfigurationAggregatorNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     {
         "ConfigRuleName": str,
-        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
-_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
+_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     {
-        "Message": str,
-        "ExpirationTime": Union[datetime, str],
+        "ResourceKeys": Sequence[ResourceKeyTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
-class PutRemediationExceptionsRequestRequestTypeDef(
-    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
-    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
+class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
+    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+):
+    pass
+
+
+DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    {
+        "RetentionConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+        "ConfigRuleName": str,
+        "AccountId": str,
+        "AwsRegion": str,
+    },
+)
+_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceType": ComplianceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleName": str,
+    },
+)
+_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+
+GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "ResourceEvaluationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+    },
+)
+_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
+    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceIds": Sequence[str],
+        "resourceName": str,
+        "includeDeletedResources": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
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
+_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "Expression": str,
+            "ConfigurationAggregatorName": str,
+        },
+    )
+)
+_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "MaxResults": int,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
+    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "Expression": str,
+    },
+)
+_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
+    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
 ):
     pass
 
 
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeConfigRulesRequestRequestTypeDef",
     {
@@ -3133,42 +3178,42 @@
 )
 
 DescribeOrganizationConfigRuleStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     {
         "OrganizationConfigRuleStatuses": List[OrganizationConfigRuleStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePackStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     {
         "OrganizationConformancePackStatuses": List[OrganizationConformancePackStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePendingAggregationRequestsResponseTypeDef = TypedDict(
     "DescribePendingAggregationRequestsResponseTypeDef",
     {
         "PendingAggregationRequests": List[PendingAggregationRequestTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRemediationExceptionsResponseTypeDef = TypedDict(
     "DescribeRemediationExceptionsResponseTypeDef",
     {
         "RemediationExceptions": List[RemediationExceptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationExceptionBatchTypeDef = TypedDict(
     "FailedRemediationExceptionBatchTypeDef",
     {
         "FailureMessage": str,
@@ -3178,80 +3223,182 @@
 )
 
 DescribeRetentionConfigurationsResponseTypeDef = TypedDict(
     "DescribeRetentionConfigurationsResponseTypeDef",
     {
         "RetentionConfigurations": List[RetentionConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRetentionConfigurationResponseTypeDef = TypedDict(
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutEvaluationsResponseTypeDef = TypedDict(
+    "PutEvaluationsResponseTypeDef",
+    {
+        "FailedEvaluations": List[EvaluationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
     total=False,
 )
 
-_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEvaluationsRequestRequestTypeDef",
+_RequiredEvaluationTypeDef = TypedDict(
+    "_RequiredEvaluationTypeDef",
     {
-        "ResultToken": str,
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
     },
 )
-_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEvaluationsRequestRequestTypeDef",
+_OptionalEvaluationTypeDef = TypedDict(
+    "_OptionalEvaluationTypeDef",
     {
-        "Evaluations": Sequence[EvaluationTypeDef],
-        "TestMode": bool,
+        "Annotation": str,
     },
     total=False,
 )
 
 
-class PutEvaluationsRequestRequestTypeDef(
-    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
+    pass
+
+
+_RequiredExternalEvaluationTypeDef = TypedDict(
+    "_RequiredExternalEvaluationTypeDef",
+    {
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
+    },
+)
+_OptionalExternalEvaluationTypeDef = TypedDict(
+    "_OptionalExternalEvaluationTypeDef",
+    {
+        "Annotation": str,
+    },
+    total=False,
+)
+
+
+class ExternalEvaluationTypeDef(
+    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
 
-PutEvaluationsResponseTypeDef = TypedDict(
-    "PutEvaluationsResponseTypeDef",
+_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     {
-        "FailedEvaluations": List[EvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
     },
 )
+_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ExecutionControlsTypeDef = TypedDict(
-    "ExecutionControlsTypeDef",
+
+class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
+    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
-        "SsmControls": SsmControlsTypeDef,
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "limit": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-PutExternalEvaluationRequestRequestTypeDef = TypedDict(
-    "PutExternalEvaluationRequestRequestTypeDef",
+
+class GetResourceConfigHistoryRequestRequestTypeDef(
+    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
+    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
-        "ExternalEvaluation": ExternalEvaluationTypeDef,
+        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
+    },
+)
+_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
+    {
+        "Message": str,
+        "ExpirationTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+
+class PutRemediationExceptionsRequestRequestTypeDef(
+    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
+    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
+):
+    pass
+
+
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+ExecutionControlsTypeDef = TypedDict(
+    "ExecutionControlsTypeDef",
+    {
+        "SsmControls": SsmControlsTypeDef,
     },
+    total=False,
 )
 
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
@@ -3286,39 +3433,39 @@
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetDiscoveredResourceCountsResponseTypeDef",
     {
         "totalDiscoveredResources": int,
         "resourceCounts": List[ResourceCountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "Filters": StatusDetailFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
@@ -3352,29 +3499,29 @@
 
 
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
@@ -3410,29 +3557,29 @@
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceEvaluationSummaryResponseTypeDef = TypedDict(
     "GetResourceEvaluationSummaryResponseTypeDef",
     {
         "ResourceEvaluationId": str,
         "EvaluationMode": EvaluationModeType,
         "EvaluationStatus": EvaluationStatusTypeDef,
         "EvaluationStartTimestamp": datetime,
         "Compliance": ComplianceTypeType,
         "EvaluationContext": EvaluationContextTypeDef,
         "ResourceDetails": ResourceDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredStartResourceEvaluationRequestRequestTypeDef",
     {
         "ResourceDetails": ResourceDetailsTypeDef,
@@ -3457,30 +3604,30 @@
     pass
 
 
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "Filters": ResourceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
@@ -3515,42 +3662,42 @@
 
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceEvaluationsResponseTypeDef = TypedDict(
     "ListResourceEvaluationsResponseTypeDef",
     {
         "ResourceEvaluations": List[ResourceEvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStoredQueriesResponseTypeDef = TypedDict(
     "ListStoredQueriesResponseTypeDef",
     {
         "StoredQueryMetadata": List[StoredQueryMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
@@ -3569,38 +3716,14 @@
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-
-class PutConfigurationAggregatorRequestRequestTypeDef(
-    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
-    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
-):
-    pass
-
-
 _RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
     },
 )
 _OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
@@ -3622,40 +3745,49 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+OrganizationAggregationSourceUnionTypeDef = Union[
+    OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
+]
 _RequiredOrganizationConfigRuleTypeDef = TypedDict(
     "_RequiredOrganizationConfigRuleTypeDef",
     {
         "OrganizationConfigRuleName": str,
         "OrganizationConfigRuleArn": str,
     },
 )
 _OptionalOrganizationConfigRuleTypeDef = TypedDict(
     "_OptionalOrganizationConfigRuleTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
         "ExcludedAccounts": List[str],
         "LastUpdateTime": datetime,
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
 
 class OrganizationConfigRuleTypeDef(
     _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
 
+OrganizationCustomRuleMetadataUnionTypeDef = Union[
+    OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
+]
+OrganizationManagedRuleMetadataUnionTypeDef = Union[
+    OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
+]
 _RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
@@ -3673,20 +3805,32 @@
 class PutOrganizationConfigRuleRequestRequestTypeDef(
     _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
     _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
 
+RecordingGroupOutputTypeDef = TypedDict(
+    "RecordingGroupOutputTypeDef",
+    {
+        "allSupported": bool,
+        "includeGlobalResourceTypes": bool,
+        "resourceTypes": List[ResourceTypeType],
+        "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
+        "recordingStrategy": RecordingStrategyTypeDef,
+    },
+    total=False,
+)
+
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesTypeDef,
         "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
@@ -3697,72 +3841,116 @@
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
+RemediationParameterValueOutputTypeDef = TypedDict(
+    "RemediationParameterValueOutputTypeDef",
+    {
+        "ResourceValue": ResourceValueTypeDef,
+        "StaticValue": StaticValueOutputTypeDef,
+    },
+    total=False,
+)
+
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-ResourceEvaluationFiltersTypeDef = TypedDict(
-    "ResourceEvaluationFiltersTypeDef",
+_RequiredSourceOutputTypeDef = TypedDict(
+    "_RequiredSourceOutputTypeDef",
     {
-        "EvaluationMode": EvaluationModeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "EvaluationContextIdentifier": str,
+        "Owner": OwnerType,
+    },
+)
+_OptionalSourceOutputTypeDef = TypedDict(
+    "_OptionalSourceOutputTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceDetails": List[SourceDetailTypeDef],
+        "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+
+class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
+    pass
+
+
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailTypeDef],
+        "SourceDetails": Sequence[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
 
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
 
+_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "AccountAggregationSources": Sequence[AccountAggregationSourceUnionTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutConfigurationAggregatorRequestRequestTypeDef(
+    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
+    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
+):
+    pass
+
+
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     {
         "AggregateConformancePackComplianceSummaries": List[
             AggregateConformancePackComplianceSummaryTypeDef
         ],
         "GroupByKey": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceCountTypeDef = TypedDict(
     "AggregateComplianceCountTypeDef",
     {
         "GroupName": str,
@@ -3780,15 +3968,15 @@
     total=False,
 )
 
 GetComplianceSummaryByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     {
         "ComplianceSummary": ComplianceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceByConfigRuleTypeDef = TypedDict(
     "AggregateComplianceByConfigRuleTypeDef",
     {
         "ConfigRuleName": str,
@@ -3818,98 +4006,98 @@
     total=False,
 )
 
 DescribeDeliveryChannelsResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelsResponseTypeDef",
     {
         "DeliveryChannels": List[DeliveryChannelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDeliveryChannelRequestRequestTypeDef = TypedDict(
     "PutDeliveryChannelRequestRequestTypeDef",
     {
         "DeliveryChannel": DeliveryChannelTypeDef,
     },
 )
 
 DescribeDeliveryChannelStatusResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelStatusResponseTypeDef",
     {
         "DeliveryChannelsStatus": List[DeliveryChannelStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationAggregatorsResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsResponseTypeDef",
     {
         "ConfigurationAggregators": List[ConfigurationAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationAggregatorResponseTypeDef = TypedDict(
     "PutConfigurationAggregatorResponseTypeDef",
     {
         "ConfigurationAggregator": ConfigurationAggregatorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateResourceConfigResponseTypeDef = TypedDict(
     "GetAggregateResourceConfigResponseTypeDef",
     {
         "ConfigurationItem": ConfigurationItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceConfigHistoryResponseTypeDef = TypedDict(
     "GetResourceConfigHistoryResponseTypeDef",
     {
         "configurationItems": List[ConfigurationItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePacksResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksResponseTypeDef",
     {
         "OrganizationConformancePacks": List[OrganizationConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePacksResponseTypeDef = TypedDict(
     "DescribeConformancePacksResponseTypeDef",
     {
         "ConformancePackDetails": List[ConformancePackDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRemediationExceptionsResponseTypeDef = TypedDict(
     "DeleteRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRemediationExceptionsResponseTypeDef = TypedDict(
     "PutRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationExceptionBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateEvaluationResultTypeDef = TypedDict(
     "AggregateEvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
@@ -3956,41 +4144,70 @@
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
+EvaluationUnionTypeDef = Union[EvaluationTypeDef, EvaluationOutputTypeDef]
+PutExternalEvaluationRequestRequestTypeDef = TypedDict(
+    "PutExternalEvaluationRequestRequestTypeDef",
+    {
+        "ConfigRuleName": str,
+        "ExternalEvaluation": ExternalEvaluationTypeDef,
+    },
+)
+
+ResourceEvaluationFiltersTypeDef = TypedDict(
+    "ResourceEvaluationFiltersTypeDef",
+    {
+        "EvaluationMode": EvaluationModeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "EvaluationContextIdentifier": str,
+    },
+    total=False,
+)
+
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectResourceConfigResponseTypeDef = TypedDict(
     "SelectResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigRulesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesResponseTypeDef",
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfigurationRecorderOutputTypeDef = TypedDict(
+    "ConfigurationRecorderOutputTypeDef",
+    {
+        "name": str,
+        "roleARN": str,
+        "recordingGroup": RecordingGroupOutputTypeDef,
     },
+    total=False,
 )
 
 ConfigurationRecorderTypeDef = TypedDict(
     "ConfigurationRecorderTypeDef",
     {
         "name": str,
         "roleARN": str,
@@ -4000,31 +4217,62 @@
 )
 
 DescribeRemediationExecutionStatusResponseTypeDef = TypedDict(
     "DescribeRemediationExecutionStatusResponseTypeDef",
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRemediationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredRemediationConfigurationOutputTypeDef",
+    {
+        "ConfigRuleName": str,
+        "TargetType": Literal["SSM_DOCUMENT"],
+        "TargetId": str,
+    },
+)
+_OptionalRemediationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalRemediationConfigurationOutputTypeDef",
+    {
+        "TargetVersion": str,
+        "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
+        "ResourceType": str,
+        "Automatic": bool,
+        "ExecutionControls": ExecutionControlsTypeDef,
+        "MaximumAutomaticAttempts": int,
+        "RetryAttemptSeconds": int,
+        "Arn": str,
+        "CreatedByService": str,
+    },
+    total=False,
+)
+
+
+class RemediationConfigurationOutputTypeDef(
+    _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
 )
 _OptionalRemediationConfigurationTypeDef = TypedDict(
     "_OptionalRemediationConfigurationTypeDef",
     {
         "TargetVersion": str,
-        "Parameters": Dict[str, RemediationParameterValueTypeDef],
+        "Parameters": Mapping[str, RemediationParameterValueTypeDef],
         "ResourceType": str,
         "Automatic": bool,
         "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
@@ -4035,33 +4283,42 @@
 
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
 
-ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+_RequiredConfigRuleOutputTypeDef = TypedDict(
+    "_RequiredConfigRuleOutputTypeDef",
     {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Source": SourceOutputTypeDef,
     },
-    total=False,
 )
-
-ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestRequestTypeDef",
+_OptionalConfigRuleOutputTypeDef = TypedDict(
+    "_OptionalConfigRuleOutputTypeDef",
     {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "Limit": int,
-        "NextToken": str,
+        "ConfigRuleName": str,
+        "ConfigRuleArn": str,
+        "ConfigRuleId": str,
+        "Description": str,
+        "Scope": ScopeOutputTypeDef,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ConfigRuleState": ConfigRuleStateType,
+        "CreatedBy": str,
+        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
+
+class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
+    pass
+
+
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -4072,15 +4329,15 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
+        "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
 
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
@@ -4088,138 +4345,179 @@
 
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceSummaryByResourceTypeResponseTypeDef = TypedDict(
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     {
         "ComplianceSummariesByResourceType": List[ComplianceSummaryByResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAggregateComplianceByConfigRulesResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     {
         "AggregateComplianceByConfigRules": List[AggregateComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByConfigRuleResponseTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleResponseTypeDef",
     {
         "ComplianceByConfigRules": List[ComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByResourceResponseTypeDef = TypedDict(
     "DescribeComplianceByResourceResponseTypeDef",
     {
         "ComplianceByResources": List[ComplianceByResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "AggregateEvaluationResults": List[AggregateEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConformancePackComplianceDetailsResponseTypeDef = TypedDict(
     "GetConformancePackComplianceDetailsResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleEvaluationResults": List[ConformancePackEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByResourceResponseTypeDef = TypedDict(
     "GetComplianceDetailsByResourceResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEvaluationsRequestRequestTypeDef",
+    {
+        "ResultToken": str,
+    },
+)
+_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEvaluationsRequestRequestTypeDef",
+    {
+        "Evaluations": Sequence[EvaluationUnionTypeDef],
+        "TestMode": bool,
+    },
+    total=False,
+)
+
+
+class PutEvaluationsRequestRequestTypeDef(
+    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+):
+    pass
+
+
+ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestRequestTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "Limit": int,
+        "NextToken": str,
     },
+    total=False,
 )
 
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
-        "ConfigurationRecorders": List[ConfigurationRecorderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationRecorderUnionTypeDef = Union[
+    ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
+]
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
-        "RemediationConfigurations": List[RemediationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[RemediationConfigurationTypeDef],
+        "FailedItems": List[RemediationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-    {
-        "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
-    },
-)
-
+RemediationConfigurationUnionTypeDef = Union[
+    RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef
+]
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
-        "ConfigRules": List[ConfigRuleTypeDef],
+        "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigRuleUnionTypeDef = Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef]
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
     },
 )
 _OptionalPutConfigRuleRequestRequestTypeDef = TypedDict(
@@ -4237,10 +4535,17 @@
     pass
 
 
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+    {
+        "RemediationConfigurations": Sequence[RemediationConfigurationUnionTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config/type_defs.pyi` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for config service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_config.type_defs import AccountAggregationSourceTypeDef
+    from types_aiobotocore_config.type_defs import AccountAggregationSourceOutputTypeDef
 
-    data: AccountAggregationSourceTypeDef = {...}
+    data: AccountAggregationSourceOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -53,34 +53,37 @@
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "AccountAggregationSourceOutputTypeDef",
     "AccountAggregationSourceTypeDef",
     "AggregateConformancePackComplianceTypeDef",
     "AggregateConformancePackComplianceCountTypeDef",
     "AggregateConformancePackComplianceFiltersTypeDef",
     "AggregateConformancePackComplianceSummaryFiltersTypeDef",
     "AggregateResourceIdentifierTypeDef",
     "AggregatedSourceStatusTypeDef",
     "AggregationAuthorizationTypeDef",
     "BaseConfigurationItemTypeDef",
+    "ResponseMetadataTypeDef",
     "ResourceKeyTypeDef",
     "ComplianceContributorCountTypeDef",
     "ConfigExportDeliveryInfoTypeDef",
     "ConfigRuleComplianceFiltersTypeDef",
     "ConfigRuleComplianceSummaryFiltersTypeDef",
     "ConfigRuleEvaluationStatusTypeDef",
     "EvaluationModeConfigurationTypeDef",
+    "ScopeOutputTypeDef",
     "ScopeTypeDef",
     "ConfigSnapshotDeliveryPropertiesTypeDef",
     "ConfigStreamDeliveryInfoTypeDef",
-    "OrganizationAggregationSourceTypeDef",
+    "OrganizationAggregationSourceOutputTypeDef",
     "RelationshipTypeDef",
     "ConfigurationRecorderStatusTypeDef",
     "ConformancePackComplianceFiltersTypeDef",
     "ConformancePackComplianceScoreTypeDef",
     "ConformancePackComplianceScoresFiltersTypeDef",
     "ConformancePackComplianceSummaryTypeDef",
     "ConformancePackInputParameterTypeDef",
@@ -101,148 +104,125 @@
     "DeletePendingAggregationRequestRequestRequestTypeDef",
     "DeleteRemediationConfigurationRequestRequestTypeDef",
     "RemediationExceptionResourceKeyTypeDef",
     "DeleteResourceConfigRequestRequestTypeDef",
     "DeleteRetentionConfigurationRequestRequestTypeDef",
     "DeleteStoredQueryRequestRequestTypeDef",
     "DeliverConfigSnapshotRequestRequestTypeDef",
-    "DeliverConfigSnapshotResponseTypeDef",
-    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
     "DescribeComplianceByResourceRequestRequestTypeDef",
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     "DescribeConfigRulesFiltersTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
     "DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     "DescribeConfigurationRecorderStatusRequestRequestTypeDef",
     "DescribeConfigurationRecordersRequestRequestTypeDef",
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
     "DescribeConformancePackStatusRequestRequestTypeDef",
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
     "DescribeConformancePacksRequestRequestTypeDef",
     "DescribeDeliveryChannelStatusRequestRequestTypeDef",
     "DescribeDeliveryChannelsRequestRequestTypeDef",
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     "OrganizationConfigRuleStatusTypeDef",
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     "OrganizationConformancePackStatusTypeDef",
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     "PendingAggregationRequestTypeDef",
     "DescribeRemediationConfigurationsRequestRequestTypeDef",
     "RemediationExceptionTypeDef",
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     "RetentionConfigurationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluationContextTypeDef",
+    "EvaluationOutputTypeDef",
     "EvaluationResultQualifierTypeDef",
     "EvaluationStatusTypeDef",
-    "EvaluationTypeDef",
+    "TimestampTypeDef",
+    "ExclusionByResourceTypesOutputTypeDef",
     "ExclusionByResourceTypesTypeDef",
     "SsmControlsTypeDef",
-    "ExternalEvaluationTypeDef",
     "FieldInfoTypeDef",
-    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     "ResourceCountFiltersTypeDef",
     "GroupedResourceCountTypeDef",
-    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
     "GetComplianceDetailsByConfigRuleRequestRequestTypeDef",
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
-    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
     "GetConformancePackComplianceSummaryRequestRequestTypeDef",
     "GetCustomRulePolicyRequestRequestTypeDef",
-    "GetCustomRulePolicyResponseTypeDef",
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     "ResourceCountTypeDef",
     "StatusDetailFiltersTypeDef",
     "MemberAccountStatusTypeDef",
     "OrganizationResourceDetailedStatusFiltersTypeDef",
     "OrganizationConformancePackDetailedStatusTypeDef",
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    "GetResourceConfigHistoryRequestRequestTypeDef",
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     "ResourceDetailsTypeDef",
     "GetStoredQueryRequestRequestTypeDef",
     "StoredQueryTypeDef",
     "ResourceFiltersTypeDef",
-    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
     "ResourceIdentifierTypeDef",
     "ResourceEvaluationTypeDef",
     "ListStoredQueriesRequestRequestTypeDef",
     "StoredQueryMetadataTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
+    "OrganizationAggregationSourceTypeDef",
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
+    "OrganizationCustomRuleMetadataOutputTypeDef",
+    "OrganizationManagedRuleMetadataOutputTypeDef",
+    "OrganizationCustomPolicyRuleMetadataTypeDef",
     "OrganizationCustomRuleMetadataTypeDef",
     "OrganizationManagedRuleMetadataTypeDef",
-    "OrganizationCustomPolicyRuleMetadataTypeDef",
-    "PaginatorConfigTypeDef",
-    "PutConformancePackResponseTypeDef",
-    "PutOrganizationConfigRuleResponseTypeDef",
-    "PutOrganizationConformancePackResponseTypeDef",
     "PutResourceConfigRequestRequestTypeDef",
     "PutRetentionConfigurationRequestRequestTypeDef",
-    "PutStoredQueryResponseTypeDef",
     "RecordingStrategyTypeDef",
     "RemediationExecutionStepTypeDef",
     "ResourceValueTypeDef",
+    "StaticValueOutputTypeDef",
     "StaticValueTypeDef",
-    "TimeWindowTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectAggregateResourceConfigRequestRequestTypeDef",
-    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
     "SelectResourceConfigRequestRequestTypeDef",
-    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "SourceDetailTypeDef",
     "StartConfigRulesEvaluationRequestRequestTypeDef",
     "StartConfigurationRecorderRequestRequestTypeDef",
-    "StartResourceEvaluationResponseTypeDef",
     "StopConfigurationRecorderRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "AccountAggregationSourceUnionTypeDef",
     "AggregateComplianceByConformancePackTypeDef",
     "AggregateConformancePackComplianceSummaryTypeDef",
-    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
     "DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     "GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef",
     "BatchGetAggregateResourceConfigRequestRequestTypeDef",
     "GetAggregateResourceConfigRequestRequestTypeDef",
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
-    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "DeliverConfigSnapshotResponseTypeDef",
     "DescribeAggregationAuthorizationsResponseTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCustomRulePolicyResponseTypeDef",
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
     "PutAggregationAuthorizationResponseTypeDef",
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+    "PutConformancePackResponseTypeDef",
+    "PutOrganizationConfigRuleResponseTypeDef",
+    "PutOrganizationConformancePackResponseTypeDef",
+    "PutStoredQueryResponseTypeDef",
+    "StartResourceEvaluationResponseTypeDef",
     "BatchGetResourceConfigRequestRequestTypeDef",
     "BatchGetResourceConfigResponseTypeDef",
-    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     "DescribeRemediationExecutionStatusRequestRequestTypeDef",
     "StartRemediationExecutionRequestRequestTypeDef",
     "StartRemediationExecutionResponseTypeDef",
     "ComplianceSummaryTypeDef",
     "ComplianceTypeDef",
-    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
     "DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     "GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef",
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     "DeliveryChannelTypeDef",
     "DeliveryChannelStatusTypeDef",
     "ConfigurationAggregatorTypeDef",
     "ConfigurationItemTypeDef",
@@ -257,29 +237,57 @@
     "PutConformancePackRequestRequestTypeDef",
     "GetConformancePackComplianceDetailsRequestRequestTypeDef",
     "DescribeConformancePackComplianceResponseTypeDef",
     "DescribeConformancePackStatusResponseTypeDef",
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     "DescribeRemediationExceptionsRequestRequestTypeDef",
     "FailedDeleteRemediationExceptionsBatchTypeDef",
-    "PutRemediationExceptionsRequestRequestTypeDef",
+    "DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    "DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    "DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    "GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    "GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    "ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+    "SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     "DescribeConfigRulesRequestRequestTypeDef",
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     "DescribePendingAggregationRequestsResponseTypeDef",
     "DescribeRemediationExceptionsResponseTypeDef",
     "FailedRemediationExceptionBatchTypeDef",
     "DescribeRetentionConfigurationsResponseTypeDef",
     "PutRetentionConfigurationResponseTypeDef",
-    "EvaluationResultIdentifierTypeDef",
-    "PutEvaluationsRequestRequestTypeDef",
     "PutEvaluationsResponseTypeDef",
+    "EvaluationResultIdentifierTypeDef",
+    "EvaluationTypeDef",
+    "ExternalEvaluationTypeDef",
+    "GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    "GetResourceConfigHistoryRequestRequestTypeDef",
+    "PutRemediationExceptionsRequestRequestTypeDef",
+    "TimeWindowTypeDef",
     "ExecutionControlsTypeDef",
-    "PutExternalEvaluationRequestRequestTypeDef",
     "QueryInfoTypeDef",
     "GetAggregateDiscoveredResourceCountsRequestRequestTypeDef",
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     "GetDiscoveredResourceCountsResponseTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     "GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef",
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
@@ -292,24 +300,29 @@
     "ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     "ListAggregateDiscoveredResourcesRequestRequestTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "ListResourceEvaluationsResponseTypeDef",
     "ListStoredQueriesResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "PutAggregationAuthorizationRequestRequestTypeDef",
-    "PutConfigurationAggregatorRequestRequestTypeDef",
     "PutStoredQueryRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "OrganizationAggregationSourceUnionTypeDef",
     "OrganizationConfigRuleTypeDef",
+    "OrganizationCustomRuleMetadataUnionTypeDef",
+    "OrganizationManagedRuleMetadataUnionTypeDef",
     "PutOrganizationConfigRuleRequestRequestTypeDef",
+    "RecordingGroupOutputTypeDef",
     "RecordingGroupTypeDef",
     "RemediationExecutionStatusTypeDef",
+    "RemediationParameterValueOutputTypeDef",
     "RemediationParameterValueTypeDef",
-    "ResourceEvaluationFiltersTypeDef",
+    "SourceOutputTypeDef",
     "SourceTypeDef",
+    "PutConfigurationAggregatorRequestRequestTypeDef",
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     "AggregateComplianceCountTypeDef",
     "ComplianceSummaryByResourceTypeTypeDef",
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     "AggregateComplianceByConfigRuleTypeDef",
     "ComplianceByConfigRuleTypeDef",
@@ -324,53 +337,83 @@
     "DescribeOrganizationConformancePacksResponseTypeDef",
     "DescribeConformancePacksResponseTypeDef",
     "DeleteRemediationExceptionsResponseTypeDef",
     "PutRemediationExceptionsResponseTypeDef",
     "AggregateEvaluationResultTypeDef",
     "ConformancePackEvaluationResultTypeDef",
     "EvaluationResultTypeDef",
+    "EvaluationUnionTypeDef",
+    "PutExternalEvaluationRequestRequestTypeDef",
+    "ResourceEvaluationFiltersTypeDef",
     "SelectAggregateResourceConfigResponseTypeDef",
     "SelectResourceConfigResponseTypeDef",
     "DescribeOrganizationConfigRulesResponseTypeDef",
+    "ConfigurationRecorderOutputTypeDef",
     "ConfigurationRecorderTypeDef",
     "DescribeRemediationExecutionStatusResponseTypeDef",
+    "RemediationConfigurationOutputTypeDef",
     "RemediationConfigurationTypeDef",
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
-    "ListResourceEvaluationsRequestRequestTypeDef",
+    "ConfigRuleOutputTypeDef",
     "ConfigRuleTypeDef",
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     "DescribeComplianceByConfigRuleResponseTypeDef",
     "DescribeComplianceByResourceResponseTypeDef",
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     "GetConformancePackComplianceDetailsResponseTypeDef",
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     "GetComplianceDetailsByResourceResponseTypeDef",
+    "PutEvaluationsRequestRequestTypeDef",
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    "ListResourceEvaluationsRequestRequestTypeDef",
     "DescribeConfigurationRecordersResponseTypeDef",
+    "ConfigurationRecorderUnionTypeDef",
     "PutConfigurationRecorderRequestRequestTypeDef",
     "DescribeRemediationConfigurationsResponseTypeDef",
     "FailedRemediationBatchTypeDef",
-    "PutRemediationConfigurationsRequestRequestTypeDef",
+    "RemediationConfigurationUnionTypeDef",
     "DescribeConfigRulesResponseTypeDef",
+    "ConfigRuleUnionTypeDef",
     "PutConfigRuleRequestRequestTypeDef",
     "PutRemediationConfigurationsResponseTypeDef",
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+)
+
+_RequiredAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredAccountAggregationSourceOutputTypeDef",
+    {
+        "AccountIds": List[str],
+    },
+)
+_OptionalAccountAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalAccountAggregationSourceOutputTypeDef",
+    {
+        "AllAwsRegions": bool,
+        "AwsRegions": List[str],
+    },
+    total=False,
 )
 
+class AccountAggregationSourceOutputTypeDef(
+    _RequiredAccountAggregationSourceOutputTypeDef, _OptionalAccountAggregationSourceOutputTypeDef
+):
+    pass
+
 _RequiredAccountAggregationSourceTypeDef = TypedDict(
     "_RequiredAccountAggregationSourceTypeDef",
     {
-        "AccountIds": List[str],
+        "AccountIds": Sequence[str],
     },
 )
 _OptionalAccountAggregationSourceTypeDef = TypedDict(
     "_OptionalAccountAggregationSourceTypeDef",
     {
         "AllAwsRegions": bool,
-        "AwsRegions": List[str],
+        "AwsRegions": Sequence[str],
     },
     total=False,
 )
 
 class AccountAggregationSourceTypeDef(
     _RequiredAccountAggregationSourceTypeDef, _OptionalAccountAggregationSourceTypeDef
 ):
@@ -480,14 +523,25 @@
         "resourceCreationTime": datetime,
         "configuration": str,
         "supplementaryConfiguration": Dict[str, str],
     },
     total=False,
 )
 
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
 ResourceKeyTypeDef = TypedDict(
     "ResourceKeyTypeDef",
     {
         "resourceType": ResourceTypeType,
         "resourceId": str,
     },
 )
@@ -560,18 +614,29 @@
     "EvaluationModeConfigurationTypeDef",
     {
         "Mode": EvaluationModeType,
     },
     total=False,
 )
 
+ScopeOutputTypeDef = TypedDict(
+    "ScopeOutputTypeDef",
+    {
+        "ComplianceResourceTypes": List[str],
+        "TagKey": str,
+        "TagValue": str,
+        "ComplianceResourceId": str,
+    },
+    total=False,
+)
+
 ScopeTypeDef = TypedDict(
     "ScopeTypeDef",
     {
-        "ComplianceResourceTypes": List[str],
+        "ComplianceResourceTypes": Sequence[str],
         "TagKey": str,
         "TagValue": str,
         "ComplianceResourceId": str,
     },
     total=False,
 )
 
@@ -590,31 +655,32 @@
         "lastErrorCode": str,
         "lastErrorMessage": str,
         "lastStatusChangeTime": datetime,
     },
     total=False,
 )
 
-_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
-    "_RequiredOrganizationAggregationSourceTypeDef",
+_RequiredOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceOutputTypeDef",
     {
         "RoleArn": str,
     },
 )
-_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
-    "_OptionalOrganizationAggregationSourceTypeDef",
+_OptionalOrganizationAggregationSourceOutputTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceOutputTypeDef",
     {
         "AwsRegions": List[str],
         "AllAwsRegions": bool,
     },
     total=False,
 )
 
-class OrganizationAggregationSourceTypeDef(
-    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+class OrganizationAggregationSourceOutputTypeDef(
+    _RequiredOrganizationAggregationSourceOutputTypeDef,
+    _OptionalOrganizationAggregationSourceOutputTypeDef,
 ):
     pass
 
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "resourceType": ResourceTypeType,
@@ -893,93 +959,55 @@
 DeliverConfigSnapshotRequestRequestTypeDef = TypedDict(
     "DeliverConfigSnapshotRequestRequestTypeDef",
     {
         "deliveryChannelName": str,
     },
 )
 
-DeliverConfigSnapshotResponseTypeDef = TypedDict(
-    "DeliverConfigSnapshotResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "configSnapshotId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
-)
-
-DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
-    TypedDict(
-        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
+    total=False,
 )
 
 DescribeAggregationAuthorizationsRequestRequestTypeDef = TypedDict(
     "DescribeAggregationAuthorizationsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
-    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByConfigRuleRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
-    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeComplianceByResourceRequestRequestTypeDef = TypedDict(
     "DescribeComplianceByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
-    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
-    {
-        "ConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigRuleEvaluationStatusRequestRequestTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusRequestRequestTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -990,35 +1018,14 @@
     "DescribeConfigRulesFiltersTypeDef",
     {
         "EvaluationMode": EvaluationModeType,
     },
     total=False,
 )
 
-_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
-    {
-        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
-    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef = TypedDict(
@@ -1033,23 +1040,14 @@
 
 class DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef(
     _RequiredDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
     _OptionalDescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
 ):
     pass
 
-DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
-    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
-    {
-        "ConfigurationAggregatorNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConfigurationAggregatorsRequestRequestTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsRequestRequestTypeDef",
     {
         "ConfigurationAggregatorNames": Sequence[str],
         "NextToken": str,
         "Limit": int,
     },
@@ -1068,42 +1066,24 @@
     "DescribeConfigurationRecordersRequestRequestTypeDef",
     {
         "ConfigurationRecorderNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
-    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePackStatusRequestRequestTypeDef = TypedDict(
     "DescribeConformancePackStatusRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeConformancePacksRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1122,23 +1102,14 @@
     "DescribeDeliveryChannelsRequestRequestTypeDef",
     {
         "DeliveryChannelNames": Sequence[str],
     },
     total=False,
 )
 
-DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1163,42 +1134,24 @@
 )
 
 class OrganizationConfigRuleStatusTypeDef(
     _RequiredOrganizationConfigRuleStatusTypeDef, _OptionalOrganizationConfigRuleStatusTypeDef
 ):
     pass
 
-DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
-    {
-        "OrganizationConfigRuleNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesRequestRequestTypeDef",
     {
         "OrganizationConfigRuleNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePackStatusesRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
@@ -1224,41 +1177,24 @@
 
 class OrganizationConformancePackStatusTypeDef(
     _RequiredOrganizationConformancePackStatusTypeDef,
     _OptionalOrganizationConformancePackStatusTypeDef,
 ):
     pass
 
-DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
-    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
-    {
-        "OrganizationConformancePackNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeOrganizationConformancePacksRequestRequestTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksRequestRequestTypeDef",
     {
         "OrganizationConformancePackNames": Sequence[str],
         "Limit": int,
         "NextToken": str,
     },
     total=False,
 )
 
-DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
-    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribePendingAggregationRequestsRequestRequestTypeDef = TypedDict(
     "DescribePendingAggregationRequestsRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
     },
     total=False,
@@ -1298,23 +1234,14 @@
 )
 
 class RemediationExceptionTypeDef(
     _RequiredRemediationExceptionTypeDef, _OptionalRemediationExceptionTypeDef
 ):
     pass
 
-DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
-    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
-    {
-        "RetentionConfigurationNames": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeRetentionConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeRetentionConfigurationsRequestRequestTypeDef",
     {
         "RetentionConfigurationNames": Sequence[str],
         "NextToken": str,
     },
     total=False,
@@ -1324,29 +1251,42 @@
     "RetentionConfigurationTypeDef",
     {
         "Name": str,
         "RetentionPeriodInDays": int,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+EvaluationContextTypeDef = TypedDict(
+    "EvaluationContextTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "EvaluationContextIdentifier": str,
     },
+    total=False,
 )
 
-EvaluationContextTypeDef = TypedDict(
-    "EvaluationContextTypeDef",
+_RequiredEvaluationOutputTypeDef = TypedDict(
+    "_RequiredEvaluationOutputTypeDef",
     {
-        "EvaluationContextIdentifier": str,
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": datetime,
+    },
+)
+_OptionalEvaluationOutputTypeDef = TypedDict(
+    "_OptionalEvaluationOutputTypeDef",
+    {
+        "Annotation": str,
     },
     total=False,
 )
 
+class EvaluationOutputTypeDef(_RequiredEvaluationOutputTypeDef, _OptionalEvaluationOutputTypeDef):
+    pass
+
 EvaluationResultQualifierTypeDef = TypedDict(
     "EvaluationResultQualifierTypeDef",
     {
         "ConfigRuleName": str,
         "ResourceType": str,
         "ResourceId": str,
         "EvaluationMode": EvaluationModeType,
@@ -1367,105 +1307,48 @@
     },
     total=False,
 )
 
 class EvaluationStatusTypeDef(_RequiredEvaluationStatusTypeDef, _OptionalEvaluationStatusTypeDef):
     pass
 
-_RequiredEvaluationTypeDef = TypedDict(
-    "_RequiredEvaluationTypeDef",
+TimestampTypeDef = Union[datetime, str]
+ExclusionByResourceTypesOutputTypeDef = TypedDict(
+    "ExclusionByResourceTypesOutputTypeDef",
     {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalEvaluationTypeDef = TypedDict(
-    "_OptionalEvaluationTypeDef",
-    {
-        "Annotation": str,
+        "resourceTypes": List[ResourceTypeType],
     },
     total=False,
 )
 
-class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
-    pass
-
 ExclusionByResourceTypesTypeDef = TypedDict(
     "ExclusionByResourceTypesTypeDef",
     {
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
     },
     total=False,
 )
 
 SsmControlsTypeDef = TypedDict(
     "SsmControlsTypeDef",
     {
         "ConcurrentExecutionRatePercentage": int,
         "ErrorPercentage": int,
     },
     total=False,
 )
 
-_RequiredExternalEvaluationTypeDef = TypedDict(
-    "_RequiredExternalEvaluationTypeDef",
-    {
-        "ComplianceResourceType": str,
-        "ComplianceResourceId": str,
-        "ComplianceType": ComplianceTypeType,
-        "OrderingTimestamp": Union[datetime, str],
-    },
-)
-_OptionalExternalEvaluationTypeDef = TypedDict(
-    "_OptionalExternalEvaluationTypeDef",
-    {
-        "Annotation": str,
-    },
-    total=False,
-)
-
-class ExternalEvaluationTypeDef(
-    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
-):
-    pass
-
 FieldInfoTypeDef = TypedDict(
     "FieldInfoTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-        "ConfigRuleName": str,
-        "AccountId": str,
-        "AwsRegion": str,
-    },
-)
-_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceType": ComplianceTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
 _RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigRuleName": str,
         "AccountId": str,
         "AwsRegion": str,
@@ -1501,35 +1384,14 @@
     "GroupedResourceCountTypeDef",
     {
         "GroupName": str,
         "ResourceCount": int,
     },
 )
 
-_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ConfigRuleName": str,
-    },
-)
-_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
-    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
-    {
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
-    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
-):
-    pass
-
 _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
 _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef = TypedDict(
@@ -1544,26 +1406,14 @@
 
 class GetComplianceDetailsByConfigRuleRequestRequestTypeDef(
     _RequiredGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
     _OptionalGetComplianceDetailsByConfigRuleRequestRequestTypeDef,
 ):
     pass
 
-GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
-    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
-    {
-        "ResourceType": str,
-        "ResourceId": str,
-        "ComplianceTypes": Sequence[ComplianceTypeType],
-        "ResourceEvaluationId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetComplianceDetailsByResourceRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailsByResourceRequestRequestTypeDef",
     {
         "ResourceType": str,
         "ResourceId": str,
         "ComplianceTypes": Sequence[ComplianceTypeType],
         "NextToken": str,
@@ -1576,34 +1426,14 @@
     "GetComplianceSummaryByResourceTypeRequestRequestTypeDef",
     {
         "ResourceTypes": Sequence[str],
     },
     total=False,
 )
 
-_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "ConformancePackNames": Sequence[str],
-    },
-)
-_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
-    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
-    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
-):
-    pass
-
 _RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
     "_RequiredGetConformancePackComplianceSummaryRequestRequestTypeDef",
     {
         "ConformancePackNames": Sequence[str],
     },
 )
 _OptionalGetConformancePackComplianceSummaryRequestRequestTypeDef = TypedDict(
@@ -1625,22 +1455,14 @@
     "GetCustomRulePolicyRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
     total=False,
 )
 
-GetCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredResourceCountsRequestRequestTypeDef = TypedDict(
     "GetDiscoveredResourceCountsRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[str],
         "limit": int,
         "nextToken": str,
     },
@@ -1724,71 +1546,14 @@
 GetOrganizationCustomRulePolicyRequestRequestTypeDef = TypedDict(
     "GetOrganizationCustomRulePolicyRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 
-GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
-    "GetOrganizationCustomRulePolicyResponseTypeDef",
-    {
-        "PolicyText": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
-    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-):
-    pass
-
-_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-        "resourceId": str,
-    },
-)
-_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
-    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
-    {
-        "laterTime": Union[datetime, str],
-        "earlierTime": Union[datetime, str],
-        "chronologicalOrder": ChronologicalOrderType,
-        "limit": int,
-        "nextToken": str,
-    },
-    total=False,
-)
-
-class GetResourceConfigHistoryRequestRequestTypeDef(
-    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
-    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
-):
-    pass
-
 GetResourceEvaluationSummaryRequestRequestTypeDef = TypedDict(
     "GetResourceEvaluationSummaryRequestRequestTypeDef",
     {
         "ResourceEvaluationId": str,
     },
 )
 
@@ -1845,37 +1610,14 @@
         "ResourceId": str,
         "ResourceName": str,
         "Region": str,
     },
     total=False,
 )
 
-_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceType": ResourceTypeType,
-    },
-)
-_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
-    {
-        "resourceIds": Sequence[str],
-        "resourceName": str,
-        "includeDeletedResources": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
-    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
     },
 )
 _OptionalListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
@@ -1943,34 +1685,14 @@
 )
 
 class StoredQueryMetadataTypeDef(
     _RequiredStoredQueryMetadataTypeDef, _OptionalStoredQueryMetadataTypeDef
 ):
     pass
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
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
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -1993,14 +1715,34 @@
     {
         "Key": str,
         "Value": str,
     },
     total=False,
 )
 
+_RequiredOrganizationAggregationSourceTypeDef = TypedDict(
+    "_RequiredOrganizationAggregationSourceTypeDef",
+    {
+        "RoleArn": str,
+    },
+)
+_OptionalOrganizationAggregationSourceTypeDef = TypedDict(
+    "_OptionalOrganizationAggregationSourceTypeDef",
+    {
+        "AwsRegions": Sequence[str],
+        "AllAwsRegions": bool,
+    },
+    total=False,
+)
+
+class OrganizationAggregationSourceTypeDef(
+    _RequiredOrganizationAggregationSourceTypeDef, _OptionalOrganizationAggregationSourceTypeDef
+):
+    pass
+
 OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef = TypedDict(
     "OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef",
     {
         "Description": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeNoSNType],
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
@@ -2010,62 +1752,64 @@
         "TagValueScope": str,
         "PolicyRuntime": str,
         "DebugLogDeliveryAccounts": List[str],
     },
     total=False,
 )
 
-_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationCustomRuleMetadataTypeDef",
+_RequiredOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "LambdaFunctionArn": str,
         "OrganizationConfigRuleTriggerTypes": List[OrganizationConfigRuleTriggerTypeType],
     },
 )
-_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationCustomRuleMetadataTypeDef",
+_OptionalOrganizationCustomRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-class OrganizationCustomRuleMetadataTypeDef(
-    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+class OrganizationCustomRuleMetadataOutputTypeDef(
+    _RequiredOrganizationCustomRuleMetadataOutputTypeDef,
+    _OptionalOrganizationCustomRuleMetadataOutputTypeDef,
 ):
     pass
 
-_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_RequiredOrganizationManagedRuleMetadataTypeDef",
+_RequiredOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "RuleIdentifier": str,
     },
 )
-_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
-    "_OptionalOrganizationManagedRuleMetadataTypeDef",
+_OptionalOrganizationManagedRuleMetadataOutputTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataOutputTypeDef",
     {
         "Description": str,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ResourceTypesScope": List[str],
         "ResourceIdScope": str,
         "TagKeyScope": str,
         "TagValueScope": str,
     },
     total=False,
 )
 
-class OrganizationManagedRuleMetadataTypeDef(
-    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+class OrganizationManagedRuleMetadataOutputTypeDef(
+    _RequiredOrganizationManagedRuleMetadataOutputTypeDef,
+    _OptionalOrganizationManagedRuleMetadataOutputTypeDef,
 ):
     pass
 
 _RequiredOrganizationCustomPolicyRuleMetadataTypeDef = TypedDict(
     "_RequiredOrganizationCustomPolicyRuleMetadataTypeDef",
     {
         "PolicyRuntime": str,
@@ -2090,48 +1834,65 @@
 
 class OrganizationCustomPolicyRuleMetadataTypeDef(
     _RequiredOrganizationCustomPolicyRuleMetadataTypeDef,
     _OptionalOrganizationCustomPolicyRuleMetadataTypeDef,
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationCustomRuleMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "LambdaFunctionArn": str,
+        "OrganizationConfigRuleTriggerTypes": Sequence[OrganizationConfigRuleTriggerTypeType],
     },
-    total=False,
 )
-
-PutConformancePackResponseTypeDef = TypedDict(
-    "PutConformancePackResponseTypeDef",
+_OptionalOrganizationCustomRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationCustomRuleMetadataTypeDef",
     {
-        "ConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
     },
+    total=False,
 )
 
-PutOrganizationConfigRuleResponseTypeDef = TypedDict(
-    "PutOrganizationConfigRuleResponseTypeDef",
+class OrganizationCustomRuleMetadataTypeDef(
+    _RequiredOrganizationCustomRuleMetadataTypeDef, _OptionalOrganizationCustomRuleMetadataTypeDef
+):
+    pass
+
+_RequiredOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_RequiredOrganizationManagedRuleMetadataTypeDef",
     {
-        "OrganizationConfigRuleArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RuleIdentifier": str,
     },
 )
-
-PutOrganizationConformancePackResponseTypeDef = TypedDict(
-    "PutOrganizationConformancePackResponseTypeDef",
+_OptionalOrganizationManagedRuleMetadataTypeDef = TypedDict(
+    "_OptionalOrganizationManagedRuleMetadataTypeDef",
     {
-        "OrganizationConformancePackArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Description": str,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ResourceTypesScope": Sequence[str],
+        "ResourceIdScope": str,
+        "TagKeyScope": str,
+        "TagValueScope": str,
     },
+    total=False,
 )
 
+class OrganizationManagedRuleMetadataTypeDef(
+    _RequiredOrganizationManagedRuleMetadataTypeDef, _OptionalOrganizationManagedRuleMetadataTypeDef
+):
+    pass
+
 _RequiredPutResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourceConfigRequestRequestTypeDef",
     {
         "ResourceType": str,
         "SchemaVersionId": str,
         "ResourceId": str,
         "Configuration": str,
@@ -2154,22 +1915,14 @@
 PutRetentionConfigurationRequestRequestTypeDef = TypedDict(
     "PutRetentionConfigurationRequestRequestTypeDef",
     {
         "RetentionPeriodInDays": int,
     },
 )
 
-PutStoredQueryResponseTypeDef = TypedDict(
-    "PutStoredQueryResponseTypeDef",
-    {
-        "QueryArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RecordingStrategyTypeDef = TypedDict(
     "RecordingStrategyTypeDef",
     {
         "useOnly": RecordingStrategyTypeType,
     },
     total=False,
 )
@@ -2189,38 +1942,25 @@
 ResourceValueTypeDef = TypedDict(
     "ResourceValueTypeDef",
     {
         "Value": Literal["RESOURCE_ID"],
     },
 )
 
-StaticValueTypeDef = TypedDict(
-    "StaticValueTypeDef",
+StaticValueOutputTypeDef = TypedDict(
+    "StaticValueOutputTypeDef",
     {
         "Values": List[str],
     },
 )
 
-TimeWindowTypeDef = TypedDict(
-    "TimeWindowTypeDef",
-    {
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-    },
-    total=False,
-)
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+StaticValueTypeDef = TypedDict(
+    "StaticValueTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Values": Sequence[str],
     },
 )
 
 _RequiredSelectAggregateResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectAggregateResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
@@ -2239,40 +1979,14 @@
 
 class SelectAggregateResourceConfigRequestRequestTypeDef(
     _RequiredSelectAggregateResourceConfigRequestRequestTypeDef,
     _OptionalSelectAggregateResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "Expression": str,
-            "ConfigurationAggregatorName": str,
-        },
-    )
-)
-_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
-    TypedDict(
-        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
-        {
-            "MaxResults": int,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
-    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
-):
-    pass
-
 _RequiredSelectResourceConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSelectResourceConfigRequestRequestTypeDef",
     {
         "Expression": str,
     },
 )
 _OptionalSelectResourceConfigRequestRequestTypeDef = TypedDict(
@@ -2286,34 +2000,14 @@
 
 class SelectResourceConfigRequestRequestTypeDef(
     _RequiredSelectResourceConfigRequestRequestTypeDef,
     _OptionalSelectResourceConfigRequestRequestTypeDef,
 ):
     pass
 
-_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "Expression": str,
-    },
-)
-_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
-    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
-    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
-):
-    pass
-
 SourceDetailTypeDef = TypedDict(
     "SourceDetailTypeDef",
     {
         "EventSource": Literal["aws.config"],
         "MessageType": MessageTypeType,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
     },
@@ -2331,22 +2025,14 @@
 StartConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StartConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
-StartResourceEvaluationResponseTypeDef = TypedDict(
-    "StartResourceEvaluationResponseTypeDef",
-    {
-        "ResourceEvaluationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "StopConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorderName": str,
     },
 )
 
@@ -2354,14 +2040,17 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
+AccountAggregationSourceUnionTypeDef = Union[
+    AccountAggregationSourceTypeDef, AccountAggregationSourceOutputTypeDef
+]
 AggregateComplianceByConformancePackTypeDef = TypedDict(
     "AggregateComplianceByConformancePackTypeDef",
     {
         "ConformancePackName": str,
         "Compliance": AggregateConformancePackComplianceTypeDef,
         "AccountId": str,
         "AwsRegion": str,
@@ -2374,35 +2063,14 @@
     {
         "ComplianceSummary": AggregateConformancePackComplianceCountTypeDef,
         "GroupName": str,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
-    {
-        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConformancePacksRequestRequestTypeDef = TypedDict(
@@ -2456,94 +2124,144 @@
     "GetAggregateResourceConfigRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceIdentifier": AggregateResourceIdentifierTypeDef,
     },
 )
 
-ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
-    "ListAggregateDiscoveredResourcesResponseTypeDef",
+BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetAggregateResourceConfigResponseTypeDef",
     {
-        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeliverConfigSnapshotResponseTypeDef = TypedDict(
+    "DeliverConfigSnapshotResponseTypeDef",
+    {
+        "configSnapshotId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
+    "DescribeAggregationAuthorizationsResponseTypeDef",
+    {
+        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationAggregatorSourcesStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorSourcesStatusResponseTypeDef",
     {
         "AggregatedSourceStatusList": List[AggregatedSourceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeAggregationAuthorizationsResponseTypeDef = TypedDict(
-    "DescribeAggregationAuthorizationsResponseTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "AggregationAuthorizations": List[AggregationAuthorizationTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetOrganizationCustomRulePolicyResponseTypeDef = TypedDict(
+    "GetOrganizationCustomRulePolicyResponseTypeDef",
+    {
+        "PolicyText": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAggregateDiscoveredResourcesResponseTypeDef = TypedDict(
+    "ListAggregateDiscoveredResourcesResponseTypeDef",
+    {
+        "ResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAggregationAuthorizationResponseTypeDef = TypedDict(
     "PutAggregationAuthorizationResponseTypeDef",
     {
         "AggregationAuthorization": AggregationAuthorizationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetAggregateResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetAggregateResourceConfigResponseTypeDef",
+PutConformancePackResponseTypeDef = TypedDict(
+    "PutConformancePackResponseTypeDef",
     {
-        "BaseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "UnprocessedResourceIdentifiers": List[AggregateResourceIdentifierTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
-    "BatchGetResourceConfigRequestRequestTypeDef",
+PutOrganizationConfigRuleResponseTypeDef = TypedDict(
+    "PutOrganizationConfigRuleResponseTypeDef",
     {
-        "resourceKeys": Sequence[ResourceKeyTypeDef],
+        "OrganizationConfigRuleArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-BatchGetResourceConfigResponseTypeDef = TypedDict(
-    "BatchGetResourceConfigResponseTypeDef",
+PutOrganizationConformancePackResponseTypeDef = TypedDict(
+    "PutOrganizationConformancePackResponseTypeDef",
     {
-        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
-        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "OrganizationConformancePackArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+PutStoredQueryResponseTypeDef = TypedDict(
+    "PutStoredQueryResponseTypeDef",
     {
-        "ConfigRuleName": str,
+        "QueryArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
-    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
+
+StartResourceEvaluationResponseTypeDef = TypedDict(
+    "StartResourceEvaluationResponseTypeDef",
     {
-        "ResourceKeys": Sequence[ResourceKeyTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "ResourceEvaluationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
-    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
-):
-    pass
+BatchGetResourceConfigRequestRequestTypeDef = TypedDict(
+    "BatchGetResourceConfigRequestRequestTypeDef",
+    {
+        "resourceKeys": Sequence[ResourceKeyTypeDef],
+    },
+)
+
+BatchGetResourceConfigResponseTypeDef = TypedDict(
+    "BatchGetResourceConfigResponseTypeDef",
+    {
+        "baseConfigurationItems": List[BaseConfigurationItemTypeDef],
+        "unprocessedResourceKeys": List[ResourceKeyTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeRemediationExecutionStatusRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
     },
 )
@@ -2572,15 +2290,15 @@
 )
 
 StartRemediationExecutionResponseTypeDef = TypedDict(
     "StartRemediationExecutionResponseTypeDef",
     {
         "FailureMessage": str,
         "FailedItems": List[ResourceKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ComplianceSummaryTypeDef = TypedDict(
     "ComplianceSummaryTypeDef",
     {
         "CompliantResourceCount": ComplianceContributorCountTypeDef,
@@ -2595,35 +2313,14 @@
     {
         "ComplianceType": ComplianceTypeType,
         "ComplianceContributorCount": ComplianceContributorCountTypeDef,
     },
     total=False,
 )
 
-_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
-    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
-    {
-        "Filters": ConfigRuleComplianceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
-    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef",
     {
         "ConfigurationAggregatorName": str,
     },
 )
 _OptionalDescribeAggregateComplianceByConfigRulesRequestRequestTypeDef = TypedDict(
@@ -2666,15 +2363,15 @@
     pass
 
 DescribeConfigRuleEvaluationStatusResponseTypeDef = TypedDict(
     "DescribeConfigRuleEvaluationStatusResponseTypeDef",
     {
         "ConfigRulesEvaluationStatus": List[ConfigRuleEvaluationStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeliveryChannelTypeDef = TypedDict(
     "DeliveryChannelTypeDef",
     {
         "name": str,
@@ -2699,16 +2396,16 @@
 )
 
 ConfigurationAggregatorTypeDef = TypedDict(
     "ConfigurationAggregatorTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ConfigurationAggregatorArn": str,
-        "AccountAggregationSources": List[AccountAggregationSourceTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "AccountAggregationSources": List[AccountAggregationSourceOutputTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceOutputTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "CreatedBy": str,
     },
     total=False,
 )
 
@@ -2737,15 +2434,15 @@
     total=False,
 )
 
 DescribeConfigurationRecorderStatusResponseTypeDef = TypedDict(
     "DescribeConfigurationRecorderStatusResponseTypeDef",
     {
         "ConfigurationRecordersStatus": List[ConfigurationRecorderStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeConformancePackComplianceRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConformancePackComplianceRequestRequestTypeDef",
     {
         "ConformancePackName": str,
@@ -2768,15 +2465,15 @@
     pass
 
 ListConformancePackComplianceScoresResponseTypeDef = TypedDict(
     "ListConformancePackComplianceScoresResponseTypeDef",
     {
         "NextToken": str,
         "ConformancePackComplianceScores": List[ConformancePackComplianceScoreTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConformancePackComplianceScoresRequestRequestTypeDef = TypedDict(
     "ListConformancePackComplianceScoresRequestRequestTypeDef",
     {
         "Filters": ConformancePackComplianceScoresFiltersTypeDef,
@@ -2789,15 +2486,15 @@
 )
 
 GetConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetConformancePackComplianceSummaryResponseTypeDef",
     {
         "ConformancePackComplianceSummaryList": List[ConformancePackComplianceSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredOrganizationConformancePackTypeDef = TypedDict(
     "_RequiredOrganizationConformancePackTypeDef",
     {
         "OrganizationConformancePackName": str,
@@ -2921,24 +2618,24 @@
 
 DescribeConformancePackComplianceResponseTypeDef = TypedDict(
     "DescribeConformancePackComplianceResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleComplianceList": List[ConformancePackRuleComplianceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePackStatusResponseTypeDef = TypedDict(
     "DescribeConformancePackStatusResponseTypeDef",
     {
         "ConformancePackStatusDetails": List[ConformancePackStatusDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRemediationExceptionsRequestRequestTypeDef = TypedDict(
     "DeleteRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
@@ -2973,42 +2670,390 @@
     {
         "FailureMessage": str,
         "FailedItems": List[RemediationExceptionResourceKeyTypeDef],
     },
     total=False,
 )
 
-_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
+_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef",
+    {
+        "Filters": ConfigRuleComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+):
+    pass
+
+_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef = TypedDict(
+    "_OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef",
+    {
+        "Filters": AggregateConformancePackComplianceFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef(
+    _RequiredDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    _OptionalDescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+):
+    pass
+
+DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef = (
+    TypedDict(
+        "DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef = TypedDict(
+    "DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef = TypedDict(
+    "DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef = TypedDict(
+    "DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef",
+    {
+        "ConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef",
+    {
+        "UpdateStatus": Sequence[AggregatedSourceStatusTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef(
+    _RequiredDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    _OptionalDescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+):
+    pass
+
+DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef = TypedDict(
+    "DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef",
+    {
+        "ConfigurationAggregatorNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef = TypedDict(
+    "DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef",
+    {
+        "OrganizationConfigRuleNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef = TypedDict(
+    "DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef",
+    {
+        "OrganizationConformancePackNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef = TypedDict(
+    "DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     {
         "ConfigRuleName": str,
-        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
     },
 )
-_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
+_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef = TypedDict(
+    "_OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef",
     {
-        "Message": str,
-        "ExpirationTime": Union[datetime, str],
+        "ResourceKeys": Sequence[ResourceKeyTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PutRemediationExceptionsRequestRequestTypeDef(
-    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
-    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
+class DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef(
+    _RequiredDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    _OptionalDescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+):
+    pass
+
+DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef = TypedDict(
+    "DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef",
+    {
+        "RetentionConfigurationNames": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+        "ConfigRuleName": str,
+        "AccountId": str,
+        "AwsRegion": str,
+    },
+)
+_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceType": ComplianceTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ConfigRuleName": str,
+    },
+)
+_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef = TypedDict(
+    "_OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef",
+    {
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef(
+    _RequiredGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    _OptionalGetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+):
+    pass
+
+GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef = TypedDict(
+    "GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef",
+    {
+        "ResourceType": str,
+        "ResourceId": str,
+        "ComplianceTypes": Sequence[ComplianceTypeType],
+        "ResourceEvaluationId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "ConformancePackNames": Sequence[str],
+    },
+)
+_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef = TypedDict(
+    "_OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef(
+    _RequiredGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    _OptionalGetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+):
+    pass
+
+_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceType": ResourceTypeType,
+    },
+)
+_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef",
+    {
+        "resourceIds": Sequence[str],
+        "resourceName": str,
+        "includeDeletedResources": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef(
+    _RequiredListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    _OptionalListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
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
+
+_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "Expression": str,
+            "ConfigurationAggregatorName": str,
+        },
+    )
+)
+_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef = (
+    TypedDict(
+        "_OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef",
+        {
+            "MaxResults": int,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef(
+    _RequiredSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    _OptionalSelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+):
+    pass
+
+_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "Expression": str,
+    },
+)
+_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef = TypedDict(
+    "_OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef(
+    _RequiredSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
+    _OptionalSelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
 ):
     pass
 
 DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef = TypedDict(
     "DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef",
     {
         "ConfigRuleNames": Sequence[str],
         "Filters": DescribeConfigRulesFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 DescribeConfigRulesRequestRequestTypeDef = TypedDict(
     "DescribeConfigRulesRequestRequestTypeDef",
     {
@@ -3020,42 +3065,42 @@
 )
 
 DescribeOrganizationConfigRuleStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRuleStatusesResponseTypeDef",
     {
         "OrganizationConfigRuleStatuses": List[OrganizationConfigRuleStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePackStatusesResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePackStatusesResponseTypeDef",
     {
         "OrganizationConformancePackStatuses": List[OrganizationConformancePackStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribePendingAggregationRequestsResponseTypeDef = TypedDict(
     "DescribePendingAggregationRequestsResponseTypeDef",
     {
         "PendingAggregationRequests": List[PendingAggregationRequestTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRemediationExceptionsResponseTypeDef = TypedDict(
     "DescribeRemediationExceptionsResponseTypeDef",
     {
         "RemediationExceptions": List[RemediationExceptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationExceptionBatchTypeDef = TypedDict(
     "FailedRemediationExceptionBatchTypeDef",
     {
         "FailureMessage": str,
@@ -3065,78 +3110,172 @@
 )
 
 DescribeRetentionConfigurationsResponseTypeDef = TypedDict(
     "DescribeRetentionConfigurationsResponseTypeDef",
     {
         "RetentionConfigurations": List[RetentionConfigurationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRetentionConfigurationResponseTypeDef = TypedDict(
     "PutRetentionConfigurationResponseTypeDef",
     {
         "RetentionConfiguration": RetentionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutEvaluationsResponseTypeDef = TypedDict(
+    "PutEvaluationsResponseTypeDef",
+    {
+        "FailedEvaluations": List[EvaluationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EvaluationResultIdentifierTypeDef = TypedDict(
     "EvaluationResultIdentifierTypeDef",
     {
         "EvaluationResultQualifier": EvaluationResultQualifierTypeDef,
         "OrderingTimestamp": datetime,
         "ResourceEvaluationId": str,
     },
     total=False,
 )
 
-_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_RequiredPutEvaluationsRequestRequestTypeDef",
+_RequiredEvaluationTypeDef = TypedDict(
+    "_RequiredEvaluationTypeDef",
     {
-        "ResultToken": str,
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
     },
 )
-_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
-    "_OptionalPutEvaluationsRequestRequestTypeDef",
+_OptionalEvaluationTypeDef = TypedDict(
+    "_OptionalEvaluationTypeDef",
     {
-        "Evaluations": Sequence[EvaluationTypeDef],
-        "TestMode": bool,
+        "Annotation": str,
     },
     total=False,
 )
 
-class PutEvaluationsRequestRequestTypeDef(
-    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+class EvaluationTypeDef(_RequiredEvaluationTypeDef, _OptionalEvaluationTypeDef):
+    pass
+
+_RequiredExternalEvaluationTypeDef = TypedDict(
+    "_RequiredExternalEvaluationTypeDef",
+    {
+        "ComplianceResourceType": str,
+        "ComplianceResourceId": str,
+        "ComplianceType": ComplianceTypeType,
+        "OrderingTimestamp": TimestampTypeDef,
+    },
+)
+_OptionalExternalEvaluationTypeDef = TypedDict(
+    "_OptionalExternalEvaluationTypeDef",
+    {
+        "Annotation": str,
+    },
+    total=False,
+)
+
+class ExternalEvaluationTypeDef(
+    _RequiredExternalEvaluationTypeDef, _OptionalExternalEvaluationTypeDef
 ):
     pass
 
-PutEvaluationsResponseTypeDef = TypedDict(
-    "PutEvaluationsResponseTypeDef",
+_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
     {
-        "FailedEvaluations": List[EvaluationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
     },
 )
+_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ExecutionControlsTypeDef = TypedDict(
-    "ExecutionControlsTypeDef",
+class GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef(
+    _RequiredGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    _OptionalGetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_RequiredGetResourceConfigHistoryRequestRequestTypeDef",
     {
-        "SsmControls": SsmControlsTypeDef,
+        "resourceType": ResourceTypeType,
+        "resourceId": str,
+    },
+)
+_OptionalGetResourceConfigHistoryRequestRequestTypeDef = TypedDict(
+    "_OptionalGetResourceConfigHistoryRequestRequestTypeDef",
+    {
+        "laterTime": TimestampTypeDef,
+        "earlierTime": TimestampTypeDef,
+        "chronologicalOrder": ChronologicalOrderType,
+        "limit": int,
+        "nextToken": str,
     },
     total=False,
 )
 
-PutExternalEvaluationRequestRequestTypeDef = TypedDict(
-    "PutExternalEvaluationRequestRequestTypeDef",
+class GetResourceConfigHistoryRequestRequestTypeDef(
+    _RequiredGetResourceConfigHistoryRequestRequestTypeDef,
+    _OptionalGetResourceConfigHistoryRequestRequestTypeDef,
+):
+    pass
+
+_RequiredPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutRemediationExceptionsRequestRequestTypeDef",
     {
         "ConfigRuleName": str,
-        "ExternalEvaluation": ExternalEvaluationTypeDef,
+        "ResourceKeys": Sequence[RemediationExceptionResourceKeyTypeDef],
+    },
+)
+_OptionalPutRemediationExceptionsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutRemediationExceptionsRequestRequestTypeDef",
+    {
+        "Message": str,
+        "ExpirationTime": TimestampTypeDef,
+    },
+    total=False,
+)
+
+class PutRemediationExceptionsRequestRequestTypeDef(
+    _RequiredPutRemediationExceptionsRequestRequestTypeDef,
+    _OptionalPutRemediationExceptionsRequestRequestTypeDef,
+):
+    pass
+
+TimeWindowTypeDef = TypedDict(
+    "TimeWindowTypeDef",
+    {
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
     },
+    total=False,
+)
+
+ExecutionControlsTypeDef = TypedDict(
+    "ExecutionControlsTypeDef",
+    {
+        "SsmControls": SsmControlsTypeDef,
+    },
+    total=False,
 )
 
 QueryInfoTypeDef = TypedDict(
     "QueryInfoTypeDef",
     {
         "SelectFields": List[FieldInfoTypeDef],
     },
@@ -3169,39 +3308,39 @@
 GetAggregateDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetAggregateDiscoveredResourceCountsResponseTypeDef",
     {
         "TotalDiscoveredResources": int,
         "GroupByKey": str,
         "GroupedResourceCounts": List[GroupedResourceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDiscoveredResourceCountsResponseTypeDef = TypedDict(
     "GetDiscoveredResourceCountsResponseTypeDef",
     {
         "totalDiscoveredResources": int,
         "resourceCounts": List[ResourceCountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef",
     {
         "Filters": StatusDetailFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
@@ -3231,29 +3370,29 @@
     pass
 
 GetOrganizationConfigRuleDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConfigRuleDetailedStatusResponseTypeDef",
     {
         "OrganizationConfigRuleDetailedStatus": List[MemberAccountStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "OrganizationConformancePackName": str,
     },
 )
 _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef = TypedDict(
     "_OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef",
     {
         "Filters": OrganizationResourceDetailedStatusFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class GetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef(
     _RequiredGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
     _OptionalGetOrganizationConformancePackDetailedStatusRequestGetOrganizationConformancePackDetailedStatusPaginateTypeDef,
@@ -3285,29 +3424,29 @@
 GetOrganizationConformancePackDetailedStatusResponseTypeDef = TypedDict(
     "GetOrganizationConformancePackDetailedStatusResponseTypeDef",
     {
         "OrganizationConformancePackDetailedStatuses": List[
             OrganizationConformancePackDetailedStatusTypeDef
         ],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceEvaluationSummaryResponseTypeDef = TypedDict(
     "GetResourceEvaluationSummaryResponseTypeDef",
     {
         "ResourceEvaluationId": str,
         "EvaluationMode": EvaluationModeType,
         "EvaluationStatus": EvaluationStatusTypeDef,
         "EvaluationStartTimestamp": datetime,
         "Compliance": ComplianceTypeType,
         "EvaluationContext": EvaluationContextTypeDef,
         "ResourceDetails": ResourceDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartResourceEvaluationRequestRequestTypeDef = TypedDict(
     "_RequiredStartResourceEvaluationRequestRequestTypeDef",
     {
         "ResourceDetails": ResourceDetailsTypeDef,
@@ -3330,30 +3469,30 @@
 ):
     pass
 
 GetStoredQueryResponseTypeDef = TypedDict(
     "GetStoredQueryResponseTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "ConfigurationAggregatorName": str,
         "ResourceType": ResourceTypeType,
     },
 )
 _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef = TypedDict(
     "_OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef",
     {
         "Filters": ResourceFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef(
     _RequiredListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     _OptionalListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
@@ -3384,42 +3523,42 @@
     pass
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "resourceIdentifiers": List[ResourceIdentifierTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceEvaluationsResponseTypeDef = TypedDict(
     "ListResourceEvaluationsResponseTypeDef",
     {
         "ResourceEvaluations": List[ResourceEvaluationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStoredQueriesResponseTypeDef = TypedDict(
     "ListStoredQueriesResponseTypeDef",
     {
         "StoredQueryMetadata": List[StoredQueryMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPutAggregationAuthorizationRequestRequestTypeDef = TypedDict(
     "_RequiredPutAggregationAuthorizationRequestRequestTypeDef",
     {
         "AuthorizedAccountId": str,
@@ -3436,36 +3575,14 @@
 
 class PutAggregationAuthorizationRequestRequestTypeDef(
     _RequiredPutAggregationAuthorizationRequestRequestTypeDef,
     _OptionalPutAggregationAuthorizationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "ConfigurationAggregatorName": str,
-    },
-)
-_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
-    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
-    {
-        "AccountAggregationSources": Sequence[AccountAggregationSourceTypeDef],
-        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
-        "Tags": Sequence[TagTypeDef],
-    },
-    total=False,
-)
-
-class PutConfigurationAggregatorRequestRequestTypeDef(
-    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
-    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
-):
-    pass
-
 _RequiredPutStoredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredPutStoredQueryRequestRequestTypeDef",
     {
         "StoredQuery": StoredQueryTypeDef,
     },
 )
 _OptionalPutStoredQueryRequestRequestTypeDef = TypedDict(
@@ -3485,38 +3602,47 @@
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+OrganizationAggregationSourceUnionTypeDef = Union[
+    OrganizationAggregationSourceTypeDef, OrganizationAggregationSourceOutputTypeDef
+]
 _RequiredOrganizationConfigRuleTypeDef = TypedDict(
     "_RequiredOrganizationConfigRuleTypeDef",
     {
         "OrganizationConfigRuleName": str,
         "OrganizationConfigRuleArn": str,
     },
 )
 _OptionalOrganizationConfigRuleTypeDef = TypedDict(
     "_OptionalOrganizationConfigRuleTypeDef",
     {
-        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataTypeDef,
-        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataTypeDef,
+        "OrganizationManagedRuleMetadata": OrganizationManagedRuleMetadataOutputTypeDef,
+        "OrganizationCustomRuleMetadata": OrganizationCustomRuleMetadataOutputTypeDef,
         "ExcludedAccounts": List[str],
         "LastUpdateTime": datetime,
         "OrganizationCustomPolicyRuleMetadata": OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
     },
     total=False,
 )
 
 class OrganizationConfigRuleTypeDef(
     _RequiredOrganizationConfigRuleTypeDef, _OptionalOrganizationConfigRuleTypeDef
 ):
     pass
 
+OrganizationCustomRuleMetadataUnionTypeDef = Union[
+    OrganizationCustomRuleMetadataTypeDef, OrganizationCustomRuleMetadataOutputTypeDef
+]
+OrganizationManagedRuleMetadataUnionTypeDef = Union[
+    OrganizationManagedRuleMetadataTypeDef, OrganizationManagedRuleMetadataOutputTypeDef
+]
 _RequiredPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutOrganizationConfigRuleRequestRequestTypeDef",
     {
         "OrganizationConfigRuleName": str,
     },
 )
 _OptionalPutOrganizationConfigRuleRequestRequestTypeDef = TypedDict(
@@ -3532,20 +3658,32 @@
 
 class PutOrganizationConfigRuleRequestRequestTypeDef(
     _RequiredPutOrganizationConfigRuleRequestRequestTypeDef,
     _OptionalPutOrganizationConfigRuleRequestRequestTypeDef,
 ):
     pass
 
+RecordingGroupOutputTypeDef = TypedDict(
+    "RecordingGroupOutputTypeDef",
+    {
+        "allSupported": bool,
+        "includeGlobalResourceTypes": bool,
+        "resourceTypes": List[ResourceTypeType],
+        "exclusionByResourceTypes": ExclusionByResourceTypesOutputTypeDef,
+        "recordingStrategy": RecordingStrategyTypeDef,
+    },
+    total=False,
+)
+
 RecordingGroupTypeDef = TypedDict(
     "RecordingGroupTypeDef",
     {
         "allSupported": bool,
         "includeGlobalResourceTypes": bool,
-        "resourceTypes": List[ResourceTypeType],
+        "resourceTypes": Sequence[ResourceTypeType],
         "exclusionByResourceTypes": ExclusionByResourceTypesTypeDef,
         "recordingStrategy": RecordingStrategyTypeDef,
     },
     total=False,
 )
 
 RemediationExecutionStatusTypeDef = TypedDict(
@@ -3556,70 +3694,110 @@
         "StepDetails": List[RemediationExecutionStepTypeDef],
         "InvocationTime": datetime,
         "LastUpdatedTime": datetime,
     },
     total=False,
 )
 
+RemediationParameterValueOutputTypeDef = TypedDict(
+    "RemediationParameterValueOutputTypeDef",
+    {
+        "ResourceValue": ResourceValueTypeDef,
+        "StaticValue": StaticValueOutputTypeDef,
+    },
+    total=False,
+)
+
 RemediationParameterValueTypeDef = TypedDict(
     "RemediationParameterValueTypeDef",
     {
         "ResourceValue": ResourceValueTypeDef,
         "StaticValue": StaticValueTypeDef,
     },
     total=False,
 )
 
-ResourceEvaluationFiltersTypeDef = TypedDict(
-    "ResourceEvaluationFiltersTypeDef",
+_RequiredSourceOutputTypeDef = TypedDict(
+    "_RequiredSourceOutputTypeDef",
     {
-        "EvaluationMode": EvaluationModeType,
-        "TimeWindow": TimeWindowTypeDef,
-        "EvaluationContextIdentifier": str,
+        "Owner": OwnerType,
+    },
+)
+_OptionalSourceOutputTypeDef = TypedDict(
+    "_OptionalSourceOutputTypeDef",
+    {
+        "SourceIdentifier": str,
+        "SourceDetails": List[SourceDetailTypeDef],
+        "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
+class SourceOutputTypeDef(_RequiredSourceOutputTypeDef, _OptionalSourceOutputTypeDef):
+    pass
+
 _RequiredSourceTypeDef = TypedDict(
     "_RequiredSourceTypeDef",
     {
         "Owner": OwnerType,
     },
 )
 _OptionalSourceTypeDef = TypedDict(
     "_OptionalSourceTypeDef",
     {
         "SourceIdentifier": str,
-        "SourceDetails": List[SourceDetailTypeDef],
+        "SourceDetails": Sequence[SourceDetailTypeDef],
         "CustomPolicyDetails": CustomPolicyDetailsTypeDef,
     },
     total=False,
 )
 
 class SourceTypeDef(_RequiredSourceTypeDef, _OptionalSourceTypeDef):
     pass
 
+_RequiredPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_RequiredPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "ConfigurationAggregatorName": str,
+    },
+)
+_OptionalPutConfigurationAggregatorRequestRequestTypeDef = TypedDict(
+    "_OptionalPutConfigurationAggregatorRequestRequestTypeDef",
+    {
+        "AccountAggregationSources": Sequence[AccountAggregationSourceUnionTypeDef],
+        "OrganizationAggregationSource": OrganizationAggregationSourceTypeDef,
+        "Tags": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutConfigurationAggregatorRequestRequestTypeDef(
+    _RequiredPutConfigurationAggregatorRequestRequestTypeDef,
+    _OptionalPutConfigurationAggregatorRequestRequestTypeDef,
+):
+    pass
+
 DescribeAggregateComplianceByConformancePacksResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConformancePacksResponseTypeDef",
     {
         "AggregateComplianceByConformancePacks": List[AggregateComplianceByConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateConformancePackComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConformancePackComplianceSummaryResponseTypeDef",
     {
         "AggregateConformancePackComplianceSummaries": List[
             AggregateConformancePackComplianceSummaryTypeDef
         ],
         "GroupByKey": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceCountTypeDef = TypedDict(
     "AggregateComplianceCountTypeDef",
     {
         "GroupName": str,
@@ -3637,15 +3815,15 @@
     total=False,
 )
 
 GetComplianceSummaryByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceSummaryByConfigRuleResponseTypeDef",
     {
         "ComplianceSummary": ComplianceSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateComplianceByConfigRuleTypeDef = TypedDict(
     "AggregateComplianceByConfigRuleTypeDef",
     {
         "ConfigRuleName": str,
@@ -3675,98 +3853,98 @@
     total=False,
 )
 
 DescribeDeliveryChannelsResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelsResponseTypeDef",
     {
         "DeliveryChannels": List[DeliveryChannelTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutDeliveryChannelRequestRequestTypeDef = TypedDict(
     "PutDeliveryChannelRequestRequestTypeDef",
     {
         "DeliveryChannel": DeliveryChannelTypeDef,
     },
 )
 
 DescribeDeliveryChannelStatusResponseTypeDef = TypedDict(
     "DescribeDeliveryChannelStatusResponseTypeDef",
     {
         "DeliveryChannelsStatus": List[DeliveryChannelStatusTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConfigurationAggregatorsResponseTypeDef = TypedDict(
     "DescribeConfigurationAggregatorsResponseTypeDef",
     {
         "ConfigurationAggregators": List[ConfigurationAggregatorTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutConfigurationAggregatorResponseTypeDef = TypedDict(
     "PutConfigurationAggregatorResponseTypeDef",
     {
         "ConfigurationAggregator": ConfigurationAggregatorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateResourceConfigResponseTypeDef = TypedDict(
     "GetAggregateResourceConfigResponseTypeDef",
     {
         "ConfigurationItem": ConfigurationItemTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceConfigHistoryResponseTypeDef = TypedDict(
     "GetResourceConfigHistoryResponseTypeDef",
     {
         "configurationItems": List[ConfigurationItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConformancePacksResponseTypeDef = TypedDict(
     "DescribeOrganizationConformancePacksResponseTypeDef",
     {
         "OrganizationConformancePacks": List[OrganizationConformancePackTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConformancePacksResponseTypeDef = TypedDict(
     "DescribeConformancePacksResponseTypeDef",
     {
         "ConformancePackDetails": List[ConformancePackDetailTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRemediationExceptionsResponseTypeDef = TypedDict(
     "DeleteRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedDeleteRemediationExceptionsBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutRemediationExceptionsResponseTypeDef = TypedDict(
     "PutRemediationExceptionsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationExceptionBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AggregateEvaluationResultTypeDef = TypedDict(
     "AggregateEvaluationResultTypeDef",
     {
         "EvaluationResultIdentifier": EvaluationResultIdentifierTypeDef,
@@ -3811,43 +3989,72 @@
         "ConfigRuleInvokedTime": datetime,
         "Annotation": str,
         "ResultToken": str,
     },
     total=False,
 )
 
+EvaluationUnionTypeDef = Union[EvaluationTypeDef, EvaluationOutputTypeDef]
+PutExternalEvaluationRequestRequestTypeDef = TypedDict(
+    "PutExternalEvaluationRequestRequestTypeDef",
+    {
+        "ConfigRuleName": str,
+        "ExternalEvaluation": ExternalEvaluationTypeDef,
+    },
+)
+
+ResourceEvaluationFiltersTypeDef = TypedDict(
+    "ResourceEvaluationFiltersTypeDef",
+    {
+        "EvaluationMode": EvaluationModeType,
+        "TimeWindow": TimeWindowTypeDef,
+        "EvaluationContextIdentifier": str,
+    },
+    total=False,
+)
+
 SelectAggregateResourceConfigResponseTypeDef = TypedDict(
     "SelectAggregateResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SelectResourceConfigResponseTypeDef = TypedDict(
     "SelectResourceConfigResponseTypeDef",
     {
         "Results": List[str],
         "QueryInfo": QueryInfoTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigRulesResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigRulesResponseTypeDef",
     {
         "OrganizationConfigRules": List[OrganizationConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationRecorderOutputTypeDef = TypedDict(
+    "ConfigurationRecorderOutputTypeDef",
+    {
+        "name": str,
+        "roleARN": str,
+        "recordingGroup": RecordingGroupOutputTypeDef,
+    },
+    total=False,
+)
+
 ConfigurationRecorderTypeDef = TypedDict(
     "ConfigurationRecorderTypeDef",
     {
         "name": str,
         "roleARN": str,
         "recordingGroup": RecordingGroupTypeDef,
     },
@@ -3855,31 +4062,60 @@
 )
 
 DescribeRemediationExecutionStatusResponseTypeDef = TypedDict(
     "DescribeRemediationExecutionStatusResponseTypeDef",
     {
         "RemediationExecutionStatuses": List[RemediationExecutionStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredRemediationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredRemediationConfigurationOutputTypeDef",
+    {
+        "ConfigRuleName": str,
+        "TargetType": Literal["SSM_DOCUMENT"],
+        "TargetId": str,
+    },
+)
+_OptionalRemediationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalRemediationConfigurationOutputTypeDef",
+    {
+        "TargetVersion": str,
+        "Parameters": Dict[str, RemediationParameterValueOutputTypeDef],
+        "ResourceType": str,
+        "Automatic": bool,
+        "ExecutionControls": ExecutionControlsTypeDef,
+        "MaximumAutomaticAttempts": int,
+        "RetryAttemptSeconds": int,
+        "Arn": str,
+        "CreatedByService": str,
+    },
+    total=False,
+)
+
+class RemediationConfigurationOutputTypeDef(
+    _RequiredRemediationConfigurationOutputTypeDef, _OptionalRemediationConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredRemediationConfigurationTypeDef = TypedDict(
     "_RequiredRemediationConfigurationTypeDef",
     {
         "ConfigRuleName": str,
         "TargetType": Literal["SSM_DOCUMENT"],
         "TargetId": str,
     },
 )
 _OptionalRemediationConfigurationTypeDef = TypedDict(
     "_OptionalRemediationConfigurationTypeDef",
     {
         "TargetVersion": str,
-        "Parameters": Dict[str, RemediationParameterValueTypeDef],
+        "Parameters": Mapping[str, RemediationParameterValueTypeDef],
         "ResourceType": str,
         "Automatic": bool,
         "ExecutionControls": ExecutionControlsTypeDef,
         "MaximumAutomaticAttempts": int,
         "RetryAttemptSeconds": int,
         "Arn": str,
         "CreatedByService": str,
@@ -3888,33 +4124,40 @@
 )
 
 class RemediationConfigurationTypeDef(
     _RequiredRemediationConfigurationTypeDef, _OptionalRemediationConfigurationTypeDef
 ):
     pass
 
-ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+_RequiredConfigRuleOutputTypeDef = TypedDict(
+    "_RequiredConfigRuleOutputTypeDef",
     {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Source": SourceOutputTypeDef,
     },
-    total=False,
 )
-
-ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
-    "ListResourceEvaluationsRequestRequestTypeDef",
+_OptionalConfigRuleOutputTypeDef = TypedDict(
+    "_OptionalConfigRuleOutputTypeDef",
     {
-        "Filters": ResourceEvaluationFiltersTypeDef,
-        "Limit": int,
-        "NextToken": str,
+        "ConfigRuleName": str,
+        "ConfigRuleArn": str,
+        "ConfigRuleId": str,
+        "Description": str,
+        "Scope": ScopeOutputTypeDef,
+        "InputParameters": str,
+        "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
+        "ConfigRuleState": ConfigRuleStateType,
+        "CreatedBy": str,
+        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
+class ConfigRuleOutputTypeDef(_RequiredConfigRuleOutputTypeDef, _OptionalConfigRuleOutputTypeDef):
+    pass
+
 _RequiredConfigRuleTypeDef = TypedDict(
     "_RequiredConfigRuleTypeDef",
     {
         "Source": SourceTypeDef,
     },
 )
 _OptionalConfigRuleTypeDef = TypedDict(
@@ -3925,152 +4168,191 @@
         "ConfigRuleId": str,
         "Description": str,
         "Scope": ScopeTypeDef,
         "InputParameters": str,
         "MaximumExecutionFrequency": MaximumExecutionFrequencyType,
         "ConfigRuleState": ConfigRuleStateType,
         "CreatedBy": str,
-        "EvaluationModes": List[EvaluationModeConfigurationTypeDef],
+        "EvaluationModes": Sequence[EvaluationModeConfigurationTypeDef],
     },
     total=False,
 )
 
 class ConfigRuleTypeDef(_RequiredConfigRuleTypeDef, _OptionalConfigRuleTypeDef):
     pass
 
 GetAggregateConfigRuleComplianceSummaryResponseTypeDef = TypedDict(
     "GetAggregateConfigRuleComplianceSummaryResponseTypeDef",
     {
         "GroupByKey": str,
         "AggregateComplianceCounts": List[AggregateComplianceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceSummaryByResourceTypeResponseTypeDef = TypedDict(
     "GetComplianceSummaryByResourceTypeResponseTypeDef",
     {
         "ComplianceSummariesByResourceType": List[ComplianceSummaryByResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAggregateComplianceByConfigRulesResponseTypeDef = TypedDict(
     "DescribeAggregateComplianceByConfigRulesResponseTypeDef",
     {
         "AggregateComplianceByConfigRules": List[AggregateComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByConfigRuleResponseTypeDef = TypedDict(
     "DescribeComplianceByConfigRuleResponseTypeDef",
     {
         "ComplianceByConfigRules": List[ComplianceByConfigRuleTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeComplianceByResourceResponseTypeDef = TypedDict(
     "DescribeComplianceByResourceResponseTypeDef",
     {
         "ComplianceByResources": List[ComplianceByResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAggregateComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetAggregateComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "AggregateEvaluationResults": List[AggregateEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConformancePackComplianceDetailsResponseTypeDef = TypedDict(
     "GetConformancePackComplianceDetailsResponseTypeDef",
     {
         "ConformancePackName": str,
         "ConformancePackRuleEvaluationResults": List[ConformancePackEvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByConfigRuleResponseTypeDef = TypedDict(
     "GetComplianceDetailsByConfigRuleResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetComplianceDetailsByResourceResponseTypeDef = TypedDict(
     "GetComplianceDetailsByResourceResponseTypeDef",
     {
         "EvaluationResults": List[EvaluationResultTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_RequiredPutEvaluationsRequestRequestTypeDef",
+    {
+        "ResultToken": str,
+    },
+)
+_OptionalPutEvaluationsRequestRequestTypeDef = TypedDict(
+    "_OptionalPutEvaluationsRequestRequestTypeDef",
+    {
+        "Evaluations": Sequence[EvaluationUnionTypeDef],
+        "TestMode": bool,
+    },
+    total=False,
+)
+
+class PutEvaluationsRequestRequestTypeDef(
+    _RequiredPutEvaluationsRequestRequestTypeDef, _OptionalPutEvaluationsRequestRequestTypeDef
+):
+    pass
+
+ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListResourceEvaluationsRequestRequestTypeDef = TypedDict(
+    "ListResourceEvaluationsRequestRequestTypeDef",
+    {
+        "Filters": ResourceEvaluationFiltersTypeDef,
+        "Limit": int,
+        "NextToken": str,
+    },
+    total=False,
+)
+
 DescribeConfigurationRecordersResponseTypeDef = TypedDict(
     "DescribeConfigurationRecordersResponseTypeDef",
     {
-        "ConfigurationRecorders": List[ConfigurationRecorderTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ConfigurationRecorders": List[ConfigurationRecorderOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigurationRecorderUnionTypeDef = Union[
+    ConfigurationRecorderTypeDef, ConfigurationRecorderOutputTypeDef
+]
 PutConfigurationRecorderRequestRequestTypeDef = TypedDict(
     "PutConfigurationRecorderRequestRequestTypeDef",
     {
         "ConfigurationRecorder": ConfigurationRecorderTypeDef,
     },
 )
 
 DescribeRemediationConfigurationsResponseTypeDef = TypedDict(
     "DescribeRemediationConfigurationsResponseTypeDef",
     {
-        "RemediationConfigurations": List[RemediationConfigurationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RemediationConfigurations": List[RemediationConfigurationOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FailedRemediationBatchTypeDef = TypedDict(
     "FailedRemediationBatchTypeDef",
     {
         "FailureMessage": str,
-        "FailedItems": List[RemediationConfigurationTypeDef],
+        "FailedItems": List[RemediationConfigurationOutputTypeDef],
     },
     total=False,
 )
 
-PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
-    "PutRemediationConfigurationsRequestRequestTypeDef",
-    {
-        "RemediationConfigurations": Sequence[RemediationConfigurationTypeDef],
-    },
-)
-
+RemediationConfigurationUnionTypeDef = Union[
+    RemediationConfigurationTypeDef, RemediationConfigurationOutputTypeDef
+]
 DescribeConfigRulesResponseTypeDef = TypedDict(
     "DescribeConfigRulesResponseTypeDef",
     {
-        "ConfigRules": List[ConfigRuleTypeDef],
+        "ConfigRules": List[ConfigRuleOutputTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ConfigRuleUnionTypeDef = Union[ConfigRuleTypeDef, ConfigRuleOutputTypeDef]
 _RequiredPutConfigRuleRequestRequestTypeDef = TypedDict(
     "_RequiredPutConfigRuleRequestRequestTypeDef",
     {
         "ConfigRule": ConfigRuleTypeDef,
     },
 )
 _OptionalPutConfigRuleRequestRequestTypeDef = TypedDict(
@@ -4086,10 +4368,17 @@
 ):
     pass
 
 PutRemediationConfigurationsResponseTypeDef = TypedDict(
     "PutRemediationConfigurationsResponseTypeDef",
     {
         "FailedBatches": List[FailedRemediationBatchTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutRemediationConfigurationsRequestRequestTypeDef = TypedDict(
+    "PutRemediationConfigurationsRequestRequestTypeDef",
+    {
+        "RemediationConfigurations": Sequence[RemediationConfigurationUnionTypeDef],
     },
 )
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/PKG-INFO` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-config
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConfigService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConfigService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore config type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore config type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-config"></a>
 
 # types-aiobotocore-config
 
 [![PyPI - types-aiobotocore-config](https://img.shields.io/pypi/v/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-config.svg?color=blue)](https://pypi.org/project/types-aiobotocore-config)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-config?color=blue)](https://pypistats.org/packages/types-aiobotocore-config)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-config)](https://pepy.tech/project/types-aiobotocore-config)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConfigService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/config.html#ConfigService)
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
 [types-aiobotocore-config docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_config/).
 
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
@@ -493,43 +492,46 @@
 )
 
 
 def check_value(value: AggregateConformancePackComplianceSummaryGroupKeyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_config.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_config.type_defs import (
+    AccountAggregationSourceOutputTypeDef,
     AccountAggregationSourceTypeDef,
     AggregateConformancePackComplianceTypeDef,
     AggregateConformancePackComplianceCountTypeDef,
     AggregateConformancePackComplianceFiltersTypeDef,
     AggregateConformancePackComplianceSummaryFiltersTypeDef,
     AggregateResourceIdentifierTypeDef,
     AggregatedSourceStatusTypeDef,
     AggregationAuthorizationTypeDef,
     BaseConfigurationItemTypeDef,
+    ResponseMetadataTypeDef,
     ResourceKeyTypeDef,
     ComplianceContributorCountTypeDef,
     ConfigExportDeliveryInfoTypeDef,
     ConfigRuleComplianceFiltersTypeDef,
     ConfigRuleComplianceSummaryFiltersTypeDef,
     ConfigRuleEvaluationStatusTypeDef,
     EvaluationModeConfigurationTypeDef,
+    ScopeOutputTypeDef,
     ScopeTypeDef,
     ConfigSnapshotDeliveryPropertiesTypeDef,
     ConfigStreamDeliveryInfoTypeDef,
-    OrganizationAggregationSourceTypeDef,
+    OrganizationAggregationSourceOutputTypeDef,
     RelationshipTypeDef,
     ConfigurationRecorderStatusTypeDef,
     ConformancePackComplianceFiltersTypeDef,
     ConformancePackComplianceScoreTypeDef,
     ConformancePackComplianceScoresFiltersTypeDef,
     ConformancePackComplianceSummaryTypeDef,
     ConformancePackInputParameterTypeDef,
@@ -550,148 +552,125 @@
     DeletePendingAggregationRequestRequestRequestTypeDef,
     DeleteRemediationConfigurationRequestRequestTypeDef,
     RemediationExceptionResourceKeyTypeDef,
     DeleteResourceConfigRequestRequestTypeDef,
     DeleteRetentionConfigurationRequestRequestTypeDef,
     DeleteStoredQueryRequestRequestTypeDef,
     DeliverConfigSnapshotRequestRequestTypeDef,
-    DeliverConfigSnapshotResponseTypeDef,
-    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeAggregationAuthorizationsRequestRequestTypeDef,
-    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
     DescribeComplianceByConfigRuleRequestRequestTypeDef,
-    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
     DescribeComplianceByResourceRequestRequestTypeDef,
-    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
     DescribeConfigRuleEvaluationStatusRequestRequestTypeDef,
     DescribeConfigRulesFiltersTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
     DescribeConfigurationAggregatorSourcesStatusRequestRequestTypeDef,
-    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
     DescribeConfigurationAggregatorsRequestRequestTypeDef,
     DescribeConfigurationRecorderStatusRequestRequestTypeDef,
     DescribeConfigurationRecordersRequestRequestTypeDef,
-    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
     DescribeConformancePackStatusRequestRequestTypeDef,
-    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
     DescribeConformancePacksRequestRequestTypeDef,
     DescribeDeliveryChannelStatusRequestRequestTypeDef,
     DescribeDeliveryChannelsRequestRequestTypeDef,
-    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
     DescribeOrganizationConfigRuleStatusesRequestRequestTypeDef,
     OrganizationConfigRuleStatusTypeDef,
-    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
     DescribeOrganizationConfigRulesRequestRequestTypeDef,
-    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
     DescribeOrganizationConformancePackStatusesRequestRequestTypeDef,
     OrganizationConformancePackStatusTypeDef,
-    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
     DescribeOrganizationConformancePacksRequestRequestTypeDef,
-    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
     DescribePendingAggregationRequestsRequestRequestTypeDef,
     PendingAggregationRequestTypeDef,
     DescribeRemediationConfigurationsRequestRequestTypeDef,
     RemediationExceptionTypeDef,
-    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
     DescribeRetentionConfigurationsRequestRequestTypeDef,
     RetentionConfigurationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationContextTypeDef,
+    EvaluationOutputTypeDef,
     EvaluationResultQualifierTypeDef,
     EvaluationStatusTypeDef,
-    EvaluationTypeDef,
+    TimestampTypeDef,
+    ExclusionByResourceTypesOutputTypeDef,
     ExclusionByResourceTypesTypeDef,
     SsmControlsTypeDef,
-    ExternalEvaluationTypeDef,
     FieldInfoTypeDef,
-    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
     GetAggregateComplianceDetailsByConfigRuleRequestRequestTypeDef,
     ResourceCountFiltersTypeDef,
     GroupedResourceCountTypeDef,
-    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
     GetComplianceDetailsByConfigRuleRequestRequestTypeDef,
-    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
     GetComplianceDetailsByResourceRequestRequestTypeDef,
     GetComplianceSummaryByResourceTypeRequestRequestTypeDef,
-    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
     GetConformancePackComplianceSummaryRequestRequestTypeDef,
     GetCustomRulePolicyRequestRequestTypeDef,
-    GetCustomRulePolicyResponseTypeDef,
     GetDiscoveredResourceCountsRequestRequestTypeDef,
     ResourceCountTypeDef,
     StatusDetailFiltersTypeDef,
     MemberAccountStatusTypeDef,
     OrganizationResourceDetailedStatusFiltersTypeDef,
     OrganizationConformancePackDetailedStatusTypeDef,
     GetOrganizationCustomRulePolicyRequestRequestTypeDef,
-    GetOrganizationCustomRulePolicyResponseTypeDef,
-    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
-    GetResourceConfigHistoryRequestRequestTypeDef,
     GetResourceEvaluationSummaryRequestRequestTypeDef,
     ResourceDetailsTypeDef,
     GetStoredQueryRequestRequestTypeDef,
     StoredQueryTypeDef,
     ResourceFiltersTypeDef,
-    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
     ResourceIdentifierTypeDef,
     ResourceEvaluationTypeDef,
     ListStoredQueriesRequestRequestTypeDef,
     StoredQueryMetadataTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
+    OrganizationAggregationSourceTypeDef,
     OrganizationCustomPolicyRuleMetadataNoPolicyTypeDef,
+    OrganizationCustomRuleMetadataOutputTypeDef,
+    OrganizationManagedRuleMetadataOutputTypeDef,
+    OrganizationCustomPolicyRuleMetadataTypeDef,
     OrganizationCustomRuleMetadataTypeDef,
     OrganizationManagedRuleMetadataTypeDef,
-    OrganizationCustomPolicyRuleMetadataTypeDef,
-    PaginatorConfigTypeDef,
-    PutConformancePackResponseTypeDef,
-    PutOrganizationConfigRuleResponseTypeDef,
-    PutOrganizationConformancePackResponseTypeDef,
     PutResourceConfigRequestRequestTypeDef,
     PutRetentionConfigurationRequestRequestTypeDef,
-    PutStoredQueryResponseTypeDef,
     RecordingStrategyTypeDef,
     RemediationExecutionStepTypeDef,
     ResourceValueTypeDef,
+    StaticValueOutputTypeDef,
     StaticValueTypeDef,
-    TimeWindowTypeDef,
-    ResponseMetadataTypeDef,
     SelectAggregateResourceConfigRequestRequestTypeDef,
-    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
     SelectResourceConfigRequestRequestTypeDef,
-    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     SourceDetailTypeDef,
     StartConfigRulesEvaluationRequestRequestTypeDef,
     StartConfigurationRecorderRequestRequestTypeDef,
-    StartResourceEvaluationResponseTypeDef,
     StopConfigurationRecorderRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
+    AccountAggregationSourceUnionTypeDef,
     AggregateComplianceByConformancePackTypeDef,
     AggregateConformancePackComplianceSummaryTypeDef,
-    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
     DescribeAggregateComplianceByConformancePacksRequestRequestTypeDef,
     GetAggregateConformancePackComplianceSummaryRequestRequestTypeDef,
     BatchGetAggregateResourceConfigRequestRequestTypeDef,
     GetAggregateResourceConfigRequestRequestTypeDef,
-    ListAggregateDiscoveredResourcesResponseTypeDef,
-    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    BatchGetAggregateResourceConfigResponseTypeDef,
+    DeliverConfigSnapshotResponseTypeDef,
     DescribeAggregationAuthorizationsResponseTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCustomRulePolicyResponseTypeDef,
+    GetOrganizationCustomRulePolicyResponseTypeDef,
+    ListAggregateDiscoveredResourcesResponseTypeDef,
     PutAggregationAuthorizationResponseTypeDef,
-    BatchGetAggregateResourceConfigResponseTypeDef,
+    PutConformancePackResponseTypeDef,
+    PutOrganizationConfigRuleResponseTypeDef,
+    PutOrganizationConformancePackResponseTypeDef,
+    PutStoredQueryResponseTypeDef,
+    StartResourceEvaluationResponseTypeDef,
     BatchGetResourceConfigRequestRequestTypeDef,
     BatchGetResourceConfigResponseTypeDef,
-    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
     DescribeRemediationExecutionStatusRequestRequestTypeDef,
     StartRemediationExecutionRequestRequestTypeDef,
     StartRemediationExecutionResponseTypeDef,
     ComplianceSummaryTypeDef,
     ComplianceTypeDef,
-    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
     DescribeAggregateComplianceByConfigRulesRequestRequestTypeDef,
     GetAggregateConfigRuleComplianceSummaryRequestRequestTypeDef,
     DescribeConfigRuleEvaluationStatusResponseTypeDef,
     DeliveryChannelTypeDef,
     DeliveryChannelStatusTypeDef,
     ConfigurationAggregatorTypeDef,
     ConfigurationItemTypeDef,
@@ -706,29 +685,57 @@
     PutConformancePackRequestRequestTypeDef,
     GetConformancePackComplianceDetailsRequestRequestTypeDef,
     DescribeConformancePackComplianceResponseTypeDef,
     DescribeConformancePackStatusResponseTypeDef,
     DeleteRemediationExceptionsRequestRequestTypeDef,
     DescribeRemediationExceptionsRequestRequestTypeDef,
     FailedDeleteRemediationExceptionsBatchTypeDef,
-    PutRemediationExceptionsRequestRequestTypeDef,
+    DescribeAggregateComplianceByConfigRulesRequestDescribeAggregateComplianceByConfigRulesPaginateTypeDef,
+    DescribeAggregateComplianceByConformancePacksRequestDescribeAggregateComplianceByConformancePacksPaginateTypeDef,
+    DescribeAggregationAuthorizationsRequestDescribeAggregationAuthorizationsPaginateTypeDef,
+    DescribeComplianceByConfigRuleRequestDescribeComplianceByConfigRulePaginateTypeDef,
+    DescribeComplianceByResourceRequestDescribeComplianceByResourcePaginateTypeDef,
+    DescribeConfigRuleEvaluationStatusRequestDescribeConfigRuleEvaluationStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorSourcesStatusRequestDescribeConfigurationAggregatorSourcesStatusPaginateTypeDef,
+    DescribeConfigurationAggregatorsRequestDescribeConfigurationAggregatorsPaginateTypeDef,
+    DescribeConformancePackStatusRequestDescribeConformancePackStatusPaginateTypeDef,
+    DescribeConformancePacksRequestDescribeConformancePacksPaginateTypeDef,
+    DescribeOrganizationConfigRuleStatusesRequestDescribeOrganizationConfigRuleStatusesPaginateTypeDef,
+    DescribeOrganizationConfigRulesRequestDescribeOrganizationConfigRulesPaginateTypeDef,
+    DescribeOrganizationConformancePackStatusesRequestDescribeOrganizationConformancePackStatusesPaginateTypeDef,
+    DescribeOrganizationConformancePacksRequestDescribeOrganizationConformancePacksPaginateTypeDef,
+    DescribePendingAggregationRequestsRequestDescribePendingAggregationRequestsPaginateTypeDef,
+    DescribeRemediationExecutionStatusRequestDescribeRemediationExecutionStatusPaginateTypeDef,
+    DescribeRetentionConfigurationsRequestDescribeRetentionConfigurationsPaginateTypeDef,
+    GetAggregateComplianceDetailsByConfigRuleRequestGetAggregateComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByConfigRuleRequestGetComplianceDetailsByConfigRulePaginateTypeDef,
+    GetComplianceDetailsByResourceRequestGetComplianceDetailsByResourcePaginateTypeDef,
+    GetConformancePackComplianceSummaryRequestGetConformancePackComplianceSummaryPaginateTypeDef,
+    ListDiscoveredResourcesRequestListDiscoveredResourcesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    SelectAggregateResourceConfigRequestSelectAggregateResourceConfigPaginateTypeDef,
+    SelectResourceConfigRequestSelectResourceConfigPaginateTypeDef,
     DescribeConfigRulesRequestDescribeConfigRulesPaginateTypeDef,
     DescribeConfigRulesRequestRequestTypeDef,
     DescribeOrganizationConfigRuleStatusesResponseTypeDef,
     DescribeOrganizationConformancePackStatusesResponseTypeDef,
     DescribePendingAggregationRequestsResponseTypeDef,
     DescribeRemediationExceptionsResponseTypeDef,
     FailedRemediationExceptionBatchTypeDef,
     DescribeRetentionConfigurationsResponseTypeDef,
     PutRetentionConfigurationResponseTypeDef,
-    EvaluationResultIdentifierTypeDef,
-    PutEvaluationsRequestRequestTypeDef,
     PutEvaluationsResponseTypeDef,
+    EvaluationResultIdentifierTypeDef,
+    EvaluationTypeDef,
+    ExternalEvaluationTypeDef,
+    GetResourceConfigHistoryRequestGetResourceConfigHistoryPaginateTypeDef,
+    GetResourceConfigHistoryRequestRequestTypeDef,
+    PutRemediationExceptionsRequestRequestTypeDef,
+    TimeWindowTypeDef,
     ExecutionControlsTypeDef,
-    PutExternalEvaluationRequestRequestTypeDef,
     QueryInfoTypeDef,
     GetAggregateDiscoveredResourceCountsRequestRequestTypeDef,
     GetAggregateDiscoveredResourceCountsResponseTypeDef,
     GetDiscoveredResourceCountsResponseTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestGetOrganizationConfigRuleDetailedStatusPaginateTypeDef,
     GetOrganizationConfigRuleDetailedStatusRequestRequestTypeDef,
     GetOrganizationConfigRuleDetailedStatusResponseTypeDef,
@@ -741,24 +748,29 @@
     ListAggregateDiscoveredResourcesRequestListAggregateDiscoveredResourcesPaginateTypeDef,
     ListAggregateDiscoveredResourcesRequestRequestTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     ListResourceEvaluationsResponseTypeDef,
     ListStoredQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutAggregationAuthorizationRequestRequestTypeDef,
-    PutConfigurationAggregatorRequestRequestTypeDef,
     PutStoredQueryRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
+    OrganizationAggregationSourceUnionTypeDef,
     OrganizationConfigRuleTypeDef,
+    OrganizationCustomRuleMetadataUnionTypeDef,
+    OrganizationManagedRuleMetadataUnionTypeDef,
     PutOrganizationConfigRuleRequestRequestTypeDef,
+    RecordingGroupOutputTypeDef,
     RecordingGroupTypeDef,
     RemediationExecutionStatusTypeDef,
+    RemediationParameterValueOutputTypeDef,
     RemediationParameterValueTypeDef,
-    ResourceEvaluationFiltersTypeDef,
+    SourceOutputTypeDef,
     SourceTypeDef,
+    PutConfigurationAggregatorRequestRequestTypeDef,
     DescribeAggregateComplianceByConformancePacksResponseTypeDef,
     GetAggregateConformancePackComplianceSummaryResponseTypeDef,
     AggregateComplianceCountTypeDef,
     ComplianceSummaryByResourceTypeTypeDef,
     GetComplianceSummaryByConfigRuleResponseTypeDef,
     AggregateComplianceByConfigRuleTypeDef,
     ComplianceByConfigRuleTypeDef,
@@ -773,44 +785,54 @@
     DescribeOrganizationConformancePacksResponseTypeDef,
     DescribeConformancePacksResponseTypeDef,
     DeleteRemediationExceptionsResponseTypeDef,
     PutRemediationExceptionsResponseTypeDef,
     AggregateEvaluationResultTypeDef,
     ConformancePackEvaluationResultTypeDef,
     EvaluationResultTypeDef,
+    EvaluationUnionTypeDef,
+    PutExternalEvaluationRequestRequestTypeDef,
+    ResourceEvaluationFiltersTypeDef,
     SelectAggregateResourceConfigResponseTypeDef,
     SelectResourceConfigResponseTypeDef,
     DescribeOrganizationConfigRulesResponseTypeDef,
+    ConfigurationRecorderOutputTypeDef,
     ConfigurationRecorderTypeDef,
     DescribeRemediationExecutionStatusResponseTypeDef,
+    RemediationConfigurationOutputTypeDef,
     RemediationConfigurationTypeDef,
-    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
-    ListResourceEvaluationsRequestRequestTypeDef,
+    ConfigRuleOutputTypeDef,
     ConfigRuleTypeDef,
     GetAggregateConfigRuleComplianceSummaryResponseTypeDef,
     GetComplianceSummaryByResourceTypeResponseTypeDef,
     DescribeAggregateComplianceByConfigRulesResponseTypeDef,
     DescribeComplianceByConfigRuleResponseTypeDef,
     DescribeComplianceByResourceResponseTypeDef,
     GetAggregateComplianceDetailsByConfigRuleResponseTypeDef,
     GetConformancePackComplianceDetailsResponseTypeDef,
     GetComplianceDetailsByConfigRuleResponseTypeDef,
     GetComplianceDetailsByResourceResponseTypeDef,
+    PutEvaluationsRequestRequestTypeDef,
+    ListResourceEvaluationsRequestListResourceEvaluationsPaginateTypeDef,
+    ListResourceEvaluationsRequestRequestTypeDef,
     DescribeConfigurationRecordersResponseTypeDef,
+    ConfigurationRecorderUnionTypeDef,
     PutConfigurationRecorderRequestRequestTypeDef,
     DescribeRemediationConfigurationsResponseTypeDef,
     FailedRemediationBatchTypeDef,
-    PutRemediationConfigurationsRequestRequestTypeDef,
+    RemediationConfigurationUnionTypeDef,
     DescribeConfigRulesResponseTypeDef,
+    ConfigRuleUnionTypeDef,
     PutConfigRuleRequestRequestTypeDef,
     PutRemediationConfigurationsResponseTypeDef,
+    PutRemediationConfigurationsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountAggregationSourceTypeDef:
+def get_value() -> AccountAggregationSourceOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-config-2.5.2/types_aiobotocore_config.egg-info/SOURCES.txt` & `types-aiobotocore-config-2.5.2.post1/types_aiobotocore_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*


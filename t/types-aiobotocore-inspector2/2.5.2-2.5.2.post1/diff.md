# Comparing `tmp/types-aiobotocore-inspector2-2.5.2.tar.gz` & `tmp/types-aiobotocore-inspector2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-inspector2-2.5.2.tar", last modified: Sat Jul  8 01:43:44 2023, max compression
+gzip compressed data, was "types-aiobotocore-inspector2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:24 2023, max compression
```

## Comparing `types-aiobotocore-inspector2-2.5.2.tar` & `types-aiobotocore-inspector2-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.310257 types-aiobotocore-inspector2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23625 2023-07-08 01:43:44.310257 types-aiobotocore-inspector2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22048 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:44.310257 types-aiobotocore-inspector2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:32:16.000000 types-aiobotocore-inspector2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.310257 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38025 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    37961 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-07-08 01:32:18.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13214 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13202 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    72426 2023-07-08 01:32:19.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    72345 2023-07-08 01:32:18.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:17.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:44.310257 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23625 2023-07-08 01:43:44.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:44.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:44.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:44.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:44.000000 types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22228 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.201569 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38060 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37996 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17575 2023-08-02 14:40:18.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17573 2023-08-02 14:40:18.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13204 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13192 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    75995 2023-08-02 14:40:19.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75914 2023-08-02 14:40:18.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:17.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:24.205569 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23758 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:24.000000 types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-inspector2-2.5.2/LICENSE` & `types-aiobotocore-inspector2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2/PKG-INFO` & `types-aiobotocore-inspector2-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Inspector2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Inspector2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore inspector2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore inspector2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-inspector2"></a>
 
 # types-aiobotocore-inspector2
 
 [![PyPI - types-aiobotocore-inspector2](https://img.shields.io/pypi/v/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-inspector2?color=blue)](https://pypistats.org/packages/types-aiobotocore-inspector2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector2)](https://pepy.tech/project/types-aiobotocore-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Inspector2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [types-aiobotocore-inspector2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/).
 
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
@@ -408,31 +407,31 @@
 )
 
 
 def check_value(value: AccountSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_inspector2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_inspector2.type_defs import (
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    AssociateMemberResponseTypeDef,
+    ResponseMetadataTypeDef,
     AtigDataTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
@@ -440,98 +439,78 @@
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
-    CancelFindingsReportResponseTypeDef,
     CancelSbomExportRequestRequestTypeDef,
-    CancelSbomExportResponseTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
-    CoverageDateFilterTypeDef,
+    TimestampTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
-    CreateFilterResponseTypeDef,
     DestinationTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
-    DateFilterTypeDef,
+    DateFilterOutputTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
-    DeleteFilterResponseTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
-    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
-    GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
-    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
     GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
-    ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
-    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateEncryptionKeyRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
@@ -547,87 +526,113 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
+    AssociateMemberResponseTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    DeleteFilterResponseTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
+    DisassociateMemberResponseTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
-    CoverageFilterCriteriaTypeDef,
+    CoverageDateFilterTypeDef,
+    DateFilterTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
     SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
-    ListCoverageRequestListCoveragePaginateTypeDef,
-    ListCoverageRequestRequestTypeDef,
-    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
-    ListCoverageStatisticsRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
-    CreateSbomExportRequestRequestTypeDef,
     GetSbomExportResponseTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
+    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
+    ListCoverageStatisticsRequestRequestTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
-    CreateFilterRequestRequestTypeDef,
-    CreateFindingsReportRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    CreateFindingsReportRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-inspector2-2.5.2/README.md` & `types-aiobotocore-inspector2-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-inspector2"></a>
 
 # types-aiobotocore-inspector2
 
 [![PyPI - types-aiobotocore-inspector2](https://img.shields.io/pypi/v/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-inspector2?color=blue)](https://pypistats.org/packages/types-aiobotocore-inspector2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector2)](https://pepy.tech/project/types-aiobotocore-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Inspector2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [types-aiobotocore-inspector2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/).
 
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
@@ -375,31 +375,31 @@
 )
 
 
 def check_value(value: AccountSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_inspector2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_inspector2.type_defs import (
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    AssociateMemberResponseTypeDef,
+    ResponseMetadataTypeDef,
     AtigDataTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
@@ -407,98 +407,78 @@
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
-    CancelFindingsReportResponseTypeDef,
     CancelSbomExportRequestRequestTypeDef,
-    CancelSbomExportResponseTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
-    CoverageDateFilterTypeDef,
+    TimestampTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
-    CreateFilterResponseTypeDef,
     DestinationTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
-    DateFilterTypeDef,
+    DateFilterOutputTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
-    DeleteFilterResponseTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
-    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
-    GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
-    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
     GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
-    ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
-    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateEncryptionKeyRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
@@ -514,87 +494,113 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
+    AssociateMemberResponseTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    DeleteFilterResponseTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
+    DisassociateMemberResponseTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
-    CoverageFilterCriteriaTypeDef,
+    CoverageDateFilterTypeDef,
+    DateFilterTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
     SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
-    ListCoverageRequestListCoveragePaginateTypeDef,
-    ListCoverageRequestRequestTypeDef,
-    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
-    ListCoverageStatisticsRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
-    CreateSbomExportRequestRequestTypeDef,
     GetSbomExportResponseTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
+    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
+    ListCoverageStatisticsRequestRequestTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
-    CreateFilterRequestRequestTypeDef,
-    CreateFindingsReportRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    CreateFindingsReportRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-inspector2-2.5.2/setup.py` & `types-aiobotocore-inspector2-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-inspector2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_inspector2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Inspector2 2.5.2 service generated with"
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
-    keywords="aiobotocore inspector2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore inspector2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_inspector2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/"
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/__init__.py` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/__init__.pyi` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/__main__.py` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Inspector2 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Inspector2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2\nOther"
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

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/client.py` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
     GetSbomExportResponseTypeDef,
@@ -82,15 +82,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
@@ -237,15 +237,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#close)
         """
 
     async def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaTypeDef,
+        filterCriteria: FilterCriteriaUnionTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -255,29 +255,29 @@
         """
 
     async def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...
+        filterCriteria: FilterCriteriaUnionTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_findings_report)
         """
 
     async def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_sbom_export)
         """
@@ -514,15 +514,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_finding_aggregations)
         """
 
     async def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -630,15 +630,15 @@
 
     async def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/client.pyi` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     DestinationTypeDef,
     DisableDelegatedAdminAccountResponseTypeDef,
     DisableResponseTypeDef,
     DisassociateMemberResponseTypeDef,
     EcrConfigurationTypeDef,
     EnableDelegatedAdminAccountResponseTypeDef,
     EnableResponseTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     GetConfigurationResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusResponseTypeDef,
     GetMemberResponseTypeDef,
     GetSbomExportResponseTypeDef,
@@ -82,15 +82,15 @@
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListMembersResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListUsageTotalsResponseTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
-    ResourceFilterCriteriaTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
     SortCriteriaTypeDef,
     StringFilterTypeDef,
     UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
@@ -222,15 +222,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#close)
         """
     async def create_filter(
         self,
         *,
         action: FilterActionType,
-        filterCriteria: FilterCriteriaTypeDef,
+        filterCriteria: FilterCriteriaUnionTypeDef,
         name: str,
         description: str = ...,
         reason: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
         Creates a filter resource using specified filter criteria.
@@ -239,28 +239,28 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_filter)
         """
     async def create_findings_report(
         self,
         *,
         reportFormat: ReportFormatType,
         s3Destination: DestinationTypeDef,
-        filterCriteria: FilterCriteriaTypeDef = ...
+        filterCriteria: FilterCriteriaUnionTypeDef = ...
     ) -> CreateFindingsReportResponseTypeDef:
         """
         Creates a finding report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_findings_report)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_findings_report)
         """
     async def create_sbom_export(
         self,
         *,
         reportFormat: SbomReportFormatType,
         s3Destination: DestinationTypeDef,
-        resourceFilterCriteria: ResourceFilterCriteriaTypeDef = ...
+        resourceFilterCriteria: ResourceFilterCriteriaUnionTypeDef = ...
     ) -> CreateSbomExportResponseTypeDef:
         """
         Creates a software bill of materials (SBOM) report.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.create_sbom_export)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#create_sbom_export)
         """
@@ -475,15 +475,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Client.list_finding_aggregations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/client/#list_finding_aggregations)
         """
     async def list_findings(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists findings for your environment.
 
@@ -580,15 +580,15 @@
         """
     async def update_filter(
         self,
         *,
         filterArn: str,
         action: FilterActionType = ...,
         description: str = ...,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         name: str = ...,
         reason: str = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Specifies the action that is to be applied to the findings that match the
         filter.
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/literals.py` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/literals.pyi` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/paginator.py` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -91,15 +91,15 @@
 class ListAccountPermissionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listaccountpermissionspaginator)
     """
 
     def paginate(
-        self, *, service: ServiceType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, service: ServiceType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listaccountpermissionspaginator)
         """
 
 
@@ -109,15 +109,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
         """
 
 
@@ -128,30 +128,30 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 
 class ListDelegatedAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listdelegatedadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDelegatedAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listdelegatedadminaccountspaginator)
         """
 
 
@@ -162,15 +162,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfilterspaginator)
         """
 
 
@@ -182,15 +182,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 
@@ -199,47 +199,47 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
         """
 
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listmemberspaginator)
         """
 
 
 class ListUsageTotalsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listusagetotalspaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsageTotalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listusagetotalspaginator)
         """
 
 
@@ -249,13 +249,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchVulnerabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
         """
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/paginator.pyi` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/paginator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import AggregationTypeType, FilterActionType, GroupKeyType, ServiceType
 from .type_defs import (
     AggregationRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
-    FilterCriteriaTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListAccountPermissionsResponseTypeDef,
     ListCoverageResponseTypeDef,
     ListCoverageStatisticsResponseTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -88,15 +88,15 @@
 class ListAccountPermissionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listaccountpermissionspaginator)
     """
 
     def paginate(
-        self, *, service: ServiceType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, service: ServiceType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListAccountPermissions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listaccountpermissionspaginator)
         """
 
 class ListCoveragePaginator(AioPaginator):
@@ -105,15 +105,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragepaginator)
         """
 
 class ListCoverageStatisticsPaginator(AioPaginator):
@@ -123,29 +123,29 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: CoverageFilterCriteriaTypeDef = ...,
         groupBy: GroupKeyType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoverageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListCoverageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listcoveragestatisticspaginator)
         """
 
 class ListDelegatedAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listdelegatedadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDelegatedAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListDelegatedAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listdelegatedadminaccountspaginator)
         """
 
 class ListFiltersPaginator(AioPaginator):
@@ -155,15 +155,15 @@
     """
 
     def paginate(
         self,
         *,
         action: FilterActionType = ...,
         arns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfilterspaginator)
         """
 
 class ListFindingAggregationsPaginator(AioPaginator):
@@ -174,15 +174,15 @@
 
     def paginate(
         self,
         *,
         aggregationType: AggregationTypeType,
         accountIds: Sequence[StringFilterTypeDef] = ...,
         aggregationRequest: AggregationRequestTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingAggregationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindingAggregations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingaggregationspaginator)
         """
 
 class ListFindingsPaginator(AioPaginator):
@@ -190,45 +190,45 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        filterCriteria: FilterCriteriaTypeDef = ...,
+        filterCriteria: FilterCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listfindingspaginator)
         """
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listmemberspaginator)
         """
 
 class ListUsageTotalsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listusagetotalspaginator)
     """
 
     def paginate(
-        self, *, accountIds: Sequence[str] = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accountIds: Sequence[str] = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListUsageTotalsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.ListUsageTotals.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#listusagetotalspaginator)
         """
 
 class SearchVulnerabilitiesPaginator(AioPaginator):
@@ -237,13 +237,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
     """
 
     def paginate(
         self,
         *,
         filterCriteria: SearchVulnerabilitiesFilterCriteriaTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchVulnerabilitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2.Paginator.SearchVulnerabilities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/paginators/#searchvulnerabilitiespaginator)
         """
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/type_defs.py` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_inspector2.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -89,15 +89,15 @@
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
-    "AssociateMemberResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AtigDataTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
@@ -105,98 +105,78 @@
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
-    "CancelFindingsReportResponseTypeDef",
     "CancelSbomExportRequestRequestTypeDef",
-    "CancelSbomExportResponseTypeDef",
     "CisaDataTypeDef",
     "CodeFilePathTypeDef",
     "CodeLineTypeDef",
     "SuggestedFixTypeDef",
     "CountsTypeDef",
-    "CoverageDateFilterTypeDef",
+    "TimestampTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
-    "CreateFilterResponseTypeDef",
     "DestinationTypeDef",
-    "CreateFindingsReportResponseTypeDef",
-    "CreateSbomExportResponseTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
-    "DateFilterTypeDef",
+    "DateFilterOutputTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
-    "DeleteFilterResponseTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
-    "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
-    "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
-    "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
-    "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
     "GetMemberRequestRequestTypeDef",
     "MemberTypeDef",
     "GetSbomExportRequestRequestTypeDef",
     "LambdaFunctionMetadataTypeDef",
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "SortCriteriaTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "ResetEncryptionKeyRequestRequestTypeDef",
     "ResourceMapFilterTypeDef",
     "ResourceStringFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
     "UpdateEncryptionKeyRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     "UsageTypeDef",
     "AccountAggregationResponseTypeDef",
     "AmiAggregationResponseTypeDef",
     "AwsEcrContainerAggregationResponseTypeDef",
     "Ec2InstanceAggregationResponseTypeDef",
     "FindingTypeAggregationResponseTypeDef",
@@ -212,76 +192,102 @@
     "AmiAggregationTypeDef",
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
+    "AssociateMemberResponseTypeDef",
+    "CancelFindingsReportResponseTypeDef",
+    "CancelSbomExportResponseTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateFindingsReportResponseTypeDef",
+    "CreateSbomExportResponseTypeDef",
+    "DeleteFilterResponseTypeDef",
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    "DisassociateMemberResponseTypeDef",
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    "GetEncryptionKeyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateOrganizationConfigurationResponseTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
-    "CoverageFilterCriteriaTypeDef",
+    "CoverageDateFilterTypeDef",
+    "DateFilterTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    "ListCoverageRequestRequestTypeDef",
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    "ListCoverageStatisticsRequestRequestTypeDef",
+    "CoverageFilterCriteriaTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
+    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "CreateSbomExportRequestRequestTypeDef",
     "GetSbomExportResponseTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
+    "ResourceFilterCriteriaUnionTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    "ListCoverageRequestRequestTypeDef",
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    "ListCoverageStatisticsRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "CreateFilterRequestRequestTypeDef",
-    "CreateFindingsReportRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "CreateFindingsReportRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -361,19 +367,22 @@
 AssociateMemberRequestRequestTypeDef = TypedDict(
     "AssociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-AssociateMemberResponseTypeDef = TypedDict(
-    "AssociateMemberResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AtigDataTypeDef = TypedDict(
     "AtigDataTypeDef",
     {
         "firstSeen": datetime,
@@ -564,37 +573,21 @@
 CancelFindingsReportRequestRequestTypeDef = TypedDict(
     "CancelFindingsReportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelFindingsReportResponseTypeDef = TypedDict(
-    "CancelFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelSbomExportRequestRequestTypeDef = TypedDict(
     "CancelSbomExportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelSbomExportResponseTypeDef = TypedDict(
-    "CancelSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CisaDataTypeDef = TypedDict(
     "CisaDataTypeDef",
     {
         "action": str,
         "dateAdded": datetime,
         "dateDue": datetime,
     },
@@ -633,23 +626,15 @@
     {
         "count": int,
         "groupKey": GroupKeyType,
     },
     total=False,
 )
 
-CoverageDateFilterTypeDef = TypedDict(
-    "CoverageDateFilterTypeDef",
-    {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredCoverageMapFilterTypeDef = TypedDict(
     "_RequiredCoverageMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -680,22 +665,14 @@
     "ScanStatusTypeDef",
     {
         "reason": ScanStatusReasonType,
         "statusCode": ScanStatusCodeType,
     },
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -708,30 +685,14 @@
 )
 
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
 
-CreateFindingsReportResponseTypeDef = TypedDict(
-    "CreateFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSbomExportResponseTypeDef = TypedDict(
-    "CreateSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 Cvss2TypeDef = TypedDict(
     "Cvss2TypeDef",
     {
         "baseScore": float,
         "scoringVector": str,
     },
     total=False,
@@ -760,19 +721,19 @@
         "baseScore": float,
         "scoringVector": str,
         "source": str,
         "version": str,
     },
 )
 
-DateFilterTypeDef = TypedDict(
-    "DateFilterTypeDef",
+DateFilterOutputTypeDef = TypedDict(
+    "DateFilterOutputTypeDef",
     {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
+        "endInclusive": datetime,
+        "startInclusive": datetime,
     },
     total=False,
 )
 
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
     {
@@ -794,37 +755,21 @@
 DeleteFilterRequestRequestTypeDef = TypedDict(
     "DeleteFilterRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteFilterResponseTypeDef = TypedDict(
-    "DeleteFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
-DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisableRequestRequestTypeDef = TypedDict(
     "DisableRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
     total=False,
@@ -833,22 +778,14 @@
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-DisassociateMemberResponseTypeDef = TypedDict(
-    "DisassociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapFilterTypeDef = TypedDict(
     "_RequiredMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -927,22 +864,14 @@
 class EnableDelegatedAdminAccountRequestRequestTypeDef(
     _RequiredEnableDelegatedAdminAccountRequestRequestTypeDef,
     _OptionalEnableDelegatedAdminAccountRequestRequestTypeDef,
 ):
     pass
 
 
-EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
 )
 _OptionalEnableRequestRequestTypeDef = TypedDict(
@@ -1018,41 +947,22 @@
         "end": datetime,
         "start": datetime,
         "status": FreeTrialStatusType,
         "type": FreeTrialTypeType,
     },
 )
 
-GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEncryptionKeyRequestRequestTypeDef = TypedDict(
     "GetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-GetEncryptionKeyResponseTypeDef = TypedDict(
-    "GetEncryptionKeyResponseTypeDef",
-    {
-        "kmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFindingsReportStatusRequestRequestTypeDef = TypedDict(
     "GetFindingsReportStatusRequestRequestTypeDef",
     {
         "reportId": str,
     },
     total=False,
 )
@@ -1089,19 +999,20 @@
         "functionTags": Dict[str, str],
         "layers": List[str],
         "runtime": RuntimeType,
     },
     total=False,
 )
 
-ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "service": ServiceType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountPermissionsRequestRequestTypeDef = TypedDict(
     "ListAccountPermissionsRequestRequestTypeDef",
     {
@@ -1116,41 +1027,23 @@
     "PermissionTypeDef",
     {
         "operation": OperationType,
         "service": ServiceType,
     },
 )
 
-ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDelegatedAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "action": FilterActionType,
-        "arns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "arns": Sequence[str],
         "maxResults": int,
         "nextToken": str,
@@ -1162,23 +1055,14 @@
     "SortCriteriaTypeDef",
     {
         "field": SortFieldType,
         "sortOrder": SortOrderType,
     },
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": bool,
     },
@@ -1188,31 +1072,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsageTotalsRequestRequestTypeDef = TypedDict(
     "ListUsageTotalsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -1261,24 +1128,14 @@
 
 class VulnerablePackageTypeDef(
     _RequiredVulnerablePackageTypeDef, _OptionalVulnerablePackageTypeDef
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
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Url": str,
         "text": str,
     },
     total=False,
@@ -1318,25 +1175,14 @@
     "ResourceStringFilterTypeDef",
     {
         "comparison": ResourceStringComparisonType,
         "value": str,
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
 SearchVulnerabilitiesFilterCriteriaTypeDef = TypedDict(
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     {
         "vulnerabilityIds": Sequence[str],
     },
 )
 
@@ -1361,42 +1207,23 @@
     {
         "activateDeepInspection": bool,
         "packagePaths": Sequence[str],
     },
     total=False,
 )
 
-UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEncryptionKeyRequestRequestTypeDef = TypedDict(
     "UpdateEncryptionKeyRequestRequestTypeDef",
     {
         "kmsKeyId": str,
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     {
         "orgPackagePaths": Sequence[str],
     },
 )
 
@@ -1777,35 +1604,161 @@
         "sortOrder": SortOrderType,
         "titles": Sequence[StringFilterTypeDef],
         "vulnerabilityIds": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
+AssociateMemberResponseTypeDef = TypedDict(
+    "AssociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelFindingsReportResponseTypeDef = TypedDict(
+    "CancelFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelSbomExportResponseTypeDef = TypedDict(
+    "CancelSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsReportResponseTypeDef = TypedDict(
+    "CreateFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSbomExportResponseTypeDef = TypedDict(
+    "CreateSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFilterResponseTypeDef = TypedDict(
+    "DeleteFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateMemberResponseTypeDef = TypedDict(
+    "DisassociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEncryptionKeyResponseTypeDef = TypedDict(
+    "GetEncryptionKeyResponseTypeDef",
+    {
+        "kmsKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
         "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
     },
 )
 
 UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
     "UpdateOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1835,24 +1788,24 @@
 
 
 BatchGetMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     {
         "accountIds": Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],
@@ -1900,34 +1853,32 @@
 
 ListCoverageStatisticsResponseTypeDef = TypedDict(
     "ListCoverageStatisticsResponseTypeDef",
     {
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CoverageFilterCriteriaTypeDef = TypedDict(
-    "CoverageFilterCriteriaTypeDef",
+CoverageDateFilterTypeDef = TypedDict(
+    "CoverageDateFilterTypeDef",
     {
-        "accountId": Sequence[CoverageStringFilterTypeDef],
-        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
-        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
-        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
-        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
-        "resourceId": Sequence[CoverageStringFilterTypeDef],
-        "resourceType": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
-        "scanType": Sequence[CoverageStringFilterTypeDef],
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DateFilterTypeDef = TypedDict(
+    "DateFilterTypeDef",
+    {
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
     },
     total=False,
 )
 
 _RequiredCvssScoreDetailsTypeDef = TypedDict(
     "_RequiredCvssScoreDetailsTypeDef",
     {
@@ -1952,23 +1903,23 @@
 
 
 ListDelegatedAdminAccountsResponseTypeDef = TypedDict(
     "ListDelegatedAdminAccountsResponseTypeDef",
     {
         "delegatedAdminAccounts": List[DelegatedAdminAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": Sequence[StringFilterTypeDef],
@@ -2065,44 +2016,89 @@
     },
 )
 
 GetMemberResponseTypeDef = TypedDict(
     "GetMemberResponseTypeDef",
     {
         "member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceScanMetadataTypeDef = TypedDict(
     "ResourceScanMetadataTypeDef",
     {
         "ec2": Ec2MetadataTypeDef,
         "ecrImage": EcrContainerImageMetadataTypeDef,
         "ecrRepository": EcrRepositoryMetadataTypeDef,
         "lambdaFunction": LambdaFunctionMetadataTypeDef,
     },
     total=False,
 )
 
+ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    {
+        "service": ServiceType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "action": FilterActionType,
+        "arns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccountPermissionsResponseTypeDef = TypedDict(
     "ListAccountPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkPathTypeDef = TypedDict(
     "NetworkPathTypeDef",
     {
         "steps": List[StepTypeDef],
@@ -2143,14 +2139,29 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+ResourceFilterCriteriaOutputTypeDef = TypedDict(
+    "ResourceFilterCriteriaOutputTypeDef",
+    {
+        "accountId": List[ResourceStringFilterTypeDef],
+        "ec2InstanceTags": List[ResourceMapFilterTypeDef],
+        "ecrImageTags": List[ResourceStringFilterTypeDef],
+        "ecrRepositoryName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionTags": List[ResourceMapFilterTypeDef],
+        "resourceId": List[ResourceStringFilterTypeDef],
+        "resourceType": List[ResourceStringFilterTypeDef],
+    },
+    total=False,
+)
+
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": Sequence[ResourceStringFilterTypeDef],
         "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
         "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
         "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
@@ -2189,15 +2200,15 @@
     {
         "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
     },
 )
 _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(
     _RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
@@ -2243,24 +2254,24 @@
 )
 
 DisableResponseTypeDef = TypedDict(
     "DisableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableResponseTypeDef = TypedDict(
     "EnableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEc2Instance": AwsEc2InstanceDetailsTypeDef,
@@ -2271,53 +2282,34 @@
 )
 
 BatchGetCodeSnippetResponseTypeDef = TypedDict(
     "BatchGetCodeSnippetResponseTypeDef",
     {
         "codeSnippetResults": List[CodeSnippetResultTypeDef],
         "errors": List[CodeSnippetErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListCoverageRequestRequestTypeDef = TypedDict(
-    "ListCoverageRequestRequestTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "maxResults": int,
-        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestRequestTypeDef",
+CoverageFilterCriteriaTypeDef = TypedDict(
+    "CoverageFilterCriteriaTypeDef",
     {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "nextToken": str,
+        "accountId": Sequence[CoverageStringFilterTypeDef],
+        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
+        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
+        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
+        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
+        "resourceId": Sequence[CoverageStringFilterTypeDef],
+        "resourceType": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
+        "scanType": Sequence[CoverageStringFilterTypeDef],
     },
     total=False,
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
@@ -2344,25 +2336,74 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchVulnerabilitiesResponseTypeDef = TypedDict(
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FilterCriteriaOutputTypeDef = TypedDict(
+    "FilterCriteriaOutputTypeDef",
+    {
+        "awsAccountId": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorName": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorTags": List[StringFilterTypeDef],
+        "codeVulnerabilityFilePath": List[StringFilterTypeDef],
+        "componentId": List[StringFilterTypeDef],
+        "componentType": List[StringFilterTypeDef],
+        "ec2InstanceImageId": List[StringFilterTypeDef],
+        "ec2InstanceSubnetId": List[StringFilterTypeDef],
+        "ec2InstanceVpcId": List[StringFilterTypeDef],
+        "ecrImageArchitecture": List[StringFilterTypeDef],
+        "ecrImageHash": List[StringFilterTypeDef],
+        "ecrImagePushedAt": List[DateFilterOutputTypeDef],
+        "ecrImageRegistry": List[StringFilterTypeDef],
+        "ecrImageRepositoryName": List[StringFilterTypeDef],
+        "ecrImageTags": List[StringFilterTypeDef],
+        "epssScore": List[NumberFilterTypeDef],
+        "exploitAvailable": List[StringFilterTypeDef],
+        "findingArn": List[StringFilterTypeDef],
+        "findingStatus": List[StringFilterTypeDef],
+        "findingType": List[StringFilterTypeDef],
+        "firstObservedAt": List[DateFilterOutputTypeDef],
+        "fixAvailable": List[StringFilterTypeDef],
+        "inspectorScore": List[NumberFilterTypeDef],
+        "lambdaFunctionExecutionRoleArn": List[StringFilterTypeDef],
+        "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
+        "lambdaFunctionLayers": List[StringFilterTypeDef],
+        "lambdaFunctionName": List[StringFilterTypeDef],
+        "lambdaFunctionRuntime": List[StringFilterTypeDef],
+        "lastObservedAt": List[DateFilterOutputTypeDef],
+        "networkProtocol": List[StringFilterTypeDef],
+        "portRange": List[PortRangeFilterTypeDef],
+        "relatedVulnerabilities": List[StringFilterTypeDef],
+        "resourceId": List[StringFilterTypeDef],
+        "resourceTags": List[MapFilterTypeDef],
+        "resourceType": List[StringFilterTypeDef],
+        "severity": List[StringFilterTypeDef],
+        "title": List[StringFilterTypeDef],
+        "updatedAt": List[DateFilterOutputTypeDef],
+        "vendorSeverity": List[StringFilterTypeDef],
+        "vulnerabilityId": List[StringFilterTypeDef],
+        "vulnerabilitySource": List[StringFilterTypeDef],
+        "vulnerablePackages": List[PackageFilterTypeDef],
     },
+    total=False,
 )
 
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
@@ -2411,15 +2452,15 @@
 )
 
 BatchGetFreeTrialInfoResponseTypeDef = TypedDict(
     "BatchGetFreeTrialInfoResponseTypeDef",
     {
         "accounts": List[FreeTrialAccountInfoTypeDef],
         "failedAccounts": List[FreeTrialInfoErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCoveredResourceTypeDef = TypedDict(
     "_RequiredCoveredResourceTypeDef",
     {
         "accountId": str,
@@ -2448,14 +2489,28 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
         "s3Destination": DestinationTypeDef,
     },
 )
@@ -2470,53 +2525,42 @@
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
 
-GetSbomExportResponseTypeDef = TypedDict(
-    "GetSbomExportResponseTypeDef",
-    {
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaTypeDef,
-        "format": SbomReportFormatType,
-        "reportId": str,
-        "s3Destination": DestinationTypeDef,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+ResourceFilterCriteriaUnionTypeDef = Union[
+    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+]
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingAggregationsResponseTypeDef = TypedDict(
     "ListFindingAggregationsResponseTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "nextToken": str,
         "responses": List[AggregationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAccountStatusResponseTypeDef = TypedDict(
     "BatchGetAccountStatusResponseTypeDef",
     {
         "accounts": List[AccountStateTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "id": str,
@@ -2535,26 +2579,65 @@
 )
 
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
 
+ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageRequestRequestTypeDef = TypedDict(
+    "ListCoverageRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "aggregationType": AggregationTypeType,
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "accountIds": Sequence[StringFilterTypeDef],
         "aggregationRequest": AggregationRequestTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(
     _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
@@ -2584,14 +2667,54 @@
 class ListFindingAggregationsRequestRequestTypeDef(
     _RequiredListFindingAggregationsRequestRequestTypeDef,
     _OptionalListFindingAggregationsRequestRequestTypeDef,
 ):
     pass
 
 
+_RequiredFilterTypeDef = TypedDict(
+    "_RequiredFilterTypeDef",
+    {
+        "action": FilterActionType,
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": FilterCriteriaOutputTypeDef,
+        "name": str,
+        "ownerId": str,
+        "updatedAt": datetime,
+    },
+)
+_OptionalFilterTypeDef = TypedDict(
+    "_OptionalFilterTypeDef",
+    {
+        "description": str,
+        "reason": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
+    pass
+
+
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
+    {
+        "destination": DestinationTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaOutputTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
         "name": str,
     },
@@ -2632,60 +2755,21 @@
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredFilterTypeDef = TypedDict(
-    "_RequiredFilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-    },
-)
-_OptionalFilterTypeDef = TypedDict(
-    "_OptionalFilterTypeDef",
-    {
-        "description": str,
-        "reason": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-
-class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
-    pass
-
-
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
-    {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2723,15 +2807,15 @@
 
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "coveredResources": List[CoveredResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "awsAccountId": str,
@@ -2770,19 +2854,19 @@
 
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsResponseTypeDef = TypedDict(
     "ListFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2/type_defs.pyi` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_inspector2.type_defs import SeverityCountsTypeDef
 
-    data: SeverityCountsTypeDef = {...}
+    data: SeverityCountsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
@@ -88,15 +88,15 @@
     "SeverityCountsTypeDef",
     "AccountAggregationTypeDef",
     "StateTypeDef",
     "ResourceStatusTypeDef",
     "FindingTypeAggregationTypeDef",
     "StringFilterTypeDef",
     "AssociateMemberRequestRequestTypeDef",
-    "AssociateMemberResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AtigDataTypeDef",
     "AutoEnableTypeDef",
     "AwsEc2InstanceDetailsTypeDef",
     "AwsEcrContainerImageDetailsTypeDef",
     "LambdaVpcConfigTypeDef",
     "BatchGetAccountStatusRequestRequestTypeDef",
     "BatchGetCodeSnippetRequestRequestTypeDef",
@@ -104,98 +104,78 @@
     "BatchGetFreeTrialInfoRequestRequestTypeDef",
     "FreeTrialInfoErrorTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "FailedMemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusStateTypeDef",
     "MemberAccountEc2DeepInspectionStatusTypeDef",
     "CancelFindingsReportRequestRequestTypeDef",
-    "CancelFindingsReportResponseTypeDef",
     "CancelSbomExportRequestRequestTypeDef",
-    "CancelSbomExportResponseTypeDef",
     "CisaDataTypeDef",
     "CodeFilePathTypeDef",
     "CodeLineTypeDef",
     "SuggestedFixTypeDef",
     "CountsTypeDef",
-    "CoverageDateFilterTypeDef",
+    "TimestampTypeDef",
     "CoverageMapFilterTypeDef",
     "CoverageStringFilterTypeDef",
     "ScanStatusTypeDef",
-    "CreateFilterResponseTypeDef",
     "DestinationTypeDef",
-    "CreateFindingsReportResponseTypeDef",
-    "CreateSbomExportResponseTypeDef",
     "Cvss2TypeDef",
     "Cvss3TypeDef",
     "CvssScoreAdjustmentTypeDef",
     "CvssScoreTypeDef",
-    "DateFilterTypeDef",
+    "DateFilterOutputTypeDef",
     "DelegatedAdminAccountTypeDef",
     "DelegatedAdminTypeDef",
     "DeleteFilterRequestRequestTypeDef",
-    "DeleteFilterResponseTypeDef",
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
-    "DisableDelegatedAdminAccountResponseTypeDef",
     "DisableRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
-    "DisassociateMemberResponseTypeDef",
     "MapFilterTypeDef",
     "Ec2MetadataTypeDef",
     "EcrRescanDurationStateTypeDef",
     "EcrConfigurationTypeDef",
     "EcrContainerImageMetadataTypeDef",
     "EcrRepositoryMetadataTypeDef",
     "EnableDelegatedAdminAccountRequestRequestTypeDef",
-    "EnableDelegatedAdminAccountResponseTypeDef",
     "EnableRequestRequestTypeDef",
     "EpssDetailsTypeDef",
     "EpssTypeDef",
     "ExploitObservedTypeDef",
     "ExploitabilityDetailsTypeDef",
     "NumberFilterTypeDef",
     "PortRangeFilterTypeDef",
     "FreeTrialInfoTypeDef",
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
     "GetEncryptionKeyRequestRequestTypeDef",
-    "GetEncryptionKeyResponseTypeDef",
     "GetFindingsReportStatusRequestRequestTypeDef",
     "GetMemberRequestRequestTypeDef",
     "MemberTypeDef",
     "GetSbomExportRequestRequestTypeDef",
     "LambdaFunctionMetadataTypeDef",
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountPermissionsRequestRequestTypeDef",
     "PermissionTypeDef",
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
     "SortCriteriaTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListUsageTotalsRequestRequestTypeDef",
     "StepTypeDef",
     "PortRangeTypeDef",
     "VulnerablePackageTypeDef",
-    "PaginatorConfigTypeDef",
     "RecommendationTypeDef",
     "ResetEncryptionKeyRequestRequestTypeDef",
     "ResourceMapFilterTypeDef",
     "ResourceStringFilterTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef",
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
     "UpdateEncryptionKeyRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     "UsageTypeDef",
     "AccountAggregationResponseTypeDef",
     "AmiAggregationResponseTypeDef",
     "AwsEcrContainerAggregationResponseTypeDef",
     "Ec2InstanceAggregationResponseTypeDef",
     "FindingTypeAggregationResponseTypeDef",
@@ -211,76 +191,102 @@
     "AmiAggregationTypeDef",
     "AwsEcrContainerAggregationTypeDef",
     "ImageLayerAggregationTypeDef",
     "LambdaLayerAggregationTypeDef",
     "PackageAggregationTypeDef",
     "RepositoryAggregationTypeDef",
     "TitleAggregationTypeDef",
+    "AssociateMemberResponseTypeDef",
+    "CancelFindingsReportResponseTypeDef",
+    "CancelSbomExportResponseTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateFindingsReportResponseTypeDef",
+    "CreateSbomExportResponseTypeDef",
+    "DeleteFilterResponseTypeDef",
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    "DisassociateMemberResponseTypeDef",
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    "GetEncryptionKeyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "DescribeOrganizationConfigurationResponseTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateOrganizationConfigurationResponseTypeDef",
     "AwsLambdaFunctionDetailsTypeDef",
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     "CodeVulnerabilityDetailsTypeDef",
     "CodeSnippetResultTypeDef",
     "ListCoverageStatisticsResponseTypeDef",
-    "CoverageFilterCriteriaTypeDef",
+    "CoverageDateFilterTypeDef",
+    "DateFilterTypeDef",
     "CvssScoreDetailsTypeDef",
     "ListDelegatedAdminAccountsResponseTypeDef",
     "GetDelegatedAdminAccountResponseTypeDef",
     "Ec2InstanceAggregationTypeDef",
     "LambdaFunctionAggregationTypeDef",
     "EcrConfigurationStateTypeDef",
     "UpdateConfigurationRequestRequestTypeDef",
     "VulnerabilityTypeDef",
     "PackageFilterTypeDef",
     "FreeTrialAccountInfoTypeDef",
     "GetMemberResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ResourceScanMetadataTypeDef",
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
     "ListAccountPermissionsResponseTypeDef",
     "NetworkPathTypeDef",
     "PackageVulnerabilityDetailsTypeDef",
     "RemediationTypeDef",
+    "ResourceFilterCriteriaOutputTypeDef",
     "ResourceFilterCriteriaTypeDef",
     "SearchVulnerabilitiesRequestRequestTypeDef",
     "SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     "UsageTotalTypeDef",
     "AggregationResponseTypeDef",
     "AccountStateTypeDef",
     "DisableResponseTypeDef",
     "EnableResponseTypeDef",
     "ResourceDetailsTypeDef",
     "BatchGetCodeSnippetResponseTypeDef",
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    "ListCoverageRequestRequestTypeDef",
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    "ListCoverageStatisticsRequestRequestTypeDef",
+    "CoverageFilterCriteriaTypeDef",
     "InspectorScoreDetailsTypeDef",
     "AggregationRequestTypeDef",
     "GetConfigurationResponseTypeDef",
     "SearchVulnerabilitiesResponseTypeDef",
+    "FilterCriteriaOutputTypeDef",
     "FilterCriteriaTypeDef",
     "BatchGetFreeTrialInfoResponseTypeDef",
     "CoveredResourceTypeDef",
     "NetworkReachabilityDetailsTypeDef",
-    "CreateSbomExportRequestRequestTypeDef",
     "GetSbomExportResponseTypeDef",
+    "CreateSbomExportRequestRequestTypeDef",
+    "ResourceFilterCriteriaUnionTypeDef",
     "ListUsageTotalsResponseTypeDef",
     "ListFindingAggregationsResponseTypeDef",
     "BatchGetAccountStatusResponseTypeDef",
     "ResourceTypeDef",
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    "ListCoverageRequestRequestTypeDef",
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    "ListCoverageStatisticsRequestRequestTypeDef",
     "ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     "ListFindingAggregationsRequestRequestTypeDef",
-    "CreateFilterRequestRequestTypeDef",
-    "CreateFindingsReportRequestRequestTypeDef",
     "FilterTypeDef",
     "GetFindingsReportStatusResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "CreateFindingsReportRequestRequestTypeDef",
+    "FilterCriteriaUnionTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "ListCoverageResponseTypeDef",
     "FindingTypeDef",
     "ListFiltersResponseTypeDef",
     "ListFindingsResponseTypeDef",
@@ -358,19 +364,22 @@
 AssociateMemberRequestRequestTypeDef = TypedDict(
     "AssociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-AssociateMemberResponseTypeDef = TypedDict(
-    "AssociateMemberResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AtigDataTypeDef = TypedDict(
     "AtigDataTypeDef",
     {
         "firstSeen": datetime,
@@ -553,37 +562,21 @@
 CancelFindingsReportRequestRequestTypeDef = TypedDict(
     "CancelFindingsReportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelFindingsReportResponseTypeDef = TypedDict(
-    "CancelFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CancelSbomExportRequestRequestTypeDef = TypedDict(
     "CancelSbomExportRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-CancelSbomExportResponseTypeDef = TypedDict(
-    "CancelSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CisaDataTypeDef = TypedDict(
     "CisaDataTypeDef",
     {
         "action": str,
         "dateAdded": datetime,
         "dateDue": datetime,
     },
@@ -622,23 +615,15 @@
     {
         "count": int,
         "groupKey": GroupKeyType,
     },
     total=False,
 )
 
-CoverageDateFilterTypeDef = TypedDict(
-    "CoverageDateFilterTypeDef",
-    {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
-    },
-    total=False,
-)
-
+TimestampTypeDef = Union[datetime, str]
 _RequiredCoverageMapFilterTypeDef = TypedDict(
     "_RequiredCoverageMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -667,22 +652,14 @@
     "ScanStatusTypeDef",
     {
         "reason": ScanStatusReasonType,
         "statusCode": ScanStatusCodeType,
     },
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "bucketName": str,
         "kmsKeyArn": str,
     },
 )
@@ -693,30 +670,14 @@
     },
     total=False,
 )
 
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-CreateFindingsReportResponseTypeDef = TypedDict(
-    "CreateFindingsReportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateSbomExportResponseTypeDef = TypedDict(
-    "CreateSbomExportResponseTypeDef",
-    {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 Cvss2TypeDef = TypedDict(
     "Cvss2TypeDef",
     {
         "baseScore": float,
         "scoringVector": str,
     },
     total=False,
@@ -745,19 +706,19 @@
         "baseScore": float,
         "scoringVector": str,
         "source": str,
         "version": str,
     },
 )
 
-DateFilterTypeDef = TypedDict(
-    "DateFilterTypeDef",
+DateFilterOutputTypeDef = TypedDict(
+    "DateFilterOutputTypeDef",
     {
-        "endInclusive": Union[datetime, str],
-        "startInclusive": Union[datetime, str],
+        "endInclusive": datetime,
+        "startInclusive": datetime,
     },
     total=False,
 )
 
 DelegatedAdminAccountTypeDef = TypedDict(
     "DelegatedAdminAccountTypeDef",
     {
@@ -779,37 +740,21 @@
 DeleteFilterRequestRequestTypeDef = TypedDict(
     "DeleteFilterRequestRequestTypeDef",
     {
         "arn": str,
     },
 )
 
-DeleteFilterResponseTypeDef = TypedDict(
-    "DeleteFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisableDelegatedAdminAccountRequestRequestTypeDef = TypedDict(
     "DisableDelegatedAdminAccountRequestRequestTypeDef",
     {
         "delegatedAdminAccountId": str,
     },
 )
 
-DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "DisableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisableRequestRequestTypeDef = TypedDict(
     "DisableRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
     total=False,
@@ -818,22 +763,14 @@
 DisassociateMemberRequestRequestTypeDef = TypedDict(
     "DisassociateMemberRequestRequestTypeDef",
     {
         "accountId": str,
     },
 )
 
-DisassociateMemberResponseTypeDef = TypedDict(
-    "DisassociateMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredMapFilterTypeDef = TypedDict(
     "_RequiredMapFilterTypeDef",
     {
         "comparison": Literal["EQUALS"],
         "key": str,
     },
 )
@@ -908,22 +845,14 @@
 
 class EnableDelegatedAdminAccountRequestRequestTypeDef(
     _RequiredEnableDelegatedAdminAccountRequestRequestTypeDef,
     _OptionalEnableDelegatedAdminAccountRequestRequestTypeDef,
 ):
     pass
 
-EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
-    "EnableDelegatedAdminAccountResponseTypeDef",
-    {
-        "delegatedAdminAccountId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredEnableRequestRequestTypeDef = TypedDict(
     "_RequiredEnableRequestRequestTypeDef",
     {
         "resourceTypes": Sequence[ResourceScanTypeType],
     },
 )
 _OptionalEnableRequestRequestTypeDef = TypedDict(
@@ -997,41 +926,22 @@
         "end": datetime,
         "start": datetime,
         "status": FreeTrialStatusType,
         "type": FreeTrialTypeType,
     },
 )
 
-GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "GetEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetEncryptionKeyRequestRequestTypeDef = TypedDict(
     "GetEncryptionKeyRequestRequestTypeDef",
     {
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-GetEncryptionKeyResponseTypeDef = TypedDict(
-    "GetEncryptionKeyResponseTypeDef",
-    {
-        "kmsKeyId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetFindingsReportStatusRequestRequestTypeDef = TypedDict(
     "GetFindingsReportStatusRequestRequestTypeDef",
     {
         "reportId": str,
     },
     total=False,
 )
@@ -1068,19 +978,20 @@
         "functionTags": Dict[str, str],
         "layers": List[str],
         "runtime": RuntimeType,
     },
     total=False,
 )
 
-ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
-    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "service": ServiceType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListAccountPermissionsRequestRequestTypeDef = TypedDict(
     "ListAccountPermissionsRequestRequestTypeDef",
     {
@@ -1095,41 +1006,23 @@
     "PermissionTypeDef",
     {
         "operation": OperationType,
         "service": ServiceType,
     },
 )
 
-ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
-    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDelegatedAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListDelegatedAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "ListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "action": FilterActionType,
-        "arns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFiltersRequestRequestTypeDef = TypedDict(
     "ListFiltersRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "arns": Sequence[str],
         "maxResults": int,
         "nextToken": str,
@@ -1141,23 +1034,14 @@
     "SortCriteriaTypeDef",
     {
         "field": SortFieldType,
         "sortOrder": SortOrderType,
     },
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMembersRequestRequestTypeDef = TypedDict(
     "ListMembersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "onlyAssociated": bool,
     },
@@ -1167,31 +1051,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
-    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
-    {
-        "accountIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListUsageTotalsRequestRequestTypeDef = TypedDict(
     "ListUsageTotalsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
         "maxResults": int,
         "nextToken": str,
     },
@@ -1238,24 +1105,14 @@
 )
 
 class VulnerablePackageTypeDef(
     _RequiredVulnerablePackageTypeDef, _OptionalVulnerablePackageTypeDef
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
-
 RecommendationTypeDef = TypedDict(
     "RecommendationTypeDef",
     {
         "Url": str,
         "text": str,
     },
     total=False,
@@ -1293,25 +1150,14 @@
     "ResourceStringFilterTypeDef",
     {
         "comparison": ResourceStringComparisonType,
         "value": str,
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
 SearchVulnerabilitiesFilterCriteriaTypeDef = TypedDict(
     "SearchVulnerabilitiesFilterCriteriaTypeDef",
     {
         "vulnerabilityIds": Sequence[str],
     },
 )
 
@@ -1336,42 +1182,23 @@
     {
         "activateDeepInspection": bool,
         "packagePaths": Sequence[str],
     },
     total=False,
 )
 
-UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
-    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
-    {
-        "errorMessage": str,
-        "orgPackagePaths": List[str],
-        "packagePaths": List[str],
-        "status": Ec2DeepInspectionStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateEncryptionKeyRequestRequestTypeDef = TypedDict(
     "UpdateEncryptionKeyRequestRequestTypeDef",
     {
         "kmsKeyId": str,
         "resourceType": ResourceTypeType,
         "scanType": ScanTypeType,
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef",
     {
         "orgPackagePaths": Sequence[str],
     },
 )
 
@@ -1730,35 +1557,161 @@
         "sortOrder": SortOrderType,
         "titles": Sequence[StringFilterTypeDef],
         "vulnerabilityIds": Sequence[StringFilterTypeDef],
     },
     total=False,
 )
 
+AssociateMemberResponseTypeDef = TypedDict(
+    "AssociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelFindingsReportResponseTypeDef = TypedDict(
+    "CancelFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CancelSbomExportResponseTypeDef = TypedDict(
+    "CancelSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsReportResponseTypeDef = TypedDict(
+    "CreateFindingsReportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSbomExportResponseTypeDef = TypedDict(
+    "CreateSbomExportResponseTypeDef",
+    {
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteFilterResponseTypeDef = TypedDict(
+    "DeleteFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "DisableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateMemberResponseTypeDef = TypedDict(
+    "DisassociateMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EnableDelegatedAdminAccountResponseTypeDef = TypedDict(
+    "EnableDelegatedAdminAccountResponseTypeDef",
+    {
+        "delegatedAdminAccountId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "GetEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetEncryptionKeyResponseTypeDef = TypedDict(
+    "GetEncryptionKeyResponseTypeDef",
+    {
+        "kmsKeyId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateEc2DeepInspectionConfigurationResponseTypeDef = TypedDict(
+    "UpdateEc2DeepInspectionConfigurationResponseTypeDef",
+    {
+        "errorMessage": str,
+        "orgPackagePaths": List[str],
+        "packagePaths": List[str],
+        "status": Ec2DeepInspectionStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
         "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
     },
 )
 
 UpdateOrganizationConfigurationResponseTypeDef = TypedDict(
     "UpdateOrganizationConfigurationResponseTypeDef",
     {
         "autoEnable": AutoEnableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAwsLambdaFunctionDetailsTypeDef = TypedDict(
     "_RequiredAwsLambdaFunctionDetailsTypeDef",
     {
         "codeSha256": str,
@@ -1786,24 +1739,24 @@
     pass
 
 BatchGetMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchGetMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef",
     {
         "accountIds": List[MemberAccountEc2DeepInspectionStatusStateTypeDef],
         "failedAccountIds": List[FailedMemberAccountEc2DeepInspectionStatusStateTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef = TypedDict(
     "BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef",
     {
         "accountIds": Sequence[MemberAccountEc2DeepInspectionStatusTypeDef],
@@ -1849,34 +1802,32 @@
 
 ListCoverageStatisticsResponseTypeDef = TypedDict(
     "ListCoverageStatisticsResponseTypeDef",
     {
         "countsByGroup": List[CountsTypeDef],
         "nextToken": str,
         "totalCounts": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CoverageFilterCriteriaTypeDef = TypedDict(
-    "CoverageFilterCriteriaTypeDef",
+CoverageDateFilterTypeDef = TypedDict(
+    "CoverageDateFilterTypeDef",
     {
-        "accountId": Sequence[CoverageStringFilterTypeDef],
-        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
-        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
-        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
-        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
-        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
-        "resourceId": Sequence[CoverageStringFilterTypeDef],
-        "resourceType": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
-        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
-        "scanType": Sequence[CoverageStringFilterTypeDef],
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
+    },
+    total=False,
+)
+
+DateFilterTypeDef = TypedDict(
+    "DateFilterTypeDef",
+    {
+        "endInclusive": TimestampTypeDef,
+        "startInclusive": TimestampTypeDef,
     },
     total=False,
 )
 
 _RequiredCvssScoreDetailsTypeDef = TypedDict(
     "_RequiredCvssScoreDetailsTypeDef",
     {
@@ -1899,23 +1850,23 @@
     pass
 
 ListDelegatedAdminAccountsResponseTypeDef = TypedDict(
     "ListDelegatedAdminAccountsResponseTypeDef",
     {
         "delegatedAdminAccounts": List[DelegatedAdminAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDelegatedAdminAccountResponseTypeDef = TypedDict(
     "GetDelegatedAdminAccountResponseTypeDef",
     {
         "delegatedAdmin": DelegatedAdminTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 Ec2InstanceAggregationTypeDef = TypedDict(
     "Ec2InstanceAggregationTypeDef",
     {
         "amis": Sequence[StringFilterTypeDef],
@@ -2010,44 +1961,89 @@
     },
 )
 
 GetMemberResponseTypeDef = TypedDict(
     "GetMemberResponseTypeDef",
     {
         "member": MemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "members": List[MemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceScanMetadataTypeDef = TypedDict(
     "ResourceScanMetadataTypeDef",
     {
         "ec2": Ec2MetadataTypeDef,
         "ecrImage": EcrContainerImageMetadataTypeDef,
         "ecrRepository": EcrRepositoryMetadataTypeDef,
         "lambdaFunction": LambdaFunctionMetadataTypeDef,
     },
     total=False,
 )
 
+ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef = TypedDict(
+    "ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef",
+    {
+        "service": ServiceType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef = TypedDict(
+    "ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "action": FilterActionType,
+        "arns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListUsageTotalsRequestListUsageTotalsPaginateTypeDef = TypedDict(
+    "ListUsageTotalsRequestListUsageTotalsPaginateTypeDef",
+    {
+        "accountIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAccountPermissionsResponseTypeDef = TypedDict(
     "ListAccountPermissionsResponseTypeDef",
     {
         "nextToken": str,
         "permissions": List[PermissionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkPathTypeDef = TypedDict(
     "NetworkPathTypeDef",
     {
         "steps": List[StepTypeDef],
@@ -2086,14 +2082,29 @@
     "RemediationTypeDef",
     {
         "recommendation": RecommendationTypeDef,
     },
     total=False,
 )
 
+ResourceFilterCriteriaOutputTypeDef = TypedDict(
+    "ResourceFilterCriteriaOutputTypeDef",
+    {
+        "accountId": List[ResourceStringFilterTypeDef],
+        "ec2InstanceTags": List[ResourceMapFilterTypeDef],
+        "ecrImageTags": List[ResourceStringFilterTypeDef],
+        "ecrRepositoryName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionName": List[ResourceStringFilterTypeDef],
+        "lambdaFunctionTags": List[ResourceMapFilterTypeDef],
+        "resourceId": List[ResourceStringFilterTypeDef],
+        "resourceType": List[ResourceStringFilterTypeDef],
+    },
+    total=False,
+)
+
 ResourceFilterCriteriaTypeDef = TypedDict(
     "ResourceFilterCriteriaTypeDef",
     {
         "accountId": Sequence[ResourceStringFilterTypeDef],
         "ec2InstanceTags": Sequence[ResourceMapFilterTypeDef],
         "ecrImageTags": Sequence[ResourceStringFilterTypeDef],
         "ecrRepositoryName": Sequence[ResourceStringFilterTypeDef],
@@ -2130,15 +2141,15 @@
     {
         "filterCriteria": SearchVulnerabilitiesFilterCriteriaTypeDef,
     },
 )
 _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef = TypedDict(
     "_OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef(
     _RequiredSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     _OptionalSearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
@@ -2182,24 +2193,24 @@
 )
 
 DisableResponseTypeDef = TypedDict(
     "DisableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableResponseTypeDef = TypedDict(
     "EnableResponseTypeDef",
     {
         "accounts": List[AccountTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceDetailsTypeDef = TypedDict(
     "ResourceDetailsTypeDef",
     {
         "awsEc2Instance": AwsEc2InstanceDetailsTypeDef,
@@ -2210,53 +2221,34 @@
 )
 
 BatchGetCodeSnippetResponseTypeDef = TypedDict(
     "BatchGetCodeSnippetResponseTypeDef",
     {
         "codeSnippetResults": List[CodeSnippetResultTypeDef],
         "errors": List[CodeSnippetErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
-    "ListCoverageRequestListCoveragePaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListCoverageRequestRequestTypeDef = TypedDict(
-    "ListCoverageRequestRequestTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "maxResults": int,
-        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
-    {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
-    "ListCoverageStatisticsRequestRequestTypeDef",
+CoverageFilterCriteriaTypeDef = TypedDict(
+    "CoverageFilterCriteriaTypeDef",
     {
-        "filterCriteria": CoverageFilterCriteriaTypeDef,
-        "groupBy": GroupKeyType,
-        "nextToken": str,
+        "accountId": Sequence[CoverageStringFilterTypeDef],
+        "ec2InstanceTags": Sequence[CoverageMapFilterTypeDef],
+        "ecrImageTags": Sequence[CoverageStringFilterTypeDef],
+        "ecrRepositoryName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionName": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionRuntime": Sequence[CoverageStringFilterTypeDef],
+        "lambdaFunctionTags": Sequence[CoverageMapFilterTypeDef],
+        "lastScannedAt": Sequence[CoverageDateFilterTypeDef],
+        "resourceId": Sequence[CoverageStringFilterTypeDef],
+        "resourceType": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusCode": Sequence[CoverageStringFilterTypeDef],
+        "scanStatusReason": Sequence[CoverageStringFilterTypeDef],
+        "scanType": Sequence[CoverageStringFilterTypeDef],
     },
     total=False,
 )
 
 InspectorScoreDetailsTypeDef = TypedDict(
     "InspectorScoreDetailsTypeDef",
     {
@@ -2283,27 +2275,76 @@
     total=False,
 )
 
 GetConfigurationResponseTypeDef = TypedDict(
     "GetConfigurationResponseTypeDef",
     {
         "ecrConfiguration": EcrConfigurationStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchVulnerabilitiesResponseTypeDef = TypedDict(
     "SearchVulnerabilitiesResponseTypeDef",
     {
         "nextToken": str,
         "vulnerabilities": List[VulnerabilityTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FilterCriteriaOutputTypeDef = TypedDict(
+    "FilterCriteriaOutputTypeDef",
+    {
+        "awsAccountId": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorName": List[StringFilterTypeDef],
+        "codeVulnerabilityDetectorTags": List[StringFilterTypeDef],
+        "codeVulnerabilityFilePath": List[StringFilterTypeDef],
+        "componentId": List[StringFilterTypeDef],
+        "componentType": List[StringFilterTypeDef],
+        "ec2InstanceImageId": List[StringFilterTypeDef],
+        "ec2InstanceSubnetId": List[StringFilterTypeDef],
+        "ec2InstanceVpcId": List[StringFilterTypeDef],
+        "ecrImageArchitecture": List[StringFilterTypeDef],
+        "ecrImageHash": List[StringFilterTypeDef],
+        "ecrImagePushedAt": List[DateFilterOutputTypeDef],
+        "ecrImageRegistry": List[StringFilterTypeDef],
+        "ecrImageRepositoryName": List[StringFilterTypeDef],
+        "ecrImageTags": List[StringFilterTypeDef],
+        "epssScore": List[NumberFilterTypeDef],
+        "exploitAvailable": List[StringFilterTypeDef],
+        "findingArn": List[StringFilterTypeDef],
+        "findingStatus": List[StringFilterTypeDef],
+        "findingType": List[StringFilterTypeDef],
+        "firstObservedAt": List[DateFilterOutputTypeDef],
+        "fixAvailable": List[StringFilterTypeDef],
+        "inspectorScore": List[NumberFilterTypeDef],
+        "lambdaFunctionExecutionRoleArn": List[StringFilterTypeDef],
+        "lambdaFunctionLastModifiedAt": List[DateFilterOutputTypeDef],
+        "lambdaFunctionLayers": List[StringFilterTypeDef],
+        "lambdaFunctionName": List[StringFilterTypeDef],
+        "lambdaFunctionRuntime": List[StringFilterTypeDef],
+        "lastObservedAt": List[DateFilterOutputTypeDef],
+        "networkProtocol": List[StringFilterTypeDef],
+        "portRange": List[PortRangeFilterTypeDef],
+        "relatedVulnerabilities": List[StringFilterTypeDef],
+        "resourceId": List[StringFilterTypeDef],
+        "resourceTags": List[MapFilterTypeDef],
+        "resourceType": List[StringFilterTypeDef],
+        "severity": List[StringFilterTypeDef],
+        "title": List[StringFilterTypeDef],
+        "updatedAt": List[DateFilterOutputTypeDef],
+        "vendorSeverity": List[StringFilterTypeDef],
+        "vulnerabilityId": List[StringFilterTypeDef],
+        "vulnerabilitySource": List[StringFilterTypeDef],
+        "vulnerablePackages": List[PackageFilterTypeDef],
+    },
+    total=False,
+)
+
 FilterCriteriaTypeDef = TypedDict(
     "FilterCriteriaTypeDef",
     {
         "awsAccountId": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorName": Sequence[StringFilterTypeDef],
         "codeVulnerabilityDetectorTags": Sequence[StringFilterTypeDef],
         "codeVulnerabilityFilePath": Sequence[StringFilterTypeDef],
@@ -2350,15 +2391,15 @@
 )
 
 BatchGetFreeTrialInfoResponseTypeDef = TypedDict(
     "BatchGetFreeTrialInfoResponseTypeDef",
     {
         "accounts": List[FreeTrialAccountInfoTypeDef],
         "failedAccounts": List[FreeTrialInfoErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCoveredResourceTypeDef = TypedDict(
     "_RequiredCoveredResourceTypeDef",
     {
         "accountId": str,
@@ -2385,14 +2426,28 @@
     {
         "networkPath": NetworkPathTypeDef,
         "openPortRange": PortRangeTypeDef,
         "protocol": NetworkProtocolType,
     },
 )
 
+GetSbomExportResponseTypeDef = TypedDict(
+    "GetSbomExportResponseTypeDef",
+    {
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": ResourceFilterCriteriaOutputTypeDef,
+        "format": SbomReportFormatType,
+        "reportId": str,
+        "s3Destination": DestinationTypeDef,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateSbomExportRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSbomExportRequestRequestTypeDef",
     {
         "reportFormat": SbomReportFormatType,
         "s3Destination": DestinationTypeDef,
     },
 )
@@ -2405,53 +2460,42 @@
 )
 
 class CreateSbomExportRequestRequestTypeDef(
     _RequiredCreateSbomExportRequestRequestTypeDef, _OptionalCreateSbomExportRequestRequestTypeDef
 ):
     pass
 
-GetSbomExportResponseTypeDef = TypedDict(
-    "GetSbomExportResponseTypeDef",
-    {
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": ResourceFilterCriteriaTypeDef,
-        "format": SbomReportFormatType,
-        "reportId": str,
-        "s3Destination": DestinationTypeDef,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+ResourceFilterCriteriaUnionTypeDef = Union[
+    ResourceFilterCriteriaTypeDef, ResourceFilterCriteriaOutputTypeDef
+]
 ListUsageTotalsResponseTypeDef = TypedDict(
     "ListUsageTotalsResponseTypeDef",
     {
         "nextToken": str,
         "totals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingAggregationsResponseTypeDef = TypedDict(
     "ListFindingAggregationsResponseTypeDef",
     {
         "aggregationType": AggregationTypeType,
         "nextToken": str,
         "responses": List[AggregationResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetAccountStatusResponseTypeDef = TypedDict(
     "BatchGetAccountStatusResponseTypeDef",
     {
         "accounts": List[AccountStateTypeDef],
         "failedAccounts": List[FailedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "id": str,
@@ -2468,26 +2512,65 @@
     },
     total=False,
 )
 
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+ListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
+    "ListCoverageRequestListCoveragePaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageRequestRequestTypeDef = TypedDict(
+    "ListCoverageRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "maxResults": int,
+        "nextToken": str,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCoverageStatisticsRequestRequestTypeDef = TypedDict(
+    "ListCoverageStatisticsRequestRequestTypeDef",
+    {
+        "filterCriteria": CoverageFilterCriteriaTypeDef,
+        "groupBy": GroupKeyType,
+        "nextToken": str,
+    },
+    total=False,
+)
+
 _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "aggregationType": AggregationTypeType,
     },
 )
 _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef = TypedDict(
     "_OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef",
     {
         "accountIds": Sequence[StringFilterTypeDef],
         "aggregationRequest": AggregationRequestTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef(
     _RequiredListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     _OptionalListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
@@ -2513,14 +2596,52 @@
 
 class ListFindingAggregationsRequestRequestTypeDef(
     _RequiredListFindingAggregationsRequestRequestTypeDef,
     _OptionalListFindingAggregationsRequestRequestTypeDef,
 ):
     pass
 
+_RequiredFilterTypeDef = TypedDict(
+    "_RequiredFilterTypeDef",
+    {
+        "action": FilterActionType,
+        "arn": str,
+        "createdAt": datetime,
+        "criteria": FilterCriteriaOutputTypeDef,
+        "name": str,
+        "ownerId": str,
+        "updatedAt": datetime,
+    },
+)
+_OptionalFilterTypeDef = TypedDict(
+    "_OptionalFilterTypeDef",
+    {
+        "description": str,
+        "reason": str,
+        "tags": Dict[str, str],
+    },
+    total=False,
+)
+
+class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
+    pass
+
+GetFindingsReportStatusResponseTypeDef = TypedDict(
+    "GetFindingsReportStatusResponseTypeDef",
+    {
+        "destination": DestinationTypeDef,
+        "errorCode": ReportingErrorCodeType,
+        "errorMessage": str,
+        "filterCriteria": FilterCriteriaOutputTypeDef,
+        "reportId": str,
+        "status": ExternalReportStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "action": FilterActionType,
         "filterCriteria": FilterCriteriaTypeDef,
         "name": str,
     },
@@ -2557,58 +2678,21 @@
 
 class CreateFindingsReportRequestRequestTypeDef(
     _RequiredCreateFindingsReportRequestRequestTypeDef,
     _OptionalCreateFindingsReportRequestRequestTypeDef,
 ):
     pass
 
-_RequiredFilterTypeDef = TypedDict(
-    "_RequiredFilterTypeDef",
-    {
-        "action": FilterActionType,
-        "arn": str,
-        "createdAt": datetime,
-        "criteria": FilterCriteriaTypeDef,
-        "name": str,
-        "ownerId": str,
-        "updatedAt": datetime,
-    },
-)
-_OptionalFilterTypeDef = TypedDict(
-    "_OptionalFilterTypeDef",
-    {
-        "description": str,
-        "reason": str,
-        "tags": Dict[str, str],
-    },
-    total=False,
-)
-
-class FilterTypeDef(_RequiredFilterTypeDef, _OptionalFilterTypeDef):
-    pass
-
-GetFindingsReportStatusResponseTypeDef = TypedDict(
-    "GetFindingsReportStatusResponseTypeDef",
-    {
-        "destination": DestinationTypeDef,
-        "errorCode": ReportingErrorCodeType,
-        "errorMessage": str,
-        "filterCriteria": FilterCriteriaTypeDef,
-        "reportId": str,
-        "status": ExternalReportStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+FilterCriteriaUnionTypeDef = Union[FilterCriteriaTypeDef, FilterCriteriaOutputTypeDef]
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "filterCriteria": FilterCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2644,15 +2728,15 @@
     pass
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "coveredResources": List[CoveredResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFindingTypeDef = TypedDict(
     "_RequiredFindingTypeDef",
     {
         "awsAccountId": str,
@@ -2689,19 +2773,19 @@
     pass
 
 ListFiltersResponseTypeDef = TypedDict(
     "ListFiltersResponseTypeDef",
     {
         "filters": List[FilterTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsResponseTypeDef = TypedDict(
     "ListFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/PKG-INFO` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-inspector2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Inspector2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Inspector2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore inspector2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore inspector2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-inspector2"></a>
 
 # types-aiobotocore-inspector2
 
 [![PyPI - types-aiobotocore-inspector2](https://img.shields.io/pypi/v/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-inspector2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-inspector2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-inspector2?color=blue)](https://pypistats.org/packages/types-aiobotocore-inspector2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-inspector2)](https://pepy.tech/project/types-aiobotocore-inspector2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Inspector2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/inspector2.html#Inspector2)
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
 [types-aiobotocore-inspector2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_inspector2/).
 
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
@@ -408,31 +407,31 @@
 )
 
 
 def check_value(value: AccountSortByType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_inspector2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_inspector2.type_defs import (
     SeverityCountsTypeDef,
     AccountAggregationTypeDef,
     StateTypeDef,
     ResourceStatusTypeDef,
     FindingTypeAggregationTypeDef,
     StringFilterTypeDef,
     AssociateMemberRequestRequestTypeDef,
-    AssociateMemberResponseTypeDef,
+    ResponseMetadataTypeDef,
     AtigDataTypeDef,
     AutoEnableTypeDef,
     AwsEc2InstanceDetailsTypeDef,
     AwsEcrContainerImageDetailsTypeDef,
     LambdaVpcConfigTypeDef,
     BatchGetAccountStatusRequestRequestTypeDef,
     BatchGetCodeSnippetRequestRequestTypeDef,
@@ -440,98 +439,78 @@
     BatchGetFreeTrialInfoRequestRequestTypeDef,
     FreeTrialInfoErrorTypeDef,
     BatchGetMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     FailedMemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusStateTypeDef,
     MemberAccountEc2DeepInspectionStatusTypeDef,
     CancelFindingsReportRequestRequestTypeDef,
-    CancelFindingsReportResponseTypeDef,
     CancelSbomExportRequestRequestTypeDef,
-    CancelSbomExportResponseTypeDef,
     CisaDataTypeDef,
     CodeFilePathTypeDef,
     CodeLineTypeDef,
     SuggestedFixTypeDef,
     CountsTypeDef,
-    CoverageDateFilterTypeDef,
+    TimestampTypeDef,
     CoverageMapFilterTypeDef,
     CoverageStringFilterTypeDef,
     ScanStatusTypeDef,
-    CreateFilterResponseTypeDef,
     DestinationTypeDef,
-    CreateFindingsReportResponseTypeDef,
-    CreateSbomExportResponseTypeDef,
     Cvss2TypeDef,
     Cvss3TypeDef,
     CvssScoreAdjustmentTypeDef,
     CvssScoreTypeDef,
-    DateFilterTypeDef,
+    DateFilterOutputTypeDef,
     DelegatedAdminAccountTypeDef,
     DelegatedAdminTypeDef,
     DeleteFilterRequestRequestTypeDef,
-    DeleteFilterResponseTypeDef,
     DisableDelegatedAdminAccountRequestRequestTypeDef,
-    DisableDelegatedAdminAccountResponseTypeDef,
     DisableRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
-    DisassociateMemberResponseTypeDef,
     MapFilterTypeDef,
     Ec2MetadataTypeDef,
     EcrRescanDurationStateTypeDef,
     EcrConfigurationTypeDef,
     EcrContainerImageMetadataTypeDef,
     EcrRepositoryMetadataTypeDef,
     EnableDelegatedAdminAccountRequestRequestTypeDef,
-    EnableDelegatedAdminAccountResponseTypeDef,
     EnableRequestRequestTypeDef,
     EpssDetailsTypeDef,
     EpssTypeDef,
     ExploitObservedTypeDef,
     ExploitabilityDetailsTypeDef,
     NumberFilterTypeDef,
     PortRangeFilterTypeDef,
     FreeTrialInfoTypeDef,
-    GetEc2DeepInspectionConfigurationResponseTypeDef,
     GetEncryptionKeyRequestRequestTypeDef,
-    GetEncryptionKeyResponseTypeDef,
     GetFindingsReportStatusRequestRequestTypeDef,
     GetMemberRequestRequestTypeDef,
     MemberTypeDef,
     GetSbomExportRequestRequestTypeDef,
     LambdaFunctionMetadataTypeDef,
-    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountPermissionsRequestRequestTypeDef,
     PermissionTypeDef,
-    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
     ListDelegatedAdminAccountsRequestRequestTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
     SortCriteriaTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListUsageTotalsRequestRequestTypeDef,
     StepTypeDef,
     PortRangeTypeDef,
     VulnerablePackageTypeDef,
-    PaginatorConfigTypeDef,
     RecommendationTypeDef,
     ResetEncryptionKeyRequestRequestTypeDef,
     ResourceMapFilterTypeDef,
     ResourceStringFilterTypeDef,
-    ResponseMetadataTypeDef,
     SearchVulnerabilitiesFilterCriteriaTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEc2DeepInspectionConfigurationRequestRequestTypeDef,
-    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
     UpdateEncryptionKeyRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateOrgEc2DeepInspectionConfigurationRequestRequestTypeDef,
     UsageTypeDef,
     AccountAggregationResponseTypeDef,
     AmiAggregationResponseTypeDef,
     AwsEcrContainerAggregationResponseTypeDef,
     Ec2InstanceAggregationResponseTypeDef,
     FindingTypeAggregationResponseTypeDef,
@@ -547,87 +526,113 @@
     AmiAggregationTypeDef,
     AwsEcrContainerAggregationTypeDef,
     ImageLayerAggregationTypeDef,
     LambdaLayerAggregationTypeDef,
     PackageAggregationTypeDef,
     RepositoryAggregationTypeDef,
     TitleAggregationTypeDef,
+    AssociateMemberResponseTypeDef,
+    CancelFindingsReportResponseTypeDef,
+    CancelSbomExportResponseTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateFindingsReportResponseTypeDef,
+    CreateSbomExportResponseTypeDef,
+    DeleteFilterResponseTypeDef,
+    DisableDelegatedAdminAccountResponseTypeDef,
+    DisassociateMemberResponseTypeDef,
+    EnableDelegatedAdminAccountResponseTypeDef,
+    GetEc2DeepInspectionConfigurationResponseTypeDef,
+    GetEncryptionKeyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateEc2DeepInspectionConfigurationResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateOrganizationConfigurationResponseTypeDef,
     AwsLambdaFunctionDetailsTypeDef,
     BatchGetMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusResponseTypeDef,
     BatchUpdateMemberEc2DeepInspectionStatusRequestRequestTypeDef,
     CodeVulnerabilityDetailsTypeDef,
     CodeSnippetResultTypeDef,
     ListCoverageStatisticsResponseTypeDef,
-    CoverageFilterCriteriaTypeDef,
+    CoverageDateFilterTypeDef,
+    DateFilterTypeDef,
     CvssScoreDetailsTypeDef,
     ListDelegatedAdminAccountsResponseTypeDef,
     GetDelegatedAdminAccountResponseTypeDef,
     Ec2InstanceAggregationTypeDef,
     LambdaFunctionAggregationTypeDef,
     EcrConfigurationStateTypeDef,
     UpdateConfigurationRequestRequestTypeDef,
     VulnerabilityTypeDef,
     PackageFilterTypeDef,
     FreeTrialAccountInfoTypeDef,
     GetMemberResponseTypeDef,
     ListMembersResponseTypeDef,
     ResourceScanMetadataTypeDef,
+    ListAccountPermissionsRequestListAccountPermissionsPaginateTypeDef,
+    ListDelegatedAdminAccountsRequestListDelegatedAdminAccountsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListUsageTotalsRequestListUsageTotalsPaginateTypeDef,
     ListAccountPermissionsResponseTypeDef,
     NetworkPathTypeDef,
     PackageVulnerabilityDetailsTypeDef,
     RemediationTypeDef,
+    ResourceFilterCriteriaOutputTypeDef,
     ResourceFilterCriteriaTypeDef,
     SearchVulnerabilitiesRequestRequestTypeDef,
     SearchVulnerabilitiesRequestSearchVulnerabilitiesPaginateTypeDef,
     UsageTotalTypeDef,
     AggregationResponseTypeDef,
     AccountStateTypeDef,
     DisableResponseTypeDef,
     EnableResponseTypeDef,
     ResourceDetailsTypeDef,
     BatchGetCodeSnippetResponseTypeDef,
-    ListCoverageRequestListCoveragePaginateTypeDef,
-    ListCoverageRequestRequestTypeDef,
-    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
-    ListCoverageStatisticsRequestRequestTypeDef,
+    CoverageFilterCriteriaTypeDef,
     InspectorScoreDetailsTypeDef,
     AggregationRequestTypeDef,
     GetConfigurationResponseTypeDef,
     SearchVulnerabilitiesResponseTypeDef,
+    FilterCriteriaOutputTypeDef,
     FilterCriteriaTypeDef,
     BatchGetFreeTrialInfoResponseTypeDef,
     CoveredResourceTypeDef,
     NetworkReachabilityDetailsTypeDef,
-    CreateSbomExportRequestRequestTypeDef,
     GetSbomExportResponseTypeDef,
+    CreateSbomExportRequestRequestTypeDef,
+    ResourceFilterCriteriaUnionTypeDef,
     ListUsageTotalsResponseTypeDef,
     ListFindingAggregationsResponseTypeDef,
     BatchGetAccountStatusResponseTypeDef,
     ResourceTypeDef,
+    ListCoverageRequestListCoveragePaginateTypeDef,
+    ListCoverageRequestRequestTypeDef,
+    ListCoverageStatisticsRequestListCoverageStatisticsPaginateTypeDef,
+    ListCoverageStatisticsRequestRequestTypeDef,
     ListFindingAggregationsRequestListFindingAggregationsPaginateTypeDef,
     ListFindingAggregationsRequestRequestTypeDef,
-    CreateFilterRequestRequestTypeDef,
-    CreateFindingsReportRequestRequestTypeDef,
     FilterTypeDef,
     GetFindingsReportStatusResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    CreateFindingsReportRequestRequestTypeDef,
+    FilterCriteriaUnionTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     ListCoverageResponseTypeDef,
     FindingTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> SeverityCountsTypeDef:
+def get_value() -> SeverityCountsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-inspector2-2.5.2/types_aiobotocore_inspector2.egg-info/SOURCES.txt` & `types-aiobotocore-inspector2-2.5.2.post1/types_aiobotocore_inspector2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


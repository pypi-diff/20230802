# Comparing `tmp/types-aiobotocore-macie2-2.5.2.tar.gz` & `tmp/types-aiobotocore-macie2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-macie2-2.5.2.tar", last modified: Sat Jul  8 01:43:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-macie2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:36 2023, max compression
```

## Comparing `types-aiobotocore-macie2-2.5.2.tar` & `types-aiobotocore-macie2-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:56.010477 types-aiobotocore-macie2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    29178 2023-07-08 01:43:55.998477 types-aiobotocore-macie2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27617 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:56.010477 types-aiobotocore-macie2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:34:31.000000 types-aiobotocore-macie2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.998477 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63125 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    63020 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    20367 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    88919 2023-07-08 01:34:36.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    88864 2023-07-08 01:34:35.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-08 01:34:32.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.998477 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29178 2023-07-08 01:43:55.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 01:43:55.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:55.000000 types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28469 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:42:42.000000 types-aiobotocore-macie2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.293532 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63190 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63085 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17332 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20363 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94186 2023-08-02 14:42:47.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94131 2023-08-02 14:42:46.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-08-02 14:42:43.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.301532 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29983 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:52:36.000000 types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-macie2-2.5.2/LICENSE` & `types-aiobotocore-macie2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/PKG-INFO` & `types-aiobotocore-macie2-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore macie2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore macie2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-macie2"></a>
 
 # types-aiobotocore-macie2
 
 [![PyPI - types-aiobotocore-macie2](https://img.shields.io/pypi/v/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-macie2?color=blue)](https://pypistats.org/packages/types-aiobotocore-macie2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Macie2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [types-aiobotocore-macie2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/).
 
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
@@ -451,20 +450,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_macie2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
@@ -473,14 +472,15 @@
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
     BatchGetCustomDataIdentifiersRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BucketCountByEffectivePermissionTypeDef,
     BucketCountByEncryptionTypeTypeDef,
     BucketCountBySharedAccessTypeTypeDef,
     BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef,
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketPolicyTypeDef,
     BucketServerSideEncryptionTypeDef,
@@ -491,166 +491,172 @@
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
-    CreateAllowListResponseTypeDef,
-    CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
-    CreateCustomDataIdentifierResponseTypeDef,
-    CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
-    CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
+    SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
+    CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMemberRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClassificationJobRequestRequestTypeDef,
     LastRunErrorStatusTypeDef,
     StatisticsTypeDef,
     UserPausedDetailsTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DetectedDataDetailsTypeDef,
     DetectionTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DomainDetailsTypeDef,
     EnableMacieRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     SeverityTypeDef,
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
-    GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
     SecurityHubConfigurationTypeDef,
     SortCriteriaTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
-    GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
     RevealConfigurationTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
-    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesOutputTypeDef,
+    SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
+    SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
-    S3BucketDefinitionForJobTypeDef,
-    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    S3BucketDefinitionForJobOutputTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
-    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
-    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
-    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
     ListFindingsFiltersRequestRequestTypeDef,
-    ListFindingsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListJobsFilterTermTypeDef,
-    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
     ListManagedDataIdentifiersRequestRequestTypeDef,
     ManagedDataIdentifierSummaryTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
     ListResourceProfileArtifactsRequestRequestTypeDef,
     ResourceProfileArtifactTypeDef,
-    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
     ListResourceProfileDetectionsRequestRequestTypeDef,
-    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
-    TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
-    UpdateFindingsFilterResponseTypeDef,
     UpdateMacieSessionRequestRequestTypeDef,
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
     AllowListCriteriaTypeDef,
-    ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
+    CreateAllowListResponseTypeDef,
+    CreateClassificationJobResponseTypeDef,
+    CreateCustomDataIdentifierResponseTypeDef,
+    CreateFindingsFilterResponseTypeDef,
+    CreateMemberResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    GetAutomatedDiscoveryConfigurationResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetMacieSessionResponseTypeDef,
+    GetMemberResponseTypeDef,
+    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
+    ListAllowListsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TestCustomDataIdentifierResponseTypeDef,
+    UpdateAllowListResponseTypeDef,
+    UpdateFindingsFilterResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
-    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
     GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
+    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
+    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
+    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
+    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
@@ -659,96 +665,111 @@
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
-    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
+    JobScheduleFrequencyOutputTypeDef,
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
+    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
+    TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
+    TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
     CreateAllowListRequestRequestTypeDef,
     GetAllowListResponseTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
+    GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
-    GetFindingsFilterResponseTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
     AssumedRoleTypeDef,
     FederatedUserTypeDef,
+    CriteriaForJobOutputTypeDef,
     CriteriaForJobTypeDef,
+    JobScopeTermOutputTypeDef,
     JobScopeTermTypeDef,
     BucketPublicAccessTypeDef,
     SearchResourcesResponseTypeDef,
     CustomDetectionTypeDef,
     DefaultDetectionTypeDef,
     SearchResourcesCriteriaBlockTypeDef,
     GetUsageStatisticsResponseTypeDef,
     UserIdentityTypeDef,
+    CriteriaBlockForJobOutputTypeDef,
     CriteriaBlockForJobTypeDef,
+    JobScopingBlockOutputTypeDef,
     JobScopingBlockTypeDef,
     BucketMetadataTypeDef,
     S3BucketTypeDef,
     CustomDataIdentifiersTypeDef,
     SensitiveDataItemTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     FindingActorTypeDef,
+    S3BucketCriteriaForJobOutputTypeDef,
     S3BucketCriteriaForJobTypeDef,
+    ScopingOutputTypeDef,
     ScopingTypeDef,
     DescribeBucketsResponseTypeDef,
     ResourcesAffectedTypeDef,
     ClassificationResultTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     PolicyDetailsTypeDef,
     JobSummaryTypeDef,
+    S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
-    CreateClassificationJobRequestRequestTypeDef,
     DescribeClassificationJobResponseTypeDef,
+    CreateClassificationJobRequestRequestTypeDef,
+    S3JobDefinitionUnionTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInvitationRequestRequestTypeDef:
+def get_value() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-macie2-2.5.2/README.md` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-macie2
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore macie2 type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-macie2"></a>
 
 # types-aiobotocore-macie2
 
 [![PyPI - types-aiobotocore-macie2](https://img.shields.io/pypi/v/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-macie2?color=blue)](https://pypistats.org/packages/types-aiobotocore-macie2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Macie2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [types-aiobotocore-macie2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +74,15 @@
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
@@ -418,20 +450,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_macie2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
@@ -440,14 +472,15 @@
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
     BatchGetCustomDataIdentifiersRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BucketCountByEffectivePermissionTypeDef,
     BucketCountByEncryptionTypeTypeDef,
     BucketCountBySharedAccessTypeTypeDef,
     BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef,
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketPolicyTypeDef,
     BucketServerSideEncryptionTypeDef,
@@ -458,166 +491,172 @@
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
-    CreateAllowListResponseTypeDef,
-    CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
-    CreateCustomDataIdentifierResponseTypeDef,
-    CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
-    CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
+    SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
+    CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMemberRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClassificationJobRequestRequestTypeDef,
     LastRunErrorStatusTypeDef,
     StatisticsTypeDef,
     UserPausedDetailsTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DetectedDataDetailsTypeDef,
     DetectionTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DomainDetailsTypeDef,
     EnableMacieRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     SeverityTypeDef,
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
-    GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
     SecurityHubConfigurationTypeDef,
     SortCriteriaTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
-    GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
     RevealConfigurationTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
-    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesOutputTypeDef,
+    SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
+    SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
-    S3BucketDefinitionForJobTypeDef,
-    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    S3BucketDefinitionForJobOutputTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
-    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
-    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
-    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
     ListFindingsFiltersRequestRequestTypeDef,
-    ListFindingsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListJobsFilterTermTypeDef,
-    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
     ListManagedDataIdentifiersRequestRequestTypeDef,
     ManagedDataIdentifierSummaryTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
     ListResourceProfileArtifactsRequestRequestTypeDef,
     ResourceProfileArtifactTypeDef,
-    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
     ListResourceProfileDetectionsRequestRequestTypeDef,
-    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
-    TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
-    UpdateFindingsFilterResponseTypeDef,
     UpdateMacieSessionRequestRequestTypeDef,
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
     AllowListCriteriaTypeDef,
-    ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
+    CreateAllowListResponseTypeDef,
+    CreateClassificationJobResponseTypeDef,
+    CreateCustomDataIdentifierResponseTypeDef,
+    CreateFindingsFilterResponseTypeDef,
+    CreateMemberResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    GetAutomatedDiscoveryConfigurationResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetMacieSessionResponseTypeDef,
+    GetMemberResponseTypeDef,
+    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
+    ListAllowListsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TestCustomDataIdentifierResponseTypeDef,
+    UpdateAllowListResponseTypeDef,
+    UpdateFindingsFilterResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
-    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
     GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
+    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
+    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
+    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
+    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
@@ -626,96 +665,111 @@
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
-    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
+    JobScheduleFrequencyOutputTypeDef,
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
+    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
+    TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
+    TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
     CreateAllowListRequestRequestTypeDef,
     GetAllowListResponseTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
+    GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
-    GetFindingsFilterResponseTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
     AssumedRoleTypeDef,
     FederatedUserTypeDef,
+    CriteriaForJobOutputTypeDef,
     CriteriaForJobTypeDef,
+    JobScopeTermOutputTypeDef,
     JobScopeTermTypeDef,
     BucketPublicAccessTypeDef,
     SearchResourcesResponseTypeDef,
     CustomDetectionTypeDef,
     DefaultDetectionTypeDef,
     SearchResourcesCriteriaBlockTypeDef,
     GetUsageStatisticsResponseTypeDef,
     UserIdentityTypeDef,
+    CriteriaBlockForJobOutputTypeDef,
     CriteriaBlockForJobTypeDef,
+    JobScopingBlockOutputTypeDef,
     JobScopingBlockTypeDef,
     BucketMetadataTypeDef,
     S3BucketTypeDef,
     CustomDataIdentifiersTypeDef,
     SensitiveDataItemTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     FindingActorTypeDef,
+    S3BucketCriteriaForJobOutputTypeDef,
     S3BucketCriteriaForJobTypeDef,
+    ScopingOutputTypeDef,
     ScopingTypeDef,
     DescribeBucketsResponseTypeDef,
     ResourcesAffectedTypeDef,
     ClassificationResultTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     PolicyDetailsTypeDef,
     JobSummaryTypeDef,
+    S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
-    CreateClassificationJobRequestRequestTypeDef,
     DescribeClassificationJobResponseTypeDef,
+    CreateClassificationJobRequestRequestTypeDef,
+    S3JobDefinitionUnionTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInvitationRequestRequestTypeDef:
+def get_value() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-macie2-2.5.2/setup.py` & `types-aiobotocore-macie2-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-macie2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_macie2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore macie2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore macie2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_macie2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/"
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/__init__.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/__init__.pyi` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/__main__.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Macie2 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Macie2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2\nOther"
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

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/client.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     CreateInvitationsResponseTypeDef,
     CreateMemberResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DescribeBucketsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetAllowListResponseTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     GetClassificationScopeResponseTypeDef,
@@ -88,15 +88,15 @@
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     GetUsageTotalsResponseTypeDef,
-    JobScheduleFrequencyTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
@@ -108,21 +108,21 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     RevealConfigurationTypeDef,
     S3ClassificationScopeUpdateTypeDef,
-    S3JobDefinitionTypeDef,
+    S3JobDefinitionUnionTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     SearchResourcesResponseTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SecurityHubConfigurationTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     SeverityLevelTypeDef,
     SortCriteriaTypeDef,
     SuppressDataIdentifierTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateFindingsFilterResponseTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
@@ -232,23 +232,23 @@
 
     async def create_classification_job(
         self,
         *,
         clientToken: str,
         jobType: JobTypeType,
         name: str,
-        s3JobDefinition: S3JobDefinitionTypeDef,
+        s3JobDefinition: S3JobDefinitionUnionTypeDef,
         allowListIds: Sequence[str] = ...,
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
-        scheduleFrequency: JobScheduleFrequencyTypeDef = ...,
+        scheduleFrequency: JobScheduleFrequencyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_classification_job)
@@ -275,15 +275,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_custom_data_identifier)
         """
 
     async def create_findings_filter(
         self,
         *,
         action: FindingsFilterActionType,
-        findingCriteria: FindingCriteriaTypeDef,
+        findingCriteria: FindingCriteriaUnionTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFindingsFilterResponseTypeDef:
         """
@@ -565,15 +565,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_custom_data_identifier)
         """
 
     async def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         size: int = ...,
         sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
@@ -760,15 +760,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_custom_data_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_custom_data_identifiers)
         """
 
     async def list_findings(
         self,
         *,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
@@ -990,15 +990,15 @@
     async def update_findings_filter(
         self,
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         name: str = ...,
         position: int = ...
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
@@ -1072,16 +1072,16 @@
         """
 
     async def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
-        excludes: SensitivityInspectionTemplateExcludesTypeDef = ...,
-        includes: SensitivityInspectionTemplateIncludesTypeDef = ...
+        excludes: SensitivityInspectionTemplateExcludesUnionTypeDef = ...,
+        includes: SensitivityInspectionTemplateIncludesUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/client.pyi` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     CreateInvitationsResponseTypeDef,
     CreateMemberResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DescribeBucketsResponseTypeDef,
     DescribeClassificationJobResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetAllowListResponseTypeDef,
     GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     GetClassificationScopeResponseTypeDef,
@@ -88,15 +88,15 @@
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
     GetUsageStatisticsResponseTypeDef,
     GetUsageTotalsResponseTypeDef,
-    JobScheduleFrequencyTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
@@ -108,21 +108,21 @@
     ListResourceProfileArtifactsResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
     RevealConfigurationTypeDef,
     S3ClassificationScopeUpdateTypeDef,
-    S3JobDefinitionTypeDef,
+    S3JobDefinitionUnionTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     SearchResourcesResponseTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SecurityHubConfigurationTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
     SeverityLevelTypeDef,
     SortCriteriaTypeDef,
     SuppressDataIdentifierTypeDef,
     TestCustomDataIdentifierResponseTypeDef,
     UpdateAllowListResponseTypeDef,
     UpdateFindingsFilterResponseTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
@@ -222,23 +222,23 @@
         """
     async def create_classification_job(
         self,
         *,
         clientToken: str,
         jobType: JobTypeType,
         name: str,
-        s3JobDefinition: S3JobDefinitionTypeDef,
+        s3JobDefinition: S3JobDefinitionUnionTypeDef,
         allowListIds: Sequence[str] = ...,
         customDataIdentifierIds: Sequence[str] = ...,
         description: str = ...,
         initialRun: bool = ...,
         managedDataIdentifierIds: Sequence[str] = ...,
         managedDataIdentifierSelector: ManagedDataIdentifierSelectorType = ...,
         samplingPercentage: int = ...,
-        scheduleFrequency: JobScheduleFrequencyTypeDef = ...,
+        scheduleFrequency: JobScheduleFrequencyUnionTypeDef = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateClassificationJobResponseTypeDef:
         """
         Creates and defines the settings for a classification job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_classification_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_classification_job)
@@ -263,15 +263,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.create_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#create_custom_data_identifier)
         """
     async def create_findings_filter(
         self,
         *,
         action: FindingsFilterActionType,
-        findingCriteria: FindingCriteriaTypeDef,
+        findingCriteria: FindingCriteriaUnionTypeDef,
         name: str,
         clientToken: str = ...,
         description: str = ...,
         position: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateFindingsFilterResponseTypeDef:
         """
@@ -525,15 +525,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_custom_data_identifier)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#get_custom_data_identifier)
         """
     async def get_finding_statistics(
         self,
         *,
         groupBy: GroupByType,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         size: int = ...,
         sortCriteria: FindingStatisticsSortCriteriaTypeDef = ...
     ) -> GetFindingStatisticsResponseTypeDef:
         """
         Retrieves (queries) aggregated statistical data about findings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.get_finding_statistics)
@@ -701,15 +701,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.list_custom_data_identifiers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#list_custom_data_identifiers)
         """
     async def list_findings(
         self,
         *,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         maxResults: int = ...,
         nextToken: str = ...,
         sortCriteria: SortCriteriaTypeDef = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Retrieves a subset of information about one or more findings.
 
@@ -911,15 +911,15 @@
     async def update_findings_filter(
         self,
         *,
         id: str,
         action: FindingsFilterActionType = ...,
         clientToken: str = ...,
         description: str = ...,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         name: str = ...,
         position: int = ...
     ) -> UpdateFindingsFilterResponseTypeDef:
         """
         Updates the criteria and other settings for a findings filter.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_findings_filter)
@@ -986,16 +986,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_reveal_configuration)
         """
     async def update_sensitivity_inspection_template(
         self,
         *,
         id: str,
         description: str = ...,
-        excludes: SensitivityInspectionTemplateExcludesTypeDef = ...,
-        includes: SensitivityInspectionTemplateIncludesTypeDef = ...
+        excludes: SensitivityInspectionTemplateExcludesUnionTypeDef = ...,
+        includes: SensitivityInspectionTemplateIncludesUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the settings for the sensitivity inspection template for an account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Client.update_sensitivity_inspection_template)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/client/#update_sensitivity_inspection_template)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/literals.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/literals.pyi` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/paginator.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from botocore.paginate import PageIterator
 
 from .literals import TimeRangeType
 from .type_defs import (
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketSortCriteriaTypeDef,
     DescribeBucketsResponseTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -123,15 +123,15 @@
     """
 
     def paginate(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         sortCriteria: BucketSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBucketsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#describebucketspaginator)
         """
 
 
@@ -143,30 +143,30 @@
 
     def paginate(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
         timeRange: TimeRangeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetUsageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#getusagestatisticspaginator)
         """
 
 
 class ListAllowListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listallowlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAllowListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listallowlistspaginator)
         """
 
 
@@ -177,45 +177,45 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         sortCriteria: ListJobsSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationjobspaginator)
         """
 
 
 class ListClassificationScopesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationscopespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClassificationScopesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationscopespaginator)
         """
 
 
 class ListCustomDataIdentifiersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listcustomdataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listcustomdataidentifierspaginator)
         """
 
 
@@ -224,137 +224,137 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
         """
 
 
 class ListFindingsFiltersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingsfilterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingsfilterspaginator)
         """
 
 
 class ListInvitationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listinvitationspaginator)
         """
 
 
 class ListManagedDataIdentifiersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmanageddataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmanageddataidentifierspaginator)
         """
 
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmemberspaginator)
         """
 
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listorganizationadminaccountspaginator)
         """
 
 
 class ListResourceProfileArtifactsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofileartifactspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceProfileArtifactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofileartifactspaginator)
         """
 
 
 class ListResourceProfileDetectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofiledetectionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceProfileDetectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofiledetectionspaginator)
         """
 
 
 class ListSensitivityInspectionTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSensitivityInspectionTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
         """
 
 
@@ -365,13 +365,13 @@
     """
 
     def paginate(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/paginator.pyi` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/paginator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 from botocore.paginate import PageIterator
 
 from .literals import TimeRangeType
 from .type_defs import (
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketSortCriteriaTypeDef,
     DescribeBucketsResponseTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListAllowListsResponseTypeDef,
     ListClassificationJobsResponseTypeDef,
     ListClassificationScopesResponseTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
@@ -120,15 +120,15 @@
     """
 
     def paginate(
         self,
         *,
         criteria: Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef] = ...,
         sortCriteria: BucketSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBucketsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.DescribeBuckets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#describebucketspaginator)
         """
 
 class GetUsageStatisticsPaginator(AioPaginator):
@@ -139,29 +139,29 @@
 
     def paginate(
         self,
         *,
         filterBy: Sequence[UsageStatisticsFilterTypeDef] = ...,
         sortBy: UsageStatisticsSortByTypeDef = ...,
         timeRange: TimeRangeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetUsageStatisticsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.GetUsageStatistics.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#getusagestatisticspaginator)
         """
 
 class ListAllowListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listallowlistspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAllowListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListAllowLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listallowlistspaginator)
         """
 
 class ListClassificationJobsPaginator(AioPaginator):
@@ -171,43 +171,43 @@
     """
 
     def paginate(
         self,
         *,
         filterCriteria: ListJobsFilterCriteriaTypeDef = ...,
         sortCriteria: ListJobsSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClassificationJobsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationJobs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationjobspaginator)
         """
 
 class ListClassificationScopesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationscopespaginator)
     """
 
     def paginate(
-        self, *, name: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, name: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListClassificationScopesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListClassificationScopes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listclassificationscopespaginator)
         """
 
 class ListCustomDataIdentifiersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listcustomdataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCustomDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListCustomDataIdentifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listcustomdataidentifierspaginator)
         """
 
 class ListFindingsPaginator(AioPaginator):
@@ -215,129 +215,129 @@
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
-        findingCriteria: FindingCriteriaTypeDef = ...,
+        findingCriteria: FindingCriteriaUnionTypeDef = ...,
         sortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingspaginator)
         """
 
 class ListFindingsFiltersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingsfilterspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListFindingsFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listfindingsfilterspaginator)
         """
 
 class ListInvitationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listinvitationspaginator)
         """
 
 class ListManagedDataIdentifiersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmanageddataidentifierspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListManagedDataIdentifiersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListManagedDataIdentifiers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmanageddataidentifierspaginator)
         """
 
 class ListMembersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmemberspaginator)
     """
 
     def paginate(
-        self, *, onlyAssociated: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, onlyAssociated: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listorganizationadminaccountspaginator)
         """
 
 class ListResourceProfileArtifactsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofileartifactspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceProfileArtifactsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileArtifacts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofileartifactspaginator)
         """
 
 class ListResourceProfileDetectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofiledetectionspaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceProfileDetectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListResourceProfileDetections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listresourceprofiledetectionspaginator)
         """
 
 class ListSensitivityInspectionTemplatesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSensitivityInspectionTemplatesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.ListSensitivityInspectionTemplates.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#listsensitivityinspectiontemplatespaginator)
         """
 
 class SearchResourcesPaginator(AioPaginator):
@@ -347,13 +347,13 @@
     """
 
     def paginate(
         self,
         *,
         bucketCriteria: SearchResourcesBucketCriteriaTypeDef = ...,
         sortCriteria: SearchResourcesSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2.Paginator.SearchResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/paginators/#searchresourcespaginator)
         """
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/type_defs.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_macie2.type_defs import AcceptInvitationRequestRequestTypeDef
 
-    data: AcceptInvitationRequestRequestTypeDef = {...}
+    data: AcceptInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AllowListStatusCodeType,
     AllowsUnencryptedObjectUploadsType,
     AutomatedDiscoveryStatusType,
     AvailabilityCodeType,
@@ -88,14 +88,15 @@
     "AllowListStatusTypeDef",
     "AllowListSummaryTypeDef",
     "ApiCallDetailsTypeDef",
     "AwsAccountTypeDef",
     "AwsServiceTypeDef",
     "BatchGetCustomDataIdentifierSummaryTypeDef",
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BucketCountByEffectivePermissionTypeDef",
     "BucketCountByEncryptionTypeTypeDef",
     "BucketCountBySharedAccessTypeTypeDef",
     "BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef",
     "BucketCriteriaAdditionalPropertiesTypeDef",
     "BucketPolicyTypeDef",
     "BucketServerSideEncryptionTypeDef",
@@ -106,166 +107,172 @@
     "ReplicationDetailsTypeDef",
     "BucketSortCriteriaTypeDef",
     "SensitivityAggregationsTypeDef",
     "CellTypeDef",
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
-    "CreateAllowListResponseTypeDef",
-    "CreateClassificationJobResponseTypeDef",
     "SeverityLevelTypeDef",
-    "CreateCustomDataIdentifierResponseTypeDef",
-    "CreateFindingsFilterResponseTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
-    "CreateMemberResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
+    "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
+    "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMemberRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClassificationJobRequestRequestTypeDef",
     "LastRunErrorStatusTypeDef",
     "StatisticsTypeDef",
     "UserPausedDetailsTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
     "DetectedDataDetailsTypeDef",
     "DetectionTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "EnableMacieRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "FindingStatisticsSortCriteriaTypeDef",
     "SeverityTypeDef",
     "FindingsFilterListItemTypeDef",
     "InvitationTypeDef",
     "GetAllowListRequestRequestTypeDef",
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
     "GetBucketStatisticsRequestRequestTypeDef",
     "GetClassificationScopeRequestRequestTypeDef",
     "GetCustomDataIdentifierRequestRequestTypeDef",
     "GroupCountTypeDef",
     "GetFindingsFilterRequestRequestTypeDef",
     "SecurityHubConfigurationTypeDef",
     "SortCriteriaTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "GetMacieSessionResponseTypeDef",
     "GetMemberRequestRequestTypeDef",
-    "GetMemberResponseTypeDef",
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
     "RevealConfigurationTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    "SensitivityInspectionTemplateIncludesTypeDef",
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
+    "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
-    "S3BucketDefinitionForJobTypeDef",
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    "S3BucketDefinitionForJobOutputTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
     "ListFindingsFiltersRequestRequestTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListJobsFilterTermTypeDef",
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     "ManagedDataIdentifierSummaryTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "MemberTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
     "ListResourceProfileArtifactsRequestRequestTypeDef",
     "ResourceProfileArtifactTypeDef",
-    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
     "ListResourceProfileDetectionsRequestRequestTypeDef",
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagValuePairTypeDef",
     "TestCustomDataIdentifierRequestRequestTypeDef",
-    "TestCustomDataIdentifierResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAllowListResponseTypeDef",
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     "UpdateClassificationJobRequestRequestTypeDef",
-    "UpdateFindingsFilterResponseTypeDef",
     "UpdateMacieSessionRequestRequestTypeDef",
     "UpdateMemberSessionRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateResourceProfileRequestRequestTypeDef",
     "UserIdentityRootTypeDef",
     "CreateMemberRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
     "AllowListCriteriaTypeDef",
-    "ListAllowListsResponseTypeDef",
     "FindingActionTypeDef",
     "BatchGetCustomDataIdentifiersResponseTypeDef",
+    "CreateAllowListResponseTypeDef",
+    "CreateClassificationJobResponseTypeDef",
+    "CreateCustomDataIdentifierResponseTypeDef",
+    "CreateFindingsFilterResponseTypeDef",
+    "CreateMemberResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetMacieSessionResponseTypeDef",
+    "GetMemberResponseTypeDef",
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    "ListAllowListsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TestCustomDataIdentifierResponseTypeDef",
+    "UpdateAllowListResponseTypeDef",
+    "UpdateFindingsFilterResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "MatchingBucketTypeDef",
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "DescribeBucketsRequestRequestTypeDef",
     "BucketStatisticsBySensitivityTypeDef",
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
     "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "GetSensitiveDataOccurrencesResponseTypeDef",
     "ListResourceProfileDetectionsResponseTypeDef",
     "ListFindingsFiltersResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetFindingStatisticsResponseTypeDef",
@@ -274,90 +281,105 @@
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
     "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
-    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
+    "JobScheduleFrequencyOutputTypeDef",
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
+    "SensitivityInspectionTemplateExcludesUnionTypeDef",
+    "SensitivityInspectionTemplateIncludesUnionTypeDef",
+    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
+    "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
+    "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
     "CreateAllowListRequestRequestTypeDef",
     "GetAllowListResponseTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
+    "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
-    "GetFindingsFilterResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
+    "JobScheduleFrequencyUnionTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
     "AssumedRoleTypeDef",
     "FederatedUserTypeDef",
+    "CriteriaForJobOutputTypeDef",
     "CriteriaForJobTypeDef",
+    "JobScopeTermOutputTypeDef",
     "JobScopeTermTypeDef",
     "BucketPublicAccessTypeDef",
     "SearchResourcesResponseTypeDef",
     "CustomDetectionTypeDef",
     "DefaultDetectionTypeDef",
     "SearchResourcesCriteriaBlockTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "UserIdentityTypeDef",
+    "CriteriaBlockForJobOutputTypeDef",
     "CriteriaBlockForJobTypeDef",
+    "JobScopingBlockOutputTypeDef",
     "JobScopingBlockTypeDef",
     "BucketMetadataTypeDef",
     "S3BucketTypeDef",
     "CustomDataIdentifiersTypeDef",
     "SensitiveDataItemTypeDef",
     "SearchResourcesBucketCriteriaTypeDef",
     "FindingActorTypeDef",
+    "S3BucketCriteriaForJobOutputTypeDef",
     "S3BucketCriteriaForJobTypeDef",
+    "ScopingOutputTypeDef",
     "ScopingTypeDef",
     "DescribeBucketsResponseTypeDef",
     "ResourcesAffectedTypeDef",
     "ClassificationResultTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "PolicyDetailsTypeDef",
     "JobSummaryTypeDef",
+    "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
-    "CreateClassificationJobRequestRequestTypeDef",
     "DescribeClassificationJobResponseTypeDef",
+    "CreateClassificationJobRequestRequestTypeDef",
+    "S3JobDefinitionUnionTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -502,14 +524,25 @@
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
     {
         "ids": Sequence[str],
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
 BucketCountByEffectivePermissionTypeDef = TypedDict(
     "BucketCountByEffectivePermissionTypeDef",
     {
         "publiclyAccessible": int,
         "publiclyReadable": int,
         "publiclyWritable": int,
         "unknown": int,
@@ -698,57 +731,22 @@
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
-CreateAllowListResponseTypeDef = TypedDict(
-    "CreateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateClassificationJobResponseTypeDef = TypedDict(
-    "CreateClassificationJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SeverityLevelTypeDef = TypedDict(
     "SeverityLevelTypeDef",
     {
         "occurrencesThreshold": int,
         "severity": DataIdentifierSeverityType,
     },
 )
 
-CreateCustomDataIdentifierResponseTypeDef = TypedDict(
-    "CreateCustomDataIdentifierResponseTypeDef",
-    {
-        "customDataIdentifierId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFindingsFilterResponseTypeDef = TypedDict(
-    "CreateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateInvitationsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInvitationsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 _OptionalCreateInvitationsRequestRequestTypeDef = TypedDict(
@@ -773,40 +771,56 @@
         "accountId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
     total=False,
 )
 
-CreateMemberResponseTypeDef = TypedDict(
-    "CreateMemberResponseTypeDef",
+CreateSampleFindingsRequestRequestTypeDef = TypedDict(
+    "CreateSampleFindingsRequestRequestTypeDef",
     {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "findingTypes": Sequence[FindingTypeType],
     },
+    total=False,
 )
 
-CreateSampleFindingsRequestRequestTypeDef = TypedDict(
-    "CreateSampleFindingsRequestRequestTypeDef",
+SimpleCriterionForJobOutputTypeDef = TypedDict(
+    "SimpleCriterionForJobOutputTypeDef",
     {
-        "findingTypes": Sequence[FindingTypeType],
+        "comparator": JobComparatorType,
+        "key": SimpleCriterionKeyForJobType,
+        "values": List[str],
     },
     total=False,
 )
 
 SimpleCriterionForJobTypeDef = TypedDict(
     "SimpleCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "key": SimpleCriterionKeyForJobType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+CriterionAdditionalPropertiesOutputTypeDef = TypedDict(
+    "CriterionAdditionalPropertiesOutputTypeDef",
+    {
+        "eq": List[str],
+        "eqExactMatch": List[str],
+        "gt": int,
+        "gte": int,
+        "lt": int,
+        "lte": int,
+        "neq": List[str],
+    },
+    total=False,
+)
+
 CriterionAdditionalPropertiesTypeDef = TypedDict(
     "CriterionAdditionalPropertiesTypeDef",
     {
         "eq": Sequence[str],
         "eqExactMatch": Sequence[str],
         "gt": int,
         "gte": int,
@@ -881,14 +895,24 @@
 DeleteMemberRequestRequestTypeDef = TypedDict(
     "DeleteMemberRequestRequestTypeDef",
     {
         "id": str,
     },
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
 DescribeClassificationJobRequestRequestTypeDef = TypedDict(
     "DescribeClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -915,23 +939,14 @@
         "jobExpiresAt": datetime,
         "jobImminentExpirationHealthEventArn": str,
         "jobPausedAt": datetime,
     },
     total=False,
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "autoEnable": bool,
-        "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectedDataDetailsTypeDef = TypedDict(
     "DetectedDataDetailsTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1046,27 +1061,14 @@
 GetAllowListRequestRequestTypeDef = TypedDict(
     "GetAllowListRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
-    {
-        "classificationScopeId": str,
-        "disabledAt": datetime,
-        "firstEnabledAt": datetime,
-        "lastUpdatedAt": datetime,
-        "sensitivityInspectionTemplateId": str,
-        "status": AutomatedDiscoveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBucketStatisticsRequestRequestTypeDef = TypedDict(
     "GetBucketStatisticsRequestRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
@@ -1114,57 +1116,21 @@
     {
         "attributeName": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "invitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMacieSessionResponseTypeDef = TypedDict(
-    "GetMacieSessionResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "findingPublishingFrequency": FindingPublishingFrequencyType,
-        "serviceRole": str,
-        "status": MacieStatusType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMemberRequestRequestTypeDef = TypedDict(
     "GetMemberRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetMemberResponseTypeDef = TypedDict(
-    "GetMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "administratorAccountId": str,
-        "arn": str,
-        "email": str,
-        "invitedAt": datetime,
-        "masterAccountId": str,
-        "relationshipStatus": RelationshipStatusType,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceProfileRequestRequestTypeDef = TypedDict(
     "GetResourceProfileRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1208,23 +1174,14 @@
 GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 
-GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
-    {
-        "code": AvailabilityCodeType,
-        "reasons": List[UnavailabilityReasonCodeType],
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
@@ -1240,24 +1197,24 @@
 GetSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesTypeDef",
+SensitivityInspectionTemplateExcludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
     {
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesTypeDef",
+SensitivityInspectionTemplateIncludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     {
         "allowListIds": List[str],
         "customDataIdentifierIds": List[str],
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
@@ -1359,38 +1316,40 @@
     "WeeklyScheduleTypeDef",
     {
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-SimpleScopeTermTypeDef = TypedDict(
-    "SimpleScopeTermTypeDef",
+SimpleScopeTermOutputTypeDef = TypedDict(
+    "SimpleScopeTermOutputTypeDef",
     {
         "comparator": JobComparatorType,
         "key": ScopeFilterKeyType,
-        "values": Sequence[str],
+        "values": List[str],
     },
     total=False,
 )
 
-S3BucketDefinitionForJobTypeDef = TypedDict(
-    "S3BucketDefinitionForJobTypeDef",
+SimpleScopeTermTypeDef = TypedDict(
+    "SimpleScopeTermTypeDef",
     {
-        "accountId": str,
-        "buckets": Sequence[str],
+        "comparator": JobComparatorType,
+        "key": ScopeFilterKeyType,
+        "values": Sequence[str],
     },
+    total=False,
 )
 
-ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+S3BucketDefinitionForJobOutputTypeDef = TypedDict(
+    "S3BucketDefinitionForJobOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "accountId": str,
+        "buckets": List[str],
     },
-    total=False,
 )
 
 ListAllowListsRequestRequestTypeDef = TypedDict(
     "ListAllowListsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
@@ -1403,83 +1362,41 @@
     {
         "attributeName": ListJobsSortAttributeNameType,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClassificationScopesRequestRequestTypeDef = TypedDict(
     "ListClassificationScopesRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListCustomDataIdentifiersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFindingsFiltersRequestRequestTypeDef = TypedDict(
     "ListFindingsFiltersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1491,22 +1408,14 @@
         "comparator": JobComparatorType,
         "key": ListJobsFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1516,23 +1425,14 @@
     {
         "category": SensitiveDataItemCategoryType,
         "id": str,
     },
     total=False,
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": str,
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
         "onlyAssociated": str,
     },
@@ -1551,53 +1451,23 @@
         "relationshipStatus": RelationshipStatusType,
         "tags": Dict[str, str],
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
-    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileArtifactsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
@@ -1634,40 +1504,14 @@
 
 class ResourceProfileArtifactTypeDef(
     _RequiredResourceProfileArtifactTypeDef, _OptionalResourceProfileArtifactTypeDef
 ):
     pass
 
 
-_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "resourceArn": str,
-        },
-    )
-)
-_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
-    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileDetectionsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
@@ -1683,22 +1527,14 @@
 class ListResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredListResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalListResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
 
-ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSensitivityInspectionTemplatesRequestRequestTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1716,22 +1552,14 @@
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
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "end": int,
         "start": int,
         "startColumn": int,
     },
@@ -1743,32 +1571,19 @@
     {
         "jsonPath": str,
         "recordIndex": int,
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3BucketDefinitionForJobTypeDef = TypedDict(
+    "S3BucketDefinitionForJobTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accountId": str,
+        "buckets": Sequence[str],
     },
 )
 
 S3BucketOwnerTypeDef = TypedDict(
     "S3BucketOwnerTypeDef",
     {
         "displayName": str,
@@ -1825,14 +1640,32 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    {
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
+SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesTypeDef",
+    {
+        "allowListIds": Sequence[str],
+        "customDataIdentifierIds": Sequence[str],
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
 ServiceLimitTypeDef = TypedDict(
     "ServiceLimitTypeDef",
     {
         "isServiceLimited": bool,
         "unit": Literal["TERABYTES"],
         "value": int,
     },
@@ -1916,39 +1749,22 @@
 class TestCustomDataIdentifierRequestRequestTypeDef(
     _RequiredTestCustomDataIdentifierRequestRequestTypeDef,
     _OptionalTestCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
 
-TestCustomDataIdentifierResponseTypeDef = TypedDict(
-    "TestCustomDataIdentifierResponseTypeDef",
-    {
-        "matchCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAllowListResponseTypeDef = TypedDict(
-    "UpdateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     {
         "status": AutomatedDiscoveryStatusType,
     },
 )
 
@@ -1956,23 +1772,14 @@
     "UpdateClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
         "jobStatus": JobStatusType,
     },
 )
 
-UpdateFindingsFilterResponseTypeDef = TypedDict(
-    "UpdateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateMacieSessionRequestRequestTypeDef = TypedDict(
     "UpdateMacieSessionRequestRequestTypeDef",
     {
         "findingPublishingFrequency": FindingPublishingFrequencyType,
         "status": MacieStatusType,
     },
     total=False,
@@ -2050,56 +1857,209 @@
     "AccountLevelPermissionsTypeDef",
     {
         "blockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "adminAccounts": List[AdminAccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AllowListCriteriaTypeDef = TypedDict(
     "AllowListCriteriaTypeDef",
     {
         "regex": str,
         "s3WordsList": S3WordsListTypeDef,
     },
     total=False,
 )
 
-ListAllowListsResponseTypeDef = TypedDict(
-    "ListAllowListsResponseTypeDef",
-    {
-        "allowLists": List[AllowListSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FindingActionTypeDef = TypedDict(
     "FindingActionTypeDef",
     {
         "actionType": Literal["AWS_API_CALL"],
         "apiCallDetails": ApiCallDetailsTypeDef,
     },
     total=False,
 )
 
 BatchGetCustomDataIdentifiersResponseTypeDef = TypedDict(
     "BatchGetCustomDataIdentifiersResponseTypeDef",
     {
         "customDataIdentifiers": List[BatchGetCustomDataIdentifierSummaryTypeDef],
         "notFoundIdentifierIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAllowListResponseTypeDef = TypedDict(
+    "CreateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateClassificationJobResponseTypeDef = TypedDict(
+    "CreateClassificationJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDataIdentifierResponseTypeDef = TypedDict(
+    "CreateCustomDataIdentifierResponseTypeDef",
+    {
+        "customDataIdentifierId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsFilterResponseTypeDef = TypedDict(
+    "CreateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberResponseTypeDef = TypedDict(
+    "CreateMemberResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "autoEnable": bool,
+        "maxAccountLimitReached": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    {
+        "classificationScopeId": str,
+        "disabledAt": datetime,
+        "firstEnabledAt": datetime,
+        "lastUpdatedAt": datetime,
+        "sensitivityInspectionTemplateId": str,
+        "status": AutomatedDiscoveryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "invitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMacieSessionResponseTypeDef = TypedDict(
+    "GetMacieSessionResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "findingPublishingFrequency": FindingPublishingFrequencyType,
+        "serviceRole": str,
+        "status": MacieStatusType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMemberResponseTypeDef = TypedDict(
+    "GetMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "administratorAccountId": str,
+        "arn": str,
+        "email": str,
+        "invitedAt": datetime,
+        "masterAccountId": str,
+        "relationshipStatus": RelationshipStatusType,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    {
+        "code": AvailabilityCodeType,
+        "reasons": List[UnavailabilityReasonCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAllowListsResponseTypeDef = TypedDict(
+    "ListAllowListsResponseTypeDef",
+    {
+        "allowLists": List[AllowListSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "adminAccounts": List[AdminAccountTypeDef],
+        "nextToken": str,
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
+TestCustomDataIdentifierResponseTypeDef = TypedDict(
+    "TestCustomDataIdentifierResponseTypeDef",
+    {
+        "matchCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAllowListResponseTypeDef = TypedDict(
+    "UpdateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFindingsFilterResponseTypeDef = TypedDict(
+    "UpdateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "accessControlList": AccessControlListTypeDef,
@@ -2127,24 +2087,14 @@
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
     },
     total=False,
 )
 
-DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
-    {
-        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
-        "sortCriteria": BucketSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeBucketsRequestRequestTypeDef = TypedDict(
     "DescribeBucketsRequestRequestTypeDef",
     {
         "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
         "maxResults": int,
         "nextToken": str,
         "sortCriteria": BucketSortCriteriaTypeDef,
@@ -2172,15 +2122,15 @@
 )
 
 ListClassificationScopesResponseTypeDef = TypedDict(
     "ListClassificationScopesResponseTypeDef",
     {
         "classificationScopes": List[ClassificationScopeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDataIdentifierRequestRequestTypeDef",
     {
         "name": str,
@@ -2220,40 +2170,48 @@
         "ignoreWords": List[str],
         "keywords": List[str],
         "maximumMatchDistance": int,
         "name": str,
         "regex": str,
         "severityLevels": List[SeverityLevelTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInvitationsResponseTypeDef = TypedDict(
     "CreateInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
     },
+    total=False,
 )
 
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "criterion": Mapping[str, CriterionAdditionalPropertiesTypeDef],
     },
@@ -2261,84 +2219,216 @@
 )
 
 ListCustomDataIdentifiersResponseTypeDef = TypedDict(
     "ListCustomDataIdentifiersResponseTypeDef",
     {
         "items": List[CustomDataIdentifierSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    {
+        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
+        "sortCriteria": BucketSortCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    {
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
+    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "resourceArn": str,
+        },
+    )
+)
+_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
+    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+):
+    pass
+
+
+ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 GetSensitiveDataOccurrencesResponseTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesResponseTypeDef",
     {
         "error": str,
         "sensitiveDataOccurrences": Dict[str, List[DetectedDataDetailsTypeDef]],
         "status": RevealRequestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceProfileDetectionsResponseTypeDef = TypedDict(
     "ListResourceProfileDetectionsResponseTypeDef",
     {
         "detections": List[DetectionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsFiltersResponseTypeDef = TypedDict(
     "ListFindingsFiltersResponseTypeDef",
     {
         "findingsFilterListItems": List[FindingsFilterListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "administrator": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "master": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "invitations": List[InvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingStatisticsResponseTypeDef = TypedDict(
     "GetFindingStatisticsResponseTypeDef",
     {
         "countsByGroup": List[GroupCountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsPublicationConfigurationResponseTypeDef = TypedDict(
     "GetFindingsPublicationConfigurationResponseTypeDef",
     {
         "securityHubConfiguration": SecurityHubConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutFindingsPublicationConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -2371,38 +2461,38 @@
 GetResourceProfileResponseTypeDef = TypedDict(
     "GetResourceProfileResponseTypeDef",
     {
         "profileUpdatedAt": datetime,
         "sensitivityScore": int,
         "sensitivityScoreOverridden": bool,
         "statistics": ResourceStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRevealConfigurationResponseTypeDef = TypedDict(
     "GetRevealConfigurationResponseTypeDef",
     {
         "configuration": RevealConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRevealConfigurationRequestRequestTypeDef",
     {
         "configuration": RevealConfigurationTypeDef,
     },
 )
 
 UpdateRevealConfigurationResponseTypeDef = TypedDict(
     "UpdateRevealConfigurationResponseTypeDef",
     {
         "configuration": RevealConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef = TypedDict(
     "_RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     {
         "findingId": str,
@@ -2424,53 +2514,29 @@
     pass
 
 
 GetSensitivityInspectionTemplateResponseTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+        "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
-    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-):
-    pass
-
-
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "GetUsageStatisticsRequestRequestTypeDef",
     {
@@ -2484,15 +2550,15 @@
 )
 
 GetUsageTotalsResponseTypeDef = TypedDict(
     "GetUsageTotalsResponseTypeDef",
     {
         "timeRange": TimeRangeType,
         "usageTotals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IpAddressDetailsTypeDef = TypedDict(
     "IpAddressDetailsTypeDef",
     {
         "ipAddressV4": str,
@@ -2500,14 +2566,24 @@
         "ipCountry": IpCountryTypeDef,
         "ipGeoLocation": IpGeoLocationTypeDef,
         "ipOwner": IpOwnerTypeDef,
     },
     total=False,
 )
 
+JobScheduleFrequencyOutputTypeDef = TypedDict(
+    "JobScheduleFrequencyOutputTypeDef",
+    {
+        "dailySchedule": Dict[str, Any],
+        "monthlySchedule": MonthlyScheduleTypeDef,
+        "weeklySchedule": WeeklyScheduleTypeDef,
+    },
+    total=False,
+)
+
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
         "dailySchedule": Mapping[str, Any],
         "monthlySchedule": MonthlyScheduleTypeDef,
         "weeklySchedule": WeeklyScheduleTypeDef,
     },
@@ -2524,42 +2600,42 @@
 )
 
 ListManagedDataIdentifiersResponseTypeDef = TypedDict(
     "ListManagedDataIdentifiersResponseTypeDef",
     {
         "items": List[ManagedDataIdentifierSummaryTypeDef],
         "nextToken": str,
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
 
 ListResourceProfileArtifactsResponseTypeDef = TypedDict(
     "ListResourceProfileArtifactsResponseTypeDef",
     {
         "artifacts": List[ResourceProfileArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSensitivityInspectionTemplatesResponseTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "sensitivityInspectionTemplates": List[SensitivityInspectionTemplatesEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "lineRange": RangeTypeDef,
@@ -2607,14 +2683,44 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateExcludesTypeDef, SensitivityInspectionTemplateExcludesOutputTypeDef
+]
+SensitivityInspectionTemplateIncludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateIncludesTypeDef, SensitivityInspectionTemplateIncludesOutputTypeDef
+]
+_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "description": str,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
+    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+):
+    pass
+
+
 UsageByAccountTypeDef = TypedDict(
     "UsageByAccountTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedCost": str,
         "serviceLimit": ServiceLimitTypeDef,
         "type": UsageTypeType,
@@ -2649,23 +2755,43 @@
 class UpdateResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredUpdateResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalUpdateResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
 
+TagCriterionForJobOutputTypeDef = TypedDict(
+    "TagCriterionForJobOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "tagValues": List[TagCriterionPairForJobTypeDef],
+    },
+    total=False,
+)
+
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "tagValues": Sequence[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
+TagScopeTermOutputTypeDef = TypedDict(
+    "TagScopeTermOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": str,
+        "tagValues": List[TagValuePairTypeDef],
+        "target": Literal["S3_OBJECT"],
+    },
+    total=False,
+)
+
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
@@ -2705,15 +2831,15 @@
         "criteria": AllowListCriteriaTypeDef,
         "description": str,
         "id": str,
         "name": str,
         "status": AllowListStatusTypeDef,
         "tags": Dict[str, str],
         "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAllowListRequestRequestTypeDef",
     {
         "criteria": AllowListCriteriaTypeDef,
@@ -2768,38 +2894,53 @@
         "classifiableSizeInBytes": int,
         "lastUpdated": datetime,
         "objectCount": int,
         "sizeInBytes": int,
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClassificationExportConfigurationResponseTypeDef = TypedDict(
     "GetClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
     },
 )
 
 PutClassificationExportConfigurationResponseTypeDef = TypedDict(
     "PutClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFindingsFilterResponseTypeDef = TypedDict(
+    "GetFindingsFilterResponseTypeDef",
+    {
+        "action": FindingsFilterActionType,
+        "arn": str,
+        "description": str,
+        "findingCriteria": FindingCriteriaOutputTypeDef,
+        "id": str,
+        "name": str,
+        "position": int,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
         "action": FindingsFilterActionType,
@@ -2822,14 +2963,15 @@
 class CreateFindingsFilterRequestRequestTypeDef(
     _RequiredCreateFindingsFilterRequestRequestTypeDef,
     _OptionalCreateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
 
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingStatisticsRequestRequestTypeDef",
     {
         "groupBy": GroupByType,
     },
 )
 _OptionalGetFindingStatisticsRequestRequestTypeDef = TypedDict(
@@ -2846,35 +2988,20 @@
 class GetFindingStatisticsRequestRequestTypeDef(
     _RequiredGetFindingStatisticsRequestRequestTypeDef,
     _OptionalGetFindingStatisticsRequestRequestTypeDef,
 ):
     pass
 
 
-GetFindingsFilterResponseTypeDef = TypedDict(
-    "GetFindingsFilterResponseTypeDef",
-    {
-        "action": FindingsFilterActionType,
-        "arn": str,
-        "description": str,
-        "findingCriteria": FindingCriteriaTypeDef,
-        "id": str,
-        "name": str,
-        "position": int,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2909,20 +3036,23 @@
 class UpdateFindingsFilterRequestRequestTypeDef(
     _RequiredUpdateFindingsFilterRequestRequestTypeDef,
     _OptionalUpdateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
 
+JobScheduleFrequencyUnionTypeDef = Union[
+    JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
+]
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListClassificationJobsRequestRequestTypeDef",
     {
@@ -2948,15 +3078,15 @@
 
 GetClassificationScopeResponseTypeDef = TypedDict(
     "GetClassificationScopeResponseTypeDef",
     {
         "id": str,
         "name": str,
         "s3": S3ClassificationScopeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateClassificationScopeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClassificationScopeRequestRequestTypeDef",
     {
         "id": str,
@@ -3018,23 +3148,41 @@
         "arn": str,
         "principalId": str,
         "sessionContext": SessionContextTypeDef,
     },
     total=False,
 )
 
+CriteriaForJobOutputTypeDef = TypedDict(
+    "CriteriaForJobOutputTypeDef",
+    {
+        "simpleCriterion": SimpleCriterionForJobOutputTypeDef,
+        "tagCriterion": TagCriterionForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 CriteriaForJobTypeDef = TypedDict(
     "CriteriaForJobTypeDef",
     {
         "simpleCriterion": SimpleCriterionForJobTypeDef,
         "tagCriterion": TagCriterionForJobTypeDef,
     },
     total=False,
 )
 
+JobScopeTermOutputTypeDef = TypedDict(
+    "JobScopeTermOutputTypeDef",
+    {
+        "simpleScopeTerm": SimpleScopeTermOutputTypeDef,
+        "tagScopeTerm": TagScopeTermOutputTypeDef,
+    },
+    total=False,
+)
+
 JobScopeTermTypeDef = TypedDict(
     "JobScopeTermTypeDef",
     {
         "simpleScopeTerm": SimpleScopeTermTypeDef,
         "tagScopeTerm": TagScopeTermTypeDef,
     },
     total=False,
@@ -3050,15 +3198,15 @@
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "matchingResources": List[MatchingResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDetectionTypeDef = TypedDict(
     "CustomDetectionTypeDef",
     {
         "arn": str,
@@ -3089,15 +3237,15 @@
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "nextToken": str,
         "records": List[UsageRecordTypeDef],
         "timeRange": TimeRangeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "assumedRole": AssumedRoleTypeDef,
@@ -3107,22 +3255,38 @@
         "iamUser": IamUserTypeDef,
         "root": UserIdentityRootTypeDef,
         "type": UserIdentityTypeType,
     },
     total=False,
 )
 
+CriteriaBlockForJobOutputTypeDef = TypedDict(
+    "CriteriaBlockForJobOutputTypeDef",
+    {
+        "and": List[CriteriaForJobOutputTypeDef],
+    },
+    total=False,
+)
+
 CriteriaBlockForJobTypeDef = TypedDict(
     "CriteriaBlockForJobTypeDef",
     {
         "and": Sequence[CriteriaForJobTypeDef],
     },
     total=False,
 )
 
+JobScopingBlockOutputTypeDef = TypedDict(
+    "JobScopingBlockOutputTypeDef",
+    {
+        "and": List[JobScopeTermOutputTypeDef],
+    },
+    total=False,
+)
+
 JobScopingBlockTypeDef = TypedDict(
     "JobScopingBlockTypeDef",
     {
         "and": Sequence[JobScopeTermTypeDef],
     },
     total=False,
 )
@@ -3209,38 +3373,56 @@
         "domainDetails": DomainDetailsTypeDef,
         "ipAddressDetails": IpAddressDetailsTypeDef,
         "userIdentity": UserIdentityTypeDef,
     },
     total=False,
 )
 
+S3BucketCriteriaForJobOutputTypeDef = TypedDict(
+    "S3BucketCriteriaForJobOutputTypeDef",
+    {
+        "excludes": CriteriaBlockForJobOutputTypeDef,
+        "includes": CriteriaBlockForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 S3BucketCriteriaForJobTypeDef = TypedDict(
     "S3BucketCriteriaForJobTypeDef",
     {
         "excludes": CriteriaBlockForJobTypeDef,
         "includes": CriteriaBlockForJobTypeDef,
     },
     total=False,
 )
 
+ScopingOutputTypeDef = TypedDict(
+    "ScopingOutputTypeDef",
+    {
+        "excludes": JobScopingBlockOutputTypeDef,
+        "includes": JobScopingBlockOutputTypeDef,
+    },
+    total=False,
+)
+
 ScopingTypeDef = TypedDict(
     "ScopingTypeDef",
     {
         "excludes": JobScopingBlockTypeDef,
         "includes": JobScopingBlockTypeDef,
     },
     total=False,
 )
 
 DescribeBucketsResponseTypeDef = TypedDict(
     "DescribeBucketsResponseTypeDef",
     {
         "buckets": List[BucketMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourcesAffectedTypeDef = TypedDict(
     "ResourcesAffectedTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
@@ -3274,15 +3456,15 @@
 )
 
 SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     {
         "bucketCriteria": SearchResourcesBucketCriteriaTypeDef,
         "sortCriteria": SearchResourcesSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 PolicyDetailsTypeDef = TypedDict(
     "PolicyDetailsTypeDef",
     {
@@ -3291,27 +3473,37 @@
     },
     total=False,
 )
 
 JobSummaryTypeDef = TypedDict(
     "JobSummaryTypeDef",
     {
-        "bucketCriteria": S3BucketCriteriaForJobTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobTypeDef],
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
         "createdAt": datetime,
         "jobId": str,
         "jobStatus": JobStatusType,
         "jobType": JobTypeType,
         "lastRunErrorStatus": LastRunErrorStatusTypeDef,
         "name": str,
         "userPausedDetails": UserPausedDetailsTypeDef,
     },
     total=False,
 )
 
+S3JobDefinitionOutputTypeDef = TypedDict(
+    "S3JobDefinitionOutputTypeDef",
+    {
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
+        "scoping": ScopingOutputTypeDef,
+    },
+    total=False,
+)
+
 S3JobDefinitionTypeDef = TypedDict(
     "S3JobDefinitionTypeDef",
     {
         "bucketCriteria": S3BucketCriteriaForJobTypeDef,
         "bucketDefinitions": Sequence[S3BucketDefinitionForJobTypeDef],
         "scoping": ScopingTypeDef,
     },
@@ -3331,15 +3523,43 @@
 )
 
 ListClassificationJobsResponseTypeDef = TypedDict(
     "ListClassificationJobsResponseTypeDef",
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeClassificationJobResponseTypeDef = TypedDict(
+    "DescribeClassificationJobResponseTypeDef",
+    {
+        "allowListIds": List[str],
+        "clientToken": str,
+        "createdAt": datetime,
+        "customDataIdentifierIds": List[str],
+        "description": str,
+        "initialRun": bool,
+        "jobArn": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "jobType": JobTypeType,
+        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
+        "lastRunTime": datetime,
+        "managedDataIdentifierIds": List[str],
+        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
+        "name": str,
+        "s3JobDefinition": S3JobDefinitionOutputTypeDef,
+        "samplingPercentage": int,
+        "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
+        "statistics": StatisticsTypeDef,
+        "tags": Dict[str, str],
+        "userPausedDetails": UserPausedDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -3368,42 +3588,15 @@
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeClassificationJobResponseTypeDef = TypedDict(
-    "DescribeClassificationJobResponseTypeDef",
-    {
-        "allowListIds": List[str],
-        "clientToken": str,
-        "createdAt": datetime,
-        "customDataIdentifierIds": List[str],
-        "description": str,
-        "initialRun": bool,
-        "jobArn": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "jobType": JobTypeType,
-        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
-        "lastRunTime": datetime,
-        "managedDataIdentifierIds": List[str],
-        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
-        "name": str,
-        "s3JobDefinition": S3JobDefinitionTypeDef,
-        "samplingPercentage": int,
-        "scheduleFrequency": JobScheduleFrequencyTypeDef,
-        "statistics": StatisticsTypeDef,
-        "tags": Dict[str, str],
-        "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+S3JobDefinitionUnionTypeDef = Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef]
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
@@ -3425,10 +3618,10 @@
     total=False,
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/type_defs.pyi` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_macie2.type_defs import AcceptInvitationRequestRequestTypeDef
 
-    data: AcceptInvitationRequestRequestTypeDef = {...}
+    data: AcceptInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AllowListStatusCodeType,
     AllowsUnencryptedObjectUploadsType,
     AutomatedDiscoveryStatusType,
     AvailabilityCodeType,
@@ -87,14 +87,15 @@
     "AllowListStatusTypeDef",
     "AllowListSummaryTypeDef",
     "ApiCallDetailsTypeDef",
     "AwsAccountTypeDef",
     "AwsServiceTypeDef",
     "BatchGetCustomDataIdentifierSummaryTypeDef",
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "BucketCountByEffectivePermissionTypeDef",
     "BucketCountByEncryptionTypeTypeDef",
     "BucketCountBySharedAccessTypeTypeDef",
     "BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef",
     "BucketCriteriaAdditionalPropertiesTypeDef",
     "BucketPolicyTypeDef",
     "BucketServerSideEncryptionTypeDef",
@@ -105,166 +106,172 @@
     "ReplicationDetailsTypeDef",
     "BucketSortCriteriaTypeDef",
     "SensitivityAggregationsTypeDef",
     "CellTypeDef",
     "S3DestinationTypeDef",
     "ClassificationResultStatusTypeDef",
     "ClassificationScopeSummaryTypeDef",
-    "CreateAllowListResponseTypeDef",
-    "CreateClassificationJobResponseTypeDef",
     "SeverityLevelTypeDef",
-    "CreateCustomDataIdentifierResponseTypeDef",
-    "CreateFindingsFilterResponseTypeDef",
     "CreateInvitationsRequestRequestTypeDef",
     "UnprocessedAccountTypeDef",
-    "CreateMemberResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
+    "SimpleCriterionForJobOutputTypeDef",
     "SimpleCriterionForJobTypeDef",
+    "CriterionAdditionalPropertiesOutputTypeDef",
     "CriterionAdditionalPropertiesTypeDef",
     "CustomDataIdentifierSummaryTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DeleteAllowListRequestRequestTypeDef",
     "DeleteCustomDataIdentifierRequestRequestTypeDef",
     "DeleteFindingsFilterRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMemberRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeClassificationJobRequestRequestTypeDef",
     "LastRunErrorStatusTypeDef",
     "StatisticsTypeDef",
     "UserPausedDetailsTypeDef",
-    "DescribeOrganizationConfigurationResponseTypeDef",
     "DetectedDataDetailsTypeDef",
     "DetectionTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
     "DisassociateMemberRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "EnableMacieRequestRequestTypeDef",
     "EnableOrganizationAdminAccountRequestRequestTypeDef",
     "FindingStatisticsSortCriteriaTypeDef",
     "SeverityTypeDef",
     "FindingsFilterListItemTypeDef",
     "InvitationTypeDef",
     "GetAllowListRequestRequestTypeDef",
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
     "GetBucketStatisticsRequestRequestTypeDef",
     "GetClassificationScopeRequestRequestTypeDef",
     "GetCustomDataIdentifierRequestRequestTypeDef",
     "GroupCountTypeDef",
     "GetFindingsFilterRequestRequestTypeDef",
     "SecurityHubConfigurationTypeDef",
     "SortCriteriaTypeDef",
-    "GetInvitationsCountResponseTypeDef",
-    "GetMacieSessionResponseTypeDef",
     "GetMemberRequestRequestTypeDef",
-    "GetMemberResponseTypeDef",
     "GetResourceProfileRequestRequestTypeDef",
     "ResourceStatisticsTypeDef",
     "RevealConfigurationTypeDef",
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
     "WaiterConfigTypeDef",
     "GetSensitiveDataOccurrencesRequestRequestTypeDef",
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
-    "SensitivityInspectionTemplateExcludesTypeDef",
-    "SensitivityInspectionTemplateIncludesTypeDef",
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     "UsageStatisticsFilterTypeDef",
     "UsageStatisticsSortByTypeDef",
     "GetUsageTotalsRequestRequestTypeDef",
     "UsageTotalTypeDef",
     "IamUserTypeDef",
     "IpCityTypeDef",
     "IpCountryTypeDef",
     "IpGeoLocationTypeDef",
     "IpOwnerTypeDef",
     "MonthlyScheduleTypeDef",
     "WeeklyScheduleTypeDef",
+    "SimpleScopeTermOutputTypeDef",
     "SimpleScopeTermTypeDef",
-    "S3BucketDefinitionForJobTypeDef",
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    "S3BucketDefinitionForJobOutputTypeDef",
     "ListAllowListsRequestRequestTypeDef",
     "ListJobsSortCriteriaTypeDef",
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
     "ListClassificationScopesRequestRequestTypeDef",
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
     "ListCustomDataIdentifiersRequestRequestTypeDef",
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
     "ListFindingsFiltersRequestRequestTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
     "ListJobsFilterTermTypeDef",
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     "ManagedDataIdentifierSummaryTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
     "MemberTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
-    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
     "ListResourceProfileArtifactsRequestRequestTypeDef",
     "ResourceProfileArtifactTypeDef",
-    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
     "ListResourceProfileDetectionsRequestRequestTypeDef",
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     "SensitivityInspectionTemplatesEntryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "RangeTypeDef",
     "RecordTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "S3BucketDefinitionForJobTypeDef",
     "S3BucketOwnerTypeDef",
     "ServerSideEncryptionTypeDef",
     "S3ClassificationScopeExclusionTypeDef",
     "S3ClassificationScopeExclusionUpdateTypeDef",
     "SearchResourcesSimpleCriterionTypeDef",
     "SearchResourcesSortCriteriaTypeDef",
     "SearchResourcesTagCriterionPairTypeDef",
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    "SensitivityInspectionTemplateIncludesTypeDef",
     "ServiceLimitTypeDef",
     "SessionContextAttributesTypeDef",
     "SessionIssuerTypeDef",
     "SuppressDataIdentifierTypeDef",
     "TagCriterionPairForJobTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TagValuePairTypeDef",
     "TestCustomDataIdentifierRequestRequestTypeDef",
-    "TestCustomDataIdentifierResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateAllowListResponseTypeDef",
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     "UpdateClassificationJobRequestRequestTypeDef",
-    "UpdateFindingsFilterResponseTypeDef",
     "UpdateMacieSessionRequestRequestTypeDef",
     "UpdateMemberSessionRequestRequestTypeDef",
     "UpdateOrganizationConfigurationRequestRequestTypeDef",
     "UpdateResourceProfileRequestRequestTypeDef",
     "UserIdentityRootTypeDef",
     "CreateMemberRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
     "AllowListCriteriaTypeDef",
-    "ListAllowListsResponseTypeDef",
     "FindingActionTypeDef",
     "BatchGetCustomDataIdentifiersResponseTypeDef",
+    "CreateAllowListResponseTypeDef",
+    "CreateClassificationJobResponseTypeDef",
+    "CreateCustomDataIdentifierResponseTypeDef",
+    "CreateFindingsFilterResponseTypeDef",
+    "CreateMemberResponseTypeDef",
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetMacieSessionResponseTypeDef",
+    "GetMemberResponseTypeDef",
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    "ListAllowListsResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "TestCustomDataIdentifierResponseTypeDef",
+    "UpdateAllowListResponseTypeDef",
+    "UpdateFindingsFilterResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
     "MatchingBucketTypeDef",
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
     "DescribeBucketsRequestRequestTypeDef",
     "BucketStatisticsBySensitivityTypeDef",
     "ClassificationExportConfigurationTypeDef",
     "ListClassificationScopesResponseTypeDef",
     "CreateCustomDataIdentifierRequestRequestTypeDef",
     "GetCustomDataIdentifierResponseTypeDef",
     "CreateInvitationsResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ListCustomDataIdentifiersResponseTypeDef",
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    "ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
     "GetSensitiveDataOccurrencesResponseTypeDef",
     "ListResourceProfileDetectionsResponseTypeDef",
     "ListFindingsFiltersResponseTypeDef",
     "GetAdministratorAccountResponseTypeDef",
     "GetMasterAccountResponseTypeDef",
     "ListInvitationsResponseTypeDef",
     "GetFindingStatisticsResponseTypeDef",
@@ -273,90 +280,105 @@
     "GetFindingsRequestRequestTypeDef",
     "GetResourceProfileResponseTypeDef",
     "GetRevealConfigurationResponseTypeDef",
     "UpdateRevealConfigurationRequestRequestTypeDef",
     "UpdateRevealConfigurationResponseTypeDef",
     "GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     "GetSensitivityInspectionTemplateResponseTypeDef",
-    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     "GetUsageStatisticsRequestRequestTypeDef",
     "GetUsageTotalsResponseTypeDef",
     "IpAddressDetailsTypeDef",
+    "JobScheduleFrequencyOutputTypeDef",
     "JobScheduleFrequencyTypeDef",
     "ListJobsFilterCriteriaTypeDef",
     "ListManagedDataIdentifiersResponseTypeDef",
     "ListMembersResponseTypeDef",
     "ListResourceProfileArtifactsResponseTypeDef",
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     "PageTypeDef",
     "S3ObjectTypeDef",
     "S3ClassificationScopeTypeDef",
     "S3ClassificationScopeUpdateTypeDef",
     "SearchResourcesTagCriterionTypeDef",
+    "SensitivityInspectionTemplateExcludesUnionTypeDef",
+    "SensitivityInspectionTemplateIncludesUnionTypeDef",
+    "UpdateSensitivityInspectionTemplateRequestRequestTypeDef",
     "UsageByAccountTypeDef",
     "SessionContextTypeDef",
     "UpdateResourceProfileDetectionsRequestRequestTypeDef",
+    "TagCriterionForJobOutputTypeDef",
     "TagCriterionForJobTypeDef",
+    "TagScopeTermOutputTypeDef",
     "TagScopeTermTypeDef",
     "CreateAllowListRequestRequestTypeDef",
     "GetAllowListResponseTypeDef",
     "UpdateAllowListRequestRequestTypeDef",
     "BucketPermissionConfigurationTypeDef",
     "MatchingResourceTypeDef",
     "GetBucketStatisticsResponseTypeDef",
     "GetClassificationExportConfigurationResponseTypeDef",
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     "PutClassificationExportConfigurationResponseTypeDef",
+    "GetFindingsFilterResponseTypeDef",
     "CreateFindingsFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingStatisticsRequestRequestTypeDef",
-    "GetFindingsFilterResponseTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFindingsFilterRequestRequestTypeDef",
+    "JobScheduleFrequencyUnionTypeDef",
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     "ListClassificationJobsRequestRequestTypeDef",
     "OccurrencesTypeDef",
     "GetClassificationScopeResponseTypeDef",
     "UpdateClassificationScopeRequestRequestTypeDef",
     "SearchResourcesCriteriaTypeDef",
     "UsageRecordTypeDef",
     "AssumedRoleTypeDef",
     "FederatedUserTypeDef",
+    "CriteriaForJobOutputTypeDef",
     "CriteriaForJobTypeDef",
+    "JobScopeTermOutputTypeDef",
     "JobScopeTermTypeDef",
     "BucketPublicAccessTypeDef",
     "SearchResourcesResponseTypeDef",
     "CustomDetectionTypeDef",
     "DefaultDetectionTypeDef",
     "SearchResourcesCriteriaBlockTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "UserIdentityTypeDef",
+    "CriteriaBlockForJobOutputTypeDef",
     "CriteriaBlockForJobTypeDef",
+    "JobScopingBlockOutputTypeDef",
     "JobScopingBlockTypeDef",
     "BucketMetadataTypeDef",
     "S3BucketTypeDef",
     "CustomDataIdentifiersTypeDef",
     "SensitiveDataItemTypeDef",
     "SearchResourcesBucketCriteriaTypeDef",
     "FindingActorTypeDef",
+    "S3BucketCriteriaForJobOutputTypeDef",
     "S3BucketCriteriaForJobTypeDef",
+    "ScopingOutputTypeDef",
     "ScopingTypeDef",
     "DescribeBucketsResponseTypeDef",
     "ResourcesAffectedTypeDef",
     "ClassificationResultTypeDef",
     "SearchResourcesRequestRequestTypeDef",
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     "PolicyDetailsTypeDef",
     "JobSummaryTypeDef",
+    "S3JobDefinitionOutputTypeDef",
     "S3JobDefinitionTypeDef",
     "ClassificationDetailsTypeDef",
     "ListClassificationJobsResponseTypeDef",
-    "CreateClassificationJobRequestRequestTypeDef",
     "DescribeClassificationJobResponseTypeDef",
+    "CreateClassificationJobRequestRequestTypeDef",
+    "S3JobDefinitionUnionTypeDef",
     "FindingTypeDef",
     "GetFindingsResponseTypeDef",
 )
 
 _RequiredAcceptInvitationRequestRequestTypeDef = TypedDict(
     "_RequiredAcceptInvitationRequestRequestTypeDef",
     {
@@ -497,14 +519,25 @@
     "BatchGetCustomDataIdentifiersRequestRequestTypeDef",
     {
         "ids": Sequence[str],
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
 BucketCountByEffectivePermissionTypeDef = TypedDict(
     "BucketCountByEffectivePermissionTypeDef",
     {
         "publiclyAccessible": int,
         "publiclyReadable": int,
         "publiclyWritable": int,
         "unknown": int,
@@ -691,57 +724,22 @@
     {
         "id": str,
         "name": str,
     },
     total=False,
 )
 
-CreateAllowListResponseTypeDef = TypedDict(
-    "CreateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateClassificationJobResponseTypeDef = TypedDict(
-    "CreateClassificationJobResponseTypeDef",
-    {
-        "jobArn": str,
-        "jobId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SeverityLevelTypeDef = TypedDict(
     "SeverityLevelTypeDef",
     {
         "occurrencesThreshold": int,
         "severity": DataIdentifierSeverityType,
     },
 )
 
-CreateCustomDataIdentifierResponseTypeDef = TypedDict(
-    "CreateCustomDataIdentifierResponseTypeDef",
-    {
-        "customDataIdentifierId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateFindingsFilterResponseTypeDef = TypedDict(
-    "CreateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateInvitationsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateInvitationsRequestRequestTypeDef",
     {
         "accountIds": Sequence[str],
     },
 )
 _OptionalCreateInvitationsRequestRequestTypeDef = TypedDict(
@@ -764,40 +762,56 @@
         "accountId": str,
         "errorCode": ErrorCodeType,
         "errorMessage": str,
     },
     total=False,
 )
 
-CreateMemberResponseTypeDef = TypedDict(
-    "CreateMemberResponseTypeDef",
+CreateSampleFindingsRequestRequestTypeDef = TypedDict(
+    "CreateSampleFindingsRequestRequestTypeDef",
     {
-        "arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "findingTypes": Sequence[FindingTypeType],
     },
+    total=False,
 )
 
-CreateSampleFindingsRequestRequestTypeDef = TypedDict(
-    "CreateSampleFindingsRequestRequestTypeDef",
+SimpleCriterionForJobOutputTypeDef = TypedDict(
+    "SimpleCriterionForJobOutputTypeDef",
     {
-        "findingTypes": Sequence[FindingTypeType],
+        "comparator": JobComparatorType,
+        "key": SimpleCriterionKeyForJobType,
+        "values": List[str],
     },
     total=False,
 )
 
 SimpleCriterionForJobTypeDef = TypedDict(
     "SimpleCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "key": SimpleCriterionKeyForJobType,
         "values": Sequence[str],
     },
     total=False,
 )
 
+CriterionAdditionalPropertiesOutputTypeDef = TypedDict(
+    "CriterionAdditionalPropertiesOutputTypeDef",
+    {
+        "eq": List[str],
+        "eqExactMatch": List[str],
+        "gt": int,
+        "gte": int,
+        "lt": int,
+        "lte": int,
+        "neq": List[str],
+    },
+    total=False,
+)
+
 CriterionAdditionalPropertiesTypeDef = TypedDict(
     "CriterionAdditionalPropertiesTypeDef",
     {
         "eq": Sequence[str],
         "eqExactMatch": Sequence[str],
         "gt": int,
         "gte": int,
@@ -870,14 +884,24 @@
 DeleteMemberRequestRequestTypeDef = TypedDict(
     "DeleteMemberRequestRequestTypeDef",
     {
         "id": str,
     },
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
 DescribeClassificationJobRequestRequestTypeDef = TypedDict(
     "DescribeClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
     },
 )
 
@@ -904,23 +928,14 @@
         "jobExpiresAt": datetime,
         "jobImminentExpirationHealthEventArn": str,
         "jobPausedAt": datetime,
     },
     total=False,
 )
 
-DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
-    "DescribeOrganizationConfigurationResponseTypeDef",
-    {
-        "autoEnable": bool,
-        "maxAccountLimitReached": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DetectedDataDetailsTypeDef = TypedDict(
     "DetectedDataDetailsTypeDef",
     {
         "value": str,
     },
 )
 
@@ -1033,27 +1048,14 @@
 GetAllowListRequestRequestTypeDef = TypedDict(
     "GetAllowListRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
-    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
-    {
-        "classificationScopeId": str,
-        "disabledAt": datetime,
-        "firstEnabledAt": datetime,
-        "lastUpdatedAt": datetime,
-        "sensitivityInspectionTemplateId": str,
-        "status": AutomatedDiscoveryStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetBucketStatisticsRequestRequestTypeDef = TypedDict(
     "GetBucketStatisticsRequestRequestTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
@@ -1101,57 +1103,21 @@
     {
         "attributeName": str,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "invitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetMacieSessionResponseTypeDef = TypedDict(
-    "GetMacieSessionResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "findingPublishingFrequency": FindingPublishingFrequencyType,
-        "serviceRole": str,
-        "status": MacieStatusType,
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMemberRequestRequestTypeDef = TypedDict(
     "GetMemberRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-GetMemberResponseTypeDef = TypedDict(
-    "GetMemberResponseTypeDef",
-    {
-        "accountId": str,
-        "administratorAccountId": str,
-        "arn": str,
-        "email": str,
-        "invitedAt": datetime,
-        "masterAccountId": str,
-        "relationshipStatus": RelationshipStatusType,
-        "tags": Dict[str, str],
-        "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourceProfileRequestRequestTypeDef = TypedDict(
     "GetResourceProfileRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
@@ -1193,23 +1159,14 @@
 GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef",
     {
         "findingId": str,
     },
 )
 
-GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
-    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
-    {
-        "code": AvailabilityCodeType,
-        "reasons": List[UnavailabilityReasonCodeType],
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
@@ -1225,24 +1182,24 @@
 GetSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateRequestRequestTypeDef",
     {
         "id": str,
     },
 )
 
-SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateExcludesTypeDef",
+SensitivityInspectionTemplateExcludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesOutputTypeDef",
     {
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
 
-SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
-    "SensitivityInspectionTemplateIncludesTypeDef",
+SensitivityInspectionTemplateIncludesOutputTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesOutputTypeDef",
     {
         "allowListIds": List[str],
         "customDataIdentifierIds": List[str],
         "managedDataIdentifierIds": List[str],
     },
     total=False,
 )
@@ -1344,38 +1301,40 @@
     "WeeklyScheduleTypeDef",
     {
         "dayOfWeek": DayOfWeekType,
     },
     total=False,
 )
 
-SimpleScopeTermTypeDef = TypedDict(
-    "SimpleScopeTermTypeDef",
+SimpleScopeTermOutputTypeDef = TypedDict(
+    "SimpleScopeTermOutputTypeDef",
     {
         "comparator": JobComparatorType,
         "key": ScopeFilterKeyType,
-        "values": Sequence[str],
+        "values": List[str],
     },
     total=False,
 )
 
-S3BucketDefinitionForJobTypeDef = TypedDict(
-    "S3BucketDefinitionForJobTypeDef",
+SimpleScopeTermTypeDef = TypedDict(
+    "SimpleScopeTermTypeDef",
     {
-        "accountId": str,
-        "buckets": Sequence[str],
+        "comparator": JobComparatorType,
+        "key": ScopeFilterKeyType,
+        "values": Sequence[str],
     },
+    total=False,
 )
 
-ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
-    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+S3BucketDefinitionForJobOutputTypeDef = TypedDict(
+    "S3BucketDefinitionForJobOutputTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "accountId": str,
+        "buckets": List[str],
     },
-    total=False,
 )
 
 ListAllowListsRequestRequestTypeDef = TypedDict(
     "ListAllowListsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
@@ -1388,83 +1347,41 @@
     {
         "attributeName": ListJobsSortAttributeNameType,
         "orderBy": OrderByType,
     },
     total=False,
 )
 
-ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
-    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
-    {
-        "name": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListClassificationScopesRequestRequestTypeDef = TypedDict(
     "ListClassificationScopesRequestRequestTypeDef",
     {
         "name": str,
         "nextToken": str,
     },
     total=False,
 )
 
-ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCustomDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListCustomDataIdentifiersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
-    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListFindingsFiltersRequestRequestTypeDef = TypedDict(
     "ListFindingsFiltersRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "findingIds": List[str],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListInvitationsRequestRequestTypeDef = TypedDict(
     "ListInvitationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1476,22 +1393,14 @@
         "comparator": JobComparatorType,
         "key": ListJobsFilterKeyType,
         "values": Sequence[str],
     },
     total=False,
 )
 
-ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
-    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListManagedDataIdentifiersRequestRequestTypeDef = TypedDict(
     "ListManagedDataIdentifiersRequestRequestTypeDef",
     {
         "nextToken": str,
     },
     total=False,
 )
@@ -1501,23 +1410,14 @@
     {
         "category": SensitiveDataItemCategoryType,
         "id": str,
     },
     total=False,
 )
 
-ListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "ListMembersRequestListMembersPaginateTypeDef",
-    {
-        "onlyAssociated": str,
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
         "onlyAssociated": str,
     },
@@ -1536,51 +1436,23 @@
         "relationshipStatus": RelationshipStatusType,
         "tags": Dict[str, str],
         "updatedAt": datetime,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListOrganizationAdminAccountsRequestRequestTypeDef = TypedDict(
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
-    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileArtifactsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileArtifactsRequestRequestTypeDef = TypedDict(
@@ -1613,38 +1485,14 @@
 )
 
 class ResourceProfileArtifactTypeDef(
     _RequiredResourceProfileArtifactTypeDef, _OptionalResourceProfileArtifactTypeDef
 ):
     pass
 
-_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "resourceArn": str,
-        },
-    )
-)
-_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
-    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceProfileDetectionsRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListResourceProfileDetectionsRequestRequestTypeDef = TypedDict(
@@ -1658,22 +1506,14 @@
 
 class ListResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredListResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalListResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
-ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
-    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSensitivityInspectionTemplatesRequestRequestTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -1691,22 +1531,14 @@
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
 RangeTypeDef = TypedDict(
     "RangeTypeDef",
     {
         "end": int,
         "start": int,
         "startColumn": int,
     },
@@ -1718,32 +1550,19 @@
     {
         "jsonPath": str,
         "recordIndex": int,
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
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+S3BucketDefinitionForJobTypeDef = TypedDict(
+    "S3BucketDefinitionForJobTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accountId": str,
+        "buckets": Sequence[str],
     },
 )
 
 S3BucketOwnerTypeDef = TypedDict(
     "S3BucketOwnerTypeDef",
     {
         "displayName": str,
@@ -1800,14 +1619,32 @@
     {
         "key": str,
         "value": str,
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateExcludesTypeDef",
+    {
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
+SensitivityInspectionTemplateIncludesTypeDef = TypedDict(
+    "SensitivityInspectionTemplateIncludesTypeDef",
+    {
+        "allowListIds": Sequence[str],
+        "customDataIdentifierIds": Sequence[str],
+        "managedDataIdentifierIds": Sequence[str],
+    },
+    total=False,
+)
+
 ServiceLimitTypeDef = TypedDict(
     "ServiceLimitTypeDef",
     {
         "isServiceLimited": bool,
         "unit": Literal["TERABYTES"],
         "value": int,
     },
@@ -1889,39 +1726,22 @@
 
 class TestCustomDataIdentifierRequestRequestTypeDef(
     _RequiredTestCustomDataIdentifierRequestRequestTypeDef,
     _OptionalTestCustomDataIdentifierRequestRequestTypeDef,
 ):
     pass
 
-TestCustomDataIdentifierResponseTypeDef = TypedDict(
-    "TestCustomDataIdentifierResponseTypeDef",
-    {
-        "matchCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
 
-UpdateAllowListResponseTypeDef = TypedDict(
-    "UpdateAllowListResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef",
     {
         "status": AutomatedDiscoveryStatusType,
     },
 )
 
@@ -1929,23 +1749,14 @@
     "UpdateClassificationJobRequestRequestTypeDef",
     {
         "jobId": str,
         "jobStatus": JobStatusType,
     },
 )
 
-UpdateFindingsFilterResponseTypeDef = TypedDict(
-    "UpdateFindingsFilterResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdateMacieSessionRequestRequestTypeDef = TypedDict(
     "UpdateMacieSessionRequestRequestTypeDef",
     {
         "findingPublishingFrequency": FindingPublishingFrequencyType,
         "status": MacieStatusType,
     },
     total=False,
@@ -2019,56 +1830,209 @@
     "AccountLevelPermissionsTypeDef",
     {
         "blockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "adminAccounts": List[AdminAccountTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AllowListCriteriaTypeDef = TypedDict(
     "AllowListCriteriaTypeDef",
     {
         "regex": str,
         "s3WordsList": S3WordsListTypeDef,
     },
     total=False,
 )
 
-ListAllowListsResponseTypeDef = TypedDict(
-    "ListAllowListsResponseTypeDef",
-    {
-        "allowLists": List[AllowListSummaryTypeDef],
-        "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FindingActionTypeDef = TypedDict(
     "FindingActionTypeDef",
     {
         "actionType": Literal["AWS_API_CALL"],
         "apiCallDetails": ApiCallDetailsTypeDef,
     },
     total=False,
 )
 
 BatchGetCustomDataIdentifiersResponseTypeDef = TypedDict(
     "BatchGetCustomDataIdentifiersResponseTypeDef",
     {
         "customDataIdentifiers": List[BatchGetCustomDataIdentifierSummaryTypeDef],
         "notFoundIdentifierIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAllowListResponseTypeDef = TypedDict(
+    "CreateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateClassificationJobResponseTypeDef = TypedDict(
+    "CreateClassificationJobResponseTypeDef",
+    {
+        "jobArn": str,
+        "jobId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCustomDataIdentifierResponseTypeDef = TypedDict(
+    "CreateCustomDataIdentifierResponseTypeDef",
+    {
+        "customDataIdentifierId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFindingsFilterResponseTypeDef = TypedDict(
+    "CreateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateMemberResponseTypeDef = TypedDict(
+    "CreateMemberResponseTypeDef",
+    {
+        "arn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
+    "DescribeOrganizationConfigurationResponseTypeDef",
+    {
+        "autoEnable": bool,
+        "maxAccountLimitReached": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAutomatedDiscoveryConfigurationResponseTypeDef = TypedDict(
+    "GetAutomatedDiscoveryConfigurationResponseTypeDef",
+    {
+        "classificationScopeId": str,
+        "disabledAt": datetime,
+        "firstEnabledAt": datetime,
+        "lastUpdatedAt": datetime,
+        "sensitivityInspectionTemplateId": str,
+        "status": AutomatedDiscoveryStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "invitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMacieSessionResponseTypeDef = TypedDict(
+    "GetMacieSessionResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "findingPublishingFrequency": FindingPublishingFrequencyType,
+        "serviceRole": str,
+        "status": MacieStatusType,
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetMemberResponseTypeDef = TypedDict(
+    "GetMemberResponseTypeDef",
+    {
+        "accountId": str,
+        "administratorAccountId": str,
+        "arn": str,
+        "email": str,
+        "invitedAt": datetime,
+        "masterAccountId": str,
+        "relationshipStatus": RelationshipStatusType,
+        "tags": Dict[str, str],
+        "updatedAt": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSensitiveDataOccurrencesAvailabilityResponseTypeDef = TypedDict(
+    "GetSensitiveDataOccurrencesAvailabilityResponseTypeDef",
+    {
+        "code": AvailabilityCodeType,
+        "reasons": List[UnavailabilityReasonCodeType],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAllowListsResponseTypeDef = TypedDict(
+    "ListAllowListsResponseTypeDef",
+    {
+        "allowLists": List[AllowListSummaryTypeDef],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "findingIds": List[str],
+        "nextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "adminAccounts": List[AdminAccountTypeDef],
+        "nextToken": str,
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
+TestCustomDataIdentifierResponseTypeDef = TypedDict(
+    "TestCustomDataIdentifierResponseTypeDef",
+    {
+        "matchCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAllowListResponseTypeDef = TypedDict(
+    "UpdateAllowListResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFindingsFilterResponseTypeDef = TypedDict(
+    "UpdateFindingsFilterResponseTypeDef",
+    {
+        "arn": str,
+        "id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "accessControlList": AccessControlListTypeDef,
@@ -2096,24 +2060,14 @@
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
     },
     total=False,
 )
 
-DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
-    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
-    {
-        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
-        "sortCriteria": BucketSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeBucketsRequestRequestTypeDef = TypedDict(
     "DescribeBucketsRequestRequestTypeDef",
     {
         "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
         "maxResults": int,
         "nextToken": str,
         "sortCriteria": BucketSortCriteriaTypeDef,
@@ -2141,15 +2095,15 @@
 )
 
 ListClassificationScopesResponseTypeDef = TypedDict(
     "ListClassificationScopesResponseTypeDef",
     {
         "classificationScopes": List[ClassificationScopeSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateCustomDataIdentifierRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCustomDataIdentifierRequestRequestTypeDef",
     {
         "name": str,
@@ -2187,125 +2141,261 @@
         "ignoreWords": List[str],
         "keywords": List[str],
         "maximumMatchDistance": int,
         "name": str,
         "regex": str,
         "severityLevels": List[SeverityLevelTypeDef],
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateInvitationsResponseTypeDef = TypedDict(
     "CreateInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "unprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "criterion": Dict[str, CriterionAdditionalPropertiesOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "criterion": Mapping[str, CriterionAdditionalPropertiesTypeDef],
     },
     total=False,
 )
 
 ListCustomDataIdentifiersResponseTypeDef = TypedDict(
     "ListCustomDataIdentifiersResponseTypeDef",
     {
         "items": List[CustomDataIdentifierSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBucketsRequestDescribeBucketsPaginateTypeDef = TypedDict(
+    "DescribeBucketsRequestDescribeBucketsPaginateTypeDef",
+    {
+        "criteria": Mapping[str, BucketCriteriaAdditionalPropertiesTypeDef],
+        "sortCriteria": BucketSortCriteriaTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListAllowListsRequestListAllowListsPaginateTypeDef = TypedDict(
+    "ListAllowListsRequestListAllowListsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListClassificationScopesRequestListClassificationScopesPaginateTypeDef = TypedDict(
+    "ListClassificationScopesRequestListClassificationScopesPaginateTypeDef",
+    {
+        "name": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef = TypedDict(
+    "ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef = TypedDict(
+    "ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "ListMembersRequestListMembersPaginateTypeDef",
+    {
+        "onlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef(
+    _RequiredListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    _OptionalListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "resourceArn": str,
+        },
+    )
+)
+_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef(
+    _RequiredListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    _OptionalListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+):
+    pass
+
+ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef = TypedDict(
+    "ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
 GetSensitiveDataOccurrencesResponseTypeDef = TypedDict(
     "GetSensitiveDataOccurrencesResponseTypeDef",
     {
         "error": str,
         "sensitiveDataOccurrences": Dict[str, List[DetectedDataDetailsTypeDef]],
         "status": RevealRequestStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceProfileDetectionsResponseTypeDef = TypedDict(
     "ListResourceProfileDetectionsResponseTypeDef",
     {
         "detections": List[DetectionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFindingsFiltersResponseTypeDef = TypedDict(
     "ListFindingsFiltersResponseTypeDef",
     {
         "findingsFilterListItems": List[FindingsFilterListItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAdministratorAccountResponseTypeDef = TypedDict(
     "GetAdministratorAccountResponseTypeDef",
     {
         "administrator": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "master": InvitationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "invitations": List[InvitationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingStatisticsResponseTypeDef = TypedDict(
     "GetFindingStatisticsResponseTypeDef",
     {
         "countsByGroup": List[GroupCountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFindingsPublicationConfigurationResponseTypeDef = TypedDict(
     "GetFindingsPublicationConfigurationResponseTypeDef",
     {
         "securityHubConfiguration": SecurityHubConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutFindingsPublicationConfigurationRequestRequestTypeDef = TypedDict(
     "PutFindingsPublicationConfigurationRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -2336,38 +2426,38 @@
 GetResourceProfileResponseTypeDef = TypedDict(
     "GetResourceProfileResponseTypeDef",
     {
         "profileUpdatedAt": datetime,
         "sensitivityScore": int,
         "sensitivityScoreOverridden": bool,
         "statistics": ResourceStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRevealConfigurationResponseTypeDef = TypedDict(
     "GetRevealConfigurationResponseTypeDef",
     {
         "configuration": RevealConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRevealConfigurationRequestRequestTypeDef = TypedDict(
     "UpdateRevealConfigurationRequestRequestTypeDef",
     {
         "configuration": RevealConfigurationTypeDef,
     },
 )
 
 UpdateRevealConfigurationResponseTypeDef = TypedDict(
     "UpdateRevealConfigurationResponseTypeDef",
     {
         "configuration": RevealConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef = TypedDict(
     "_RequiredGetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef",
     {
         "findingId": str,
@@ -2387,51 +2477,29 @@
 ):
     pass
 
 GetSensitivityInspectionTemplateResponseTypeDef = TypedDict(
     "GetSensitivityInspectionTemplateResponseTypeDef",
     {
         "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+        "excludes": SensitivityInspectionTemplateExcludesOutputTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesOutputTypeDef,
         "name": str,
         "sensitivityInspectionTemplateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "id": str,
-    },
-)
-_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
-    {
-        "description": str,
-        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
-        "includes": SensitivityInspectionTemplateIncludesTypeDef,
-    },
-    total=False,
-)
-
-class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
-    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
-):
-    pass
-
 GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef = TypedDict(
     "GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef",
     {
         "filterBy": Sequence[UsageStatisticsFilterTypeDef],
         "sortBy": UsageStatisticsSortByTypeDef,
         "timeRange": TimeRangeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "GetUsageStatisticsRequestRequestTypeDef",
     {
@@ -2445,15 +2513,15 @@
 )
 
 GetUsageTotalsResponseTypeDef = TypedDict(
     "GetUsageTotalsResponseTypeDef",
     {
         "timeRange": TimeRangeType,
         "usageTotals": List[UsageTotalTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IpAddressDetailsTypeDef = TypedDict(
     "IpAddressDetailsTypeDef",
     {
         "ipAddressV4": str,
@@ -2461,14 +2529,24 @@
         "ipCountry": IpCountryTypeDef,
         "ipGeoLocation": IpGeoLocationTypeDef,
         "ipOwner": IpOwnerTypeDef,
     },
     total=False,
 )
 
+JobScheduleFrequencyOutputTypeDef = TypedDict(
+    "JobScheduleFrequencyOutputTypeDef",
+    {
+        "dailySchedule": Dict[str, Any],
+        "monthlySchedule": MonthlyScheduleTypeDef,
+        "weeklySchedule": WeeklyScheduleTypeDef,
+    },
+    total=False,
+)
+
 JobScheduleFrequencyTypeDef = TypedDict(
     "JobScheduleFrequencyTypeDef",
     {
         "dailySchedule": Mapping[str, Any],
         "monthlySchedule": MonthlyScheduleTypeDef,
         "weeklySchedule": WeeklyScheduleTypeDef,
     },
@@ -2485,42 +2563,42 @@
 )
 
 ListManagedDataIdentifiersResponseTypeDef = TypedDict(
     "ListManagedDataIdentifiersResponseTypeDef",
     {
         "items": List[ManagedDataIdentifierSummaryTypeDef],
         "nextToken": str,
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
 
 ListResourceProfileArtifactsResponseTypeDef = TypedDict(
     "ListResourceProfileArtifactsResponseTypeDef",
     {
         "artifacts": List[ResourceProfileArtifactTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSensitivityInspectionTemplatesResponseTypeDef = TypedDict(
     "ListSensitivityInspectionTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "sensitivityInspectionTemplates": List[SensitivityInspectionTemplatesEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PageTypeDef = TypedDict(
     "PageTypeDef",
     {
         "lineRange": RangeTypeDef,
@@ -2568,14 +2646,42 @@
     {
         "comparator": SearchResourcesComparatorType,
         "tagValues": Sequence[SearchResourcesTagCriterionPairTypeDef],
     },
     total=False,
 )
 
+SensitivityInspectionTemplateExcludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateExcludesTypeDef, SensitivityInspectionTemplateExcludesOutputTypeDef
+]
+SensitivityInspectionTemplateIncludesUnionTypeDef = Union[
+    SensitivityInspectionTemplateIncludesTypeDef, SensitivityInspectionTemplateIncludesOutputTypeDef
+]
+_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "id": str,
+    },
+)
+_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef",
+    {
+        "description": str,
+        "excludes": SensitivityInspectionTemplateExcludesTypeDef,
+        "includes": SensitivityInspectionTemplateIncludesTypeDef,
+    },
+    total=False,
+)
+
+class UpdateSensitivityInspectionTemplateRequestRequestTypeDef(
+    _RequiredUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+    _OptionalUpdateSensitivityInspectionTemplateRequestRequestTypeDef,
+):
+    pass
+
 UsageByAccountTypeDef = TypedDict(
     "UsageByAccountTypeDef",
     {
         "currency": Literal["USD"],
         "estimatedCost": str,
         "serviceLimit": ServiceLimitTypeDef,
         "type": UsageTypeType,
@@ -2608,23 +2714,43 @@
 
 class UpdateResourceProfileDetectionsRequestRequestTypeDef(
     _RequiredUpdateResourceProfileDetectionsRequestRequestTypeDef,
     _OptionalUpdateResourceProfileDetectionsRequestRequestTypeDef,
 ):
     pass
 
+TagCriterionForJobOutputTypeDef = TypedDict(
+    "TagCriterionForJobOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "tagValues": List[TagCriterionPairForJobTypeDef],
+    },
+    total=False,
+)
+
 TagCriterionForJobTypeDef = TypedDict(
     "TagCriterionForJobTypeDef",
     {
         "comparator": JobComparatorType,
         "tagValues": Sequence[TagCriterionPairForJobTypeDef],
     },
     total=False,
 )
 
+TagScopeTermOutputTypeDef = TypedDict(
+    "TagScopeTermOutputTypeDef",
+    {
+        "comparator": JobComparatorType,
+        "key": str,
+        "tagValues": List[TagValuePairTypeDef],
+        "target": Literal["S3_OBJECT"],
+    },
+    total=False,
+)
+
 TagScopeTermTypeDef = TypedDict(
     "TagScopeTermTypeDef",
     {
         "comparator": JobComparatorType,
         "key": str,
         "tagValues": Sequence[TagValuePairTypeDef],
         "target": Literal["S3_OBJECT"],
@@ -2662,15 +2788,15 @@
         "criteria": AllowListCriteriaTypeDef,
         "description": str,
         "id": str,
         "name": str,
         "status": AllowListStatusTypeDef,
         "tags": Dict[str, str],
         "updatedAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateAllowListRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAllowListRequestRequestTypeDef",
     {
         "criteria": AllowListCriteriaTypeDef,
@@ -2723,38 +2849,53 @@
         "classifiableSizeInBytes": int,
         "lastUpdated": datetime,
         "objectCount": int,
         "sizeInBytes": int,
         "sizeInBytesCompressed": int,
         "unclassifiableObjectCount": ObjectLevelStatisticsTypeDef,
         "unclassifiableObjectSizeInBytes": ObjectLevelStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetClassificationExportConfigurationResponseTypeDef = TypedDict(
     "GetClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutClassificationExportConfigurationRequestRequestTypeDef = TypedDict(
     "PutClassificationExportConfigurationRequestRequestTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
     },
 )
 
 PutClassificationExportConfigurationResponseTypeDef = TypedDict(
     "PutClassificationExportConfigurationResponseTypeDef",
     {
         "configuration": ClassificationExportConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetFindingsFilterResponseTypeDef = TypedDict(
+    "GetFindingsFilterResponseTypeDef",
+    {
+        "action": FindingsFilterActionType,
+        "arn": str,
+        "description": str,
+        "findingCriteria": FindingCriteriaOutputTypeDef,
+        "id": str,
+        "name": str,
+        "position": int,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateFindingsFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFindingsFilterRequestRequestTypeDef",
     {
         "action": FindingsFilterActionType,
@@ -2775,14 +2916,15 @@
 
 class CreateFindingsFilterRequestRequestTypeDef(
     _RequiredCreateFindingsFilterRequestRequestTypeDef,
     _OptionalCreateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingStatisticsRequestRequestTypeDef",
     {
         "groupBy": GroupByType,
     },
 )
 _OptionalGetFindingStatisticsRequestRequestTypeDef = TypedDict(
@@ -2797,35 +2939,20 @@
 
 class GetFindingStatisticsRequestRequestTypeDef(
     _RequiredGetFindingStatisticsRequestRequestTypeDef,
     _OptionalGetFindingStatisticsRequestRequestTypeDef,
 ):
     pass
 
-GetFindingsFilterResponseTypeDef = TypedDict(
-    "GetFindingsFilterResponseTypeDef",
-    {
-        "action": FindingsFilterActionType,
-        "arn": str,
-        "description": str,
-        "findingCriteria": FindingCriteriaTypeDef,
-        "id": str,
-        "name": str,
-        "position": int,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "ListFindingsRequestListFindingsPaginateTypeDef",
     {
         "findingCriteria": FindingCriteriaTypeDef,
         "sortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListFindingsRequestRequestTypeDef = TypedDict(
     "ListFindingsRequestRequestTypeDef",
     {
@@ -2858,20 +2985,23 @@
 
 class UpdateFindingsFilterRequestRequestTypeDef(
     _RequiredUpdateFindingsFilterRequestRequestTypeDef,
     _OptionalUpdateFindingsFilterRequestRequestTypeDef,
 ):
     pass
 
+JobScheduleFrequencyUnionTypeDef = Union[
+    JobScheduleFrequencyTypeDef, JobScheduleFrequencyOutputTypeDef
+]
 ListClassificationJobsRequestListClassificationJobsPaginateTypeDef = TypedDict(
     "ListClassificationJobsRequestListClassificationJobsPaginateTypeDef",
     {
         "filterCriteria": ListJobsFilterCriteriaTypeDef,
         "sortCriteria": ListJobsSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListClassificationJobsRequestRequestTypeDef = TypedDict(
     "ListClassificationJobsRequestRequestTypeDef",
     {
@@ -2897,15 +3027,15 @@
 
 GetClassificationScopeResponseTypeDef = TypedDict(
     "GetClassificationScopeResponseTypeDef",
     {
         "id": str,
         "name": str,
         "s3": S3ClassificationScopeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateClassificationScopeRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateClassificationScopeRequestRequestTypeDef",
     {
         "id": str,
@@ -2965,23 +3095,41 @@
         "arn": str,
         "principalId": str,
         "sessionContext": SessionContextTypeDef,
     },
     total=False,
 )
 
+CriteriaForJobOutputTypeDef = TypedDict(
+    "CriteriaForJobOutputTypeDef",
+    {
+        "simpleCriterion": SimpleCriterionForJobOutputTypeDef,
+        "tagCriterion": TagCriterionForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 CriteriaForJobTypeDef = TypedDict(
     "CriteriaForJobTypeDef",
     {
         "simpleCriterion": SimpleCriterionForJobTypeDef,
         "tagCriterion": TagCriterionForJobTypeDef,
     },
     total=False,
 )
 
+JobScopeTermOutputTypeDef = TypedDict(
+    "JobScopeTermOutputTypeDef",
+    {
+        "simpleScopeTerm": SimpleScopeTermOutputTypeDef,
+        "tagScopeTerm": TagScopeTermOutputTypeDef,
+    },
+    total=False,
+)
+
 JobScopeTermTypeDef = TypedDict(
     "JobScopeTermTypeDef",
     {
         "simpleScopeTerm": SimpleScopeTermTypeDef,
         "tagScopeTerm": TagScopeTermTypeDef,
     },
     total=False,
@@ -2997,15 +3145,15 @@
 )
 
 SearchResourcesResponseTypeDef = TypedDict(
     "SearchResourcesResponseTypeDef",
     {
         "matchingResources": List[MatchingResourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CustomDetectionTypeDef = TypedDict(
     "CustomDetectionTypeDef",
     {
         "arn": str,
@@ -3036,15 +3184,15 @@
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "nextToken": str,
         "records": List[UsageRecordTypeDef],
         "timeRange": TimeRangeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserIdentityTypeDef = TypedDict(
     "UserIdentityTypeDef",
     {
         "assumedRole": AssumedRoleTypeDef,
@@ -3054,22 +3202,38 @@
         "iamUser": IamUserTypeDef,
         "root": UserIdentityRootTypeDef,
         "type": UserIdentityTypeType,
     },
     total=False,
 )
 
+CriteriaBlockForJobOutputTypeDef = TypedDict(
+    "CriteriaBlockForJobOutputTypeDef",
+    {
+        "and": List[CriteriaForJobOutputTypeDef],
+    },
+    total=False,
+)
+
 CriteriaBlockForJobTypeDef = TypedDict(
     "CriteriaBlockForJobTypeDef",
     {
         "and": Sequence[CriteriaForJobTypeDef],
     },
     total=False,
 )
 
+JobScopingBlockOutputTypeDef = TypedDict(
+    "JobScopingBlockOutputTypeDef",
+    {
+        "and": List[JobScopeTermOutputTypeDef],
+    },
+    total=False,
+)
+
 JobScopingBlockTypeDef = TypedDict(
     "JobScopingBlockTypeDef",
     {
         "and": Sequence[JobScopeTermTypeDef],
     },
     total=False,
 )
@@ -3156,38 +3320,56 @@
         "domainDetails": DomainDetailsTypeDef,
         "ipAddressDetails": IpAddressDetailsTypeDef,
         "userIdentity": UserIdentityTypeDef,
     },
     total=False,
 )
 
+S3BucketCriteriaForJobOutputTypeDef = TypedDict(
+    "S3BucketCriteriaForJobOutputTypeDef",
+    {
+        "excludes": CriteriaBlockForJobOutputTypeDef,
+        "includes": CriteriaBlockForJobOutputTypeDef,
+    },
+    total=False,
+)
+
 S3BucketCriteriaForJobTypeDef = TypedDict(
     "S3BucketCriteriaForJobTypeDef",
     {
         "excludes": CriteriaBlockForJobTypeDef,
         "includes": CriteriaBlockForJobTypeDef,
     },
     total=False,
 )
 
+ScopingOutputTypeDef = TypedDict(
+    "ScopingOutputTypeDef",
+    {
+        "excludes": JobScopingBlockOutputTypeDef,
+        "includes": JobScopingBlockOutputTypeDef,
+    },
+    total=False,
+)
+
 ScopingTypeDef = TypedDict(
     "ScopingTypeDef",
     {
         "excludes": JobScopingBlockTypeDef,
         "includes": JobScopingBlockTypeDef,
     },
     total=False,
 )
 
 DescribeBucketsResponseTypeDef = TypedDict(
     "DescribeBucketsResponseTypeDef",
     {
         "buckets": List[BucketMetadataTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourcesAffectedTypeDef = TypedDict(
     "ResourcesAffectedTypeDef",
     {
         "s3Bucket": S3BucketTypeDef,
@@ -3221,15 +3403,15 @@
 )
 
 SearchResourcesRequestSearchResourcesPaginateTypeDef = TypedDict(
     "SearchResourcesRequestSearchResourcesPaginateTypeDef",
     {
         "bucketCriteria": SearchResourcesBucketCriteriaTypeDef,
         "sortCriteria": SearchResourcesSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 PolicyDetailsTypeDef = TypedDict(
     "PolicyDetailsTypeDef",
     {
@@ -3238,27 +3420,37 @@
     },
     total=False,
 )
 
 JobSummaryTypeDef = TypedDict(
     "JobSummaryTypeDef",
     {
-        "bucketCriteria": S3BucketCriteriaForJobTypeDef,
-        "bucketDefinitions": List[S3BucketDefinitionForJobTypeDef],
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
         "createdAt": datetime,
         "jobId": str,
         "jobStatus": JobStatusType,
         "jobType": JobTypeType,
         "lastRunErrorStatus": LastRunErrorStatusTypeDef,
         "name": str,
         "userPausedDetails": UserPausedDetailsTypeDef,
     },
     total=False,
 )
 
+S3JobDefinitionOutputTypeDef = TypedDict(
+    "S3JobDefinitionOutputTypeDef",
+    {
+        "bucketCriteria": S3BucketCriteriaForJobOutputTypeDef,
+        "bucketDefinitions": List[S3BucketDefinitionForJobOutputTypeDef],
+        "scoping": ScopingOutputTypeDef,
+    },
+    total=False,
+)
+
 S3JobDefinitionTypeDef = TypedDict(
     "S3JobDefinitionTypeDef",
     {
         "bucketCriteria": S3BucketCriteriaForJobTypeDef,
         "bucketDefinitions": Sequence[S3BucketDefinitionForJobTypeDef],
         "scoping": ScopingTypeDef,
     },
@@ -3278,15 +3470,43 @@
 )
 
 ListClassificationJobsResponseTypeDef = TypedDict(
     "ListClassificationJobsResponseTypeDef",
     {
         "items": List[JobSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeClassificationJobResponseTypeDef = TypedDict(
+    "DescribeClassificationJobResponseTypeDef",
+    {
+        "allowListIds": List[str],
+        "clientToken": str,
+        "createdAt": datetime,
+        "customDataIdentifierIds": List[str],
+        "description": str,
+        "initialRun": bool,
+        "jobArn": str,
+        "jobId": str,
+        "jobStatus": JobStatusType,
+        "jobType": JobTypeType,
+        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
+        "lastRunTime": datetime,
+        "managedDataIdentifierIds": List[str],
+        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
+        "name": str,
+        "s3JobDefinition": S3JobDefinitionOutputTypeDef,
+        "samplingPercentage": int,
+        "scheduleFrequency": JobScheduleFrequencyOutputTypeDef,
+        "statistics": StatisticsTypeDef,
+        "tags": Dict[str, str],
+        "userPausedDetails": UserPausedDetailsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateClassificationJobRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClassificationJobRequestRequestTypeDef",
     {
         "clientToken": str,
@@ -3313,42 +3533,15 @@
 
 class CreateClassificationJobRequestRequestTypeDef(
     _RequiredCreateClassificationJobRequestRequestTypeDef,
     _OptionalCreateClassificationJobRequestRequestTypeDef,
 ):
     pass
 
-DescribeClassificationJobResponseTypeDef = TypedDict(
-    "DescribeClassificationJobResponseTypeDef",
-    {
-        "allowListIds": List[str],
-        "clientToken": str,
-        "createdAt": datetime,
-        "customDataIdentifierIds": List[str],
-        "description": str,
-        "initialRun": bool,
-        "jobArn": str,
-        "jobId": str,
-        "jobStatus": JobStatusType,
-        "jobType": JobTypeType,
-        "lastRunErrorStatus": LastRunErrorStatusTypeDef,
-        "lastRunTime": datetime,
-        "managedDataIdentifierIds": List[str],
-        "managedDataIdentifierSelector": ManagedDataIdentifierSelectorType,
-        "name": str,
-        "s3JobDefinition": S3JobDefinitionTypeDef,
-        "samplingPercentage": int,
-        "scheduleFrequency": JobScheduleFrequencyTypeDef,
-        "statistics": StatisticsTypeDef,
-        "tags": Dict[str, str],
-        "userPausedDetails": UserPausedDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+S3JobDefinitionUnionTypeDef = Union[S3JobDefinitionTypeDef, S3JobDefinitionOutputTypeDef]
 FindingTypeDef = TypedDict(
     "FindingTypeDef",
     {
         "accountId": str,
         "archived": bool,
         "category": FindingCategoryType,
         "classificationDetails": ClassificationDetailsTypeDef,
@@ -3370,10 +3563,10 @@
     total=False,
 )
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/waiter.py` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2/waiter.pyi` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/PKG-INFO` & `types-aiobotocore-macie2-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-macie2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Macie2 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore macie2 type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-macie2"></a>
 
 # types-aiobotocore-macie2
 
 [![PyPI - types-aiobotocore-macie2](https://img.shields.io/pypi/v/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-macie2?color=blue)](https://pypistats.org/packages/types-aiobotocore-macie2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie2)](https://pepy.tech/project/types-aiobotocore-macie2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Macie2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie2.html#Macie2)
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
 [types-aiobotocore-macie2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie2/).
 
 See how it helps to find and fix potential bugs:
 
@@ -75,15 +42,15 @@
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
@@ -451,20 +418,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_macie2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_macie2.type_defs import (
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccountDetailTypeDef,
     BlockPublicAccessTypeDef,
@@ -473,14 +440,15 @@
     AllowListStatusTypeDef,
     AllowListSummaryTypeDef,
     ApiCallDetailsTypeDef,
     AwsAccountTypeDef,
     AwsServiceTypeDef,
     BatchGetCustomDataIdentifierSummaryTypeDef,
     BatchGetCustomDataIdentifiersRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     BucketCountByEffectivePermissionTypeDef,
     BucketCountByEncryptionTypeTypeDef,
     BucketCountBySharedAccessTypeTypeDef,
     BucketCountPolicyAllowsUnencryptedObjectUploadsTypeDef,
     BucketCriteriaAdditionalPropertiesTypeDef,
     BucketPolicyTypeDef,
     BucketServerSideEncryptionTypeDef,
@@ -491,166 +459,172 @@
     ReplicationDetailsTypeDef,
     BucketSortCriteriaTypeDef,
     SensitivityAggregationsTypeDef,
     CellTypeDef,
     S3DestinationTypeDef,
     ClassificationResultStatusTypeDef,
     ClassificationScopeSummaryTypeDef,
-    CreateAllowListResponseTypeDef,
-    CreateClassificationJobResponseTypeDef,
     SeverityLevelTypeDef,
-    CreateCustomDataIdentifierResponseTypeDef,
-    CreateFindingsFilterResponseTypeDef,
     CreateInvitationsRequestRequestTypeDef,
     UnprocessedAccountTypeDef,
-    CreateMemberResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
+    SimpleCriterionForJobOutputTypeDef,
     SimpleCriterionForJobTypeDef,
+    CriterionAdditionalPropertiesOutputTypeDef,
     CriterionAdditionalPropertiesTypeDef,
     CustomDataIdentifierSummaryTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DeleteAllowListRequestRequestTypeDef,
     DeleteCustomDataIdentifierRequestRequestTypeDef,
     DeleteFindingsFilterRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMemberRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     DescribeClassificationJobRequestRequestTypeDef,
     LastRunErrorStatusTypeDef,
     StatisticsTypeDef,
     UserPausedDetailsTypeDef,
-    DescribeOrganizationConfigurationResponseTypeDef,
     DetectedDataDetailsTypeDef,
     DetectionTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
     DisassociateMemberRequestRequestTypeDef,
     DomainDetailsTypeDef,
     EnableMacieRequestRequestTypeDef,
     EnableOrganizationAdminAccountRequestRequestTypeDef,
     FindingStatisticsSortCriteriaTypeDef,
     SeverityTypeDef,
     FindingsFilterListItemTypeDef,
     InvitationTypeDef,
     GetAllowListRequestRequestTypeDef,
-    GetAutomatedDiscoveryConfigurationResponseTypeDef,
     GetBucketStatisticsRequestRequestTypeDef,
     GetClassificationScopeRequestRequestTypeDef,
     GetCustomDataIdentifierRequestRequestTypeDef,
     GroupCountTypeDef,
     GetFindingsFilterRequestRequestTypeDef,
     SecurityHubConfigurationTypeDef,
     SortCriteriaTypeDef,
-    GetInvitationsCountResponseTypeDef,
-    GetMacieSessionResponseTypeDef,
     GetMemberRequestRequestTypeDef,
-    GetMemberResponseTypeDef,
     GetResourceProfileRequestRequestTypeDef,
     ResourceStatisticsTypeDef,
     RevealConfigurationTypeDef,
     GetSensitiveDataOccurrencesAvailabilityRequestRequestTypeDef,
-    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
     WaiterConfigTypeDef,
     GetSensitiveDataOccurrencesRequestRequestTypeDef,
     GetSensitivityInspectionTemplateRequestRequestTypeDef,
-    SensitivityInspectionTemplateExcludesTypeDef,
-    SensitivityInspectionTemplateIncludesTypeDef,
+    SensitivityInspectionTemplateExcludesOutputTypeDef,
+    SensitivityInspectionTemplateIncludesOutputTypeDef,
     UsageStatisticsFilterTypeDef,
     UsageStatisticsSortByTypeDef,
     GetUsageTotalsRequestRequestTypeDef,
     UsageTotalTypeDef,
     IamUserTypeDef,
     IpCityTypeDef,
     IpCountryTypeDef,
     IpGeoLocationTypeDef,
     IpOwnerTypeDef,
     MonthlyScheduleTypeDef,
     WeeklyScheduleTypeDef,
+    SimpleScopeTermOutputTypeDef,
     SimpleScopeTermTypeDef,
-    S3BucketDefinitionForJobTypeDef,
-    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    S3BucketDefinitionForJobOutputTypeDef,
     ListAllowListsRequestRequestTypeDef,
     ListJobsSortCriteriaTypeDef,
-    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
     ListClassificationScopesRequestRequestTypeDef,
-    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
     ListCustomDataIdentifiersRequestRequestTypeDef,
-    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
     ListFindingsFiltersRequestRequestTypeDef,
-    ListFindingsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
     ListJobsFilterTermTypeDef,
-    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
     ListManagedDataIdentifiersRequestRequestTypeDef,
     ManagedDataIdentifierSummaryTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
     MemberTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
-    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
     ListResourceProfileArtifactsRequestRequestTypeDef,
     ResourceProfileArtifactTypeDef,
-    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
     ListResourceProfileDetectionsRequestRequestTypeDef,
-    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     ListSensitivityInspectionTemplatesRequestRequestTypeDef,
     SensitivityInspectionTemplatesEntryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     RangeTypeDef,
     RecordTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    S3BucketDefinitionForJobTypeDef,
     S3BucketOwnerTypeDef,
     ServerSideEncryptionTypeDef,
     S3ClassificationScopeExclusionTypeDef,
     S3ClassificationScopeExclusionUpdateTypeDef,
     SearchResourcesSimpleCriterionTypeDef,
     SearchResourcesSortCriteriaTypeDef,
     SearchResourcesTagCriterionPairTypeDef,
+    SensitivityInspectionTemplateExcludesTypeDef,
+    SensitivityInspectionTemplateIncludesTypeDef,
     ServiceLimitTypeDef,
     SessionContextAttributesTypeDef,
     SessionIssuerTypeDef,
     SuppressDataIdentifierTypeDef,
     TagCriterionPairForJobTypeDef,
     TagResourceRequestRequestTypeDef,
     TagValuePairTypeDef,
     TestCustomDataIdentifierRequestRequestTypeDef,
-    TestCustomDataIdentifierResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateAllowListResponseTypeDef,
     UpdateAutomatedDiscoveryConfigurationRequestRequestTypeDef,
     UpdateClassificationJobRequestRequestTypeDef,
-    UpdateFindingsFilterResponseTypeDef,
     UpdateMacieSessionRequestRequestTypeDef,
     UpdateMemberSessionRequestRequestTypeDef,
     UpdateOrganizationConfigurationRequestRequestTypeDef,
     UpdateResourceProfileRequestRequestTypeDef,
     UserIdentityRootTypeDef,
     CreateMemberRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
     AllowListCriteriaTypeDef,
-    ListAllowListsResponseTypeDef,
     FindingActionTypeDef,
     BatchGetCustomDataIdentifiersResponseTypeDef,
+    CreateAllowListResponseTypeDef,
+    CreateClassificationJobResponseTypeDef,
+    CreateCustomDataIdentifierResponseTypeDef,
+    CreateFindingsFilterResponseTypeDef,
+    CreateMemberResponseTypeDef,
+    DescribeOrganizationConfigurationResponseTypeDef,
+    GetAutomatedDiscoveryConfigurationResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetMacieSessionResponseTypeDef,
+    GetMemberResponseTypeDef,
+    GetSensitiveDataOccurrencesAvailabilityResponseTypeDef,
+    ListAllowListsResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    TestCustomDataIdentifierResponseTypeDef,
+    UpdateAllowListResponseTypeDef,
+    UpdateFindingsFilterResponseTypeDef,
     BucketLevelPermissionsTypeDef,
     MatchingBucketTypeDef,
-    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
     DescribeBucketsRequestRequestTypeDef,
     BucketStatisticsBySensitivityTypeDef,
     ClassificationExportConfigurationTypeDef,
     ListClassificationScopesResponseTypeDef,
     CreateCustomDataIdentifierRequestRequestTypeDef,
     GetCustomDataIdentifierResponseTypeDef,
     CreateInvitationsResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ListCustomDataIdentifiersResponseTypeDef,
+    DescribeBucketsRequestDescribeBucketsPaginateTypeDef,
+    ListAllowListsRequestListAllowListsPaginateTypeDef,
+    ListClassificationScopesRequestListClassificationScopesPaginateTypeDef,
+    ListCustomDataIdentifiersRequestListCustomDataIdentifiersPaginateTypeDef,
+    ListFindingsFiltersRequestListFindingsFiltersPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListManagedDataIdentifiersRequestListManagedDataIdentifiersPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListResourceProfileArtifactsRequestListResourceProfileArtifactsPaginateTypeDef,
+    ListResourceProfileDetectionsRequestListResourceProfileDetectionsPaginateTypeDef,
+    ListSensitivityInspectionTemplatesRequestListSensitivityInspectionTemplatesPaginateTypeDef,
     GetSensitiveDataOccurrencesResponseTypeDef,
     ListResourceProfileDetectionsResponseTypeDef,
     ListFindingsFiltersResponseTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetMasterAccountResponseTypeDef,
     ListInvitationsResponseTypeDef,
     GetFindingStatisticsResponseTypeDef,
@@ -659,96 +633,111 @@
     GetFindingsRequestRequestTypeDef,
     GetResourceProfileResponseTypeDef,
     GetRevealConfigurationResponseTypeDef,
     UpdateRevealConfigurationRequestRequestTypeDef,
     UpdateRevealConfigurationResponseTypeDef,
     GetSensitiveDataOccurrencesRequestFindingRevealedWaitTypeDef,
     GetSensitivityInspectionTemplateResponseTypeDef,
-    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     GetUsageStatisticsRequestGetUsageStatisticsPaginateTypeDef,
     GetUsageStatisticsRequestRequestTypeDef,
     GetUsageTotalsResponseTypeDef,
     IpAddressDetailsTypeDef,
+    JobScheduleFrequencyOutputTypeDef,
     JobScheduleFrequencyTypeDef,
     ListJobsFilterCriteriaTypeDef,
     ListManagedDataIdentifiersResponseTypeDef,
     ListMembersResponseTypeDef,
     ListResourceProfileArtifactsResponseTypeDef,
     ListSensitivityInspectionTemplatesResponseTypeDef,
     PageTypeDef,
     S3ObjectTypeDef,
     S3ClassificationScopeTypeDef,
     S3ClassificationScopeUpdateTypeDef,
     SearchResourcesTagCriterionTypeDef,
+    SensitivityInspectionTemplateExcludesUnionTypeDef,
+    SensitivityInspectionTemplateIncludesUnionTypeDef,
+    UpdateSensitivityInspectionTemplateRequestRequestTypeDef,
     UsageByAccountTypeDef,
     SessionContextTypeDef,
     UpdateResourceProfileDetectionsRequestRequestTypeDef,
+    TagCriterionForJobOutputTypeDef,
     TagCriterionForJobTypeDef,
+    TagScopeTermOutputTypeDef,
     TagScopeTermTypeDef,
     CreateAllowListRequestRequestTypeDef,
     GetAllowListResponseTypeDef,
     UpdateAllowListRequestRequestTypeDef,
     BucketPermissionConfigurationTypeDef,
     MatchingResourceTypeDef,
     GetBucketStatisticsResponseTypeDef,
     GetClassificationExportConfigurationResponseTypeDef,
     PutClassificationExportConfigurationRequestRequestTypeDef,
     PutClassificationExportConfigurationResponseTypeDef,
+    GetFindingsFilterResponseTypeDef,
     CreateFindingsFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingStatisticsRequestRequestTypeDef,
-    GetFindingsFilterResponseTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFindingsFilterRequestRequestTypeDef,
+    JobScheduleFrequencyUnionTypeDef,
     ListClassificationJobsRequestListClassificationJobsPaginateTypeDef,
     ListClassificationJobsRequestRequestTypeDef,
     OccurrencesTypeDef,
     GetClassificationScopeResponseTypeDef,
     UpdateClassificationScopeRequestRequestTypeDef,
     SearchResourcesCriteriaTypeDef,
     UsageRecordTypeDef,
     AssumedRoleTypeDef,
     FederatedUserTypeDef,
+    CriteriaForJobOutputTypeDef,
     CriteriaForJobTypeDef,
+    JobScopeTermOutputTypeDef,
     JobScopeTermTypeDef,
     BucketPublicAccessTypeDef,
     SearchResourcesResponseTypeDef,
     CustomDetectionTypeDef,
     DefaultDetectionTypeDef,
     SearchResourcesCriteriaBlockTypeDef,
     GetUsageStatisticsResponseTypeDef,
     UserIdentityTypeDef,
+    CriteriaBlockForJobOutputTypeDef,
     CriteriaBlockForJobTypeDef,
+    JobScopingBlockOutputTypeDef,
     JobScopingBlockTypeDef,
     BucketMetadataTypeDef,
     S3BucketTypeDef,
     CustomDataIdentifiersTypeDef,
     SensitiveDataItemTypeDef,
     SearchResourcesBucketCriteriaTypeDef,
     FindingActorTypeDef,
+    S3BucketCriteriaForJobOutputTypeDef,
     S3BucketCriteriaForJobTypeDef,
+    ScopingOutputTypeDef,
     ScopingTypeDef,
     DescribeBucketsResponseTypeDef,
     ResourcesAffectedTypeDef,
     ClassificationResultTypeDef,
     SearchResourcesRequestRequestTypeDef,
     SearchResourcesRequestSearchResourcesPaginateTypeDef,
     PolicyDetailsTypeDef,
     JobSummaryTypeDef,
+    S3JobDefinitionOutputTypeDef,
     S3JobDefinitionTypeDef,
     ClassificationDetailsTypeDef,
     ListClassificationJobsResponseTypeDef,
-    CreateClassificationJobRequestRequestTypeDef,
     DescribeClassificationJobResponseTypeDef,
+    CreateClassificationJobRequestRequestTypeDef,
+    S3JobDefinitionUnionTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptInvitationRequestRequestTypeDef:
+def get_value() -> AcceptInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-macie2-2.5.2/types_aiobotocore_macie2.egg-info/SOURCES.txt` & `types-aiobotocore-macie2-2.5.2.post1/types_aiobotocore_macie2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


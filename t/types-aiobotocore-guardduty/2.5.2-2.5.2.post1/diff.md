# Comparing `tmp/types-aiobotocore-guardduty-2.5.2.tar.gz` & `tmp/types-aiobotocore-guardduty-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-guardduty-2.5.2.tar", last modified: Sat Jul  8 01:43:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-guardduty-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:21 2023, max compression
```

## Comparing `types-aiobotocore-guardduty-2.5.2.tar` & `types-aiobotocore-guardduty-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.234218 types-aiobotocore-guardduty-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    26224 2023-07-08 01:43:42.234218 types-aiobotocore-guardduty-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24651 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:42.234218 types-aiobotocore-guardduty-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.234218 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52639 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    52552 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-07-08 01:31:52.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12552 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    93113 2023-07-08 01:31:55.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    93026 2023-07-08 01:31:54.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:51.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.234218 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    26224 2023-07-08 01:43:42.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:42.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:42.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:42.000000 types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.913575 types-aiobotocore-guardduty-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-08-02 14:52:21.905575 types-aiobotocore-guardduty-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24838 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:21.913575 types-aiobotocore-guardduty-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.905575 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52674 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52587 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14015 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-08-02 14:39:50.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    94451 2023-08-02 14:39:53.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94364 2023-08-02 14:39:51.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:49.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:21.905575 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26364 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:21.000000 types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-guardduty-2.5.2/LICENSE` & `types-aiobotocore-guardduty-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2/PKG-INFO` & `types-aiobotocore-guardduty-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-guardduty
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore guardduty type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore guardduty type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-guardduty"></a>
 
 # types-aiobotocore-guardduty
 
 [![PyPI - types-aiobotocore-guardduty](https://img.shields.io/pypi/v/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-guardduty?color=blue)](https://pypistats.org/packages/types-aiobotocore-guardduty)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.GuardDuty 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [types-aiobotocore-guardduty docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/).
 
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
@@ -377,20 +376,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_guardduty.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_guardduty.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
@@ -403,44 +402,43 @@
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
-    CreateFilterResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
@@ -455,58 +453,42 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
-    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
     LineageObjectTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
     MemberAdditionalConfigurationResultTypeDef,
     MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
@@ -518,61 +500,80 @@
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
-    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
     StartMalwareScanRequestRequestTypeDef,
-    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateIPSetResponseTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetThreatIntelSetResponseTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
+    StartMalwareScanResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
@@ -597,25 +598,27 @@
     OrganizationFeatureConfigurationResultTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
+    ScanConditionOutputTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
-    CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -629,14 +632,15 @@
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
     CoverageResourceTypeDef,
     PublicAccessTypeDef,
     GetCoverageStatisticsRequestRequestTypeDef,
@@ -653,14 +657,15 @@
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
@@ -674,15 +679,15 @@
     GetMemberDetectorsResponseTypeDef,
     ServiceTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-guardduty-2.5.2/README.md` & `types-aiobotocore-guardduty-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-guardduty"></a>
 
 # types-aiobotocore-guardduty
 
 [![PyPI - types-aiobotocore-guardduty](https://img.shields.io/pypi/v/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-guardduty?color=blue)](https://pypistats.org/packages/types-aiobotocore-guardduty)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.GuardDuty 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [types-aiobotocore-guardduty docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/).
 
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
@@ -344,20 +344,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_guardduty.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_guardduty.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
@@ -370,44 +370,43 @@
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
-    CreateFilterResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
@@ -422,58 +421,42 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
-    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
     LineageObjectTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
     MemberAdditionalConfigurationResultTypeDef,
     MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
@@ -485,61 +468,80 @@
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
-    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
     StartMalwareScanRequestRequestTypeDef,
-    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateIPSetResponseTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetThreatIntelSetResponseTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
+    StartMalwareScanResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
@@ -564,25 +566,27 @@
     OrganizationFeatureConfigurationResultTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
+    ScanConditionOutputTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
-    CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -596,14 +600,15 @@
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
     CoverageResourceTypeDef,
     PublicAccessTypeDef,
     GetCoverageStatisticsRequestRequestTypeDef,
@@ -620,14 +625,15 @@
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
@@ -641,15 +647,15 @@
     GetMemberDetectorsResponseTypeDef,
     ServiceTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-guardduty-2.5.2/setup.py` & `types-aiobotocore-guardduty-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-guardduty",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_guardduty"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore guardduty type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore guardduty type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_guardduty": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/"
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/__init__.py` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/__init__.pyi` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/__main__.py` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.GuardDuty 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.GuardDuty 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty\nOther"
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

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/client.py` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
@@ -91,15 +91,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
-    ScanResourceCriteriaTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
@@ -212,15 +212,15 @@
         """
 
     async def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: FindingCriteriaTypeDef,
+        FindingCriteria: FindingCriteriaUnionTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -531,15 +531,15 @@
         """
 
     async def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings_statistics)
         """
@@ -692,15 +692,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_filters)
         """
 
     async def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -860,15 +860,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_filter)
         """
@@ -904,15 +904,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_ip_set)
         """
 
     async def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
+        ScanResourceCriteria: ScanResourceCriteriaUnionTypeDef = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_malware_scan_settings)
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/client.pyi` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     DescribeMalwareScansResponseTypeDef,
     DescribeOrganizationConfigurationResponseTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     DestinationPropertiesTypeDef,
     DetectorFeatureConfigurationTypeDef,
     DisassociateMembersResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
     GetDetectorResponseTypeDef,
     GetFilterResponseTypeDef,
     GetFindingsResponseTypeDef,
     GetFindingsStatisticsResponseTypeDef,
     GetInvitationsCountResponseTypeDef,
@@ -91,15 +91,15 @@
     ListOrganizationAdminAccountsResponseTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThreatIntelSetsResponseTypeDef,
     MemberFeaturesConfigurationTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     OrganizationFeatureConfigurationTypeDef,
-    ScanResourceCriteriaTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     SortCriteriaTypeDef,
     StartMalwareScanResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateFilterResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     UsageCriteriaTypeDef,
@@ -201,15 +201,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#create_detector)
         """
     async def create_filter(
         self,
         *,
         DetectorId: str,
         Name: str,
-        FindingCriteria: FindingCriteriaTypeDef,
+        FindingCriteria: FindingCriteriaUnionTypeDef,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
         ClientToken: str = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateFilterResponseTypeDef:
         """
@@ -492,15 +492,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings)
         """
     async def get_findings_statistics(
         self,
         *,
         DetectorId: str,
         FindingStatisticTypes: Sequence[Literal["COUNT_BY_SEVERITY"]],
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> GetFindingsStatisticsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings statistics for the specified detector ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.get_findings_statistics)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#get_findings_statistics)
         """
@@ -639,15 +639,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.list_filters)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#list_filters)
         """
     async def list_findings(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
         MaxResults: int = ...,
         NextToken: str = ...
     ) -> ListFindingsResponseTypeDef:
         """
         Lists Amazon GuardDuty findings for the specified detector ID.
 
@@ -792,15 +792,15 @@
         self,
         *,
         DetectorId: str,
         FilterName: str,
         Description: str = ...,
         Action: FilterActionType = ...,
         Rank: int = ...,
-        FindingCriteria: FindingCriteriaTypeDef = ...
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...
     ) -> UpdateFilterResponseTypeDef:
         """
         Updates the filter specified by the filter name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_filter)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_filter)
         """
@@ -833,15 +833,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_ip_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_ip_set)
         """
     async def update_malware_scan_settings(
         self,
         *,
         DetectorId: str,
-        ScanResourceCriteria: ScanResourceCriteriaTypeDef = ...,
+        ScanResourceCriteria: ScanResourceCriteriaUnionTypeDef = ...,
         EbsSnapshotPreservation: EbsSnapshotPreservationType = ...
     ) -> Dict[str, Any]:
         """
         Updates the malware scan settings.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Client.update_malware_scan_settings)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/client/#update_malware_scan_settings)
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/literals.py` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/literals.pyi` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/paginator.py` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -94,15 +94,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#describemalwarescanspaginator)
         """
 
 
@@ -114,45 +114,45 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
         SortCriteria: CoverageSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listcoveragepaginator)
         """
 
 
 class ListDetectorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listdetectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDetectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listdetectorspaginator)
         """
 
 
 class ListFiltersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfilterspaginator)
         """
 
 
@@ -162,47 +162,47 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
         """
 
 
 class ListIPSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listipsetspaginator)
         """
 
 
 class ListInvitationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listinvitationspaginator)
         """
 
 
@@ -213,43 +213,43 @@
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listmemberspaginator)
         """
 
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listorganizationadminaccountspaginator)
         """
 
 
 class ListThreatIntelSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listthreatintelsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThreatIntelSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listthreatintelsetspaginator)
         """
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/paginator.pyi` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from botocore.paginate import PageIterator
 
 from .type_defs import (
     CoverageFilterCriteriaTypeDef,
     CoverageSortCriteriaTypeDef,
     DescribeMalwareScansResponseTypeDef,
     FilterCriteriaTypeDef,
-    FindingCriteriaTypeDef,
+    FindingCriteriaUnionTypeDef,
     ListCoverageResponseTypeDef,
     ListDetectorsResponseTypeDef,
     ListFiltersResponseTypeDef,
     ListFindingsResponseTypeDef,
     ListInvitationsResponseTypeDef,
     ListIPSetsResponseTypeDef,
     ListMembersResponseTypeDef,
@@ -91,15 +91,15 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: FilterCriteriaTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMalwareScansResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.DescribeMalwareScans.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#describemalwarescanspaginator)
         """
 
 class ListCoveragePaginator(AioPaginator):
@@ -110,43 +110,43 @@
 
     def paginate(
         self,
         *,
         DetectorId: str,
         FilterCriteria: CoverageFilterCriteriaTypeDef = ...,
         SortCriteria: CoverageSortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoverageResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListCoverage.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listcoveragepaginator)
         """
 
 class ListDetectorsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listdetectorspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDetectorsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListDetectors.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listdetectorspaginator)
         """
 
 class ListFiltersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfilterspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFiltersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFilters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfilterspaginator)
         """
 
 class ListFindingsPaginator(AioPaginator):
@@ -155,45 +155,45 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
-        FindingCriteria: FindingCriteriaTypeDef = ...,
+        FindingCriteria: FindingCriteriaUnionTypeDef = ...,
         SortCriteria: SortCriteriaTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFindingsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListFindings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listfindingspaginator)
         """
 
 class ListIPSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listipsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIPSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListIPSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listipsetspaginator)
         """
 
 class ListInvitationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listinvitationspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListInvitationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListInvitations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listinvitationspaginator)
         """
 
 class ListMembersPaginator(AioPaginator):
@@ -203,41 +203,41 @@
     """
 
     def paginate(
         self,
         *,
         DetectorId: str,
         OnlyAssociated: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMembersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListMembers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listmemberspaginator)
         """
 
 class ListOrganizationAdminAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listorganizationadminaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListOrganizationAdminAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListOrganizationAdminAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listorganizationadminaccountspaginator)
         """
 
 class ListThreatIntelSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listthreatintelsetspaginator)
     """
 
     def paginate(
-        self, *, DetectorId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DetectorId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThreatIntelSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty.Paginator.ListThreatIntelSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/paginators/#listthreatintelsetspaginator)
         """
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/type_defs.py` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
     CoverageFilterCriterionKeyType,
     CoverageSortKeyType,
     CoverageStatisticsTypeType,
@@ -73,44 +73,43 @@
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
-    "CreateFilterResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIPSetRequestRequestTypeDef",
-    "CreateIPSetResponseTypeDef",
     "UnprocessedAccountTypeDef",
     "DestinationPropertiesTypeDef",
-    "CreatePublishingDestinationResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "CreateThreatIntelSetRequestRequestTypeDef",
-    "CreateThreatIntelSetResponseTypeDef",
     "DNSLogsConfigurationResultTypeDef",
     "FlowLogsConfigurationResultTypeDef",
     "S3LogsConfigurationResultTypeDef",
     "S3LogsConfigurationTypeDef",
     "DataSourceFreeTrialTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DefaultServerSideEncryptionTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
     "DestinationTypeDef",
     "DetectorAdditionalConfigurationResultTypeDef",
     "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
@@ -125,58 +124,42 @@
     "FilterConditionTypeDef",
     "FindingStatisticsTypeDef",
     "GeoLocationTypeDef",
     "GetAdministratorAccountRequestRequestTypeDef",
     "GetDetectorRequestRequestTypeDef",
     "GetFilterRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
-    "GetIPSetResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
     "GetMalwareScanSettingsRequestRequestTypeDef",
     "GetMasterAccountRequestRequestTypeDef",
     "MasterTypeDef",
     "GetMemberDetectorsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "GetRemainingFreeTrialDaysRequestRequestTypeDef",
     "GetThreatIntelSetRequestRequestTypeDef",
-    "GetThreatIntelSetResponseTypeDef",
     "UsageCriteriaTypeDef",
     "HighestSeverityThreatDetailsTypeDef",
     "HostPathTypeDef",
     "IamInstanceProfileTypeDef",
     "ProductCodeTypeDef",
     "InvitationTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "KubernetesAuditLogsConfigurationResultTypeDef",
     "KubernetesAuditLogsConfigurationTypeDef",
     "KubernetesUserDetailsTypeDef",
     "LineageObjectTypeDef",
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
     "ListDetectorsRequestRequestTypeDef",
-    "ListDetectorsResponseTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
-    "ListFiltersResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListIPSetsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListPublishingDestinationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "ListThreatIntelSetsRequestRequestTypeDef",
-    "ListThreatIntelSetsResponseTypeDef",
     "LocalIpDetailsTypeDef",
     "LocalPortDetailsTypeDef",
     "LoginAttributeTypeDef",
     "ScanEc2InstanceWithFindingsTypeDef",
     "MemberAdditionalConfigurationResultTypeDef",
     "MemberAdditionalConfigurationTypeDef",
     "RemotePortDetailsTypeDef",
@@ -188,61 +171,80 @@
     "OrganizationS3LogsConfigurationTypeDef",
     "OrganizationEbsVolumesResultTypeDef",
     "OrganizationEbsVolumesTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
-    "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
     "StartMalwareScanRequestRequestTypeDef",
-    "StartMalwareScanResponseTypeDef",
     "StartMonitoringMembersRequestRequestTypeDef",
     "StopMonitoringMembersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TotalTypeDef",
     "UnarchiveFindingsRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateIPSetResponseTypeDef",
+    "CreatePublishingDestinationResponseTypeDef",
+    "CreateThreatIntelSetResponseTypeDef",
+    "GetAdministratorAccountResponseTypeDef",
     "GetCoverageStatisticsResponseTypeDef",
+    "GetIPSetResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetThreatIntelSetResponseTypeDef",
+    "ListDetectorsResponseTypeDef",
+    "ListFiltersResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListIPSetsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListThreatIntelSetsResponseTypeDef",
+    "StartMalwareScanResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
     "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
     "DetectorFeatureConfigurationResultTypeDef",
     "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
@@ -267,25 +269,27 @@
     "OrganizationFeatureConfigurationResultTypeDef",
     "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
+    "ScanConditionOutputTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
-    "CreateFilterRequestRequestTypeDef",
     "GetFilterResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -299,14 +303,15 @@
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
+    "ScanResourceCriteriaOutputTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
     "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
     "GetCoverageStatisticsRequestRequestTypeDef",
@@ -323,14 +328,15 @@
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
+    "ScanResourceCriteriaUnionTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
@@ -497,14 +503,33 @@
 CloudTrailConfigurationResultTypeDef = TypedDict(
     "CloudTrailConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "Eq": List[str],
+        "Neq": List[str],
+        "Gt": int,
+        "Gte": int,
+        "Lt": int,
+        "Lte": int,
+        "Equals": List[str],
+        "NotEquals": List[str],
+        "GreaterThan": int,
+        "GreaterThanOrEqual": int,
+        "LessThan": int,
+        "LessThanOrEqual": int,
+    },
+    total=False,
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "Eq": Sequence[str],
         "Neq": Sequence[str],
         "Gt": int,
         "Gte": int,
@@ -569,19 +594,22 @@
     {
         "CountByResourceType": Dict[Literal["EKS"], int],
         "CountByCoverageStatus": Dict[CoverageStatusType, int],
     },
     total=False,
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -603,22 +631,14 @@
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
 
-CreateIPSetResponseTypeDef = TypedDict(
-    "CreateIPSetResponseTypeDef",
-    {
-        "IpSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Result": str,
     },
 )
@@ -628,22 +648,14 @@
     {
         "DestinationArn": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-CreatePublishingDestinationResponseTypeDef = TypedDict(
-    "CreatePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSampleFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalCreateSampleFindingsRequestRequestTypeDef = TypedDict(
@@ -685,22 +697,14 @@
 class CreateThreatIntelSetRequestRequestTypeDef(
     _RequiredCreateThreatIntelSetRequestRequestTypeDef,
     _OptionalCreateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
 
-CreateThreatIntelSetResponseTypeDef = TypedDict(
-    "CreateThreatIntelSetResponseTypeDef",
-    {
-        "ThreatIntelSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DNSLogsConfigurationResultTypeDef = TypedDict(
     "DNSLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -799,14 +803,24 @@
     "DeleteThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
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
 SortCriteriaTypeDef = TypedDict(
     "SortCriteriaTypeDef",
     {
         "AttributeName": str,
         "OrderBy": OrderByType,
     },
     total=False,
@@ -1001,34 +1015,14 @@
     "GetIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
 
-GetIPSetResponseTypeDef = TypedDict(
-    "GetIPSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": IpSetFormatType,
-        "Location": str,
-        "Status": IpSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "GetMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 
@@ -1117,26 +1111,14 @@
     "GetThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
-GetThreatIntelSetResponseTypeDef = TypedDict(
-    "GetThreatIntelSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": ThreatIntelSetFormatType,
-        "Location": str,
-        "Status": ThreatIntelSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UsageCriteriaTypeDef = TypedDict(
     "UsageCriteriaTypeDef",
     {
         "AccountIds": Sequence[str],
         "DataSources": Sequence[DataSourceType],
         "Resources": Sequence[str],
         "Features": Sequence[UsageFeatureType],
@@ -1251,62 +1233,23 @@
         "ExecutablePath": str,
         "Euid": int,
         "ParentUuid": str,
     },
     total=False,
 )
 
-ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDetectorsRequestRequestTypeDef = TypedDict(
     "ListDetectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDetectorsResponseTypeDef = TypedDict(
-    "ListDetectorsResponseTypeDef",
-    {
-        "DetectorIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFiltersRequestListFiltersPaginateTypeDef(
-    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
-    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredListFiltersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFiltersRequestRequestTypeDef = TypedDict(
@@ -1321,54 +1264,14 @@
 
 class ListFiltersRequestRequestTypeDef(
     _RequiredListFiltersRequestRequestTypeDef, _OptionalListFiltersRequestRequestTypeDef
 ):
     pass
 
 
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
-    {
-        "FilterNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "FindingIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIPSetsRequestListIPSetsPaginateTypeDef(
-    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
-    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIPSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListIPSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListIPSetsRequestRequestTypeDef = TypedDict(
@@ -1383,63 +1286,23 @@
 
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
 
-ListIPSetsResponseTypeDef = TypedDict(
-    "ListIPSetsResponseTypeDef",
-    {
-        "IpSetIds": List[str],
-        "NextToken": str,
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
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersRequestListMembersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListMembersRequestListMembersPaginateTypeDef(
-    _RequiredListMembersRequestListMembersPaginateTypeDef,
-    _OptionalListMembersRequestListMembersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListMembersRequestRequestTypeDef = TypedDict(
@@ -1455,22 +1318,14 @@
 
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
 
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
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1502,44 +1357,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
-    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThreatIntelSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListThreatIntelSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListThreatIntelSetsRequestRequestTypeDef = TypedDict(
@@ -1555,23 +1380,14 @@
 class ListThreatIntelSetsRequestRequestTypeDef(
     _RequiredListThreatIntelSetsRequestRequestTypeDef,
     _OptionalListThreatIntelSetsRequestRequestTypeDef,
 ):
     pass
 
 
-ListThreatIntelSetsResponseTypeDef = TypedDict(
-    "ListThreatIntelSetsResponseTypeDef",
-    {
-        "ThreatIntelSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -1727,24 +1543,14 @@
     "OwnerTypeDef",
     {
         "Id": str,
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
 RdsDbUserDetailsTypeDef = TypedDict(
     "RdsDbUserDetailsTypeDef",
     {
         "User": str,
         "Application": str,
         "Database": str,
         "Ssl": str,
@@ -1757,25 +1563,14 @@
     "ResourceDetailsTypeDef",
     {
         "InstanceArn": str,
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
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
@@ -1851,22 +1646,14 @@
 StartMalwareScanRequestRequestTypeDef = TypedDict(
     "StartMalwareScanRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-StartMalwareScanResponseTypeDef = TypedDict(
-    "StartMalwareScanResponseTypeDef",
-    {
-        "ScanId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartMonitoringMembersRequestRequestTypeDef = TypedDict(
     "StartMonitoringMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -1908,22 +1695,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFindingsFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
         "Feedback": FeedbackType,
     },
@@ -2016,41 +1795,32 @@
         "CoveredNodes": int,
         "CompatibleNodes": int,
         "AddonDetails": AddonDetailsTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAdministratorAccountResponseTypeDef = TypedDict(
-    "GetAdministratorAccountResponseTypeDef",
-    {
-        "Administrator": AdministratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "Criterion": Dict[str, ConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "Criterion": Mapping[str, ConditionTypeDef],
     },
     total=False,
 )
@@ -2074,91 +1844,241 @@
     {
         "CriterionKey": CoverageFilterCriterionKeyType,
         "FilterCondition": CoverageFilterConditionTypeDef,
     },
     total=False,
 )
 
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIPSetResponseTypeDef = TypedDict(
+    "CreateIPSetResponseTypeDef",
+    {
+        "IpSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePublishingDestinationResponseTypeDef = TypedDict(
+    "CreatePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThreatIntelSetResponseTypeDef = TypedDict(
+    "CreateThreatIntelSetResponseTypeDef",
+    {
+        "ThreatIntelSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAdministratorAccountResponseTypeDef = TypedDict(
+    "GetAdministratorAccountResponseTypeDef",
+    {
+        "Administrator": AdministratorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCoverageStatisticsResponseTypeDef = TypedDict(
     "GetCoverageStatisticsResponseTypeDef",
     {
         "CoverageStatistics": CoverageStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIPSetResponseTypeDef = TypedDict(
+    "GetIPSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": IpSetFormatType,
+        "Location": str,
+        "Status": IpSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThreatIntelSetResponseTypeDef = TypedDict(
+    "GetThreatIntelSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": ThreatIntelSetFormatType,
+        "Location": str,
+        "Status": ThreatIntelSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDetectorsResponseTypeDef = TypedDict(
+    "ListDetectorsResponseTypeDef",
+    {
+        "DetectorIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
+    {
+        "FilterNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "FindingIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIPSetsResponseTypeDef = TypedDict(
+    "ListIPSetsResponseTypeDef",
+    {
+        "IpSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
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
+ListThreatIntelSetsResponseTypeDef = TypedDict(
+    "ListThreatIntelSetsResponseTypeDef",
+    {
+        "ThreatIntelSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMalwareScanResponseTypeDef = TypedDict(
+    "StartMalwareScanResponseTypeDef",
+    {
+        "ScanId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateMembersResponseTypeDef = TypedDict(
     "DisassociateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMonitoringMembersResponseTypeDef = TypedDict(
     "StartMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopMonitoringMembersResponseTypeDef = TypedDict(
     "StopMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMemberDetectorsResponseTypeDef = TypedDict(
     "UpdateMemberDetectorsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2186,15 +2106,15 @@
     "DescribePublishingDestinationResponseTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
         "PublishingFailureStartTimestamp": int,
         "DestinationProperties": DestinationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2229,14 +2149,127 @@
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     {
         "ScanEc2InstanceWithFindings": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
 
+ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFiltersRequestListFiltersPaginateTypeDef(
+    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
+    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIPSetsRequestListIPSetsPaginateTypeDef(
+    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
+    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
+):
+    pass
+
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersRequestListMembersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListMembersRequestListMembersPaginateTypeDef(
+    _RequiredListMembersRequestListMembersPaginateTypeDef,
+    _OptionalListMembersRequestListMembersPaginateTypeDef,
+):
+    pass
+
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
+    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+):
+    pass
+
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
     },
 )
@@ -2256,15 +2289,15 @@
 
 
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectorFeatureConfigurationResultTypeDef = TypedDict(
     "DetectorFeatureConfigurationResultTypeDef",
     {
         "Name": DetectorFeatureResultType,
@@ -2345,41 +2378,41 @@
     total=False,
 )
 
 GetFindingsStatisticsResponseTypeDef = TypedDict(
     "GetFindingsStatisticsResponseTypeDef",
     {
         "FindingStatistics": FindingStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": MasterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2415,15 +2448,15 @@
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KubernetesConfigurationResultTypeDef = TypedDict(
     "KubernetesConfigurationResultTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationResultTypeDef,
@@ -2571,18 +2604,25 @@
         "GeoLocation": GeoLocationTypeDef,
         "IpAddressV4": str,
         "Organization": OrganizationTypeDef,
     },
     total=False,
 )
 
+ScanConditionOutputTypeDef = TypedDict(
+    "ScanConditionOutputTypeDef",
+    {
+        "MapEquals": List[ScanConditionPairTypeDef],
+    },
+)
+
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
-        "MapEquals": List[ScanConditionPairTypeDef],
+        "MapEquals": Sequence[ScanConditionPairTypeDef],
     },
 )
 
 ScanThreatNameTypeDef = TypedDict(
     "ScanThreatNameTypeDef",
     {
         "Name": str,
@@ -2665,14 +2705,27 @@
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
 )
 
+GetFilterResponseTypeDef = TypedDict(
+    "GetFilterResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Action": FilterActionType,
+        "Rank": int,
+        "FindingCriteria": FindingCriteriaOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
@@ -2692,27 +2745,15 @@
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
 
-GetFilterResponseTypeDef = TypedDict(
-    "GetFilterResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Action": FilterActionType,
-        "Rank": int,
-        "FindingCriteria": FindingCriteriaTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -2739,15 +2780,15 @@
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListFindingsRequestListFindingsPaginateTypeDef(
     _RequiredListFindingsRequestListFindingsPaginateTypeDef,
@@ -3022,19 +3063,28 @@
     {
         "RemoteIpDetails": RemoteIpDetailsTypeDef,
         "LoginAttributes": List[LoginAttributeTypeDef],
     },
     total=False,
 )
 
+ScanResourceCriteriaOutputTypeDef = TypedDict(
+    "ScanResourceCriteriaOutputTypeDef",
+    {
+        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 ScanResourceCriteriaTypeDef = TypedDict(
     "ScanResourceCriteriaTypeDef",
     {
-        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
-        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Include": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Exclude": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
     },
     total=False,
 )
 
 ThreatDetectedByNameTypeDef = TypedDict(
     "ThreatDetectedByNameTypeDef",
     {
@@ -3047,15 +3097,15 @@
 )
 
 DescribeMalwareScansResponseTypeDef = TypedDict(
     "DescribeMalwareScansResponseTypeDef",
     {
         "Scans": List[ScanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageStatisticsTypeDef = TypedDict(
     "UsageStatisticsTypeDef",
     {
         "SumByAccount": List[UsageAccountResultTypeDef],
@@ -3120,15 +3170,15 @@
     },
 )
 _OptionalListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "_OptionalListCoverageRequestListCoveragePaginateTypeDef",
     {
         "FilterCriteria": CoverageFilterCriteriaTypeDef,
         "SortCriteria": CoverageSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class ListCoverageRequestListCoveragePaginateTypeDef(
     _RequiredListCoverageRequestListCoveragePaginateTypeDef,
@@ -3211,15 +3261,15 @@
     },
 )
 _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = TypedDict(
     "_OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     {
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef(
     _RequiredDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
@@ -3400,20 +3450,23 @@
     },
     total=False,
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
-        "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
+        "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScanResourceCriteriaUnionTypeDef = Union[
+    ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
+]
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
@@ -3445,24 +3498,24 @@
 )
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "UsageStatistics": UsageStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "Resources": List[CoverageResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3BucketDetailTypeDef = TypedDict(
     "S3BucketDetailTypeDef",
     {
         "Arn": str,
@@ -3478,30 +3531,30 @@
 )
 
 GetRemainingFreeTrialDaysResponseTypeDef = TypedDict(
     "GetRemainingFreeTrialDaysResponseTypeDef",
     {
         "Accounts": List[AccountFreeTrialInfoTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDetectorResponseTypeDef = TypedDict(
     "GetDetectorResponseTypeDef",
     {
         "CreatedAt": str,
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "ServiceRole": str,
         "Status": DetectorStatusType,
         "UpdatedAt": str,
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Tags": Dict[str, str],
         "Features": List[DetectorFeatureConfigurationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMemberDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredMemberDataSourceConfigurationTypeDef",
     {
         "AccountId": str,
@@ -3524,28 +3577,28 @@
 
 
 CreateDetectorResponseTypeDef = TypedDict(
     "CreateDetectorResponseTypeDef",
     {
         "DetectorId": str,
         "UnprocessedDataSources": UnprocessedDataSourcesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3618,15 +3671,15 @@
 )
 
 GetMemberDetectorsResponseTypeDef = TypedDict(
     "GetMemberDetectorsResponseTypeDef",
     {
         "MemberDataSourceConfigurations": List[MemberDataSourceConfigurationTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Action": ActionTypeDef,
@@ -3679,10 +3732,10 @@
     pass
 
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty/type_defs.pyi` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_guardduty.type_defs import AcceptAdministratorInvitationRequestRequestTypeDef
 
-    data: AcceptAdministratorInvitationRequestRequestTypeDef = {...}
+    data: AcceptAdministratorInvitationRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AdminStatusType,
     AutoEnableMembersType,
     CoverageFilterCriterionKeyType,
     CoverageSortKeyType,
     CoverageStatisticsTypeType,
@@ -72,44 +72,43 @@
     "AdministratorTypeDef",
     "ArchiveFindingsRequestRequestTypeDef",
     "DomainDetailsTypeDef",
     "RemoteAccountDetailsTypeDef",
     "BucketPolicyTypeDef",
     "CityTypeDef",
     "CloudTrailConfigurationResultTypeDef",
+    "ConditionOutputTypeDef",
     "ConditionTypeDef",
     "SecurityContextTypeDef",
     "VolumeMountTypeDef",
     "CountryTypeDef",
     "CoverageFilterConditionTypeDef",
     "CoverageSortCriteriaTypeDef",
     "CoverageStatisticsTypeDef",
-    "CreateFilterResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateIPSetRequestRequestTypeDef",
-    "CreateIPSetResponseTypeDef",
     "UnprocessedAccountTypeDef",
     "DestinationPropertiesTypeDef",
-    "CreatePublishingDestinationResponseTypeDef",
     "CreateSampleFindingsRequestRequestTypeDef",
     "CreateThreatIntelSetRequestRequestTypeDef",
-    "CreateThreatIntelSetResponseTypeDef",
     "DNSLogsConfigurationResultTypeDef",
     "FlowLogsConfigurationResultTypeDef",
     "S3LogsConfigurationResultTypeDef",
     "S3LogsConfigurationTypeDef",
     "DataSourceFreeTrialTypeDef",
     "DeclineInvitationsRequestRequestTypeDef",
     "DefaultServerSideEncryptionTypeDef",
     "DeleteDetectorRequestRequestTypeDef",
     "DeleteFilterRequestRequestTypeDef",
     "DeleteIPSetRequestRequestTypeDef",
     "DeleteInvitationsRequestRequestTypeDef",
     "DeleteMembersRequestRequestTypeDef",
     "DeletePublishingDestinationRequestRequestTypeDef",
     "DeleteThreatIntelSetRequestRequestTypeDef",
+    "PaginatorConfigTypeDef",
     "SortCriteriaTypeDef",
     "DescribeOrganizationConfigurationRequestRequestTypeDef",
     "DescribePublishingDestinationRequestRequestTypeDef",
     "DestinationTypeDef",
     "DetectorAdditionalConfigurationResultTypeDef",
     "DetectorAdditionalConfigurationTypeDef",
     "DisableOrganizationAdminAccountRequestRequestTypeDef",
@@ -124,58 +123,42 @@
     "FilterConditionTypeDef",
     "FindingStatisticsTypeDef",
     "GeoLocationTypeDef",
     "GetAdministratorAccountRequestRequestTypeDef",
     "GetDetectorRequestRequestTypeDef",
     "GetFilterRequestRequestTypeDef",
     "GetIPSetRequestRequestTypeDef",
-    "GetIPSetResponseTypeDef",
-    "GetInvitationsCountResponseTypeDef",
     "GetMalwareScanSettingsRequestRequestTypeDef",
     "GetMasterAccountRequestRequestTypeDef",
     "MasterTypeDef",
     "GetMemberDetectorsRequestRequestTypeDef",
     "GetMembersRequestRequestTypeDef",
     "MemberTypeDef",
     "GetRemainingFreeTrialDaysRequestRequestTypeDef",
     "GetThreatIntelSetRequestRequestTypeDef",
-    "GetThreatIntelSetResponseTypeDef",
     "UsageCriteriaTypeDef",
     "HighestSeverityThreatDetailsTypeDef",
     "HostPathTypeDef",
     "IamInstanceProfileTypeDef",
     "ProductCodeTypeDef",
     "InvitationTypeDef",
     "InviteMembersRequestRequestTypeDef",
     "KubernetesAuditLogsConfigurationResultTypeDef",
     "KubernetesAuditLogsConfigurationTypeDef",
     "KubernetesUserDetailsTypeDef",
     "LineageObjectTypeDef",
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
     "ListDetectorsRequestRequestTypeDef",
-    "ListDetectorsResponseTypeDef",
-    "ListFiltersRequestListFiltersPaginateTypeDef",
     "ListFiltersRequestRequestTypeDef",
-    "ListFiltersResponseTypeDef",
-    "ListFindingsResponseTypeDef",
-    "ListIPSetsRequestListIPSetsPaginateTypeDef",
     "ListIPSetsRequestRequestTypeDef",
-    "ListIPSetsResponseTypeDef",
-    "ListInvitationsRequestListInvitationsPaginateTypeDef",
     "ListInvitationsRequestRequestTypeDef",
-    "ListMembersRequestListMembersPaginateTypeDef",
     "ListMembersRequestRequestTypeDef",
-    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
     "ListOrganizationAdminAccountsRequestRequestTypeDef",
     "ListPublishingDestinationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "ListThreatIntelSetsRequestRequestTypeDef",
-    "ListThreatIntelSetsResponseTypeDef",
     "LocalIpDetailsTypeDef",
     "LocalPortDetailsTypeDef",
     "LoginAttributeTypeDef",
     "ScanEc2InstanceWithFindingsTypeDef",
     "MemberAdditionalConfigurationResultTypeDef",
     "MemberAdditionalConfigurationTypeDef",
     "RemotePortDetailsTypeDef",
@@ -187,61 +170,80 @@
     "OrganizationS3LogsConfigurationTypeDef",
     "OrganizationEbsVolumesResultTypeDef",
     "OrganizationEbsVolumesTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationResultTypeDef",
     "OrganizationKubernetesAuditLogsConfigurationTypeDef",
     "OrganizationTypeDef",
     "OwnerTypeDef",
-    "PaginatorConfigTypeDef",
     "RdsDbUserDetailsTypeDef",
     "ResourceDetailsTypeDef",
-    "ResponseMetadataTypeDef",
     "ScanConditionPairTypeDef",
     "ScannedItemCountTypeDef",
     "ThreatsDetectedItemCountTypeDef",
     "ScanFilePathTypeDef",
     "ScanResultDetailsTypeDef",
     "TriggerDetailsTypeDef",
     "ServiceAdditionalInfoTypeDef",
     "StartMalwareScanRequestRequestTypeDef",
-    "StartMalwareScanResponseTypeDef",
     "StartMonitoringMembersRequestRequestTypeDef",
     "StopMonitoringMembersRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TotalTypeDef",
     "UnarchiveFindingsRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateFilterResponseTypeDef",
     "UpdateFindingsFeedbackRequestRequestTypeDef",
     "UpdateIPSetRequestRequestTypeDef",
     "UpdateThreatIntelSetRequestRequestTypeDef",
     "CreateMembersRequestRequestTypeDef",
     "AccountLevelPermissionsTypeDef",
     "CoverageEksClusterDetailsTypeDef",
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    "GetAdministratorAccountResponseTypeDef",
     "BucketLevelPermissionsTypeDef",
+    "FindingCriteriaOutputTypeDef",
     "FindingCriteriaTypeDef",
     "ContainerTypeDef",
     "CoverageFilterCriterionTypeDef",
+    "CreateFilterResponseTypeDef",
+    "CreateIPSetResponseTypeDef",
+    "CreatePublishingDestinationResponseTypeDef",
+    "CreateThreatIntelSetResponseTypeDef",
+    "GetAdministratorAccountResponseTypeDef",
     "GetCoverageStatisticsResponseTypeDef",
+    "GetIPSetResponseTypeDef",
+    "GetInvitationsCountResponseTypeDef",
+    "GetThreatIntelSetResponseTypeDef",
+    "ListDetectorsResponseTypeDef",
+    "ListFiltersResponseTypeDef",
+    "ListFindingsResponseTypeDef",
+    "ListIPSetsResponseTypeDef",
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "ListThreatIntelSetsResponseTypeDef",
+    "StartMalwareScanResponseTypeDef",
+    "UpdateFilterResponseTypeDef",
     "CreateMembersResponseTypeDef",
     "DeclineInvitationsResponseTypeDef",
     "DeleteInvitationsResponseTypeDef",
     "DeleteMembersResponseTypeDef",
     "DisassociateMembersResponseTypeDef",
     "InviteMembersResponseTypeDef",
     "StartMonitoringMembersResponseTypeDef",
     "StopMonitoringMembersResponseTypeDef",
     "UpdateMemberDetectorsResponseTypeDef",
     "CreatePublishingDestinationRequestRequestTypeDef",
     "DescribePublishingDestinationResponseTypeDef",
     "UpdatePublishingDestinationRequestRequestTypeDef",
     "KubernetesDataSourceFreeTrialTypeDef",
     "MalwareProtectionDataSourceFreeTrialTypeDef",
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    "ListFiltersRequestListFiltersPaginateTypeDef",
+    "ListIPSetsRequestListIPSetsPaginateTypeDef",
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    "ListMembersRequestListMembersPaginateTypeDef",
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    "ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
     "GetFindingsRequestRequestTypeDef",
     "ListPublishingDestinationsResponseTypeDef",
     "DetectorFeatureConfigurationResultTypeDef",
     "DetectorFeatureConfigurationTypeDef",
     "EbsVolumeDetailsTypeDef",
     "ScanEc2InstanceWithFindingsResultTypeDef",
     "EksClusterDetailsTypeDef",
@@ -266,25 +268,27 @@
     "OrganizationFeatureConfigurationResultTypeDef",
     "OrganizationFeatureConfigurationTypeDef",
     "OrganizationScanEc2InstanceWithFindingsResultTypeDef",
     "OrganizationScanEc2InstanceWithFindingsTypeDef",
     "OrganizationKubernetesConfigurationResultTypeDef",
     "OrganizationKubernetesConfigurationTypeDef",
     "RemoteIpDetailsTypeDef",
+    "ScanConditionOutputTypeDef",
     "ScanConditionTypeDef",
     "ScanThreatNameTypeDef",
     "ScanTypeDef",
     "UsageAccountResultTypeDef",
     "UsageDataSourceResultTypeDef",
     "UsageFeatureResultTypeDef",
     "UsageResourceResultTypeDef",
     "CoverageResourceDetailsTypeDef",
     "PermissionConfigurationTypeDef",
-    "CreateFilterRequestRequestTypeDef",
     "GetFilterResponseTypeDef",
+    "CreateFilterRequestRequestTypeDef",
+    "FindingCriteriaUnionTypeDef",
     "GetFindingsStatisticsRequestRequestTypeDef",
     "ListFindingsRequestListFindingsPaginateTypeDef",
     "ListFindingsRequestRequestTypeDef",
     "UpdateFilterRequestRequestTypeDef",
     "CoverageFilterCriteriaTypeDef",
     "DataSourcesFreeTrialTypeDef",
     "MalwareProtectionConfigurationResultTypeDef",
@@ -298,14 +302,15 @@
     "OrganizationMalwareProtectionConfigurationResultTypeDef",
     "OrganizationMalwareProtectionConfigurationTypeDef",
     "AwsApiCallActionTypeDef",
     "KubernetesApiCallActionTypeDef",
     "NetworkConnectionActionTypeDef",
     "PortProbeDetailTypeDef",
     "RdsLoginAttemptActionTypeDef",
+    "ScanResourceCriteriaOutputTypeDef",
     "ScanResourceCriteriaTypeDef",
     "ThreatDetectedByNameTypeDef",
     "DescribeMalwareScansResponseTypeDef",
     "UsageStatisticsTypeDef",
     "CoverageResourceTypeDef",
     "PublicAccessTypeDef",
     "GetCoverageStatisticsRequestRequestTypeDef",
@@ -322,14 +327,15 @@
     "CreateDetectorRequestRequestTypeDef",
     "UpdateDetectorRequestRequestTypeDef",
     "UpdateMemberDetectorsRequestRequestTypeDef",
     "OrganizationDataSourceConfigurationsResultTypeDef",
     "OrganizationDataSourceConfigurationsTypeDef",
     "PortProbeActionTypeDef",
     "GetMalwareScanSettingsResponseTypeDef",
+    "ScanResourceCriteriaUnionTypeDef",
     "UpdateMalwareScanSettingsRequestRequestTypeDef",
     "ScanDetectionsTypeDef",
     "GetUsageStatisticsResponseTypeDef",
     "ListCoverageResponseTypeDef",
     "S3BucketDetailTypeDef",
     "GetRemainingFreeTrialDaysResponseTypeDef",
     "GetDetectorResponseTypeDef",
@@ -496,14 +502,33 @@
 CloudTrailConfigurationResultTypeDef = TypedDict(
     "CloudTrailConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
+ConditionOutputTypeDef = TypedDict(
+    "ConditionOutputTypeDef",
+    {
+        "Eq": List[str],
+        "Neq": List[str],
+        "Gt": int,
+        "Gte": int,
+        "Lt": int,
+        "Lte": int,
+        "Equals": List[str],
+        "NotEquals": List[str],
+        "GreaterThan": int,
+        "GreaterThanOrEqual": int,
+        "LessThan": int,
+        "LessThanOrEqual": int,
+    },
+    total=False,
+)
+
 ConditionTypeDef = TypedDict(
     "ConditionTypeDef",
     {
         "Eq": Sequence[str],
         "Neq": Sequence[str],
         "Gt": int,
         "Gte": int,
@@ -568,19 +593,22 @@
     {
         "CountByResourceType": Dict[Literal["EKS"], int],
         "CountByCoverageStatus": Dict[CoverageStatusType, int],
     },
     total=False,
 )
 
-CreateFilterResponseTypeDef = TypedDict(
-    "CreateFilterResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateIPSetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -600,22 +628,14 @@
 )
 
 class CreateIPSetRequestRequestTypeDef(
     _RequiredCreateIPSetRequestRequestTypeDef, _OptionalCreateIPSetRequestRequestTypeDef
 ):
     pass
 
-CreateIPSetResponseTypeDef = TypedDict(
-    "CreateIPSetResponseTypeDef",
-    {
-        "IpSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UnprocessedAccountTypeDef = TypedDict(
     "UnprocessedAccountTypeDef",
     {
         "AccountId": str,
         "Result": str,
     },
 )
@@ -625,22 +645,14 @@
     {
         "DestinationArn": str,
         "KmsKeyArn": str,
     },
     total=False,
 )
 
-CreatePublishingDestinationResponseTypeDef = TypedDict(
-    "CreatePublishingDestinationResponseTypeDef",
-    {
-        "DestinationId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSampleFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSampleFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalCreateSampleFindingsRequestRequestTypeDef = TypedDict(
@@ -678,22 +690,14 @@
 
 class CreateThreatIntelSetRequestRequestTypeDef(
     _RequiredCreateThreatIntelSetRequestRequestTypeDef,
     _OptionalCreateThreatIntelSetRequestRequestTypeDef,
 ):
     pass
 
-CreateThreatIntelSetResponseTypeDef = TypedDict(
-    "CreateThreatIntelSetResponseTypeDef",
-    {
-        "ThreatIntelSetId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DNSLogsConfigurationResultTypeDef = TypedDict(
     "DNSLogsConfigurationResultTypeDef",
     {
         "Status": DataSourceStatusType,
     },
 )
 
@@ -792,14 +796,24 @@
     "DeleteThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
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
 SortCriteriaTypeDef = TypedDict(
     "SortCriteriaTypeDef",
     {
         "AttributeName": str,
         "OrderBy": OrderByType,
     },
     total=False,
@@ -992,34 +1006,14 @@
     "GetIPSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "IpSetId": str,
     },
 )
 
-GetIPSetResponseTypeDef = TypedDict(
-    "GetIPSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": IpSetFormatType,
-        "Location": str,
-        "Status": IpSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetInvitationsCountResponseTypeDef = TypedDict(
-    "GetInvitationsCountResponseTypeDef",
-    {
-        "InvitationsCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "GetMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 
@@ -1104,26 +1098,14 @@
     "GetThreatIntelSetRequestRequestTypeDef",
     {
         "DetectorId": str,
         "ThreatIntelSetId": str,
     },
 )
 
-GetThreatIntelSetResponseTypeDef = TypedDict(
-    "GetThreatIntelSetResponseTypeDef",
-    {
-        "Name": str,
-        "Format": ThreatIntelSetFormatType,
-        "Location": str,
-        "Status": ThreatIntelSetStatusType,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UsageCriteriaTypeDef = TypedDict(
     "UsageCriteriaTypeDef",
     {
         "AccountIds": Sequence[str],
         "DataSources": Sequence[DataSourceType],
         "Resources": Sequence[str],
         "Features": Sequence[UsageFeatureType],
@@ -1236,60 +1218,23 @@
         "ExecutablePath": str,
         "Euid": int,
         "ParentUuid": str,
     },
     total=False,
 )
 
-ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
-    "ListDetectorsRequestListDetectorsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDetectorsRequestRequestTypeDef = TypedDict(
     "ListDetectorsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDetectorsResponseTypeDef = TypedDict(
-    "ListDetectorsResponseTypeDef",
-    {
-        "DetectorIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
-    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFiltersRequestListFiltersPaginateTypeDef(
-    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
-    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
-):
-    pass
-
 _RequiredListFiltersRequestRequestTypeDef = TypedDict(
     "_RequiredListFiltersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListFiltersRequestRequestTypeDef = TypedDict(
@@ -1302,52 +1247,14 @@
 )
 
 class ListFiltersRequestRequestTypeDef(
     _RequiredListFiltersRequestRequestTypeDef, _OptionalListFiltersRequestRequestTypeDef
 ):
     pass
 
-ListFiltersResponseTypeDef = TypedDict(
-    "ListFiltersResponseTypeDef",
-    {
-        "FilterNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListFindingsResponseTypeDef = TypedDict(
-    "ListFindingsResponseTypeDef",
-    {
-        "FindingIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
-    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIPSetsRequestListIPSetsPaginateTypeDef(
-    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
-    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListIPSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListIPSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListIPSetsRequestRequestTypeDef = TypedDict(
@@ -1360,61 +1267,23 @@
 )
 
 class ListIPSetsRequestRequestTypeDef(
     _RequiredListIPSetsRequestRequestTypeDef, _OptionalListIPSetsRequestRequestTypeDef
 ):
     pass
 
-ListIPSetsResponseTypeDef = TypedDict(
-    "ListIPSetsResponseTypeDef",
-    {
-        "IpSetIds": List[str],
-        "NextToken": str,
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
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_RequiredListMembersRequestListMembersPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
-    "_OptionalListMembersRequestListMembersPaginateTypeDef",
-    {
-        "OnlyAssociated": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListMembersRequestListMembersPaginateTypeDef(
-    _RequiredListMembersRequestListMembersPaginateTypeDef,
-    _OptionalListMembersRequestListMembersPaginateTypeDef,
-):
-    pass
-
 _RequiredListMembersRequestRequestTypeDef = TypedDict(
     "_RequiredListMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListMembersRequestRequestTypeDef = TypedDict(
@@ -1428,22 +1297,14 @@
 )
 
 class ListMembersRequestRequestTypeDef(
     _RequiredListMembersRequestRequestTypeDef, _OptionalListMembersRequestRequestTypeDef
 ):
     pass
 
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
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1473,42 +1334,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "DetectorId": str,
-    },
-)
-_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
-    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
-    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListThreatIntelSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListThreatIntelSetsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalListThreatIntelSetsRequestRequestTypeDef = TypedDict(
@@ -1522,23 +1355,14 @@
 
 class ListThreatIntelSetsRequestRequestTypeDef(
     _RequiredListThreatIntelSetsRequestRequestTypeDef,
     _OptionalListThreatIntelSetsRequestRequestTypeDef,
 ):
     pass
 
-ListThreatIntelSetsResponseTypeDef = TypedDict(
-    "ListThreatIntelSetsResponseTypeDef",
-    {
-        "ThreatIntelSetIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocalIpDetailsTypeDef = TypedDict(
     "LocalIpDetailsTypeDef",
     {
         "IpAddressV4": str,
     },
     total=False,
 )
@@ -1694,24 +1518,14 @@
     "OwnerTypeDef",
     {
         "Id": str,
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
 RdsDbUserDetailsTypeDef = TypedDict(
     "RdsDbUserDetailsTypeDef",
     {
         "User": str,
         "Application": str,
         "Database": str,
         "Ssl": str,
@@ -1724,25 +1538,14 @@
     "ResourceDetailsTypeDef",
     {
         "InstanceArn": str,
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
 _RequiredScanConditionPairTypeDef = TypedDict(
     "_RequiredScanConditionPairTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalScanConditionPairTypeDef = TypedDict(
@@ -1816,22 +1619,14 @@
 StartMalwareScanRequestRequestTypeDef = TypedDict(
     "StartMalwareScanRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-StartMalwareScanResponseTypeDef = TypedDict(
-    "StartMalwareScanResponseTypeDef",
-    {
-        "ScanId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartMonitoringMembersRequestRequestTypeDef = TypedDict(
     "StartMonitoringMembersRequestRequestTypeDef",
     {
         "DetectorId": str,
         "AccountIds": Sequence[str],
     },
 )
@@ -1873,22 +1668,14 @@
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
 
-UpdateFilterResponseTypeDef = TypedDict(
-    "UpdateFilterResponseTypeDef",
-    {
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateFindingsFeedbackRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateFindingsFeedbackRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
         "Feedback": FeedbackType,
     },
@@ -1975,41 +1762,32 @@
         "CoveredNodes": int,
         "CompatibleNodes": int,
         "AddonDetails": AddonDetailsTypeDef,
     },
     total=False,
 )
 
-ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
-    "ListOrganizationAdminAccountsResponseTypeDef",
-    {
-        "AdminAccounts": List[AdminAccountTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAdministratorAccountResponseTypeDef = TypedDict(
-    "GetAdministratorAccountResponseTypeDef",
-    {
-        "Administrator": AdministratorTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BucketLevelPermissionsTypeDef = TypedDict(
     "BucketLevelPermissionsTypeDef",
     {
         "AccessControlList": AccessControlListTypeDef,
         "BucketPolicy": BucketPolicyTypeDef,
         "BlockPublicAccess": BlockPublicAccessTypeDef,
     },
     total=False,
 )
 
+FindingCriteriaOutputTypeDef = TypedDict(
+    "FindingCriteriaOutputTypeDef",
+    {
+        "Criterion": Dict[str, ConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 FindingCriteriaTypeDef = TypedDict(
     "FindingCriteriaTypeDef",
     {
         "Criterion": Mapping[str, ConditionTypeDef],
     },
     total=False,
 )
@@ -2033,91 +1811,241 @@
     {
         "CriterionKey": CoverageFilterCriterionKeyType,
         "FilterCondition": CoverageFilterConditionTypeDef,
     },
     total=False,
 )
 
+CreateFilterResponseTypeDef = TypedDict(
+    "CreateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIPSetResponseTypeDef = TypedDict(
+    "CreateIPSetResponseTypeDef",
+    {
+        "IpSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePublishingDestinationResponseTypeDef = TypedDict(
+    "CreatePublishingDestinationResponseTypeDef",
+    {
+        "DestinationId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateThreatIntelSetResponseTypeDef = TypedDict(
+    "CreateThreatIntelSetResponseTypeDef",
+    {
+        "ThreatIntelSetId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAdministratorAccountResponseTypeDef = TypedDict(
+    "GetAdministratorAccountResponseTypeDef",
+    {
+        "Administrator": AdministratorTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetCoverageStatisticsResponseTypeDef = TypedDict(
     "GetCoverageStatisticsResponseTypeDef",
     {
         "CoverageStatistics": CoverageStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIPSetResponseTypeDef = TypedDict(
+    "GetIPSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": IpSetFormatType,
+        "Location": str,
+        "Status": IpSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetInvitationsCountResponseTypeDef = TypedDict(
+    "GetInvitationsCountResponseTypeDef",
+    {
+        "InvitationsCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThreatIntelSetResponseTypeDef = TypedDict(
+    "GetThreatIntelSetResponseTypeDef",
+    {
+        "Name": str,
+        "Format": ThreatIntelSetFormatType,
+        "Location": str,
+        "Status": ThreatIntelSetStatusType,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDetectorsResponseTypeDef = TypedDict(
+    "ListDetectorsResponseTypeDef",
+    {
+        "DetectorIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFiltersResponseTypeDef = TypedDict(
+    "ListFiltersResponseTypeDef",
+    {
+        "FilterNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListFindingsResponseTypeDef = TypedDict(
+    "ListFindingsResponseTypeDef",
+    {
+        "FindingIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIPSetsResponseTypeDef = TypedDict(
+    "ListIPSetsResponseTypeDef",
+    {
+        "IpSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListOrganizationAdminAccountsResponseTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountTypeDef],
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
+ListThreatIntelSetsResponseTypeDef = TypedDict(
+    "ListThreatIntelSetsResponseTypeDef",
+    {
+        "ThreatIntelSetIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartMalwareScanResponseTypeDef = TypedDict(
+    "StartMalwareScanResponseTypeDef",
+    {
+        "ScanId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateFilterResponseTypeDef = TypedDict(
+    "UpdateFilterResponseTypeDef",
+    {
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateMembersResponseTypeDef = TypedDict(
     "CreateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeclineInvitationsResponseTypeDef = TypedDict(
     "DeclineInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteInvitationsResponseTypeDef = TypedDict(
     "DeleteInvitationsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMembersResponseTypeDef = TypedDict(
     "DeleteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateMembersResponseTypeDef = TypedDict(
     "DisassociateMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InviteMembersResponseTypeDef = TypedDict(
     "InviteMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMonitoringMembersResponseTypeDef = TypedDict(
     "StartMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopMonitoringMembersResponseTypeDef = TypedDict(
     "StopMonitoringMembersResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMemberDetectorsResponseTypeDef = TypedDict(
     "UpdateMemberDetectorsResponseTypeDef",
     {
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2143,15 +2071,15 @@
     "DescribePublishingDestinationResponseTypeDef",
     {
         "DestinationId": str,
         "DestinationType": Literal["S3"],
         "Status": PublishingStatusType,
         "PublishingFailureStartTimestamp": int,
         "DestinationProperties": DestinationPropertiesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdatePublishingDestinationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePublishingDestinationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2184,14 +2112,119 @@
     "MalwareProtectionDataSourceFreeTrialTypeDef",
     {
         "ScanEc2InstanceWithFindings": DataSourceFreeTrialTypeDef,
     },
     total=False,
 )
 
+ListDetectorsRequestListDetectorsPaginateTypeDef = TypedDict(
+    "ListDetectorsRequestListDetectorsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_RequiredListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListFiltersRequestListFiltersPaginateTypeDef = TypedDict(
+    "_OptionalListFiltersRequestListFiltersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFiltersRequestListFiltersPaginateTypeDef(
+    _RequiredListFiltersRequestListFiltersPaginateTypeDef,
+    _OptionalListFiltersRequestListFiltersPaginateTypeDef,
+):
+    pass
+
+_RequiredListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_RequiredListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListIPSetsRequestListIPSetsPaginateTypeDef = TypedDict(
+    "_OptionalListIPSetsRequestListIPSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIPSetsRequestListIPSetsPaginateTypeDef(
+    _RequiredListIPSetsRequestListIPSetsPaginateTypeDef,
+    _OptionalListIPSetsRequestListIPSetsPaginateTypeDef,
+):
+    pass
+
+ListInvitationsRequestListInvitationsPaginateTypeDef = TypedDict(
+    "ListInvitationsRequestListInvitationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_RequiredListMembersRequestListMembersPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListMembersRequestListMembersPaginateTypeDef = TypedDict(
+    "_OptionalListMembersRequestListMembersPaginateTypeDef",
+    {
+        "OnlyAssociated": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListMembersRequestListMembersPaginateTypeDef(
+    _RequiredListMembersRequestListMembersPaginateTypeDef,
+    _OptionalListMembersRequestListMembersPaginateTypeDef,
+):
+    pass
+
+ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef = TypedDict(
+    "ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "DetectorId": str,
+    },
+)
+_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef = TypedDict(
+    "_OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef(
+    _RequiredListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+    _OptionalListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
+):
+    pass
+
 _RequiredGetFindingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingIds": Sequence[str],
     },
 )
@@ -2209,15 +2242,15 @@
     pass
 
 ListPublishingDestinationsResponseTypeDef = TypedDict(
     "ListPublishingDestinationsResponseTypeDef",
     {
         "Destinations": List[DestinationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DetectorFeatureConfigurationResultTypeDef = TypedDict(
     "DetectorFeatureConfigurationResultTypeDef",
     {
         "Name": DetectorFeatureResultType,
@@ -2298,41 +2331,41 @@
     total=False,
 )
 
 GetFindingsStatisticsResponseTypeDef = TypedDict(
     "GetFindingsStatisticsResponseTypeDef",
     {
         "FindingStatistics": FindingStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMasterAccountResponseTypeDef = TypedDict(
     "GetMasterAccountResponseTypeDef",
     {
         "Master": MasterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetMembersResponseTypeDef = TypedDict(
     "GetMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListMembersResponseTypeDef = TypedDict(
     "ListMembersResponseTypeDef",
     {
         "Members": List[MemberTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetUsageStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetUsageStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -2366,15 +2399,15 @@
 )
 
 ListInvitationsResponseTypeDef = TypedDict(
     "ListInvitationsResponseTypeDef",
     {
         "Invitations": List[InvitationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 KubernetesConfigurationResultTypeDef = TypedDict(
     "KubernetesConfigurationResultTypeDef",
     {
         "AuditLogs": KubernetesAuditLogsConfigurationResultTypeDef,
@@ -2522,18 +2555,25 @@
         "GeoLocation": GeoLocationTypeDef,
         "IpAddressV4": str,
         "Organization": OrganizationTypeDef,
     },
     total=False,
 )
 
+ScanConditionOutputTypeDef = TypedDict(
+    "ScanConditionOutputTypeDef",
+    {
+        "MapEquals": List[ScanConditionPairTypeDef],
+    },
+)
+
 ScanConditionTypeDef = TypedDict(
     "ScanConditionTypeDef",
     {
-        "MapEquals": List[ScanConditionPairTypeDef],
+        "MapEquals": Sequence[ScanConditionPairTypeDef],
     },
 )
 
 ScanThreatNameTypeDef = TypedDict(
     "ScanThreatNameTypeDef",
     {
         "Name": str,
@@ -2616,14 +2656,27 @@
     {
         "BucketLevelPermissions": BucketLevelPermissionsTypeDef,
         "AccountLevelPermissions": AccountLevelPermissionsTypeDef,
     },
     total=False,
 )
 
+GetFilterResponseTypeDef = TypedDict(
+    "GetFilterResponseTypeDef",
+    {
+        "Name": str,
+        "Description": str,
+        "Action": FilterActionType,
+        "Rank": int,
+        "FindingCriteria": FindingCriteriaOutputTypeDef,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFilterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFilterRequestRequestTypeDef",
     {
         "DetectorId": str,
         "Name": str,
         "FindingCriteria": FindingCriteriaTypeDef,
     },
@@ -2641,27 +2694,15 @@
 )
 
 class CreateFilterRequestRequestTypeDef(
     _RequiredCreateFilterRequestRequestTypeDef, _OptionalCreateFilterRequestRequestTypeDef
 ):
     pass
 
-GetFilterResponseTypeDef = TypedDict(
-    "GetFilterResponseTypeDef",
-    {
-        "Name": str,
-        "Description": str,
-        "Action": FilterActionType,
-        "Rank": int,
-        "FindingCriteria": FindingCriteriaTypeDef,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+FindingCriteriaUnionTypeDef = Union[FindingCriteriaTypeDef, FindingCriteriaOutputTypeDef]
 _RequiredGetFindingsStatisticsRequestRequestTypeDef = TypedDict(
     "_RequiredGetFindingsStatisticsRequestRequestTypeDef",
     {
         "DetectorId": str,
         "FindingStatisticTypes": Sequence[Literal["COUNT_BY_SEVERITY"]],
     },
 )
@@ -2686,15 +2727,15 @@
     },
 )
 _OptionalListFindingsRequestListFindingsPaginateTypeDef = TypedDict(
     "_OptionalListFindingsRequestListFindingsPaginateTypeDef",
     {
         "FindingCriteria": FindingCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListFindingsRequestListFindingsPaginateTypeDef(
     _RequiredListFindingsRequestListFindingsPaginateTypeDef,
     _OptionalListFindingsRequestListFindingsPaginateTypeDef,
@@ -2963,19 +3004,28 @@
     {
         "RemoteIpDetails": RemoteIpDetailsTypeDef,
         "LoginAttributes": List[LoginAttributeTypeDef],
     },
     total=False,
 )
 
+ScanResourceCriteriaOutputTypeDef = TypedDict(
+    "ScanResourceCriteriaOutputTypeDef",
+    {
+        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionOutputTypeDef],
+    },
+    total=False,
+)
+
 ScanResourceCriteriaTypeDef = TypedDict(
     "ScanResourceCriteriaTypeDef",
     {
-        "Include": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
-        "Exclude": Dict[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Include": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
+        "Exclude": Mapping[Literal["EC2_INSTANCE_TAG"], ScanConditionTypeDef],
     },
     total=False,
 )
 
 ThreatDetectedByNameTypeDef = TypedDict(
     "ThreatDetectedByNameTypeDef",
     {
@@ -2988,15 +3038,15 @@
 )
 
 DescribeMalwareScansResponseTypeDef = TypedDict(
     "DescribeMalwareScansResponseTypeDef",
     {
         "Scans": List[ScanTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UsageStatisticsTypeDef = TypedDict(
     "UsageStatisticsTypeDef",
     {
         "SumByAccount": List[UsageAccountResultTypeDef],
@@ -3059,15 +3109,15 @@
     },
 )
 _OptionalListCoverageRequestListCoveragePaginateTypeDef = TypedDict(
     "_OptionalListCoverageRequestListCoveragePaginateTypeDef",
     {
         "FilterCriteria": CoverageFilterCriteriaTypeDef,
         "SortCriteria": CoverageSortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class ListCoverageRequestListCoveragePaginateTypeDef(
     _RequiredListCoverageRequestListCoveragePaginateTypeDef,
     _OptionalListCoverageRequestListCoveragePaginateTypeDef,
@@ -3144,15 +3194,15 @@
     },
 )
 _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef = TypedDict(
     "_OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef",
     {
         "FilterCriteria": FilterCriteriaTypeDef,
         "SortCriteria": SortCriteriaTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class DescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef(
     _RequiredDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
     _OptionalDescribeMalwareScansRequestDescribeMalwareScansPaginateTypeDef,
@@ -3321,20 +3371,23 @@
     },
     total=False,
 )
 
 GetMalwareScanSettingsResponseTypeDef = TypedDict(
     "GetMalwareScanSettingsResponseTypeDef",
     {
-        "ScanResourceCriteria": ScanResourceCriteriaTypeDef,
+        "ScanResourceCriteria": ScanResourceCriteriaOutputTypeDef,
         "EbsSnapshotPreservation": EbsSnapshotPreservationType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ScanResourceCriteriaUnionTypeDef = Union[
+    ScanResourceCriteriaTypeDef, ScanResourceCriteriaOutputTypeDef
+]
 _RequiredUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateMalwareScanSettingsRequestRequestTypeDef",
     {
         "DetectorId": str,
     },
 )
 _OptionalUpdateMalwareScanSettingsRequestRequestTypeDef = TypedDict(
@@ -3364,24 +3417,24 @@
 )
 
 GetUsageStatisticsResponseTypeDef = TypedDict(
     "GetUsageStatisticsResponseTypeDef",
     {
         "UsageStatistics": UsageStatisticsTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoverageResponseTypeDef = TypedDict(
     "ListCoverageResponseTypeDef",
     {
         "Resources": List[CoverageResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 S3BucketDetailTypeDef = TypedDict(
     "S3BucketDetailTypeDef",
     {
         "Arn": str,
@@ -3397,30 +3450,30 @@
 )
 
 GetRemainingFreeTrialDaysResponseTypeDef = TypedDict(
     "GetRemainingFreeTrialDaysResponseTypeDef",
     {
         "Accounts": List[AccountFreeTrialInfoTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDetectorResponseTypeDef = TypedDict(
     "GetDetectorResponseTypeDef",
     {
         "CreatedAt": str,
         "FindingPublishingFrequency": FindingPublishingFrequencyType,
         "ServiceRole": str,
         "Status": DetectorStatusType,
         "UpdatedAt": str,
         "DataSources": DataSourceConfigurationsResultTypeDef,
         "Tags": Dict[str, str],
         "Features": List[DetectorFeatureConfigurationResultTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredMemberDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredMemberDataSourceConfigurationTypeDef",
     {
         "AccountId": str,
@@ -3441,28 +3494,28 @@
     pass
 
 CreateDetectorResponseTypeDef = TypedDict(
     "CreateDetectorResponseTypeDef",
     {
         "DetectorId": str,
         "UnprocessedDataSources": UnprocessedDataSourcesResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeOrganizationConfigurationResponseTypeDef = TypedDict(
     "DescribeOrganizationConfigurationResponseTypeDef",
     {
         "AutoEnable": bool,
         "MemberAccountLimitReached": bool,
         "DataSources": OrganizationDataSourceConfigurationsResultTypeDef,
         "Features": List[OrganizationFeatureConfigurationResultTypeDef],
         "NextToken": str,
         "AutoEnableOrganizationMembers": AutoEnableMembersType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateOrganizationConfigurationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateOrganizationConfigurationRequestRequestTypeDef",
     {
         "DetectorId": str,
@@ -3533,15 +3586,15 @@
 )
 
 GetMemberDetectorsResponseTypeDef = TypedDict(
     "GetMemberDetectorsResponseTypeDef",
     {
         "MemberDataSourceConfigurations": List[MemberDataSourceConfigurationTypeDef],
         "UnprocessedAccounts": List[UnprocessedAccountTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceTypeDef = TypedDict(
     "ServiceTypeDef",
     {
         "Action": ActionTypeDef,
@@ -3592,10 +3645,10 @@
 class FindingTypeDef(_RequiredFindingTypeDef, _OptionalFindingTypeDef):
     pass
 
 GetFindingsResponseTypeDef = TypedDict(
     "GetFindingsResponseTypeDef",
     {
         "Findings": List[FindingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/PKG-INFO` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-guardduty
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.GuardDuty 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore guardduty type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore guardduty type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-guardduty"></a>
 
 # types-aiobotocore-guardduty
 
 [![PyPI - types-aiobotocore-guardduty](https://img.shields.io/pypi/v/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-guardduty.svg?color=blue)](https://pypi.org/project/types-aiobotocore-guardduty)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-guardduty?color=blue)](https://pypistats.org/packages/types-aiobotocore-guardduty)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-guardduty)](https://pepy.tech/project/types-aiobotocore-guardduty)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.GuardDuty 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/guardduty.html#GuardDuty)
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
 [types-aiobotocore-guardduty docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_guardduty/).
 
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
@@ -377,20 +376,20 @@
 )
 
 
 def check_value(value: AdminStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_guardduty.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_guardduty.type_defs import (
     AcceptAdministratorInvitationRequestRequestTypeDef,
     AcceptInvitationRequestRequestTypeDef,
     AccessControlListTypeDef,
     AccessKeyDetailsTypeDef,
@@ -403,44 +402,43 @@
     AdministratorTypeDef,
     ArchiveFindingsRequestRequestTypeDef,
     DomainDetailsTypeDef,
     RemoteAccountDetailsTypeDef,
     BucketPolicyTypeDef,
     CityTypeDef,
     CloudTrailConfigurationResultTypeDef,
+    ConditionOutputTypeDef,
     ConditionTypeDef,
     SecurityContextTypeDef,
     VolumeMountTypeDef,
     CountryTypeDef,
     CoverageFilterConditionTypeDef,
     CoverageSortCriteriaTypeDef,
     CoverageStatisticsTypeDef,
-    CreateFilterResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateIPSetRequestRequestTypeDef,
-    CreateIPSetResponseTypeDef,
     UnprocessedAccountTypeDef,
     DestinationPropertiesTypeDef,
-    CreatePublishingDestinationResponseTypeDef,
     CreateSampleFindingsRequestRequestTypeDef,
     CreateThreatIntelSetRequestRequestTypeDef,
-    CreateThreatIntelSetResponseTypeDef,
     DNSLogsConfigurationResultTypeDef,
     FlowLogsConfigurationResultTypeDef,
     S3LogsConfigurationResultTypeDef,
     S3LogsConfigurationTypeDef,
     DataSourceFreeTrialTypeDef,
     DeclineInvitationsRequestRequestTypeDef,
     DefaultServerSideEncryptionTypeDef,
     DeleteDetectorRequestRequestTypeDef,
     DeleteFilterRequestRequestTypeDef,
     DeleteIPSetRequestRequestTypeDef,
     DeleteInvitationsRequestRequestTypeDef,
     DeleteMembersRequestRequestTypeDef,
     DeletePublishingDestinationRequestRequestTypeDef,
     DeleteThreatIntelSetRequestRequestTypeDef,
+    PaginatorConfigTypeDef,
     SortCriteriaTypeDef,
     DescribeOrganizationConfigurationRequestRequestTypeDef,
     DescribePublishingDestinationRequestRequestTypeDef,
     DestinationTypeDef,
     DetectorAdditionalConfigurationResultTypeDef,
     DetectorAdditionalConfigurationTypeDef,
     DisableOrganizationAdminAccountRequestRequestTypeDef,
@@ -455,58 +453,42 @@
     FilterConditionTypeDef,
     FindingStatisticsTypeDef,
     GeoLocationTypeDef,
     GetAdministratorAccountRequestRequestTypeDef,
     GetDetectorRequestRequestTypeDef,
     GetFilterRequestRequestTypeDef,
     GetIPSetRequestRequestTypeDef,
-    GetIPSetResponseTypeDef,
-    GetInvitationsCountResponseTypeDef,
     GetMalwareScanSettingsRequestRequestTypeDef,
     GetMasterAccountRequestRequestTypeDef,
     MasterTypeDef,
     GetMemberDetectorsRequestRequestTypeDef,
     GetMembersRequestRequestTypeDef,
     MemberTypeDef,
     GetRemainingFreeTrialDaysRequestRequestTypeDef,
     GetThreatIntelSetRequestRequestTypeDef,
-    GetThreatIntelSetResponseTypeDef,
     UsageCriteriaTypeDef,
     HighestSeverityThreatDetailsTypeDef,
     HostPathTypeDef,
     IamInstanceProfileTypeDef,
     ProductCodeTypeDef,
     InvitationTypeDef,
     InviteMembersRequestRequestTypeDef,
     KubernetesAuditLogsConfigurationResultTypeDef,
     KubernetesAuditLogsConfigurationTypeDef,
     KubernetesUserDetailsTypeDef,
     LineageObjectTypeDef,
-    ListDetectorsRequestListDetectorsPaginateTypeDef,
     ListDetectorsRequestRequestTypeDef,
-    ListDetectorsResponseTypeDef,
-    ListFiltersRequestListFiltersPaginateTypeDef,
     ListFiltersRequestRequestTypeDef,
-    ListFiltersResponseTypeDef,
-    ListFindingsResponseTypeDef,
-    ListIPSetsRequestListIPSetsPaginateTypeDef,
     ListIPSetsRequestRequestTypeDef,
-    ListIPSetsResponseTypeDef,
-    ListInvitationsRequestListInvitationsPaginateTypeDef,
     ListInvitationsRequestRequestTypeDef,
-    ListMembersRequestListMembersPaginateTypeDef,
     ListMembersRequestRequestTypeDef,
-    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
     ListOrganizationAdminAccountsRequestRequestTypeDef,
     ListPublishingDestinationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     ListThreatIntelSetsRequestRequestTypeDef,
-    ListThreatIntelSetsResponseTypeDef,
     LocalIpDetailsTypeDef,
     LocalPortDetailsTypeDef,
     LoginAttributeTypeDef,
     ScanEc2InstanceWithFindingsTypeDef,
     MemberAdditionalConfigurationResultTypeDef,
     MemberAdditionalConfigurationTypeDef,
     RemotePortDetailsTypeDef,
@@ -518,61 +500,80 @@
     OrganizationS3LogsConfigurationTypeDef,
     OrganizationEbsVolumesResultTypeDef,
     OrganizationEbsVolumesTypeDef,
     OrganizationKubernetesAuditLogsConfigurationResultTypeDef,
     OrganizationKubernetesAuditLogsConfigurationTypeDef,
     OrganizationTypeDef,
     OwnerTypeDef,
-    PaginatorConfigTypeDef,
     RdsDbUserDetailsTypeDef,
     ResourceDetailsTypeDef,
-    ResponseMetadataTypeDef,
     ScanConditionPairTypeDef,
     ScannedItemCountTypeDef,
     ThreatsDetectedItemCountTypeDef,
     ScanFilePathTypeDef,
     ScanResultDetailsTypeDef,
     TriggerDetailsTypeDef,
     ServiceAdditionalInfoTypeDef,
     StartMalwareScanRequestRequestTypeDef,
-    StartMalwareScanResponseTypeDef,
     StartMonitoringMembersRequestRequestTypeDef,
     StopMonitoringMembersRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     TotalTypeDef,
     UnarchiveFindingsRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateFilterResponseTypeDef,
     UpdateFindingsFeedbackRequestRequestTypeDef,
     UpdateIPSetRequestRequestTypeDef,
     UpdateThreatIntelSetRequestRequestTypeDef,
     CreateMembersRequestRequestTypeDef,
     AccountLevelPermissionsTypeDef,
     CoverageEksClusterDetailsTypeDef,
-    ListOrganizationAdminAccountsResponseTypeDef,
-    GetAdministratorAccountResponseTypeDef,
     BucketLevelPermissionsTypeDef,
+    FindingCriteriaOutputTypeDef,
     FindingCriteriaTypeDef,
     ContainerTypeDef,
     CoverageFilterCriterionTypeDef,
+    CreateFilterResponseTypeDef,
+    CreateIPSetResponseTypeDef,
+    CreatePublishingDestinationResponseTypeDef,
+    CreateThreatIntelSetResponseTypeDef,
+    GetAdministratorAccountResponseTypeDef,
     GetCoverageStatisticsResponseTypeDef,
+    GetIPSetResponseTypeDef,
+    GetInvitationsCountResponseTypeDef,
+    GetThreatIntelSetResponseTypeDef,
+    ListDetectorsResponseTypeDef,
+    ListFiltersResponseTypeDef,
+    ListFindingsResponseTypeDef,
+    ListIPSetsResponseTypeDef,
+    ListOrganizationAdminAccountsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    ListThreatIntelSetsResponseTypeDef,
+    StartMalwareScanResponseTypeDef,
+    UpdateFilterResponseTypeDef,
     CreateMembersResponseTypeDef,
     DeclineInvitationsResponseTypeDef,
     DeleteInvitationsResponseTypeDef,
     DeleteMembersResponseTypeDef,
     DisassociateMembersResponseTypeDef,
     InviteMembersResponseTypeDef,
     StartMonitoringMembersResponseTypeDef,
     StopMonitoringMembersResponseTypeDef,
     UpdateMemberDetectorsResponseTypeDef,
     CreatePublishingDestinationRequestRequestTypeDef,
     DescribePublishingDestinationResponseTypeDef,
     UpdatePublishingDestinationRequestRequestTypeDef,
     KubernetesDataSourceFreeTrialTypeDef,
     MalwareProtectionDataSourceFreeTrialTypeDef,
+    ListDetectorsRequestListDetectorsPaginateTypeDef,
+    ListFiltersRequestListFiltersPaginateTypeDef,
+    ListIPSetsRequestListIPSetsPaginateTypeDef,
+    ListInvitationsRequestListInvitationsPaginateTypeDef,
+    ListMembersRequestListMembersPaginateTypeDef,
+    ListOrganizationAdminAccountsRequestListOrganizationAdminAccountsPaginateTypeDef,
+    ListThreatIntelSetsRequestListThreatIntelSetsPaginateTypeDef,
     GetFindingsRequestRequestTypeDef,
     ListPublishingDestinationsResponseTypeDef,
     DetectorFeatureConfigurationResultTypeDef,
     DetectorFeatureConfigurationTypeDef,
     EbsVolumeDetailsTypeDef,
     ScanEc2InstanceWithFindingsResultTypeDef,
     EksClusterDetailsTypeDef,
@@ -597,25 +598,27 @@
     OrganizationFeatureConfigurationResultTypeDef,
     OrganizationFeatureConfigurationTypeDef,
     OrganizationScanEc2InstanceWithFindingsResultTypeDef,
     OrganizationScanEc2InstanceWithFindingsTypeDef,
     OrganizationKubernetesConfigurationResultTypeDef,
     OrganizationKubernetesConfigurationTypeDef,
     RemoteIpDetailsTypeDef,
+    ScanConditionOutputTypeDef,
     ScanConditionTypeDef,
     ScanThreatNameTypeDef,
     ScanTypeDef,
     UsageAccountResultTypeDef,
     UsageDataSourceResultTypeDef,
     UsageFeatureResultTypeDef,
     UsageResourceResultTypeDef,
     CoverageResourceDetailsTypeDef,
     PermissionConfigurationTypeDef,
-    CreateFilterRequestRequestTypeDef,
     GetFilterResponseTypeDef,
+    CreateFilterRequestRequestTypeDef,
+    FindingCriteriaUnionTypeDef,
     GetFindingsStatisticsRequestRequestTypeDef,
     ListFindingsRequestListFindingsPaginateTypeDef,
     ListFindingsRequestRequestTypeDef,
     UpdateFilterRequestRequestTypeDef,
     CoverageFilterCriteriaTypeDef,
     DataSourcesFreeTrialTypeDef,
     MalwareProtectionConfigurationResultTypeDef,
@@ -629,14 +632,15 @@
     OrganizationMalwareProtectionConfigurationResultTypeDef,
     OrganizationMalwareProtectionConfigurationTypeDef,
     AwsApiCallActionTypeDef,
     KubernetesApiCallActionTypeDef,
     NetworkConnectionActionTypeDef,
     PortProbeDetailTypeDef,
     RdsLoginAttemptActionTypeDef,
+    ScanResourceCriteriaOutputTypeDef,
     ScanResourceCriteriaTypeDef,
     ThreatDetectedByNameTypeDef,
     DescribeMalwareScansResponseTypeDef,
     UsageStatisticsTypeDef,
     CoverageResourceTypeDef,
     PublicAccessTypeDef,
     GetCoverageStatisticsRequestRequestTypeDef,
@@ -653,14 +657,15 @@
     CreateDetectorRequestRequestTypeDef,
     UpdateDetectorRequestRequestTypeDef,
     UpdateMemberDetectorsRequestRequestTypeDef,
     OrganizationDataSourceConfigurationsResultTypeDef,
     OrganizationDataSourceConfigurationsTypeDef,
     PortProbeActionTypeDef,
     GetMalwareScanSettingsResponseTypeDef,
+    ScanResourceCriteriaUnionTypeDef,
     UpdateMalwareScanSettingsRequestRequestTypeDef,
     ScanDetectionsTypeDef,
     GetUsageStatisticsResponseTypeDef,
     ListCoverageResponseTypeDef,
     S3BucketDetailTypeDef,
     GetRemainingFreeTrialDaysResponseTypeDef,
     GetDetectorResponseTypeDef,
@@ -674,15 +679,15 @@
     GetMemberDetectorsResponseTypeDef,
     ServiceTypeDef,
     FindingTypeDef,
     GetFindingsResponseTypeDef,
 )
 
 
-def get_structure() -> AcceptAdministratorInvitationRequestRequestTypeDef:
+def get_value() -> AcceptAdministratorInvitationRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-guardduty-2.5.2/types_aiobotocore_guardduty.egg-info/SOURCES.txt` & `types-aiobotocore-guardduty-2.5.2.post1/types_aiobotocore_guardduty.egg-info/SOURCES.txt`

 * *Files identical despite different names*


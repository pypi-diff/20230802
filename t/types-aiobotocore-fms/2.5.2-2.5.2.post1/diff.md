# Comparing `tmp/types-aiobotocore-fms-2.5.2.tar.gz` & `tmp/types-aiobotocore-fms-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-fms-2.5.2.tar", last modified: Sat Jul  8 01:43:39 2023, max compression
+gzip compressed data, was "types-aiobotocore-fms-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:19 2023, max compression
```

## Comparing `types-aiobotocore-fms-2.5.2.tar` & `types-aiobotocore-fms-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:39.630169 types-aiobotocore-fms-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-07-08 01:43:39.622169 types-aiobotocore-fms-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19689 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:39.630169 types-aiobotocore-fms-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:39.622169 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32969 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32910 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10164 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    59453 2023-07-08 01:31:00.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    59386 2023-07-08 01:31:00.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:59.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:39.622169 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21238 2023-07-08 01:43:39.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:39.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:39.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:39.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:39.000000 types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20134 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.141583 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32996 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32937 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12999 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12997 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10148 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    64397 2023-08-02 14:38:52.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64322 2023-08-02 14:38:52.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:51.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:19.145583 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21636 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:19.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:18.000000 types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-fms-2.5.2/LICENSE` & `types-aiobotocore-fms-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2/PKG-INFO` & `types-aiobotocore-fms-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore fms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore fms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-fms"></a>
 
 # types-aiobotocore-fms
 
 [![PyPI - types-aiobotocore-fms](https://img.shields.io/pypi/v/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-fms?color=blue)](https://pypistats.org/packages/types-aiobotocore-fms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.FMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [types-aiobotocore-fms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/).
 
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
@@ -357,183 +356,198 @@
 )
 
 
 def check_value(value: AccountRoleStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_fms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_fms.type_defs import (
+    AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeOutputTypeDef,
+    PolicyTypeScopeOutputTypeDef,
+    RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
     AppTypeDef,
+    TimestampTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
-    GetAdminAccountResponseTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
-    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProtectionStatusRequestRequestTypeDef,
-    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
-    ProtocolsListDataTypeDef,
+    ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
-    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
-    ListAdminsManagingAccountResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
-    ListMemberAccountsResponseTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
-    PaginatorConfigTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
-    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
-    ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    GetProtectionStatusRequestRequestTypeDef,
+    ProtocolsListDataTypeDef,
+    ResourceSetTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetNotificationChannelResponseTypeDef,
+    GetProtectionStatusResponseTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
+    AdminScopeUnionTypeDef,
     PutAdminAccountRequestRequestTypeDef,
-    ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
-    PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
+    ListAppsListsResponseTypeDef,
+    AppsListDataUnionTypeDef,
+    PutAppsListRequestRequestTypeDef,
+    ProtocolsListDataUnionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
+    ResourceSetUnionTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    PolicyUnionTypeDef,
+    PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-fms-2.5.2/README.md` & `types-aiobotocore-fms-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-fms"></a>
 
 # types-aiobotocore-fms
 
 [![PyPI - types-aiobotocore-fms](https://img.shields.io/pypi/v/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-fms?color=blue)](https://pypistats.org/packages/types-aiobotocore-fms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.FMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [types-aiobotocore-fms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/).
 
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
@@ -324,183 +324,198 @@
 )
 
 
 def check_value(value: AccountRoleStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_fms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_fms.type_defs import (
+    AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeOutputTypeDef,
+    PolicyTypeScopeOutputTypeDef,
+    RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
     AppTypeDef,
+    TimestampTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
-    GetAdminAccountResponseTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
-    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProtectionStatusRequestRequestTypeDef,
-    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
-    ProtocolsListDataTypeDef,
+    ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
-    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
-    ListAdminsManagingAccountResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
-    ListMemberAccountsResponseTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
-    PaginatorConfigTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
-    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
-    ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    GetProtectionStatusRequestRequestTypeDef,
+    ProtocolsListDataTypeDef,
+    ResourceSetTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetNotificationChannelResponseTypeDef,
+    GetProtectionStatusResponseTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
+    AdminScopeUnionTypeDef,
     PutAdminAccountRequestRequestTypeDef,
-    ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
-    PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
+    ListAppsListsResponseTypeDef,
+    AppsListDataUnionTypeDef,
+    PutAppsListRequestRequestTypeDef,
+    ProtocolsListDataUnionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
+    ResourceSetUnionTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    PolicyUnionTypeDef,
+    PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-fms-2.5.2/setup.py` & `types-aiobotocore-fms-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-fms",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_fms"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore fms type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore fms type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_fms": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/__init__.py` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/__init__.pyi` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/__main__.py` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.FMS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.FMS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS\nOther"
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

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/client.py` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("fms") as client:
         client: FMSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ThirdPartyFirewallType
 from .paginator import (
     ListAdminAccountsForOrganizationPaginator,
@@ -29,16 +28,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeTypeDef,
-    AppsListDataTypeDef,
+    AdminScopeUnionTypeDef,
+    AppsListDataUnionTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -59,22 +58,23 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyTypeDef,
-    ProtocolsListDataTypeDef,
+    PolicyUnionTypeDef,
+    ProtocolsListDataUnionTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -304,16 +304,16 @@
         """
 
     async def get_protection_status(
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS attack.
 
@@ -488,25 +488,25 @@
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#list_third_party_firewall_firewall_policies)
         """
 
     async def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_admin_account)
         """
 
     async def put_apps_list(
-        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_apps_list)
         """
@@ -519,35 +519,35 @@
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_notification_channel)
         """
 
     async def put_policy(
-        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_policy)
         """
 
     async def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_protocols_list)
         """
 
     async def put_resource_set(
-        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_resource_set)
         """
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/client.pyi` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("fms") as client:
         client: FMSClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ThirdPartyFirewallType
 from .paginator import (
     ListAdminAccountsForOrganizationPaginator,
@@ -29,16 +28,16 @@
     ListComplianceStatusPaginator,
     ListMemberAccountsPaginator,
     ListPoliciesPaginator,
     ListProtocolsListsPaginator,
     ListThirdPartyFirewallFirewallPoliciesPaginator,
 )
 from .type_defs import (
-    AdminScopeTypeDef,
-    AppsListDataTypeDef,
+    AdminScopeUnionTypeDef,
+    AppsListDataUnionTypeDef,
     AssociateThirdPartyFirewallResponseTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     DisassociateThirdPartyFirewallResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetAdminAccountResponseTypeDef,
     GetAdminScopeResponseTypeDef,
@@ -59,22 +58,23 @@
     ListMemberAccountsResponseTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
-    PolicyTypeDef,
-    ProtocolsListDataTypeDef,
+    PolicyUnionTypeDef,
+    ProtocolsListDataUnionTypeDef,
     PutAppsListResponseTypeDef,
     PutPolicyResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     PutResourceSetResponseTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetUnionTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -279,16 +279,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#get_policy)
         """
     async def get_protection_status(
         self,
         *,
         PolicyId: str,
         MemberAccountId: str = ...,
-        StartTime: Union[datetime, str] = ...,
-        EndTime: Union[datetime, str] = ...,
+        StartTime: TimestampTypeDef = ...,
+        EndTime: TimestampTypeDef = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> GetProtectionStatusResponseTypeDef:
         """
         If you created a Shield Advanced policy, returns policy-level attack summary
         information in the event of a potential DDoS attack.
 
@@ -446,24 +446,24 @@
         Retrieves a list of all of the third-party firewall policies that are associated
         with the third-party firewall administrator's account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.list_third_party_firewall_firewall_policies)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#list_third_party_firewall_firewall_policies)
         """
     async def put_admin_account(
-        self, *, AdminAccount: str, AdminScope: AdminScopeTypeDef = ...
+        self, *, AdminAccount: str, AdminScope: AdminScopeUnionTypeDef = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         Creates or updates an Firewall Manager administrator account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_admin_account)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_admin_account)
         """
     async def put_apps_list(
-        self, *, AppsList: AppsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, AppsList: AppsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutAppsListResponseTypeDef:
         """
         Creates an Firewall Manager applications list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_apps_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_apps_list)
         """
@@ -474,33 +474,33 @@
         Designates the IAM role and Amazon Simple Notification Service (SNS) topic that
         Firewall Manager uses to record SNS logs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_notification_channel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_notification_channel)
         """
     async def put_policy(
-        self, *, Policy: PolicyTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, Policy: PolicyUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutPolicyResponseTypeDef:
         """
         Creates an Firewall Manager policy.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_policy)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_policy)
         """
     async def put_protocols_list(
-        self, *, ProtocolsList: ProtocolsListDataTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ProtocolsList: ProtocolsListDataUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutProtocolsListResponseTypeDef:
         """
         Creates an Firewall Manager protocols list.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_protocols_list)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_protocols_list)
         """
     async def put_resource_set(
-        self, *, ResourceSet: ResourceSetTypeDef, TagList: Sequence[TagTypeDef] = ...
+        self, *, ResourceSet: ResourceSetUnionTypeDef, TagList: Sequence[TagTypeDef] = ...
     ) -> PutResourceSetResponseTypeDef:
         """
         Creates the resource set.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Client.put_resource_set)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/client/#put_resource_set)
         """
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/literals.py` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/literals.pyi` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/paginator.py` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -59,139 +59,129 @@
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListAdminAccountsForOrganizationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAdminAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminaccountsfororganizationpaginator)
         """
 
-
 class ListAdminsManagingAccountPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminsmanagingaccountpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAdminsManagingAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminsmanagingaccountpaginator)
         """
 
-
 class ListAppsListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listappslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAppsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listappslistspaginator)
         """
 
-
 class ListComplianceStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listcompliancestatuspaginator)
     """
 
     def paginate(
-        self, *, PolicyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComplianceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listcompliancestatuspaginator)
         """
 
-
 class ListMemberAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMemberAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listmemberaccountspaginator)
         """
 
-
 class ListPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listpoliciespaginator)
         """
 
-
 class ListProtocolsListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listprotocolslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtocolsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listprotocolslistspaginator)
         """
 
-
 class ListThirdPartyFirewallFirewallPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/paginator.pyi` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,129 +59,139 @@
     "ListComplianceStatusPaginator",
     "ListMemberAccountsPaginator",
     "ListPoliciesPaginator",
     "ListProtocolsListsPaginator",
     "ListThirdPartyFirewallFirewallPoliciesPaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListAdminAccountsForOrganizationPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminaccountsfororganizationpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAdminAccountsForOrganizationResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminAccountsForOrganization.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminaccountsfororganizationpaginator)
         """
 
+
 class ListAdminsManagingAccountPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminsmanagingaccountpaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAdminsManagingAccountResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAdminsManagingAccount.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listadminsmanagingaccountpaginator)
         """
 
+
 class ListAppsListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listappslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAppsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListAppsLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listappslistspaginator)
         """
 
+
 class ListComplianceStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listcompliancestatuspaginator)
     """
 
     def paginate(
-        self, *, PolicyId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PolicyId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListComplianceStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListComplianceStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listcompliancestatuspaginator)
         """
 
+
 class ListMemberAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMemberAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListMemberAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listmemberaccountspaginator)
         """
 
+
 class ListPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listpoliciespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listpoliciespaginator)
         """
 
+
 class ListProtocolsListsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listprotocolslistspaginator)
     """
 
     def paginate(
-        self, *, DefaultLists: bool = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DefaultLists: bool = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListProtocolsListsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListProtocolsLists.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listprotocolslistspaginator)
         """
 
+
 class ListThirdPartyFirewallFirewallPoliciesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
     """
 
     def paginate(
         self,
         *,
         ThirdPartyFirewall: ThirdPartyFirewallType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListThirdPartyFirewallFirewallPoliciesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS.Paginator.ListThirdPartyFirewallFirewallPolicies.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/paginators/#listthirdpartyfirewallfirewallpoliciespaginator)
         """
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/type_defs.py` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_fms.type_defs import AccountScopeTypeDef
+    from types_aiobotocore_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeTypeDef = {...}
+    data: AccountScopeOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
@@ -41,178 +41,202 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeOutputTypeDef",
+    "PolicyTypeScopeOutputTypeDef",
+    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
+    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
-    "AssociateThirdPartyFirewallResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
     "BatchDisassociateResourceRequestRequestTypeDef",
     "ComplianceViolatorTypeDef",
     "DeleteAppsListRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "DeleteProtocolsListRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
-    "DisassociateThirdPartyFirewallResponseTypeDef",
     "DiscoveredResourceTypeDef",
     "DnsDuplicateRuleGroupViolationTypeDef",
     "DnsRuleGroupLimitExceededViolationTypeDef",
     "DnsRuleGroupPriorityConflictViolationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluationResultTypeDef",
     "ExpectedRouteTypeDef",
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
-    "GetAdminAccountResponseTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
-    "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
-    "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
+    "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetTypeDef",
+    "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
-    "ListAdminsManagingAccountResponseTypeDef",
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     "ListAppsListsRequestRequestTypeDef",
-    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
-    "ListMemberAccountsResponseTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "PolicySummaryTypeDef",
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
-    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
-    "PaginatorConfigTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
     "ResourceTagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
-    "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
-    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
+    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
+    "ProtocolsListDataTypeDef",
+    "ResourceSetTypeDef",
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdminAccountResponseTypeDef",
+    "GetNotificationChannelResponseTypeDef",
+    "GetProtectionStatusResponseTypeDef",
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "ListAdminsManagingAccountResponseTypeDef",
+    "ListMemberAccountsResponseTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
+    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
-    "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
+    "ListAppsListsResponseTypeDef",
+    "AppsListDataUnionTypeDef",
+    "PutAppsListRequestRequestTypeDef",
+    "ProtocolsListDataUnionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
+    "ResourceSetUnionTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
+    "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "PolicyUnionTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeOutputTypeDef = TypedDict(
+    "AccountScopeOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AllAccountsEnabled": bool,
+        "ExcludeSpecifiedAccounts": bool,
+    },
+    total=False,
+)
+
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": List[str],
+        "Accounts": Sequence[str],
         "AllAccountsEnabled": bool,
         "ExcludeSpecifiedAccounts": bool,
     },
     total=False,
 )
 
 ActionTargetTypeDef = TypedDict(
@@ -230,70 +254,102 @@
         "AdminAccount": str,
         "DefaultAdmin": bool,
         "Status": OrganizationStatusType,
     },
     total=False,
 )
 
+OrganizationalUnitScopeOutputTypeDef = TypedDict(
+    "OrganizationalUnitScopeOutputTypeDef",
+    {
+        "OrganizationalUnits": List[str],
+        "AllOrganizationalUnitsEnabled": bool,
+        "ExcludeSpecifiedOrganizationalUnits": bool,
+    },
+    total=False,
+)
+
+PolicyTypeScopeOutputTypeDef = TypedDict(
+    "PolicyTypeScopeOutputTypeDef",
+    {
+        "PolicyTypes": List[SecurityServiceTypeType],
+        "AllPolicyTypesEnabled": bool,
+    },
+    total=False,
+)
+
+RegionScopeOutputTypeDef = TypedDict(
+    "RegionScopeOutputTypeDef",
+    {
+        "Regions": List[str],
+        "AllRegionsEnabled": bool,
+    },
+    total=False,
+)
+
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": List[str],
+        "OrganizationalUnits": Sequence[str],
         "AllOrganizationalUnitsEnabled": bool,
         "ExcludeSpecifiedOrganizationalUnits": bool,
     },
     total=False,
 )
 
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": List[SecurityServiceTypeType],
+        "PolicyTypes": Sequence[SecurityServiceTypeType],
         "AllPolicyTypesEnabled": bool,
     },
     total=False,
 )
 
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": List[str],
+        "Regions": Sequence[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "AssociateThirdPartyFirewallResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -364,21 +420,19 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
-
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
-
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -392,22 +446,14 @@
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
         "AccountId": str,
         "Type": str,
         "Name": str,
@@ -442,21 +488,14 @@
         "ConflictingPriority": int,
         "ConflictingPolicyId": str,
         "UnavailablePriorities": List[int],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "ComplianceStatus": PolicyComplianceStatusTypeType,
         "ViolatorCount": int,
         "EvaluationLimitExceeded": bool,
     },
@@ -504,23 +543,14 @@
         "VpcId": str,
         "SubnetAvailabilityZone": str,
         "SubnetAvailabilityZoneId": str,
     },
     total=False,
 )
 
-GetAdminAccountResponseTypeDef = TypedDict(
-    "GetAdminAccountResponseTypeDef",
-    {
-        "AdminAccount": str,
-        "RoleStatus": AccountRoleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAdminScopeRequestRequestTypeDef = TypedDict(
     "GetAdminScopeRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -534,238 +564,153 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
-
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
 
-GetNotificationChannelResponseTypeDef = TypedDict(
-    "GetNotificationChannelResponseTypeDef",
-    {
-        "SnsTopicArn": str,
-        "SnsRoleName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
-_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProtectionStatusRequestRequestTypeDef",
-    {
-        "MemberAccountId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class GetProtectionStatusRequestRequestTypeDef(
-    _RequiredGetProtectionStatusRequestRequestTypeDef,
-    _OptionalGetProtectionStatusRequestRequestTypeDef,
-):
-    pass
-
-
-GetProtectionStatusResponseTypeDef = TypedDict(
-    "GetProtectionStatusResponseTypeDef",
-    {
-        "AdminAccountId": str,
-        "ServiceType": SecurityServiceTypeType,
-        "Data": str,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
-
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
+_RequiredProtocolsListDataOutputTypeDef = TypedDict(
+    "_RequiredProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
+_OptionalProtocolsListDataOutputTypeDef = TypedDict(
+    "_OptionalProtocolsListDataOutputTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+class ProtocolsListDataOutputTypeDef(
+    _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
 ):
     pass
 
-
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
+_RequiredResourceSetOutputTypeDef = TypedDict(
+    "_RequiredResourceSetOutputTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
     },
 )
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
+_OptionalResourceSetOutputTypeDef = TypedDict(
+    "_OptionalResourceSetOutputTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+class ResourceSetOutputTypeDef(
+    _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
+):
     pass
 
-
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
         "ResourceId": str,
         "ResourceType": str,
     },
 )
 
-ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
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
 
 ListAdminAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAdminsManagingAccountRequestRequestTypeDef = TypedDict(
     "ListAdminsManagingAccountRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountResponseTypeDef = TypedDict(
-    "ListAdminsManagingAccountResponseTypeDef",
-    {
-        "AdminAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListAppsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListAppsListsRequestRequestTypeDef = TypedDict(
@@ -773,43 +718,19 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
-    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 _OptionalListComplianceStatusRequestRequestTypeDef = TypedDict(
@@ -817,22 +738,20 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -841,56 +760,29 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListMemberAccountsResponseTypeDef = TypedDict(
-    "ListMemberAccountsResponseTypeDef",
-    {
-        "MemberAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -907,23 +799,14 @@
         "RemediationEnabled": bool,
         "DeleteUnusedFMManagedResources": bool,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListProtocolsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListProtocolsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListProtocolsListsRequestRequestTypeDef = TypedDict(
@@ -931,22 +814,20 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
-
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -965,41 +846,37 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
-
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
-
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1028,36 +905,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
-    },
-)
-_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
-    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
@@ -1065,22 +920,20 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
-
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -1161,24 +1014,14 @@
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
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
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -1193,19 +1036,17 @@
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
-
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
@@ -1240,25 +1081,14 @@
         "VPC": str,
         "AvailabilityZone": str,
         "TargetViolationReason": str,
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
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "IPV4Range": str,
         "IPV6Range": str,
         "PrefixListId": str,
         "Protocol": str,
@@ -1288,21 +1118,19 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1310,21 +1138,19 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1336,42 +1162,38 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
-
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1381,21 +1203,19 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
-
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1406,21 +1226,19 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
-
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1428,42 +1246,66 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-
-ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationResponseTypeDef",
+AdminScopeOutputTypeDef = TypedDict(
+    "AdminScopeOutputTypeDef",
     {
-        "AdminAccounts": List[AdminAccountSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountScope": AccountScopeOutputTypeDef,
+        "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
+        "RegionScope": RegionScopeOutputTypeDef,
+        "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
     },
+    total=False,
 )
 
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": AccountScopeTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
         "RegionScope": RegionScopeTypeDef,
         "PolicyTypeScope": PolicyTypeScopeTypeDef,
     },
     total=False,
 )
 
+_RequiredAppsListDataOutputTypeDef = TypedDict(
+    "_RequiredAppsListDataOutputTypeDef",
+    {
+        "ListName": str,
+        "AppsList": List[AppTypeDef],
+    },
+)
+_OptionalAppsListDataOutputTypeDef = TypedDict(
+    "_OptionalAppsListDataOutputTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": datetime,
+        "LastUpdateTime": datetime,
+        "PreviousAppsList": Dict[str, List[AppTypeDef]],
+    },
+    total=False,
+)
+
+class AppsListDataOutputTypeDef(
+    _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
+):
+    pass
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1471,33 +1313,189 @@
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": Sequence[AppTypeDef],
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": datetime,
-        "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppTypeDef]],
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
+        "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
-
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProtectionStatusRequestRequestTypeDef",
+    {
+        "MemberAccountId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+class GetProtectionStatusRequestRequestTypeDef(
+    _RequiredGetProtectionStatusRequestRequestTypeDef,
+    _OptionalGetProtectionStatusRequestRequestTypeDef,
+):
+    pass
+
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+    },
+)
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
+        "PreviousProtocolsList": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+):
+    pass
+
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+    },
+)
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "UpdateToken": str,
+        "LastUpdateTime": TimestampTypeDef,
+        "ResourceSetStatus": ResourceSetStatusType,
+    },
+    total=False,
+)
+
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+    pass
+
+AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
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
+GetAdminAccountResponseTypeDef = TypedDict(
+    "GetAdminAccountResponseTypeDef",
+    {
+        "AdminAccount": str,
+        "RoleStatus": AccountRoleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNotificationChannelResponseTypeDef = TypedDict(
+    "GetNotificationChannelResponseTypeDef",
+    {
+        "SnsTopicArn": str,
+        "SnsRoleName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProtectionStatusResponseTypeDef = TypedDict(
+    "GetProtectionStatusResponseTypeDef",
+    {
+        "AdminAccountId": str,
+        "ServiceType": SecurityServiceTypeType,
+        "Data": str,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminsManagingAccountResponseTypeDef = TypedDict(
+    "ListAdminsManagingAccountResponseTypeDef",
+    {
+        "AdminAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMemberAccountsResponseTypeDef = TypedDict(
+    "ListMemberAccountsResponseTypeDef",
+    {
+        "MemberAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
@@ -1505,24 +1503,24 @@
 )
 
 BatchAssociateResourceResponseTypeDef = TypedDict(
     "BatchAssociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateResourceResponseTypeDef = TypedDict(
     "BatchDisassociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceDetailTypeDef = TypedDict(
     "PolicyComplianceDetailTypeDef",
     {
         "PolicyOwner": str,
@@ -1537,15 +1535,15 @@
 )
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": str,
@@ -1568,147 +1566,195 @@
     },
     total=False,
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListPoliciesResponseTypeDef = TypedDict(
-    "ListPoliciesResponseTypeDef",
+ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     {
-        "PolicyList": List[PolicySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListProtocolsListsResponseTypeDef = TypedDict(
-    "ListProtocolsListsResponseTypeDef",
+ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     {
-        "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListResourceSetResourcesResponseTypeDef = TypedDict(
-    "ListResourceSetResourcesResponseTypeDef",
+ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     {
-        "Items": List[ResourceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListResourceSetsResponseTypeDef = TypedDict(
-    "ListResourceSetsResponseTypeDef",
+_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
-        "ResourceSets": List[ResourceSetSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PolicyId": str,
     },
 )
+_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
+    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+):
+    pass
+
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
+
+ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     {
-        "TagList": Sequence[TagTypeDef],
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
+    },
+)
+_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
+    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
 ):
     pass
 
-
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
+ListPoliciesResponseTypeDef = TypedDict(
+    "ListPoliciesResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "PolicyList": List[PolicySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
+
+ListProtocolsListsResponseTypeDef = TypedDict(
+    "ListProtocolsListsResponseTypeDef",
     {
-        "TagList": Sequence[TagTypeDef],
+        "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListResourceSetResourcesResponseTypeDef = TypedDict(
+    "ListResourceSetResourcesResponseTypeDef",
+    {
+        "Items": List[ResourceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
-):
-    pass
+ListResourceSetsResponseTypeDef = TypedDict(
+    "ListResourceSetsResponseTypeDef",
+    {
+        "ResourceSets": List[ResourceSetSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -1854,103 +1900,141 @@
     },
     total=False,
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeTypeDef,
+        "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 _OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_OptionalPutAdminAccountRequestRequestTypeDef",
     {
         "AdminScope": AdminScopeTypeDef,
     },
     total=False,
 )
 
-
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
-
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppsList": AppsListDataOutputTypeDef,
+        "AppsListArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
+        "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
+    {
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
+ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
+    {
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
 
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
-        "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
+ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": List[StatelessRuleGroupTypeDef],
@@ -1975,21 +2059,19 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
-
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
-
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -2012,26 +2094,26 @@
         "ViolationTarget": str,
         "CurrentPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
         "ExpectedPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPolicyTypeDef = TypedDict(
-    "_RequiredPolicyTypeDef",
+_RequiredPolicyOutputTypeDef = TypedDict(
+    "_RequiredPolicyOutputTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
-_OptionalPolicyTypeDef = TypedDict(
-    "_OptionalPolicyTypeDef",
+_OptionalPolicyOutputTypeDef = TypedDict(
+    "_OptionalPolicyOutputTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
         "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
@@ -2039,19 +2121,47 @@
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
+class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
+    pass
+
+_RequiredPolicyTypeDef = TypedDict(
+    "_RequiredPolicyTypeDef",
+    {
+        "PolicyName": str,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "ResourceType": str,
+        "ExcludeResourceTags": bool,
+        "RemediationEnabled": bool,
+    },
+)
+_OptionalPolicyTypeDef = TypedDict(
+    "_OptionalPolicyTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyUpdateToken": str,
+        "ResourceTypeList": Sequence[str],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "DeleteUnusedFMManagedResources": bool,
+        "IncludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ExcludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ResourceSetIds": Sequence[str],
+        "PolicyDescription": str,
+        "PolicyStatus": CustomerPolicyStatusType,
+    },
+    total=False,
+)
 
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
-
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -2059,60 +2169,57 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
-
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
-
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
+        "PolicyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
+    {
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 _OptionalPutPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
-    {
-        "Policy": PolicyTypeDef,
-        "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
     total=False,
@@ -2183,19 +2290,17 @@
     {
         "ResourceTags": List[TagTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
-
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
-
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms/type_defs.pyi` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for fms service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_fms.type_defs import AccountScopeTypeDef
+    from types_aiobotocore_fms.type_defs import AccountScopeOutputTypeDef
 
-    data: AccountScopeTypeDef = {...}
+    data: AccountScopeOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence, Union
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AccountRoleStatusType,
     CustomerPolicyScopeIdTypeType,
     CustomerPolicyStatusType,
     DependentServiceNameType,
     DestinationTypeType,
@@ -41,177 +41,203 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "AccountScopeOutputTypeDef",
     "AccountScopeTypeDef",
     "ActionTargetTypeDef",
     "AdminAccountSummaryTypeDef",
+    "OrganizationalUnitScopeOutputTypeDef",
+    "PolicyTypeScopeOutputTypeDef",
+    "RegionScopeOutputTypeDef",
     "OrganizationalUnitScopeTypeDef",
     "PolicyTypeScopeTypeDef",
     "RegionScopeTypeDef",
     "AppTypeDef",
+    "TimestampTypeDef",
     "AssociateAdminAccountRequestRequestTypeDef",
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
-    "AssociateThirdPartyFirewallResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "AwsEc2NetworkInterfaceViolationTypeDef",
     "PartialMatchTypeDef",
     "BatchAssociateResourceRequestRequestTypeDef",
     "FailedItemTypeDef",
     "BatchDisassociateResourceRequestRequestTypeDef",
     "ComplianceViolatorTypeDef",
     "DeleteAppsListRequestRequestTypeDef",
     "DeletePolicyRequestRequestTypeDef",
     "DeleteProtocolsListRequestRequestTypeDef",
     "DeleteResourceSetRequestRequestTypeDef",
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
-    "DisassociateThirdPartyFirewallResponseTypeDef",
     "DiscoveredResourceTypeDef",
     "DnsDuplicateRuleGroupViolationTypeDef",
     "DnsRuleGroupLimitExceededViolationTypeDef",
     "DnsRuleGroupPriorityConflictViolationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "EvaluationResultTypeDef",
     "ExpectedRouteTypeDef",
     "FMSPolicyUpdateFirewallCreationConfigActionTypeDef",
     "FirewallSubnetIsOutOfScopeViolationTypeDef",
     "FirewallSubnetMissingVPCEndpointViolationTypeDef",
-    "GetAdminAccountResponseTypeDef",
     "GetAdminScopeRequestRequestTypeDef",
     "GetAppsListRequestRequestTypeDef",
     "GetComplianceDetailRequestRequestTypeDef",
-    "GetNotificationChannelResponseTypeDef",
     "GetPolicyRequestRequestTypeDef",
-    "GetProtectionStatusRequestRequestTypeDef",
-    "GetProtectionStatusResponseTypeDef",
     "GetProtocolsListRequestRequestTypeDef",
-    "ProtocolsListDataTypeDef",
+    "ProtocolsListDataOutputTypeDef",
     "GetResourceSetRequestRequestTypeDef",
-    "ResourceSetTypeDef",
+    "ResourceSetOutputTypeDef",
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
     "GetViolationDetailsRequestRequestTypeDef",
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     "ListAdminsManagingAccountRequestRequestTypeDef",
-    "ListAdminsManagingAccountResponseTypeDef",
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     "ListAppsListsRequestRequestTypeDef",
-    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     "ListComplianceStatusRequestRequestTypeDef",
     "ListDiscoveredResourcesRequestRequestTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
-    "ListMemberAccountsResponseTypeDef",
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     "ListPoliciesRequestRequestTypeDef",
     "PolicySummaryTypeDef",
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
     "ListProtocolsListsRequestRequestTypeDef",
     "ProtocolsListDataSummaryTypeDef",
     "ListResourceSetResourcesRequestRequestTypeDef",
     "ResourceTypeDef",
     "ListResourceSetsRequestRequestTypeDef",
     "ResourceSetSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
-    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     "RouteTypeDef",
     "NetworkFirewallMissingExpectedRTViolationTypeDef",
     "NetworkFirewallMissingFirewallViolationTypeDef",
     "NetworkFirewallMissingSubnetViolationTypeDef",
     "StatefulEngineOptionsTypeDef",
     "StatelessRuleGroupTypeDef",
     "NetworkFirewallPolicyTypeDef",
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
-    "PaginatorConfigTypeDef",
     "ThirdPartyFirewallPolicyTypeDef",
     "ResourceTagTypeDef",
     "PutNotificationChannelRequestRequestTypeDef",
     "ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef",
     "ThirdPartyFirewallMissingFirewallViolationTypeDef",
     "ThirdPartyFirewallMissingSubnetViolationTypeDef",
-    "ResponseMetadataTypeDef",
     "SecurityGroupRuleDescriptionTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "EC2AssociateRouteTableActionTypeDef",
     "EC2CopyRouteTableActionTypeDef",
     "EC2CreateRouteActionTypeDef",
     "EC2CreateRouteTableActionTypeDef",
     "EC2DeleteRouteActionTypeDef",
     "EC2ReplaceRouteActionTypeDef",
     "EC2ReplaceRouteTableAssociationActionTypeDef",
-    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "AdminScopeOutputTypeDef",
     "AdminScopeTypeDef",
+    "AppsListDataOutputTypeDef",
     "AppsListDataSummaryTypeDef",
     "AppsListDataTypeDef",
+    "GetProtectionStatusRequestRequestTypeDef",
+    "ProtocolsListDataTypeDef",
+    "ResourceSetTypeDef",
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAdminAccountResponseTypeDef",
+    "GetNotificationChannelResponseTypeDef",
+    "GetProtectionStatusResponseTypeDef",
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    "ListAdminsManagingAccountResponseTypeDef",
+    "ListMemberAccountsResponseTypeDef",
     "AwsEc2InstanceViolationTypeDef",
     "BatchAssociateResourceResponseTypeDef",
     "BatchDisassociateResourceResponseTypeDef",
     "PolicyComplianceDetailTypeDef",
     "ListDiscoveredResourcesResponseTypeDef",
     "PolicyComplianceStatusTypeDef",
     "NetworkFirewallMissingExpectedRoutesViolationTypeDef",
     "GetProtocolsListResponseTypeDef",
     "PutProtocolsListResponseTypeDef",
     "GetResourceSetResponseTypeDef",
     "PutResourceSetResponseTypeDef",
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
+    "ListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    "ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     "ListPoliciesResponseTypeDef",
     "ListProtocolsListsResponseTypeDef",
     "ListResourceSetResourcesResponseTypeDef",
     "ListResourceSetsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "PutProtocolsListRequestRequestTypeDef",
-    "PutResourceSetRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     "NetworkFirewallInternetTrafficNotInspectedViolationTypeDef",
     "NetworkFirewallInvalidRouteConfigurationViolationTypeDef",
     "NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef",
     "NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef",
     "RouteHasOutOfScopeEndpointViolationTypeDef",
     "StatefulRuleGroupTypeDef",
     "PolicyOptionTypeDef",
     "SecurityGroupRemediationActionTypeDef",
     "RemediationActionTypeDef",
     "GetAdminScopeResponseTypeDef",
+    "AdminScopeUnionTypeDef",
     "PutAdminAccountRequestRequestTypeDef",
-    "ListAppsListsResponseTypeDef",
     "GetAppsListResponseTypeDef",
-    "PutAppsListRequestRequestTypeDef",
     "PutAppsListResponseTypeDef",
+    "ListAppsListsResponseTypeDef",
+    "AppsListDataUnionTypeDef",
+    "PutAppsListRequestRequestTypeDef",
+    "ProtocolsListDataUnionTypeDef",
+    "PutProtocolsListRequestRequestTypeDef",
+    "PutResourceSetRequestRequestTypeDef",
+    "ResourceSetUnionTypeDef",
     "GetComplianceDetailResponseTypeDef",
     "ListComplianceStatusResponseTypeDef",
     "NetworkFirewallPolicyDescriptionTypeDef",
     "SecurityServicePolicyDataTypeDef",
     "AwsVPCSecurityGroupViolationTypeDef",
     "RemediationActionWithOrderTypeDef",
     "NetworkFirewallPolicyModifiedViolationTypeDef",
+    "PolicyOutputTypeDef",
     "PolicyTypeDef",
     "PossibleRemediationActionTypeDef",
     "GetPolicyResponseTypeDef",
-    "PutPolicyRequestRequestTypeDef",
     "PutPolicyResponseTypeDef",
+    "PolicyUnionTypeDef",
+    "PutPolicyRequestRequestTypeDef",
     "PossibleRemediationActionsTypeDef",
     "ResourceViolationTypeDef",
     "ViolationDetailTypeDef",
     "GetViolationDetailsResponseTypeDef",
 )
 
+AccountScopeOutputTypeDef = TypedDict(
+    "AccountScopeOutputTypeDef",
+    {
+        "Accounts": List[str],
+        "AllAccountsEnabled": bool,
+        "ExcludeSpecifiedAccounts": bool,
+    },
+    total=False,
+)
+
 AccountScopeTypeDef = TypedDict(
     "AccountScopeTypeDef",
     {
-        "Accounts": List[str],
+        "Accounts": Sequence[str],
         "AllAccountsEnabled": bool,
         "ExcludeSpecifiedAccounts": bool,
     },
     total=False,
 )
 
 ActionTargetTypeDef = TypedDict(
@@ -229,70 +255,102 @@
         "AdminAccount": str,
         "DefaultAdmin": bool,
         "Status": OrganizationStatusType,
     },
     total=False,
 )
 
+OrganizationalUnitScopeOutputTypeDef = TypedDict(
+    "OrganizationalUnitScopeOutputTypeDef",
+    {
+        "OrganizationalUnits": List[str],
+        "AllOrganizationalUnitsEnabled": bool,
+        "ExcludeSpecifiedOrganizationalUnits": bool,
+    },
+    total=False,
+)
+
+PolicyTypeScopeOutputTypeDef = TypedDict(
+    "PolicyTypeScopeOutputTypeDef",
+    {
+        "PolicyTypes": List[SecurityServiceTypeType],
+        "AllPolicyTypesEnabled": bool,
+    },
+    total=False,
+)
+
+RegionScopeOutputTypeDef = TypedDict(
+    "RegionScopeOutputTypeDef",
+    {
+        "Regions": List[str],
+        "AllRegionsEnabled": bool,
+    },
+    total=False,
+)
+
 OrganizationalUnitScopeTypeDef = TypedDict(
     "OrganizationalUnitScopeTypeDef",
     {
-        "OrganizationalUnits": List[str],
+        "OrganizationalUnits": Sequence[str],
         "AllOrganizationalUnitsEnabled": bool,
         "ExcludeSpecifiedOrganizationalUnits": bool,
     },
     total=False,
 )
 
 PolicyTypeScopeTypeDef = TypedDict(
     "PolicyTypeScopeTypeDef",
     {
-        "PolicyTypes": List[SecurityServiceTypeType],
+        "PolicyTypes": Sequence[SecurityServiceTypeType],
         "AllPolicyTypesEnabled": bool,
     },
     total=False,
 )
 
 RegionScopeTypeDef = TypedDict(
     "RegionScopeTypeDef",
     {
-        "Regions": List[str],
+        "Regions": Sequence[str],
         "AllRegionsEnabled": bool,
     },
     total=False,
 )
 
 AppTypeDef = TypedDict(
     "AppTypeDef",
     {
         "AppName": str,
         "Protocol": str,
         "Port": int,
     },
 )
 
+TimestampTypeDef = Union[datetime, str]
 AssociateAdminAccountRequestRequestTypeDef = TypedDict(
     "AssociateAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
 AssociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "AssociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "AssociateThirdPartyFirewallResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 AwsEc2NetworkInterfaceViolationTypeDef = TypedDict(
     "AwsEc2NetworkInterfaceViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -363,19 +421,21 @@
     "_OptionalDeletePolicyRequestRequestTypeDef",
     {
         "DeleteAllPolicyResources": bool,
     },
     total=False,
 )
 
+
 class DeletePolicyRequestRequestTypeDef(
     _RequiredDeletePolicyRequestRequestTypeDef, _OptionalDeletePolicyRequestRequestTypeDef
 ):
     pass
 
+
 DeleteProtocolsListRequestRequestTypeDef = TypedDict(
     "DeleteProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 
@@ -389,22 +449,14 @@
 DisassociateThirdPartyFirewallRequestRequestTypeDef = TypedDict(
     "DisassociateThirdPartyFirewallRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
-    "DisassociateThirdPartyFirewallResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscoveredResourceTypeDef = TypedDict(
     "DiscoveredResourceTypeDef",
     {
         "URI": str,
         "AccountId": str,
         "Type": str,
         "Name": str,
@@ -439,21 +491,14 @@
         "ConflictingPriority": int,
         "ConflictingPolicyId": str,
         "UnavailablePriorities": List[int],
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EvaluationResultTypeDef = TypedDict(
     "EvaluationResultTypeDef",
     {
         "ComplianceStatus": PolicyComplianceStatusTypeType,
         "ViolatorCount": int,
         "EvaluationLimitExceeded": bool,
     },
@@ -501,23 +546,14 @@
         "VpcId": str,
         "SubnetAvailabilityZone": str,
         "SubnetAvailabilityZoneId": str,
     },
     total=False,
 )
 
-GetAdminAccountResponseTypeDef = TypedDict(
-    "GetAdminAccountResponseTypeDef",
-    {
-        "AdminAccount": str,
-        "RoleStatus": AccountRoleStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAdminScopeRequestRequestTypeDef = TypedDict(
     "GetAdminScopeRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 
@@ -531,228 +567,161 @@
     "_OptionalGetAppsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetAppsListRequestRequestTypeDef(
     _RequiredGetAppsListRequestRequestTypeDef, _OptionalGetAppsListRequestRequestTypeDef
 ):
     pass
 
+
 GetComplianceDetailRequestRequestTypeDef = TypedDict(
     "GetComplianceDetailRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
     },
 )
 
-GetNotificationChannelResponseTypeDef = TypedDict(
-    "GetNotificationChannelResponseTypeDef",
-    {
-        "SnsTopicArn": str,
-        "SnsRoleName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetPolicyRequestRequestTypeDef = TypedDict(
     "GetPolicyRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
 
-_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_RequiredGetProtectionStatusRequestRequestTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
-    "_OptionalGetProtectionStatusRequestRequestTypeDef",
-    {
-        "MemberAccountId": str,
-        "StartTime": Union[datetime, str],
-        "EndTime": Union[datetime, str],
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class GetProtectionStatusRequestRequestTypeDef(
-    _RequiredGetProtectionStatusRequestRequestTypeDef,
-    _OptionalGetProtectionStatusRequestRequestTypeDef,
-):
-    pass
-
-GetProtectionStatusResponseTypeDef = TypedDict(
-    "GetProtectionStatusResponseTypeDef",
-    {
-        "AdminAccountId": str,
-        "ServiceType": SecurityServiceTypeType,
-        "Data": str,
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_RequiredGetProtocolsListRequestRequestTypeDef",
     {
         "ListId": str,
     },
 )
 _OptionalGetProtocolsListRequestRequestTypeDef = TypedDict(
     "_OptionalGetProtocolsListRequestRequestTypeDef",
     {
         "DefaultList": bool,
     },
     total=False,
 )
 
+
 class GetProtocolsListRequestRequestTypeDef(
     _RequiredGetProtocolsListRequestRequestTypeDef, _OptionalGetProtocolsListRequestRequestTypeDef
 ):
     pass
 
-_RequiredProtocolsListDataTypeDef = TypedDict(
-    "_RequiredProtocolsListDataTypeDef",
+
+_RequiredProtocolsListDataOutputTypeDef = TypedDict(
+    "_RequiredProtocolsListDataOutputTypeDef",
     {
         "ListName": str,
         "ProtocolsList": List[str],
     },
 )
-_OptionalProtocolsListDataTypeDef = TypedDict(
-    "_OptionalProtocolsListDataTypeDef",
+_OptionalProtocolsListDataOutputTypeDef = TypedDict(
+    "_OptionalProtocolsListDataOutputTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
         "CreateTime": datetime,
         "LastUpdateTime": datetime,
         "PreviousProtocolsList": Dict[str, List[str]],
     },
     total=False,
 )
 
-class ProtocolsListDataTypeDef(
-    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+
+class ProtocolsListDataOutputTypeDef(
+    _RequiredProtocolsListDataOutputTypeDef, _OptionalProtocolsListDataOutputTypeDef
 ):
     pass
 
+
 GetResourceSetRequestRequestTypeDef = TypedDict(
     "GetResourceSetRequestRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-_RequiredResourceSetTypeDef = TypedDict(
-    "_RequiredResourceSetTypeDef",
+_RequiredResourceSetOutputTypeDef = TypedDict(
+    "_RequiredResourceSetOutputTypeDef",
     {
         "Name": str,
         "ResourceTypeList": List[str],
     },
 )
-_OptionalResourceSetTypeDef = TypedDict(
-    "_OptionalResourceSetTypeDef",
+_OptionalResourceSetOutputTypeDef = TypedDict(
+    "_OptionalResourceSetOutputTypeDef",
     {
         "Id": str,
         "Description": str,
         "UpdateToken": str,
         "LastUpdateTime": datetime,
         "ResourceSetStatus": ResourceSetStatusType,
     },
     total=False,
 )
 
-class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+
+class ResourceSetOutputTypeDef(
+    _RequiredResourceSetOutputTypeDef, _OptionalResourceSetOutputTypeDef
+):
     pass
 
+
 GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef = TypedDict(
     "GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
 
-GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
-    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
-    {
-        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
-        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetViolationDetailsRequestRequestTypeDef = TypedDict(
     "GetViolationDetailsRequestRequestTypeDef",
     {
         "PolicyId": str,
         "MemberAccount": str,
         "ResourceId": str,
         "ResourceType": str,
     },
 )
 
-ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
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
 
 ListAdminAccountsForOrganizationRequestRequestTypeDef = TypedDict(
     "ListAdminAccountsForOrganizationRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
-    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAdminsManagingAccountRequestRequestTypeDef = TypedDict(
     "ListAdminsManagingAccountRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListAdminsManagingAccountResponseTypeDef = TypedDict(
-    "ListAdminsManagingAccountResponseTypeDef",
-    {
-        "AdminAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
-    "ListAppsListsRequestListAppsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListAppsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListAppsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListAppsListsRequestRequestTypeDef = TypedDict(
@@ -760,38 +729,20 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListAppsListsRequestRequestTypeDef(
     _RequiredListAppsListsRequestRequestTypeDef, _OptionalListAppsListsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PolicyId": str,
-    },
-)
-_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
-    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
-    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
-):
-    pass
 
 _RequiredListComplianceStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListComplianceStatusRequestRequestTypeDef",
     {
         "PolicyId": str,
     },
 )
@@ -800,20 +751,22 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListComplianceStatusRequestRequestTypeDef(
     _RequiredListComplianceStatusRequestRequestTypeDef,
     _OptionalListComplianceStatusRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredListDiscoveredResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDiscoveredResourcesRequestRequestTypeDef",
     {
         "MemberAccountIds": Sequence[str],
         "ResourceType": str,
     },
 )
@@ -822,54 +775,31 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListDiscoveredResourcesRequestRequestTypeDef(
     _RequiredListDiscoveredResourcesRequestRequestTypeDef,
     _OptionalListDiscoveredResourcesRequestRequestTypeDef,
 ):
     pass
 
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListMemberAccountsResponseTypeDef = TypedDict(
-    "ListMemberAccountsResponseTypeDef",
-    {
-        "MemberAccounts": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
-    "ListPoliciesRequestListPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPoliciesRequestRequestTypeDef = TypedDict(
     "ListPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -886,23 +816,14 @@
         "RemediationEnabled": bool,
         "DeleteUnusedFMManagedResources": bool,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
-ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
-    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
-    {
-        "DefaultLists": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListProtocolsListsRequestRequestTypeDef = TypedDict(
     "_RequiredListProtocolsListsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListProtocolsListsRequestRequestTypeDef = TypedDict(
@@ -910,20 +831,22 @@
     {
         "DefaultLists": bool,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListProtocolsListsRequestRequestTypeDef(
     _RequiredListProtocolsListsRequestRequestTypeDef,
     _OptionalListProtocolsListsRequestRequestTypeDef,
 ):
     pass
 
+
 ProtocolsListDataSummaryTypeDef = TypedDict(
     "ProtocolsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "ProtocolsList": List[str],
@@ -942,37 +865,41 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListResourceSetResourcesRequestRequestTypeDef(
     _RequiredListResourceSetResourcesRequestRequestTypeDef,
     _OptionalListResourceSetResourcesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredResourceTypeDef = TypedDict(
     "_RequiredResourceTypeDef",
     {
         "URI": str,
     },
 )
 _OptionalResourceTypeDef = TypedDict(
     "_OptionalResourceTypeDef",
     {
         "AccountId": str,
     },
     total=False,
 )
 
+
 class ResourceTypeDef(_RequiredResourceTypeDef, _OptionalResourceTypeDef):
     pass
 
+
 ListResourceSetsRequestRequestTypeDef = TypedDict(
     "ListResourceSetsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
@@ -1001,34 +928,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "ThirdPartyFirewall": ThirdPartyFirewallType,
-    },
-)
-_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
-    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
-    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
-):
-    pass
-
 _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef = TypedDict(
     "_RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "ThirdPartyFirewall": ThirdPartyFirewallType,
         "MaxResults": int,
     },
 )
@@ -1036,20 +943,22 @@
     "_OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef(
     _RequiredListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     _OptionalListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
 ):
     pass
 
+
 ThirdPartyFirewallFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallFirewallPolicyTypeDef",
     {
         "FirewallPolicyId": str,
         "FirewallPolicyName": str,
     },
     total=False,
@@ -1130,24 +1039,14 @@
     "NetworkFirewallStatefulRuleGroupOverrideTypeDef",
     {
         "Action": Literal["DROP_TO_ALERT"],
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
 ThirdPartyFirewallPolicyTypeDef = TypedDict(
     "ThirdPartyFirewallPolicyTypeDef",
     {
         "FirewallDeploymentModel": FirewallDeploymentModelType,
     },
     total=False,
 )
@@ -1162,17 +1061,19 @@
     "_OptionalResourceTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class ResourceTagTypeDef(_RequiredResourceTagTypeDef, _OptionalResourceTagTypeDef):
     pass
 
+
 PutNotificationChannelRequestRequestTypeDef = TypedDict(
     "PutNotificationChannelRequestRequestTypeDef",
     {
         "SnsTopicArn": str,
         "SnsRoleName": str,
     },
 )
@@ -1207,25 +1108,14 @@
         "VPC": str,
         "AvailabilityZone": str,
         "TargetViolationReason": str,
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
 SecurityGroupRuleDescriptionTypeDef = TypedDict(
     "SecurityGroupRuleDescriptionTypeDef",
     {
         "IPV4Range": str,
         "IPV6Range": str,
         "PrefixListId": str,
         "Protocol": str,
@@ -1255,19 +1145,21 @@
         "Description": str,
         "SubnetId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2AssociateRouteTableActionTypeDef(
     _RequiredEC2AssociateRouteTableActionTypeDef, _OptionalEC2AssociateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CopyRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CopyRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1275,19 +1167,21 @@
     "_OptionalEC2CopyRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CopyRouteTableActionTypeDef(
     _RequiredEC2CopyRouteTableActionTypeDef, _OptionalEC2CopyRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteActionTypeDef = TypedDict(
@@ -1299,38 +1193,42 @@
         "DestinationIpv6CidrBlock": str,
         "VpcEndpointId": ActionTargetTypeDef,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2CreateRouteActionTypeDef(
     _RequiredEC2CreateRouteActionTypeDef, _OptionalEC2CreateRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2CreateRouteTableActionTypeDef = TypedDict(
     "_RequiredEC2CreateRouteTableActionTypeDef",
     {
         "VpcId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2CreateRouteTableActionTypeDef = TypedDict(
     "_OptionalEC2CreateRouteTableActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2CreateRouteTableActionTypeDef(
     _RequiredEC2CreateRouteTableActionTypeDef, _OptionalEC2CreateRouteTableActionTypeDef
 ):
     pass
 
+
 _RequiredEC2DeleteRouteActionTypeDef = TypedDict(
     "_RequiredEC2DeleteRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2DeleteRouteActionTypeDef = TypedDict(
@@ -1340,19 +1238,21 @@
         "DestinationCidrBlock": str,
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
     },
     total=False,
 )
 
+
 class EC2DeleteRouteActionTypeDef(
     _RequiredEC2DeleteRouteActionTypeDef, _OptionalEC2DeleteRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteActionTypeDef",
     {
         "RouteTableId": ActionTargetTypeDef,
     },
 )
 _OptionalEC2ReplaceRouteActionTypeDef = TypedDict(
@@ -1363,19 +1263,21 @@
         "DestinationPrefixListId": str,
         "DestinationIpv6CidrBlock": str,
         "GatewayId": ActionTargetTypeDef,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteActionTypeDef(
     _RequiredEC2ReplaceRouteActionTypeDef, _OptionalEC2ReplaceRouteActionTypeDef
 ):
     pass
 
+
 _RequiredEC2ReplaceRouteTableAssociationActionTypeDef = TypedDict(
     "_RequiredEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "AssociationId": ActionTargetTypeDef,
         "RouteTableId": ActionTargetTypeDef,
     },
 )
@@ -1383,40 +1285,70 @@
     "_OptionalEC2ReplaceRouteTableAssociationActionTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class EC2ReplaceRouteTableAssociationActionTypeDef(
     _RequiredEC2ReplaceRouteTableAssociationActionTypeDef,
     _OptionalEC2ReplaceRouteTableAssociationActionTypeDef,
 ):
     pass
 
-ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
-    "ListAdminAccountsForOrganizationResponseTypeDef",
+
+AdminScopeOutputTypeDef = TypedDict(
+    "AdminScopeOutputTypeDef",
     {
-        "AdminAccounts": List[AdminAccountSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AccountScope": AccountScopeOutputTypeDef,
+        "OrganizationalUnitScope": OrganizationalUnitScopeOutputTypeDef,
+        "RegionScope": RegionScopeOutputTypeDef,
+        "PolicyTypeScope": PolicyTypeScopeOutputTypeDef,
     },
+    total=False,
 )
 
 AdminScopeTypeDef = TypedDict(
     "AdminScopeTypeDef",
     {
         "AccountScope": AccountScopeTypeDef,
         "OrganizationalUnitScope": OrganizationalUnitScopeTypeDef,
         "RegionScope": RegionScopeTypeDef,
         "PolicyTypeScope": PolicyTypeScopeTypeDef,
     },
     total=False,
 )
 
+_RequiredAppsListDataOutputTypeDef = TypedDict(
+    "_RequiredAppsListDataOutputTypeDef",
+    {
+        "ListName": str,
+        "AppsList": List[AppTypeDef],
+    },
+)
+_OptionalAppsListDataOutputTypeDef = TypedDict(
+    "_OptionalAppsListDataOutputTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": datetime,
+        "LastUpdateTime": datetime,
+        "PreviousAppsList": Dict[str, List[AppTypeDef]],
+    },
+    total=False,
+)
+
+
+class AppsListDataOutputTypeDef(
+    _RequiredAppsListDataOutputTypeDef, _OptionalAppsListDataOutputTypeDef
+):
+    pass
+
+
 AppsListDataSummaryTypeDef = TypedDict(
     "AppsListDataSummaryTypeDef",
     {
         "ListArn": str,
         "ListId": str,
         "ListName": str,
         "AppsList": List[AppTypeDef],
@@ -1424,56 +1356,222 @@
     total=False,
 )
 
 _RequiredAppsListDataTypeDef = TypedDict(
     "_RequiredAppsListDataTypeDef",
     {
         "ListName": str,
-        "AppsList": List[AppTypeDef],
+        "AppsList": Sequence[AppTypeDef],
     },
 )
 _OptionalAppsListDataTypeDef = TypedDict(
     "_OptionalAppsListDataTypeDef",
     {
         "ListId": str,
         "ListUpdateToken": str,
-        "CreateTime": datetime,
-        "LastUpdateTime": datetime,
-        "PreviousAppsList": Dict[str, List[AppTypeDef]],
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
+        "PreviousAppsList": Mapping[str, Sequence[AppTypeDef]],
     },
     total=False,
 )
 
+
 class AppsListDataTypeDef(_RequiredAppsListDataTypeDef, _OptionalAppsListDataTypeDef):
     pass
 
+
+_RequiredGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_RequiredGetProtectionStatusRequestRequestTypeDef",
+    {
+        "PolicyId": str,
+    },
+)
+_OptionalGetProtectionStatusRequestRequestTypeDef = TypedDict(
+    "_OptionalGetProtectionStatusRequestRequestTypeDef",
+    {
+        "MemberAccountId": str,
+        "StartTime": TimestampTypeDef,
+        "EndTime": TimestampTypeDef,
+        "NextToken": str,
+        "MaxResults": int,
+    },
+    total=False,
+)
+
+
+class GetProtectionStatusRequestRequestTypeDef(
+    _RequiredGetProtectionStatusRequestRequestTypeDef,
+    _OptionalGetProtectionStatusRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredProtocolsListDataTypeDef = TypedDict(
+    "_RequiredProtocolsListDataTypeDef",
+    {
+        "ListName": str,
+        "ProtocolsList": Sequence[str],
+    },
+)
+_OptionalProtocolsListDataTypeDef = TypedDict(
+    "_OptionalProtocolsListDataTypeDef",
+    {
+        "ListId": str,
+        "ListUpdateToken": str,
+        "CreateTime": TimestampTypeDef,
+        "LastUpdateTime": TimestampTypeDef,
+        "PreviousProtocolsList": Mapping[str, Sequence[str]],
+    },
+    total=False,
+)
+
+
+class ProtocolsListDataTypeDef(
+    _RequiredProtocolsListDataTypeDef, _OptionalProtocolsListDataTypeDef
+):
+    pass
+
+
+_RequiredResourceSetTypeDef = TypedDict(
+    "_RequiredResourceSetTypeDef",
+    {
+        "Name": str,
+        "ResourceTypeList": Sequence[str],
+    },
+)
+_OptionalResourceSetTypeDef = TypedDict(
+    "_OptionalResourceSetTypeDef",
+    {
+        "Id": str,
+        "Description": str,
+        "UpdateToken": str,
+        "LastUpdateTime": TimestampTypeDef,
+        "ResourceSetStatus": ResourceSetStatusType,
+    },
+    total=False,
+)
+
+
+class ResourceSetTypeDef(_RequiredResourceSetTypeDef, _OptionalResourceSetTypeDef):
+    pass
+
+
+AssociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "AssociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateThirdPartyFirewallResponseTypeDef = TypedDict(
+    "DisassociateThirdPartyFirewallResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
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
+GetAdminAccountResponseTypeDef = TypedDict(
+    "GetAdminAccountResponseTypeDef",
+    {
+        "AdminAccount": str,
+        "RoleStatus": AccountRoleStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetNotificationChannelResponseTypeDef = TypedDict(
+    "GetNotificationChannelResponseTypeDef",
+    {
+        "SnsTopicArn": str,
+        "SnsRoleName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetProtectionStatusResponseTypeDef = TypedDict(
+    "GetProtectionStatusResponseTypeDef",
+    {
+        "AdminAccountId": str,
+        "ServiceType": SecurityServiceTypeType,
+        "Data": str,
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetThirdPartyFirewallAssociationStatusResponseTypeDef = TypedDict(
+    "GetThirdPartyFirewallAssociationStatusResponseTypeDef",
+    {
+        "ThirdPartyFirewallStatus": ThirdPartyFirewallAssociationStatusType,
+        "MarketplaceOnboardingStatus": MarketplaceSubscriptionOnboardingStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminAccountsForOrganizationResponseTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationResponseTypeDef",
+    {
+        "AdminAccounts": List[AdminAccountSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAdminsManagingAccountResponseTypeDef = TypedDict(
+    "ListAdminsManagingAccountResponseTypeDef",
+    {
+        "AdminAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListMemberAccountsResponseTypeDef = TypedDict(
+    "ListMemberAccountsResponseTypeDef",
+    {
+        "MemberAccounts": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AwsEc2InstanceViolationTypeDef = TypedDict(
     "AwsEc2InstanceViolationTypeDef",
     {
         "ViolationTarget": str,
         "AwsEc2NetworkInterfaceViolations": List[AwsEc2NetworkInterfaceViolationTypeDef],
     },
     total=False,
 )
 
 BatchAssociateResourceResponseTypeDef = TypedDict(
     "BatchAssociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDisassociateResourceResponseTypeDef = TypedDict(
     "BatchDisassociateResourceResponseTypeDef",
     {
         "ResourceSetIdentifier": str,
         "FailedItems": List[FailedItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceDetailTypeDef = TypedDict(
     "PolicyComplianceDetailTypeDef",
     {
         "PolicyOwner": str,
@@ -1488,15 +1586,15 @@
 )
 
 ListDiscoveredResourcesResponseTypeDef = TypedDict(
     "ListDiscoveredResourcesResponseTypeDef",
     {
         "Items": List[DiscoveredResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PolicyComplianceStatusTypeDef = TypedDict(
     "PolicyComplianceStatusTypeDef",
     {
         "PolicyOwner": str,
@@ -1519,143 +1617,199 @@
     },
     total=False,
 )
 
 GetProtocolsListResponseTypeDef = TypedDict(
     "GetProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutProtocolsListResponseTypeDef = TypedDict(
     "PutProtocolsListResponseTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "ProtocolsList": ProtocolsListDataOutputTypeDef,
         "ProtocolsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceSetResponseTypeDef = TypedDict(
     "GetResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutResourceSetResponseTypeDef = TypedDict(
     "PutResourceSetResponseTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ResourceSet": ResourceSetOutputTypeDef,
         "ResourceSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListPoliciesResponseTypeDef = TypedDict(
-    "ListPoliciesResponseTypeDef",
+ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef = TypedDict(
+    "ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef",
     {
-        "PolicyList": List[PolicySummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListProtocolsListsResponseTypeDef = TypedDict(
-    "ListProtocolsListsResponseTypeDef",
+ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef = TypedDict(
+    "ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef",
     {
-        "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListResourceSetResourcesResponseTypeDef = TypedDict(
-    "ListResourceSetResourcesResponseTypeDef",
+ListAppsListsRequestListAppsListsPaginateTypeDef = TypedDict(
+    "ListAppsListsRequestListAppsListsPaginateTypeDef",
     {
-        "Items": List[ResourceTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-ListResourceSetsResponseTypeDef = TypedDict(
-    "ListResourceSetsResponseTypeDef",
+_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
-        "ResourceSets": List[ResourceSetSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PolicyId": str,
     },
 )
-
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
+_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef = TypedDict(
+    "_OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef",
     {
-        "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
-_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_RequiredPutProtocolsListRequestRequestTypeDef",
+
+class ListComplianceStatusRequestListComplianceStatusPaginateTypeDef(
+    _RequiredListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    _OptionalListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+):
+    pass
+
+
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
     {
-        "ProtocolsList": ProtocolsListDataTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
-_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
-    "_OptionalPutProtocolsListRequestRequestTypeDef",
+
+ListPoliciesRequestListPoliciesPaginateTypeDef = TypedDict(
+    "ListPoliciesRequestListPoliciesPaginateTypeDef",
     {
-        "TagList": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PutProtocolsListRequestRequestTypeDef(
-    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
-):
-    pass
+ListProtocolsListsRequestListProtocolsListsPaginateTypeDef = TypedDict(
+    "ListProtocolsListsRequestListProtocolsListsPaginateTypeDef",
+    {
+        "DefaultLists": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
-_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_RequiredPutResourceSetRequestRequestTypeDef",
+_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
-        "ResourceSet": ResourceSetTypeDef,
+        "ThirdPartyFirewall": ThirdPartyFirewallType,
     },
 )
-_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
-    "_OptionalPutResourceSetRequestRequestTypeDef",
+_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef = TypedDict(
+    "_OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef",
     {
-        "TagList": Sequence[TagTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-class PutResourceSetRequestRequestTypeDef(
-    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+
+class ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef(
+    _RequiredListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
+    _OptionalListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
 ):
     pass
 
+
+ListPoliciesResponseTypeDef = TypedDict(
+    "ListPoliciesResponseTypeDef",
+    {
+        "PolicyList": List[PolicySummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListProtocolsListsResponseTypeDef = TypedDict(
+    "ListProtocolsListsResponseTypeDef",
+    {
+        "ProtocolsLists": List[ProtocolsListDataSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceSetResourcesResponseTypeDef = TypedDict(
+    "ListResourceSetResourcesResponseTypeDef",
+    {
+        "Items": List[ResourceTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListResourceSetsResponseTypeDef = TypedDict(
+    "ListResourceSetsResponseTypeDef",
+    {
+        "ResourceSets": List[ResourceSetSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
 
 ListThirdPartyFirewallFirewallPoliciesResponseTypeDef = TypedDict(
     "ListThirdPartyFirewallFirewallPoliciesResponseTypeDef",
     {
         "ThirdPartyFirewallFirewallPolicies": List[ThirdPartyFirewallFirewallPolicyTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallBlackHoleRouteDetectedViolationTypeDef = TypedDict(
     "NetworkFirewallBlackHoleRouteDetectedViolationTypeDef",
     {
         "ViolationTarget": str,
@@ -1801,99 +1955,149 @@
     },
     total=False,
 )
 
 GetAdminScopeResponseTypeDef = TypedDict(
     "GetAdminScopeResponseTypeDef",
     {
-        "AdminScope": AdminScopeTypeDef,
+        "AdminScope": AdminScopeOutputTypeDef,
         "Status": OrganizationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+AdminScopeUnionTypeDef = Union[AdminScopeTypeDef, AdminScopeOutputTypeDef]
 _RequiredPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_RequiredPutAdminAccountRequestRequestTypeDef",
     {
         "AdminAccount": str,
     },
 )
 _OptionalPutAdminAccountRequestRequestTypeDef = TypedDict(
     "_OptionalPutAdminAccountRequestRequestTypeDef",
     {
         "AdminScope": AdminScopeTypeDef,
     },
     total=False,
 )
 
+
 class PutAdminAccountRequestRequestTypeDef(
     _RequiredPutAdminAccountRequestRequestTypeDef, _OptionalPutAdminAccountRequestRequestTypeDef
 ):
     pass
 
-ListAppsListsResponseTypeDef = TypedDict(
-    "ListAppsListsResponseTypeDef",
+
+GetAppsListResponseTypeDef = TypedDict(
+    "GetAppsListResponseTypeDef",
     {
-        "AppsLists": List[AppsListDataSummaryTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "AppsList": AppsListDataOutputTypeDef,
+        "AppsListArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-GetAppsListResponseTypeDef = TypedDict(
-    "GetAppsListResponseTypeDef",
+PutAppsListResponseTypeDef = TypedDict(
+    "PutAppsListResponseTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
+        "AppsList": AppsListDataOutputTypeDef,
         "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListAppsListsResponseTypeDef = TypedDict(
+    "ListAppsListsResponseTypeDef",
+    {
+        "AppsLists": List[AppsListDataSummaryTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+AppsListDataUnionTypeDef = Union[AppsListDataTypeDef, AppsListDataOutputTypeDef]
 _RequiredPutAppsListRequestRequestTypeDef = TypedDict(
     "_RequiredPutAppsListRequestRequestTypeDef",
     {
         "AppsList": AppsListDataTypeDef,
     },
 )
 _OptionalPutAppsListRequestRequestTypeDef = TypedDict(
     "_OptionalPutAppsListRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutAppsListRequestRequestTypeDef(
     _RequiredPutAppsListRequestRequestTypeDef, _OptionalPutAppsListRequestRequestTypeDef
 ):
     pass
 
-PutAppsListResponseTypeDef = TypedDict(
-    "PutAppsListResponseTypeDef",
+
+ProtocolsListDataUnionTypeDef = Union[ProtocolsListDataTypeDef, ProtocolsListDataOutputTypeDef]
+_RequiredPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_RequiredPutProtocolsListRequestRequestTypeDef",
     {
-        "AppsList": AppsListDataTypeDef,
-        "AppsListArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ProtocolsList": ProtocolsListDataTypeDef,
+    },
+)
+_OptionalPutProtocolsListRequestRequestTypeDef = TypedDict(
+    "_OptionalPutProtocolsListRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
+    },
+    total=False,
+)
+
+
+class PutProtocolsListRequestRequestTypeDef(
+    _RequiredPutProtocolsListRequestRequestTypeDef, _OptionalPutProtocolsListRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_RequiredPutResourceSetRequestRequestTypeDef",
+    {
+        "ResourceSet": ResourceSetTypeDef,
+    },
+)
+_OptionalPutResourceSetRequestRequestTypeDef = TypedDict(
+    "_OptionalPutResourceSetRequestRequestTypeDef",
+    {
+        "TagList": Sequence[TagTypeDef],
     },
+    total=False,
 )
 
+
+class PutResourceSetRequestRequestTypeDef(
+    _RequiredPutResourceSetRequestRequestTypeDef, _OptionalPutResourceSetRequestRequestTypeDef
+):
+    pass
+
+
+ResourceSetUnionTypeDef = Union[ResourceSetTypeDef, ResourceSetOutputTypeDef]
 GetComplianceDetailResponseTypeDef = TypedDict(
     "GetComplianceDetailResponseTypeDef",
     {
         "PolicyComplianceDetail": PolicyComplianceDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListComplianceStatusResponseTypeDef = TypedDict(
     "ListComplianceStatusResponseTypeDef",
     {
         "PolicyComplianceStatusList": List[PolicyComplianceStatusTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkFirewallPolicyDescriptionTypeDef = TypedDict(
     "NetworkFirewallPolicyDescriptionTypeDef",
     {
         "StatelessRuleGroups": List[StatelessRuleGroupTypeDef],
@@ -1918,19 +2122,21 @@
     {
         "ManagedServiceData": str,
         "PolicyOption": PolicyOptionTypeDef,
     },
     total=False,
 )
 
+
 class SecurityServicePolicyDataTypeDef(
     _RequiredSecurityServicePolicyDataTypeDef, _OptionalSecurityServicePolicyDataTypeDef
 ):
     pass
 
+
 AwsVPCSecurityGroupViolationTypeDef = TypedDict(
     "AwsVPCSecurityGroupViolationTypeDef",
     {
         "ViolationTarget": str,
         "ViolationTargetDescription": str,
         "PartialMatches": List[PartialMatchTypeDef],
         "PossibleSecurityGroupRemediationActions": List[SecurityGroupRemediationActionTypeDef],
@@ -1953,26 +2159,26 @@
         "ViolationTarget": str,
         "CurrentPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
         "ExpectedPolicyDescription": NetworkFirewallPolicyDescriptionTypeDef,
     },
     total=False,
 )
 
-_RequiredPolicyTypeDef = TypedDict(
-    "_RequiredPolicyTypeDef",
+_RequiredPolicyOutputTypeDef = TypedDict(
+    "_RequiredPolicyOutputTypeDef",
     {
         "PolicyName": str,
         "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
         "ResourceType": str,
         "ExcludeResourceTags": bool,
         "RemediationEnabled": bool,
     },
 )
-_OptionalPolicyTypeDef = TypedDict(
-    "_OptionalPolicyTypeDef",
+_OptionalPolicyOutputTypeDef = TypedDict(
+    "_OptionalPolicyOutputTypeDef",
     {
         "PolicyId": str,
         "PolicyUpdateToken": str,
         "ResourceTypeList": List[str],
         "ResourceTags": List[ResourceTagTypeDef],
         "DeleteUnusedFMManagedResources": bool,
         "IncludeMap": Dict[CustomerPolicyScopeIdTypeType, List[str]],
@@ -1980,17 +2186,51 @@
         "ResourceSetIds": List[str],
         "PolicyDescription": str,
         "PolicyStatus": CustomerPolicyStatusType,
     },
     total=False,
 )
 
+
+class PolicyOutputTypeDef(_RequiredPolicyOutputTypeDef, _OptionalPolicyOutputTypeDef):
+    pass
+
+
+_RequiredPolicyTypeDef = TypedDict(
+    "_RequiredPolicyTypeDef",
+    {
+        "PolicyName": str,
+        "SecurityServicePolicyData": SecurityServicePolicyDataTypeDef,
+        "ResourceType": str,
+        "ExcludeResourceTags": bool,
+        "RemediationEnabled": bool,
+    },
+)
+_OptionalPolicyTypeDef = TypedDict(
+    "_OptionalPolicyTypeDef",
+    {
+        "PolicyId": str,
+        "PolicyUpdateToken": str,
+        "ResourceTypeList": Sequence[str],
+        "ResourceTags": Sequence[ResourceTagTypeDef],
+        "DeleteUnusedFMManagedResources": bool,
+        "IncludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ExcludeMap": Mapping[CustomerPolicyScopeIdTypeType, Sequence[str]],
+        "ResourceSetIds": Sequence[str],
+        "PolicyDescription": str,
+        "PolicyStatus": CustomerPolicyStatusType,
+    },
+    total=False,
+)
+
+
 class PolicyTypeDef(_RequiredPolicyTypeDef, _OptionalPolicyTypeDef):
     pass
 
+
 _RequiredPossibleRemediationActionTypeDef = TypedDict(
     "_RequiredPossibleRemediationActionTypeDef",
     {
         "OrderedRemediationActions": List[RemediationActionWithOrderTypeDef],
     },
 )
 _OptionalPossibleRemediationActionTypeDef = TypedDict(
@@ -1998,55 +2238,60 @@
     {
         "Description": str,
         "IsDefaultAction": bool,
     },
     total=False,
 )
 
+
 class PossibleRemediationActionTypeDef(
     _RequiredPossibleRemediationActionTypeDef, _OptionalPossibleRemediationActionTypeDef
 ):
     pass
 
+
 GetPolicyResponseTypeDef = TypedDict(
     "GetPolicyResponseTypeDef",
     {
-        "Policy": PolicyTypeDef,
+        "Policy": PolicyOutputTypeDef,
         "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PutPolicyResponseTypeDef = TypedDict(
+    "PutPolicyResponseTypeDef",
+    {
+        "Policy": PolicyOutputTypeDef,
+        "PolicyArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PolicyUnionTypeDef = Union[PolicyTypeDef, PolicyOutputTypeDef]
 _RequiredPutPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutPolicyRequestRequestTypeDef",
     {
         "Policy": PolicyTypeDef,
     },
 )
 _OptionalPutPolicyRequestRequestTypeDef = TypedDict(
     "_OptionalPutPolicyRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class PutPolicyRequestRequestTypeDef(
     _RequiredPutPolicyRequestRequestTypeDef, _OptionalPutPolicyRequestRequestTypeDef
 ):
     pass
 
-PutPolicyResponseTypeDef = TypedDict(
-    "PutPolicyResponseTypeDef",
-    {
-        "Policy": PolicyTypeDef,
-        "PolicyArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 PossibleRemediationActionsTypeDef = TypedDict(
     "PossibleRemediationActionsTypeDef",
     {
         "Description": str,
         "Actions": List[PossibleRemediationActionTypeDef],
     },
@@ -2118,17 +2363,19 @@
     {
         "ResourceTags": List[TagTypeDef],
         "ResourceDescription": str,
     },
     total=False,
 )
 
+
 class ViolationDetailTypeDef(_RequiredViolationDetailTypeDef, _OptionalViolationDetailTypeDef):
     pass
 
+
 GetViolationDetailsResponseTypeDef = TypedDict(
     "GetViolationDetailsResponseTypeDef",
     {
         "ViolationDetail": ViolationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/PKG-INFO` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-fms
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.FMS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore fms type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore fms type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-fms"></a>
 
 # types-aiobotocore-fms
 
 [![PyPI - types-aiobotocore-fms](https://img.shields.io/pypi/v/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-fms.svg?color=blue)](https://pypi.org/project/types-aiobotocore-fms)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-fms?color=blue)](https://pypistats.org/packages/types-aiobotocore-fms)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-fms)](https://pepy.tech/project/types-aiobotocore-fms)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.FMS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/fms.html#FMS)
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
 [types-aiobotocore-fms docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_fms/).
 
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
@@ -357,183 +356,198 @@
 )
 
 
 def check_value(value: AccountRoleStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_fms.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_fms.type_defs import (
+    AccountScopeOutputTypeDef,
     AccountScopeTypeDef,
     ActionTargetTypeDef,
     AdminAccountSummaryTypeDef,
+    OrganizationalUnitScopeOutputTypeDef,
+    PolicyTypeScopeOutputTypeDef,
+    RegionScopeOutputTypeDef,
     OrganizationalUnitScopeTypeDef,
     PolicyTypeScopeTypeDef,
     RegionScopeTypeDef,
     AppTypeDef,
+    TimestampTypeDef,
     AssociateAdminAccountRequestRequestTypeDef,
     AssociateThirdPartyFirewallRequestRequestTypeDef,
-    AssociateThirdPartyFirewallResponseTypeDef,
+    ResponseMetadataTypeDef,
     AwsEc2NetworkInterfaceViolationTypeDef,
     PartialMatchTypeDef,
     BatchAssociateResourceRequestRequestTypeDef,
     FailedItemTypeDef,
     BatchDisassociateResourceRequestRequestTypeDef,
     ComplianceViolatorTypeDef,
     DeleteAppsListRequestRequestTypeDef,
     DeletePolicyRequestRequestTypeDef,
     DeleteProtocolsListRequestRequestTypeDef,
     DeleteResourceSetRequestRequestTypeDef,
     DisassociateThirdPartyFirewallRequestRequestTypeDef,
-    DisassociateThirdPartyFirewallResponseTypeDef,
     DiscoveredResourceTypeDef,
     DnsDuplicateRuleGroupViolationTypeDef,
     DnsRuleGroupLimitExceededViolationTypeDef,
     DnsRuleGroupPriorityConflictViolationTypeDef,
-    EmptyResponseMetadataTypeDef,
     EvaluationResultTypeDef,
     ExpectedRouteTypeDef,
     FMSPolicyUpdateFirewallCreationConfigActionTypeDef,
     FirewallSubnetIsOutOfScopeViolationTypeDef,
     FirewallSubnetMissingVPCEndpointViolationTypeDef,
-    GetAdminAccountResponseTypeDef,
     GetAdminScopeRequestRequestTypeDef,
     GetAppsListRequestRequestTypeDef,
     GetComplianceDetailRequestRequestTypeDef,
-    GetNotificationChannelResponseTypeDef,
     GetPolicyRequestRequestTypeDef,
-    GetProtectionStatusRequestRequestTypeDef,
-    GetProtectionStatusResponseTypeDef,
     GetProtocolsListRequestRequestTypeDef,
-    ProtocolsListDataTypeDef,
+    ProtocolsListDataOutputTypeDef,
     GetResourceSetRequestRequestTypeDef,
-    ResourceSetTypeDef,
+    ResourceSetOutputTypeDef,
     GetThirdPartyFirewallAssociationStatusRequestRequestTypeDef,
-    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
     GetViolationDetailsRequestRequestTypeDef,
-    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAdminAccountsForOrganizationRequestRequestTypeDef,
-    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
     ListAdminsManagingAccountRequestRequestTypeDef,
-    ListAdminsManagingAccountResponseTypeDef,
-    ListAppsListsRequestListAppsListsPaginateTypeDef,
     ListAppsListsRequestRequestTypeDef,
-    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
     ListComplianceStatusRequestRequestTypeDef,
     ListDiscoveredResourcesRequestRequestTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
-    ListMemberAccountsResponseTypeDef,
-    ListPoliciesRequestListPoliciesPaginateTypeDef,
     ListPoliciesRequestRequestTypeDef,
     PolicySummaryTypeDef,
-    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
     ListProtocolsListsRequestRequestTypeDef,
     ProtocolsListDataSummaryTypeDef,
     ListResourceSetResourcesRequestRequestTypeDef,
     ResourceTypeDef,
     ListResourceSetsRequestRequestTypeDef,
     ResourceSetSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
-    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListThirdPartyFirewallFirewallPoliciesRequestRequestTypeDef,
     ThirdPartyFirewallFirewallPolicyTypeDef,
     RouteTypeDef,
     NetworkFirewallMissingExpectedRTViolationTypeDef,
     NetworkFirewallMissingFirewallViolationTypeDef,
     NetworkFirewallMissingSubnetViolationTypeDef,
     StatefulEngineOptionsTypeDef,
     StatelessRuleGroupTypeDef,
     NetworkFirewallPolicyTypeDef,
     NetworkFirewallStatefulRuleGroupOverrideTypeDef,
-    PaginatorConfigTypeDef,
     ThirdPartyFirewallPolicyTypeDef,
     ResourceTagTypeDef,
     PutNotificationChannelRequestRequestTypeDef,
     ThirdPartyFirewallMissingExpectedRouteTableViolationTypeDef,
     ThirdPartyFirewallMissingFirewallViolationTypeDef,
     ThirdPartyFirewallMissingSubnetViolationTypeDef,
-    ResponseMetadataTypeDef,
     SecurityGroupRuleDescriptionTypeDef,
     UntagResourceRequestRequestTypeDef,
     EC2AssociateRouteTableActionTypeDef,
     EC2CopyRouteTableActionTypeDef,
     EC2CreateRouteActionTypeDef,
     EC2CreateRouteTableActionTypeDef,
     EC2DeleteRouteActionTypeDef,
     EC2ReplaceRouteActionTypeDef,
     EC2ReplaceRouteTableAssociationActionTypeDef,
-    ListAdminAccountsForOrganizationResponseTypeDef,
+    AdminScopeOutputTypeDef,
     AdminScopeTypeDef,
+    AppsListDataOutputTypeDef,
     AppsListDataSummaryTypeDef,
     AppsListDataTypeDef,
+    GetProtectionStatusRequestRequestTypeDef,
+    ProtocolsListDataTypeDef,
+    ResourceSetTypeDef,
+    AssociateThirdPartyFirewallResponseTypeDef,
+    DisassociateThirdPartyFirewallResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAdminAccountResponseTypeDef,
+    GetNotificationChannelResponseTypeDef,
+    GetProtectionStatusResponseTypeDef,
+    GetThirdPartyFirewallAssociationStatusResponseTypeDef,
+    ListAdminAccountsForOrganizationResponseTypeDef,
+    ListAdminsManagingAccountResponseTypeDef,
+    ListMemberAccountsResponseTypeDef,
     AwsEc2InstanceViolationTypeDef,
     BatchAssociateResourceResponseTypeDef,
     BatchDisassociateResourceResponseTypeDef,
     PolicyComplianceDetailTypeDef,
     ListDiscoveredResourcesResponseTypeDef,
     PolicyComplianceStatusTypeDef,
     NetworkFirewallMissingExpectedRoutesViolationTypeDef,
     GetProtocolsListResponseTypeDef,
     PutProtocolsListResponseTypeDef,
     GetResourceSetResponseTypeDef,
     PutResourceSetResponseTypeDef,
+    ListAdminAccountsForOrganizationRequestListAdminAccountsForOrganizationPaginateTypeDef,
+    ListAdminsManagingAccountRequestListAdminsManagingAccountPaginateTypeDef,
+    ListAppsListsRequestListAppsListsPaginateTypeDef,
+    ListComplianceStatusRequestListComplianceStatusPaginateTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListPoliciesRequestListPoliciesPaginateTypeDef,
+    ListProtocolsListsRequestListProtocolsListsPaginateTypeDef,
+    ListThirdPartyFirewallFirewallPoliciesRequestListThirdPartyFirewallFirewallPoliciesPaginateTypeDef,
     ListPoliciesResponseTypeDef,
     ListProtocolsListsResponseTypeDef,
     ListResourceSetResourcesResponseTypeDef,
     ListResourceSetsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    PutProtocolsListRequestRequestTypeDef,
-    PutResourceSetRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     ListThirdPartyFirewallFirewallPoliciesResponseTypeDef,
     NetworkFirewallBlackHoleRouteDetectedViolationTypeDef,
     NetworkFirewallInternetTrafficNotInspectedViolationTypeDef,
     NetworkFirewallInvalidRouteConfigurationViolationTypeDef,
     NetworkFirewallUnexpectedFirewallRoutesViolationTypeDef,
     NetworkFirewallUnexpectedGatewayRoutesViolationTypeDef,
     RouteHasOutOfScopeEndpointViolationTypeDef,
     StatefulRuleGroupTypeDef,
     PolicyOptionTypeDef,
     SecurityGroupRemediationActionTypeDef,
     RemediationActionTypeDef,
     GetAdminScopeResponseTypeDef,
+    AdminScopeUnionTypeDef,
     PutAdminAccountRequestRequestTypeDef,
-    ListAppsListsResponseTypeDef,
     GetAppsListResponseTypeDef,
-    PutAppsListRequestRequestTypeDef,
     PutAppsListResponseTypeDef,
+    ListAppsListsResponseTypeDef,
+    AppsListDataUnionTypeDef,
+    PutAppsListRequestRequestTypeDef,
+    ProtocolsListDataUnionTypeDef,
+    PutProtocolsListRequestRequestTypeDef,
+    PutResourceSetRequestRequestTypeDef,
+    ResourceSetUnionTypeDef,
     GetComplianceDetailResponseTypeDef,
     ListComplianceStatusResponseTypeDef,
     NetworkFirewallPolicyDescriptionTypeDef,
     SecurityServicePolicyDataTypeDef,
     AwsVPCSecurityGroupViolationTypeDef,
     RemediationActionWithOrderTypeDef,
     NetworkFirewallPolicyModifiedViolationTypeDef,
+    PolicyOutputTypeDef,
     PolicyTypeDef,
     PossibleRemediationActionTypeDef,
     GetPolicyResponseTypeDef,
-    PutPolicyRequestRequestTypeDef,
     PutPolicyResponseTypeDef,
+    PolicyUnionTypeDef,
+    PutPolicyRequestRequestTypeDef,
     PossibleRemediationActionsTypeDef,
     ResourceViolationTypeDef,
     ViolationDetailTypeDef,
     GetViolationDetailsResponseTypeDef,
 )
 
 
-def get_structure() -> AccountScopeTypeDef:
+def get_value() -> AccountScopeOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-fms-2.5.2/types_aiobotocore_fms.egg-info/SOURCES.txt` & `types-aiobotocore-fms-2.5.2.post1/types_aiobotocore_fms.egg-info/SOURCES.txt`

 * *Files identical despite different names*


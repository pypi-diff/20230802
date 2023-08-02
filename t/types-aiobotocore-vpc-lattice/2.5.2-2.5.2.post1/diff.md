# Comparing `tmp/types-aiobotocore-vpc-lattice-2.5.2.tar.gz` & `tmp/types-aiobotocore-vpc-lattice-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-vpc-lattice-2.5.2.tar", last modified: Sat Jul  8 01:44:27 2023, max compression
+gzip compressed data, was "types-aiobotocore-vpc-lattice-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:09 2023, max compression
```

## Comparing `types-aiobotocore-vpc-lattice-2.5.2.tar` & `types-aiobotocore-vpc-lattice-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.323032 types-aiobotocore-vpc-lattice-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-08 01:44:27.323032 types-aiobotocore-vpc-lattice-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19034 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:27.323032 types-aiobotocore-vpc-lattice-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.307031 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41317 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    41247 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11921 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11910 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    48701 2023-07-08 01:42:15.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    48652 2023-07-08 01:42:15.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:14.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:27.323032 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-07-08 01:44:27.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-07-08 01:44:27.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:27.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:27.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:44:27.000000 types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.193431 types-aiobotocore-vpc-lattice-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-08-02 14:53:09.189431 types-aiobotocore-vpc-lattice-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19189 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:09.193431 types-aiobotocore-vpc-lattice-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.185430 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41389 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41319 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10565 2023-08-02 14:50:50.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-08-02 14:50:50.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    49704 2023-08-02 14:50:54.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49655 2023-08-02 14:50:53.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:49.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:09.189431 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20722 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:53:09.000000 types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/LICENSE` & `types-aiobotocore-vpc-lattice-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/PKG-INFO` & `types-aiobotocore-vpc-lattice-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-vpc-lattice
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore vpc-lattice type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-vpc-lattice"></a>
 
 # types-aiobotocore-vpc-lattice
 
 [![PyPI - types-aiobotocore-vpc-lattice](https://img.shields.io/pypi/v/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-vpc-lattice?color=blue)](https://pypistats.org/packages/types-aiobotocore-vpc-lattice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VPCLattice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [types-aiobotocore-vpc-lattice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -354,161 +321,167 @@
 )
 
 
 def check_value(value: AuthPolicyStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_vpc_lattice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
-    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
-    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
     FixedResponseActionTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
-    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
-    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
     HeaderMatchTypeTypeDef,
     MatcherTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
-    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkResponseTypeDef,
     UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationResponseTypeDef,
     UpdateServiceRequestRequestTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
+    CreateServiceNetworkResponseTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DeleteTargetGroupResponseTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
+    GetAuthPolicyResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetServiceNetworkResponseTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     ListAccessLogSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutAuthPolicyResponseTypeDef,
+    UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
     HeaderMatchTypeDef,
     HealthCheckConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
+    HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
-    CreateListenerRequestRequestTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
-    UpdateListenerRequestRequestTypeDef,
     UpdateListenerResponseTypeDef,
+    CreateListenerRequestRequestTypeDef,
+    RuleActionUnionTypeDef,
+    UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
+    UpdateRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleResponseTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
+def get_value() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/README.md` & `types-aiobotocore-vpc-lattice-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-vpc-lattice
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore vpc-lattice type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-vpc-lattice"></a>
 
 # types-aiobotocore-vpc-lattice
 
 [![PyPI - types-aiobotocore-vpc-lattice](https://img.shields.io/pypi/v/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-vpc-lattice?color=blue)](https://pypistats.org/packages/types-aiobotocore-vpc-lattice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VPCLattice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [types-aiobotocore-vpc-lattice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -321,161 +353,167 @@
 )
 
 
 def check_value(value: AuthPolicyStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_vpc_lattice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
-    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
-    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
     FixedResponseActionTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
-    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
-    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
     HeaderMatchTypeTypeDef,
     MatcherTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
-    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkResponseTypeDef,
     UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationResponseTypeDef,
     UpdateServiceRequestRequestTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
+    CreateServiceNetworkResponseTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DeleteTargetGroupResponseTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
+    GetAuthPolicyResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetServiceNetworkResponseTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     ListAccessLogSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutAuthPolicyResponseTypeDef,
+    UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
     HeaderMatchTypeDef,
     HealthCheckConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
+    HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
-    CreateListenerRequestRequestTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
-    UpdateListenerRequestRequestTypeDef,
     UpdateListenerResponseTypeDef,
+    CreateListenerRequestRequestTypeDef,
+    RuleActionUnionTypeDef,
+    UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
+    UpdateRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleResponseTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
+def get_value() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/setup.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-vpc-lattice",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_vpc_lattice"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with"
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
-    keywords="aiobotocore vpc-lattice type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore vpc-lattice type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_vpc_lattice": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/"
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/__init__.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/__init__.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/__main__.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.VPCLattice 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.VPCLattice 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice\nOther"
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

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/client.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionTypeDef,
-    RuleMatchTypeDef,
+    RuleActionUnionTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -170,15 +170,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_access_log_subscription)
         """
 
     async def create_listener(
         self,
         *,
-        defaultAction: RuleActionTypeDef,
+        defaultAction: RuleActionUnionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
@@ -188,17 +188,17 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_listener)
         """
 
     async def create_rule(
         self,
         *,
-        action: RuleActionTypeDef,
+        action: RuleActionUnionTypeDef,
         listenerIdentifier: str,
-        match: RuleMatchTypeDef,
+        match: RuleMatchUnionTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
@@ -678,31 +678,35 @@
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_access_log_subscription)
         """
 
     async def update_listener(
-        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
+        self,
+        *,
+        defaultAction: RuleActionUnionTypeDef,
+        listenerIdentifier: str,
+        serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_listener)
         """
 
     async def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionTypeDef = ...,
-        match: RuleMatchTypeDef = ...,
+        action: RuleActionUnionTypeDef = ...,
+        match: RuleMatchUnionTypeDef = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_rule)
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/client.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PutAuthPolicyResponseTypeDef,
     RegisterTargetsResponseTypeDef,
-    RuleActionTypeDef,
-    RuleMatchTypeDef,
+    RuleActionUnionTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     TargetGroupConfigTypeDef,
     TargetTypeDef,
     UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateListenerResponseTypeDef,
     UpdateRuleResponseTypeDef,
     UpdateServiceNetworkResponseTypeDef,
@@ -161,15 +161,15 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_access_log_subscription)
         """
     async def create_listener(
         self,
         *,
-        defaultAction: RuleActionTypeDef,
+        defaultAction: RuleActionUnionTypeDef,
         name: str,
         protocol: ListenerProtocolType,
         serviceIdentifier: str,
         clientToken: str = ...,
         port: int = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateListenerResponseTypeDef:
@@ -178,17 +178,17 @@
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.create_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#create_listener)
         """
     async def create_rule(
         self,
         *,
-        action: RuleActionTypeDef,
+        action: RuleActionUnionTypeDef,
         listenerIdentifier: str,
-        match: RuleMatchTypeDef,
+        match: RuleMatchUnionTypeDef,
         name: str,
         priority: int,
         serviceIdentifier: str,
         clientToken: str = ...,
         tags: Mapping[str, str] = ...
     ) -> CreateRuleResponseTypeDef:
         """
@@ -624,30 +624,34 @@
         """
         Updates the specified access log subscription.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_access_log_subscription)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_access_log_subscription)
         """
     async def update_listener(
-        self, *, defaultAction: RuleActionTypeDef, listenerIdentifier: str, serviceIdentifier: str
+        self,
+        *,
+        defaultAction: RuleActionUnionTypeDef,
+        listenerIdentifier: str,
+        serviceIdentifier: str
     ) -> UpdateListenerResponseTypeDef:
         """
         Updates the specified listener for the specified service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_listener)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_listener)
         """
     async def update_rule(
         self,
         *,
         listenerIdentifier: str,
         ruleIdentifier: str,
         serviceIdentifier: str,
-        action: RuleActionTypeDef = ...,
-        match: RuleMatchTypeDef = ...,
+        action: RuleActionUnionTypeDef = ...,
+        match: RuleMatchUnionTypeDef = ...,
         priority: int = ...
     ) -> UpdateRuleResponseTypeDef:
         """
         Updates a rule for the listener.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Client.update_rule)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/client/#update_rule)
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/literals.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/literals.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/paginator.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,30 +82,30 @@
 class ListAccessLogSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessLogSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
         """
 
 
 class ListListenersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, serviceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listlistenerspaginator)
         """
 
 
@@ -116,15 +116,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listrulespaginator)
         """
 
 
@@ -135,15 +135,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 
@@ -154,45 +154,45 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 
 class ListServiceNetworksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkspaginator)
         """
 
 
 class ListServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicespaginator)
         """
 
 
@@ -203,15 +203,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 
@@ -222,13 +222,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/paginator.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -79,29 +79,29 @@
 class ListAccessLogSubscriptionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
     """
 
     def paginate(
-        self, *, resourceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccessLogSubscriptionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListAccessLogSubscriptions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listaccesslogsubscriptionspaginator)
         """
 
 class ListListenersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listlistenerspaginator)
     """
 
     def paginate(
-        self, *, serviceIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, serviceIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListListenersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListListeners.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listlistenerspaginator)
         """
 
 class ListRulesPaginator(AioPaginator):
@@ -111,15 +111,15 @@
     """
 
     def paginate(
         self,
         *,
         listenerIdentifier: str,
         serviceIdentifier: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRulesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListRules.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listrulespaginator)
         """
 
 class ListServiceNetworkServiceAssociationsPaginator(AioPaginator):
@@ -129,15 +129,15 @@
     """
 
     def paginate(
         self,
         *,
         serviceIdentifier: str = ...,
         serviceNetworkIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceNetworkServiceAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkServiceAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkserviceassociationspaginator)
         """
 
 class ListServiceNetworkVpcAssociationsPaginator(AioPaginator):
@@ -147,43 +147,43 @@
     """
 
     def paginate(
         self,
         *,
         serviceNetworkIdentifier: str = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceNetworkVpcAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworkVpcAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkvpcassociationspaginator)
         """
 
 class ListServiceNetworksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServiceNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServiceNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicenetworkspaginator)
         """
 
 class ListServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListServicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listservicespaginator)
         """
 
 class ListTargetGroupsPaginator(AioPaginator):
@@ -193,15 +193,15 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupType: TargetGroupTypeType = ...,
         vpcIdentifier: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargetGroups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetgroupspaginator)
         """
 
 class ListTargetsPaginator(AioPaginator):
@@ -211,13 +211,13 @@
     """
 
     def paginate(
         self,
         *,
         targetGroupIdentifier: str,
         targets: Sequence[TargetTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice.Paginator.ListTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/paginators/#listtargetspaginator)
         """
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/type_defs.py` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef
 
-    data: AccessLogSubscriptionSummaryTypeDef = {...}
+    data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     ListenerProtocolType,
@@ -35,145 +35,151 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
-    "CreateAccessLogSubscriptionResponseTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
-    "CreateServiceNetworkResponseTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DnsEntryTypeDef",
     "CreateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "DeleteAccessLogSubscriptionRequestRequestTypeDef",
     "DeleteAuthPolicyRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
-    "DeleteServiceResponseTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
-    "DeleteTargetGroupResponseTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
     "FixedResponseActionTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
-    "GetAccessLogSubscriptionResponseTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
-    "GetAuthPolicyResponseTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
-    "GetServiceNetworkResponseTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
     "HeaderMatchTypeTypeDef",
     "MatcherTypeDef",
-    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
-    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     "ServiceNetworkVpcAssociationSummaryTypeDef",
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
-    "PutAuthPolicyResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
-    "UpdateAccessLogSubscriptionResponseTypeDef",
     "UpdateServiceNetworkRequestRequestTypeDef",
-    "UpdateServiceNetworkResponseTypeDef",
     "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
     "UpdateServiceRequestRequestTypeDef",
-    "UpdateServiceResponseTypeDef",
+    "CreateAccessLogSubscriptionResponseTypeDef",
+    "CreateServiceNetworkResponseTypeDef",
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
+    "DeleteTargetGroupResponseTypeDef",
+    "GetAccessLogSubscriptionResponseTypeDef",
+    "GetAuthPolicyResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetServiceNetworkResponseTypeDef",
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "ListAccessLogSubscriptionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutAuthPolicyResponseTypeDef",
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    "UpdateServiceNetworkResponseTypeDef",
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    "UpdateServiceResponseTypeDef",
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
-    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
+    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
+    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
+    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
-    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerRequestRequestTypeDef",
     "UpdateListenerResponseTypeDef",
+    "CreateListenerRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
+    "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
+    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
+    "UpdateRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -183,14 +189,25 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "resourceArn": str,
         "resourceId": str,
     },
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
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": str,
         "failureMessage": str,
         "ruleIdentifier": str,
     },
@@ -217,26 +234,14 @@
 class CreateAccessLogSubscriptionRequestRequestTypeDef(
     _RequiredCreateAccessLogSubscriptionRequestRequestTypeDef,
     _OptionalCreateAccessLogSubscriptionRequestRequestTypeDef,
 ):
     pass
 
 
-CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "CreateAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "destinationArn": str,
-        "id": str,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceNetworkRequestRequestTypeDef = TypedDict(
@@ -253,25 +258,14 @@
 class CreateServiceNetworkRequestRequestTypeDef(
     _RequiredCreateServiceNetworkRequestRequestTypeDef,
     _OptionalCreateServiceNetworkRequestRequestTypeDef,
 ):
     pass
 
 
-CreateServiceNetworkResponseTypeDef = TypedDict(
-    "CreateServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
 )
@@ -322,26 +316,14 @@
 class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(
     _RequiredCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
     _OptionalCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -411,76 +393,35 @@
 DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTargetGroupRequestRequestTypeDef = TypedDict(
     "DeleteTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
-DeleteTargetGroupResponseTypeDef = TypedDict(
-    "DeleteTargetGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": TargetGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "id": str,
     },
 )
 _OptionalTargetTypeDef = TypedDict(
@@ -538,46 +479,21 @@
 GetAccessLogSubscriptionRequestRequestTypeDef = TypedDict(
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
     },
 )
 
-GetAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "GetAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "destinationArn": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAuthPolicyRequestRequestTypeDef = TypedDict(
     "GetAuthPolicyRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 
-GetAuthPolicyResponseTypeDef = TypedDict(
-    "GetAuthPolicyResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetListenerRequestRequestTypeDef = TypedDict(
     "GetListenerRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -585,22 +501,14 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "ruleIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -609,63 +517,28 @@
 GetServiceNetworkRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkRequestRequestTypeDef",
     {
         "serviceNetworkIdentifier": str,
     },
 )
 
-GetServiceNetworkResponseTypeDef = TypedDict(
-    "GetServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "createdAt": datetime,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "name": str,
-        "numberOfAssociatedServices": int,
-        "numberOfAssociatedVPCs": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
 GetServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "failureCode": str,
-        "failureMessage": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "securityGroupIds": List[str],
-        "serviceNetworkArn": str,
-        "serviceNetworkId": str,
-        "serviceNetworkName": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "vpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
@@ -690,36 +563,24 @@
     "MatcherTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
 
-_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    {
-        "resourceIdentifier": str,
-    },
-)
-_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
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
-class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
-    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessLogSubscriptionsRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 _OptionalListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -735,36 +596,14 @@
 class ListAccessLogSubscriptionsRequestRequestTypeDef(
     _RequiredListAccessLogSubscriptionsRequestRequestTypeDef,
     _OptionalListAccessLogSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -793,37 +632,14 @@
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
     },
     total=False,
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -853,47 +669,25 @@
         "lastUpdatedAt": datetime,
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
-ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-        "serviceNetworkIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworkServiceAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
     total=False,
 )
 
-ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-        {
-            "serviceNetworkIdentifier": str,
-            "vpcIdentifier": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListServiceNetworkVpcAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceNetworkIdentifier": str,
         "vpcIdentifier": str,
@@ -914,22 +708,14 @@
         "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
         "vpcId": str,
     },
     total=False,
 )
 
-ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworksRequestRequestTypeDef = TypedDict(
     "ListServiceNetworksRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -945,22 +731,14 @@
         "name": str,
         "numberOfAssociatedServices": int,
         "numberOfAssociatedVPCs": int,
     },
     total=False,
 )
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -969,32 +747,14 @@
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
-ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    {
-        "targetGroupType": TargetGroupTypeType,
-        "vpcIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTargetGroupsRequestRequestTypeDef = TypedDict(
     "ListTargetGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "targetGroupType": TargetGroupTypeType,
         "vpcIdentifier": str,
@@ -1028,24 +788,14 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
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
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
         "exact": str,
         "prefix": str,
     },
     total=False,
@@ -1055,42 +805,22 @@
     "PutAuthPolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceIdentifier": str,
     },
 )
 
-PutAuthPolicyResponseTypeDef = TypedDict(
-    "PutAuthPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1107,134 +837,295 @@
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
         "destinationArn": str,
     },
 )
 
-UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "UpdateAccessLogSubscriptionResponseTypeDef",
+UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "serviceNetworkIdentifier": str,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+    {
+        "securityGroupIds": Sequence[str],
+        "serviceNetworkVpcAssociationIdentifier": str,
+    },
+)
+
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "certificateArn": str,
+    },
+    total=False,
+)
+
+
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
+
+
+CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "CreateAccessLogSubscriptionResponseTypeDef",
     {
         "arn": str,
         "destinationArn": str,
         "id": str,
         "resourceArn": str,
         "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkRequestRequestTypeDef",
+CreateServiceNetworkResponseTypeDef = TypedDict(
+    "CreateServiceNetworkResponseTypeDef",
     {
+        "arn": str,
         "authType": AuthTypeType,
-        "serviceNetworkIdentifier": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkResponseTypeDef",
+CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "authType": AuthTypeType,
+        "createdBy": str,
         "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "serviceNetworkVpcAssociationIdentifier": str,
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkServiceAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "createdBy": str,
         "id": str,
-        "securityGroupIds": List[str],
         "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
     {
-        "serviceIdentifier": str,
+        "arn": str,
+        "id": str,
+        "name": str,
+        "status": ServiceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
+
+DeleteTargetGroupResponseTypeDef = TypedDict(
+    "DeleteTargetGroupResponseTypeDef",
     {
-        "authType": AuthTypeType,
-        "certificateArn": str,
+        "arn": str,
+        "id": str,
+        "status": TargetGroupStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "GetAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "destinationArn": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
+GetAuthPolicyResponseTypeDef = TypedDict(
+    "GetAuthPolicyResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+GetServiceNetworkResponseTypeDef = TypedDict(
+    "GetServiceNetworkResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
-        "certificateArn": str,
-        "customDomainName": str,
+        "createdAt": datetime,
         "id": str,
+        "lastUpdatedAt": datetime,
         "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "numberOfAssociatedServices": int,
+        "numberOfAssociatedVPCs": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "failureCode": str,
+        "failureMessage": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "securityGroupIds": List[str],
+        "serviceNetworkArn": str,
+        "serviceNetworkId": str,
+        "serviceNetworkName": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "vpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
     "ListAccessLogSubscriptionsResponseTypeDef",
     {
         "items": List[AccessLogSubscriptionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+PutAuthPolicyResponseTypeDef = TypedDict(
+    "PutAuthPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "destinationArn": str,
+        "id": str,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdBy": str,
+        "id": str,
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "certificateArn": str,
+        "customDomainName": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
         "createdBy": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
@@ -1248,15 +1139,15 @@
         "serviceArn": str,
         "serviceId": str,
         "serviceName": str,
         "serviceNetworkArn": str,
         "serviceNetworkId": str,
         "serviceNetworkName": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "arn": str,
@@ -1267,15 +1158,15 @@
         "dnsEntry": DnsEntryTypeDef,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceNetworkServiceAssociationSummaryTypeDef = TypedDict(
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     {
         "arn": str,
@@ -1314,37 +1205,14 @@
     "DeregisterTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
         "targets": Sequence[TargetTypeDef],
     },
 )
 
-_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targets": Sequence[TargetTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTargetsRequestListTargetsPaginateTypeDef(
-    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
-    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalListTargetsRequestRequestTypeDef = TypedDict(
@@ -1373,24 +1241,31 @@
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ForwardActionOutputTypeDef = TypedDict(
+    "ForwardActionOutputTypeDef",
+    {
+        "targetGroups": List[WeightedTargetGroupTypeDef],
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
@@ -1430,65 +1305,203 @@
         "protocol": TargetGroupProtocolType,
         "protocolVersion": HealthCheckProtocolVersionType,
         "unhealthyThresholdCount": int,
     },
     total=False,
 )
 
+_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "resourceIdentifier": str,
+    },
+)
+_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
+    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+
+ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+        "serviceNetworkIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+        {
+            "serviceNetworkIdentifier": str,
+            "vpcIdentifier": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    {
+        "targetGroupType": TargetGroupTypeType,
+        "vpcIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targets": Sequence[TargetTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTargetsRequestListTargetsPaginateTypeDef(
+    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
+    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
+):
+    pass
+
+
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "items": List[ListenerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "items": List[RuleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworkVpcAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkVpcAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworksResponseTypeDef = TypedDict(
     "ListServiceNetworksResponseTypeDef",
     {
         "items": List[ServiceNetworkSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetGroupsResponseTypeDef = TypedDict(
     "ListTargetGroupsResponseTypeDef",
     {
         "items": List[TargetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResponseTypeDef = TypedDict(
     "ListTargetsResponseTypeDef",
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
@@ -1508,27 +1521,36 @@
 
 
 ListServiceNetworkServiceAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkServiceAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "fixedResponse": FixedResponseActionTypeDef,
+        "forward": ForwardActionOutputTypeDef,
+    },
+    total=False,
+)
+
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
     },
     total=False,
@@ -1563,103 +1585,114 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
 
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+HttpMatchOutputTypeDef = TypedDict(
+    "HttpMatchOutputTypeDef",
     {
-        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "headerMatches": List[HeaderMatchTypeDef],
         "method": str,
         "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateListenerRequestRequestTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "clientToken": str,
-        "port": int,
-        "tags": Mapping[str, str],
+        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "method": str,
+        "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-
-class CreateListenerRequestRequestTypeDef(
-    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
-):
-    pass
-
-
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "name": str,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListenerRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "port": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateListenerRequestRequestTypeDef(
+    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
+):
+    pass
+
+
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
     },
 )
 
 _RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
@@ -1688,15 +1721,15 @@
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
@@ -1706,109 +1739,132 @@
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
+RuleMatchOutputTypeDef = TypedDict(
+    "RuleMatchOutputTypeDef",
     {
-        "httpMatch": HttpMatchTypeDef,
+        "httpMatch": HttpMatchOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
     {
-        "clientToken": str,
-        "tags": Mapping[str, str],
+        "httpMatch": HttpMatchTypeDef,
     },
     total=False,
 )
 
-
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
-
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+    },
+    total=False,
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+
+RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
@@ -1847,34 +1903,20 @@
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateRuleRequestRequestTypeDef = TypedDict(
     "BatchUpdateRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice/type_defs.pyi` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_vpc_lattice.type_defs import AccessLogSubscriptionSummaryTypeDef
 
-    data: AccessLogSubscriptionSummaryTypeDef = {...}
+    data: AccessLogSubscriptionSummaryTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     AuthPolicyStateType,
     AuthTypeType,
     HealthCheckProtocolVersionType,
     IpAddressTypeType,
     ListenerProtocolType,
@@ -34,145 +34,151 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccessLogSubscriptionSummaryTypeDef",
+    "ResponseMetadataTypeDef",
     "RuleUpdateFailureTypeDef",
     "CreateAccessLogSubscriptionRequestRequestTypeDef",
-    "CreateAccessLogSubscriptionResponseTypeDef",
     "CreateServiceNetworkRequestRequestTypeDef",
-    "CreateServiceNetworkResponseTypeDef",
     "CreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     "DnsEntryTypeDef",
     "CreateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     "CreateServiceRequestRequestTypeDef",
     "DeleteAccessLogSubscriptionRequestRequestTypeDef",
     "DeleteAuthPolicyRequestRequestTypeDef",
     "DeleteListenerRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteRuleRequestRequestTypeDef",
     "DeleteServiceNetworkRequestRequestTypeDef",
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     "DeleteServiceRequestRequestTypeDef",
-    "DeleteServiceResponseTypeDef",
     "DeleteTargetGroupRequestRequestTypeDef",
-    "DeleteTargetGroupResponseTypeDef",
     "TargetTypeDef",
     "TargetFailureTypeDef",
     "FixedResponseActionTypeDef",
     "WeightedTargetGroupTypeDef",
     "GetAccessLogSubscriptionRequestRequestTypeDef",
-    "GetAccessLogSubscriptionResponseTypeDef",
     "GetAuthPolicyRequestRequestTypeDef",
-    "GetAuthPolicyResponseTypeDef",
     "GetListenerRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRuleRequestRequestTypeDef",
     "GetServiceNetworkRequestRequestTypeDef",
-    "GetServiceNetworkResponseTypeDef",
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "GetServiceRequestRequestTypeDef",
     "GetTargetGroupRequestRequestTypeDef",
     "HeaderMatchTypeTypeDef",
     "MatcherTypeDef",
-    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccessLogSubscriptionsRequestRequestTypeDef",
-    "ListListenersRequestListListenersPaginateTypeDef",
     "ListListenersRequestRequestTypeDef",
     "ListenerSummaryTypeDef",
-    "ListRulesRequestListRulesPaginateTypeDef",
     "ListRulesRequestRequestTypeDef",
     "RuleSummaryTypeDef",
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
-    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     "ServiceNetworkVpcAssociationSummaryTypeDef",
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
     "ListServiceNetworksRequestRequestTypeDef",
     "ServiceNetworkSummaryTypeDef",
-    "ListServicesRequestListServicesPaginateTypeDef",
     "ListServicesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
     "ListTargetGroupsRequestRequestTypeDef",
     "TargetGroupSummaryTypeDef",
     "TargetSummaryTypeDef",
-    "PaginatorConfigTypeDef",
     "PathMatchTypeTypeDef",
     "PutAuthPolicyRequestRequestTypeDef",
-    "PutAuthPolicyResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
-    "UpdateAccessLogSubscriptionResponseTypeDef",
     "UpdateServiceNetworkRequestRequestTypeDef",
-    "UpdateServiceNetworkResponseTypeDef",
     "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
     "UpdateServiceRequestRequestTypeDef",
-    "UpdateServiceResponseTypeDef",
+    "CreateAccessLogSubscriptionResponseTypeDef",
+    "CreateServiceNetworkResponseTypeDef",
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
+    "DeleteServiceResponseTypeDef",
+    "DeleteTargetGroupResponseTypeDef",
+    "GetAccessLogSubscriptionResponseTypeDef",
+    "GetAuthPolicyResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetServiceNetworkResponseTypeDef",
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
     "ListAccessLogSubscriptionsResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutAuthPolicyResponseTypeDef",
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    "UpdateServiceNetworkResponseTypeDef",
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    "UpdateServiceResponseTypeDef",
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     "CreateServiceResponseTypeDef",
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     "GetServiceResponseTypeDef",
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     "ServiceSummaryTypeDef",
     "DeregisterTargetsRequestRequestTypeDef",
-    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListTargetsRequestRequestTypeDef",
     "RegisterTargetsRequestRequestTypeDef",
     "DeregisterTargetsResponseTypeDef",
     "RegisterTargetsResponseTypeDef",
+    "ForwardActionOutputTypeDef",
     "ForwardActionTypeDef",
     "HeaderMatchTypeDef",
     "HealthCheckConfigTypeDef",
+    "ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    "ListListenersRequestListListenersPaginateTypeDef",
+    "ListRulesRequestListRulesPaginateTypeDef",
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    "ListServicesRequestListServicesPaginateTypeDef",
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    "ListTargetsRequestListTargetsPaginateTypeDef",
     "ListListenersResponseTypeDef",
     "ListRulesResponseTypeDef",
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     "ListServiceNetworksResponseTypeDef",
     "ListTargetGroupsResponseTypeDef",
     "ListTargetsResponseTypeDef",
     "PathMatchTypeDef",
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     "ListServicesResponseTypeDef",
+    "RuleActionOutputTypeDef",
     "RuleActionTypeDef",
     "TargetGroupConfigTypeDef",
     "UpdateTargetGroupRequestRequestTypeDef",
+    "HttpMatchOutputTypeDef",
     "HttpMatchTypeDef",
-    "CreateListenerRequestRequestTypeDef",
     "CreateListenerResponseTypeDef",
     "GetListenerResponseTypeDef",
-    "UpdateListenerRequestRequestTypeDef",
     "UpdateListenerResponseTypeDef",
+    "CreateListenerRequestRequestTypeDef",
+    "RuleActionUnionTypeDef",
+    "UpdateListenerRequestRequestTypeDef",
     "CreateTargetGroupRequestRequestTypeDef",
     "CreateTargetGroupResponseTypeDef",
     "GetTargetGroupResponseTypeDef",
     "UpdateTargetGroupResponseTypeDef",
+    "RuleMatchOutputTypeDef",
     "RuleMatchTypeDef",
-    "CreateRuleRequestRequestTypeDef",
     "CreateRuleResponseTypeDef",
     "GetRuleResponseTypeDef",
     "RuleUpdateSuccessTypeDef",
+    "UpdateRuleResponseTypeDef",
+    "CreateRuleRequestRequestTypeDef",
+    "RuleMatchUnionTypeDef",
     "RuleUpdateTypeDef",
     "UpdateRuleRequestRequestTypeDef",
-    "UpdateRuleResponseTypeDef",
     "BatchUpdateRuleResponseTypeDef",
     "BatchUpdateRuleRequestRequestTypeDef",
 )
 
 AccessLogSubscriptionSummaryTypeDef = TypedDict(
     "AccessLogSubscriptionSummaryTypeDef",
     {
@@ -182,14 +188,25 @@
         "id": str,
         "lastUpdatedAt": datetime,
         "resourceArn": str,
         "resourceId": str,
     },
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
 RuleUpdateFailureTypeDef = TypedDict(
     "RuleUpdateFailureTypeDef",
     {
         "failureCode": str,
         "failureMessage": str,
         "ruleIdentifier": str,
     },
@@ -214,26 +231,14 @@
 
 class CreateAccessLogSubscriptionRequestRequestTypeDef(
     _RequiredCreateAccessLogSubscriptionRequestRequestTypeDef,
     _OptionalCreateAccessLogSubscriptionRequestRequestTypeDef,
 ):
     pass
 
-CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "CreateAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "destinationArn": str,
-        "id": str,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceNetworkRequestRequestTypeDef = TypedDict(
@@ -248,25 +253,14 @@
 
 class CreateServiceNetworkRequestRequestTypeDef(
     _RequiredCreateServiceNetworkRequestRequestTypeDef,
     _OptionalCreateServiceNetworkRequestRequestTypeDef,
 ):
     pass
 
-CreateServiceNetworkResponseTypeDef = TypedDict(
-    "CreateServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
 )
@@ -313,26 +307,14 @@
 
 class CreateServiceNetworkVpcAssociationRequestRequestTypeDef(
     _RequiredCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
     _OptionalCreateServiceNetworkVpcAssociationRequestRequestTypeDef,
 ):
     pass
 
-CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "CreateServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdBy": str,
-        "id": str,
-        "securityGroupIds": List[str],
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateServiceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateServiceRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 _OptionalCreateServiceRequestRequestTypeDef = TypedDict(
@@ -400,76 +382,35 @@
 DeleteServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "DeleteServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteServiceRequestRequestTypeDef = TypedDict(
     "DeleteServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
-DeleteServiceResponseTypeDef = TypedDict(
-    "DeleteServiceResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "name": str,
-        "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteTargetGroupRequestRequestTypeDef = TypedDict(
     "DeleteTargetGroupRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 
-DeleteTargetGroupResponseTypeDef = TypedDict(
-    "DeleteTargetGroupResponseTypeDef",
-    {
-        "arn": str,
-        "id": str,
-        "status": TargetGroupStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredTargetTypeDef = TypedDict(
     "_RequiredTargetTypeDef",
     {
         "id": str,
     },
 )
 _OptionalTargetTypeDef = TypedDict(
@@ -523,46 +464,21 @@
 GetAccessLogSubscriptionRequestRequestTypeDef = TypedDict(
     "GetAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
     },
 )
 
-GetAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "GetAccessLogSubscriptionResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "destinationArn": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "resourceArn": str,
-        "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetAuthPolicyRequestRequestTypeDef = TypedDict(
     "GetAuthPolicyRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 
-GetAuthPolicyResponseTypeDef = TypedDict(
-    "GetAuthPolicyResponseTypeDef",
-    {
-        "createdAt": datetime,
-        "lastUpdatedAt": datetime,
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetListenerRequestRequestTypeDef = TypedDict(
     "GetListenerRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -570,22 +486,14 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRuleRequestRequestTypeDef = TypedDict(
     "GetRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "ruleIdentifier": str,
         "serviceIdentifier": str,
     },
@@ -594,63 +502,28 @@
 GetServiceNetworkRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkRequestRequestTypeDef",
     {
         "serviceNetworkIdentifier": str,
     },
 )
 
-GetServiceNetworkResponseTypeDef = TypedDict(
-    "GetServiceNetworkResponseTypeDef",
-    {
-        "arn": str,
-        "authType": AuthTypeType,
-        "createdAt": datetime,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "name": str,
-        "numberOfAssociatedServices": int,
-        "numberOfAssociatedVPCs": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceNetworkServiceAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationRequestRequestTypeDef",
     {
         "serviceNetworkServiceAssociationIdentifier": str,
     },
 )
 
 GetServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
     "GetServiceNetworkVpcAssociationRequestRequestTypeDef",
     {
         "serviceNetworkVpcAssociationIdentifier": str,
     },
 )
 
-GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "GetServiceNetworkVpcAssociationResponseTypeDef",
-    {
-        "arn": str,
-        "createdAt": datetime,
-        "createdBy": str,
-        "failureCode": str,
-        "failureMessage": str,
-        "id": str,
-        "lastUpdatedAt": datetime,
-        "securityGroupIds": List[str],
-        "serviceNetworkArn": str,
-        "serviceNetworkId": str,
-        "serviceNetworkName": str,
-        "status": ServiceNetworkVpcAssociationStatusType,
-        "vpcId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetServiceRequestRequestTypeDef = TypedDict(
     "GetServiceRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 
@@ -675,34 +548,24 @@
     "MatcherTypeDef",
     {
         "httpCode": str,
     },
     total=False,
 )
 
-_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
-    {
-        "resourceIdentifier": str,
-    },
-)
-_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
-    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
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
 
-class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
-    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccessLogSubscriptionsRequestRequestTypeDef",
     {
         "resourceIdentifier": str,
     },
 )
 _OptionalListAccessLogSubscriptionsRequestRequestTypeDef = TypedDict(
@@ -716,34 +579,14 @@
 
 class ListAccessLogSubscriptionsRequestRequestTypeDef(
     _RequiredListAccessLogSubscriptionsRequestRequestTypeDef,
     _OptionalListAccessLogSubscriptionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_RequiredListListenersRequestListListenersPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
-    "_OptionalListListenersRequestListListenersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListListenersRequestListListenersPaginateTypeDef(
-    _RequiredListListenersRequestListListenersPaginateTypeDef,
-    _OptionalListListenersRequestListListenersPaginateTypeDef,
-):
-    pass
-
 _RequiredListListenersRequestRequestTypeDef = TypedDict(
     "_RequiredListListenersRequestRequestTypeDef",
     {
         "serviceIdentifier": str,
     },
 )
 _OptionalListListenersRequestRequestTypeDef = TypedDict(
@@ -770,35 +613,14 @@
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
     },
     total=False,
 )
 
-_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_RequiredListRulesRequestListRulesPaginateTypeDef",
-    {
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
-    "_OptionalListRulesRequestListRulesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRulesRequestListRulesPaginateTypeDef(
-    _RequiredListRulesRequestListRulesPaginateTypeDef,
-    _OptionalListRulesRequestListRulesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRulesRequestRequestTypeDef = TypedDict(
     "_RequiredListRulesRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
         "serviceIdentifier": str,
     },
 )
@@ -826,47 +648,25 @@
         "lastUpdatedAt": datetime,
         "name": str,
         "priority": int,
     },
     total=False,
 )
 
-ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
-    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
-    {
-        "serviceIdentifier": str,
-        "serviceNetworkIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworkServiceAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceIdentifier": str,
         "serviceNetworkIdentifier": str,
     },
     total=False,
 )
 
-ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
-    TypedDict(
-        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
-        {
-            "serviceNetworkIdentifier": str,
-            "vpcIdentifier": str,
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
 ListServiceNetworkVpcAssociationsRequestRequestTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "serviceNetworkIdentifier": str,
         "vpcIdentifier": str,
@@ -887,22 +687,14 @@
         "serviceNetworkName": str,
         "status": ServiceNetworkVpcAssociationStatusType,
         "vpcId": str,
     },
     total=False,
 )
 
-ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
-    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServiceNetworksRequestRequestTypeDef = TypedDict(
     "ListServiceNetworksRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -918,22 +710,14 @@
         "name": str,
         "numberOfAssociatedServices": int,
         "numberOfAssociatedVPCs": int,
     },
     total=False,
 )
 
-ListServicesRequestListServicesPaginateTypeDef = TypedDict(
-    "ListServicesRequestListServicesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListServicesRequestRequestTypeDef = TypedDict(
     "ListServicesRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
@@ -942,32 +726,14 @@
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
-ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
-    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
-    {
-        "targetGroupType": TargetGroupTypeType,
-        "vpcIdentifier": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListTargetGroupsRequestRequestTypeDef = TypedDict(
     "ListTargetGroupsRequestRequestTypeDef",
     {
         "maxResults": int,
         "nextToken": str,
         "targetGroupType": TargetGroupTypeType,
         "vpcIdentifier": str,
@@ -1001,24 +767,14 @@
         "port": int,
         "reasonCode": str,
         "status": TargetStatusType,
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
 PathMatchTypeTypeDef = TypedDict(
     "PathMatchTypeTypeDef",
     {
         "exact": str,
         "prefix": str,
     },
     total=False,
@@ -1028,42 +784,22 @@
     "PutAuthPolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceIdentifier": str,
     },
 )
 
-PutAuthPolicyResponseTypeDef = TypedDict(
-    "PutAuthPolicyResponseTypeDef",
-    {
-        "policy": str,
-        "state": AuthPolicyStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "policy": str,
         "resourceArn": str,
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
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -1080,132 +816,293 @@
     "UpdateAccessLogSubscriptionRequestRequestTypeDef",
     {
         "accessLogSubscriptionIdentifier": str,
         "destinationArn": str,
     },
 )
 
-UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
-    "UpdateAccessLogSubscriptionResponseTypeDef",
+UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "serviceNetworkIdentifier": str,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+    {
+        "securityGroupIds": Sequence[str],
+        "serviceNetworkVpcAssociationIdentifier": str,
+    },
+)
+
+_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateServiceRequestRequestTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateServiceRequestRequestTypeDef",
+    {
+        "authType": AuthTypeType,
+        "certificateArn": str,
+    },
+    total=False,
+)
+
+class UpdateServiceRequestRequestTypeDef(
+    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
+):
+    pass
+
+CreateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "CreateAccessLogSubscriptionResponseTypeDef",
     {
         "arn": str,
         "destinationArn": str,
         "id": str,
         "resourceArn": str,
         "resourceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkRequestRequestTypeDef",
+CreateServiceNetworkResponseTypeDef = TypedDict(
+    "CreateServiceNetworkResponseTypeDef",
     {
+        "arn": str,
         "authType": AuthTypeType,
-        "serviceNetworkIdentifier": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkResponseTypeDef",
+CreateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "CreateServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "authType": AuthTypeType,
+        "createdBy": str,
         "id": str,
-        "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationRequestRequestTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationRequestRequestTypeDef",
+DeleteServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkServiceAssociationResponseTypeDef",
     {
-        "securityGroupIds": Sequence[str],
-        "serviceNetworkVpcAssociationIdentifier": str,
+        "arn": str,
+        "id": str,
+        "status": ServiceNetworkServiceAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
-    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+DeleteServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "DeleteServiceNetworkVpcAssociationResponseTypeDef",
     {
         "arn": str,
-        "createdBy": str,
         "id": str,
-        "securityGroupIds": List[str],
         "status": ServiceNetworkVpcAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateServiceRequestRequestTypeDef",
+DeleteServiceResponseTypeDef = TypedDict(
+    "DeleteServiceResponseTypeDef",
     {
-        "serviceIdentifier": str,
+        "arn": str,
+        "id": str,
+        "name": str,
+        "status": ServiceStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateServiceRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateServiceRequestRequestTypeDef",
+
+DeleteTargetGroupResponseTypeDef = TypedDict(
+    "DeleteTargetGroupResponseTypeDef",
     {
-        "authType": AuthTypeType,
-        "certificateArn": str,
+        "arn": str,
+        "id": str,
+        "status": TargetGroupStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateServiceRequestRequestTypeDef(
-    _RequiredUpdateServiceRequestRequestTypeDef, _OptionalUpdateServiceRequestRequestTypeDef
-):
-    pass
+GetAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "GetAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "destinationArn": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateServiceResponseTypeDef = TypedDict(
-    "UpdateServiceResponseTypeDef",
+GetAuthPolicyResponseTypeDef = TypedDict(
+    "GetAuthPolicyResponseTypeDef",
+    {
+        "createdAt": datetime,
+        "lastUpdatedAt": datetime,
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceNetworkResponseTypeDef = TypedDict(
+    "GetServiceNetworkResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
-        "certificateArn": str,
-        "customDomainName": str,
+        "createdAt": datetime,
         "id": str,
+        "lastUpdatedAt": datetime,
         "name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "numberOfAssociatedServices": int,
+        "numberOfAssociatedVPCs": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "GetServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdAt": datetime,
+        "createdBy": str,
+        "failureCode": str,
+        "failureMessage": str,
+        "id": str,
+        "lastUpdatedAt": datetime,
+        "securityGroupIds": List[str],
+        "serviceNetworkArn": str,
+        "serviceNetworkId": str,
+        "serviceNetworkName": str,
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "vpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAccessLogSubscriptionsResponseTypeDef = TypedDict(
     "ListAccessLogSubscriptionsResponseTypeDef",
     {
         "items": List[AccessLogSubscriptionSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
+PutAuthPolicyResponseTypeDef = TypedDict(
+    "PutAuthPolicyResponseTypeDef",
+    {
+        "policy": str,
+        "state": AuthPolicyStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateAccessLogSubscriptionResponseTypeDef = TypedDict(
+    "UpdateAccessLogSubscriptionResponseTypeDef",
+    {
+        "arn": str,
+        "destinationArn": str,
+        "id": str,
+        "resourceArn": str,
+        "resourceId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceNetworkVpcAssociationResponseTypeDef = TypedDict(
+    "UpdateServiceNetworkVpcAssociationResponseTypeDef",
+    {
+        "arn": str,
+        "createdBy": str,
+        "id": str,
+        "securityGroupIds": List[str],
+        "status": ServiceNetworkVpcAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateServiceResponseTypeDef = TypedDict(
+    "UpdateServiceResponseTypeDef",
+    {
+        "arn": str,
+        "authType": AuthTypeType,
+        "certificateArn": str,
+        "customDomainName": str,
+        "id": str,
+        "name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "CreateServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
         "createdBy": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateServiceResponseTypeDef = TypedDict(
     "CreateServiceResponseTypeDef",
     {
         "arn": str,
         "authType": AuthTypeType,
         "certificateArn": str,
         "customDomainName": str,
         "dnsEntry": DnsEntryTypeDef,
         "id": str,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceNetworkServiceAssociationResponseTypeDef = TypedDict(
     "GetServiceNetworkServiceAssociationResponseTypeDef",
     {
         "arn": str,
@@ -1219,15 +1116,15 @@
         "serviceArn": str,
         "serviceId": str,
         "serviceName": str,
         "serviceNetworkArn": str,
         "serviceNetworkId": str,
         "serviceNetworkName": str,
         "status": ServiceNetworkServiceAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetServiceResponseTypeDef = TypedDict(
     "GetServiceResponseTypeDef",
     {
         "arn": str,
@@ -1238,15 +1135,15 @@
         "dnsEntry": DnsEntryTypeDef,
         "failureCode": str,
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "status": ServiceStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ServiceNetworkServiceAssociationSummaryTypeDef = TypedDict(
     "ServiceNetworkServiceAssociationSummaryTypeDef",
     {
         "arn": str,
@@ -1285,35 +1182,14 @@
     "DeregisterTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
         "targets": Sequence[TargetTypeDef],
     },
 )
 
-_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targetGroupIdentifier": str,
-    },
-)
-_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
-    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
-    {
-        "targets": Sequence[TargetTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTargetsRequestListTargetsPaginateTypeDef(
-    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
-    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTargetsRequestRequestTypeDef = TypedDict(
     "_RequiredListTargetsRequestRequestTypeDef",
     {
         "targetGroupIdentifier": str,
     },
 )
 _OptionalListTargetsRequestRequestTypeDef = TypedDict(
@@ -1340,24 +1216,31 @@
 )
 
 DeregisterTargetsResponseTypeDef = TypedDict(
     "DeregisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTargetsResponseTypeDef = TypedDict(
     "RegisterTargetsResponseTypeDef",
     {
         "successful": List[TargetTypeDef],
         "unsuccessful": List[TargetFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ForwardActionOutputTypeDef = TypedDict(
+    "ForwardActionOutputTypeDef",
+    {
+        "targetGroups": List[WeightedTargetGroupTypeDef],
     },
 )
 
 ForwardActionTypeDef = TypedDict(
     "ForwardActionTypeDef",
     {
         "targetGroups": Sequence[WeightedTargetGroupTypeDef],
@@ -1395,65 +1278,195 @@
         "protocol": TargetGroupProtocolType,
         "protocolVersion": HealthCheckProtocolVersionType,
         "unhealthyThresholdCount": int,
     },
     total=False,
 )
 
+_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "resourceIdentifier": str,
+    },
+)
+_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef = TypedDict(
+    "_OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef(
+    _RequiredListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    _OptionalListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_RequiredListListenersRequestListListenersPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListListenersRequestListListenersPaginateTypeDef = TypedDict(
+    "_OptionalListListenersRequestListListenersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListListenersRequestListListenersPaginateTypeDef(
+    _RequiredListListenersRequestListListenersPaginateTypeDef,
+    _OptionalListListenersRequestListListenersPaginateTypeDef,
+):
+    pass
+
+_RequiredListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_RequiredListRulesRequestListRulesPaginateTypeDef",
+    {
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalListRulesRequestListRulesPaginateTypeDef = TypedDict(
+    "_OptionalListRulesRequestListRulesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRulesRequestListRulesPaginateTypeDef(
+    _RequiredListRulesRequestListRulesPaginateTypeDef,
+    _OptionalListRulesRequestListRulesPaginateTypeDef,
+):
+    pass
+
+ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef = TypedDict(
+    "ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef",
+    {
+        "serviceIdentifier": str,
+        "serviceNetworkIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef = (
+    TypedDict(
+        "ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef",
+        {
+            "serviceNetworkIdentifier": str,
+            "vpcIdentifier": str,
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+ListServiceNetworksRequestListServiceNetworksPaginateTypeDef = TypedDict(
+    "ListServiceNetworksRequestListServiceNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListServicesRequestListServicesPaginateTypeDef = TypedDict(
+    "ListServicesRequestListServicesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListTargetGroupsRequestListTargetGroupsPaginateTypeDef = TypedDict(
+    "ListTargetGroupsRequestListTargetGroupsPaginateTypeDef",
+    {
+        "targetGroupType": TargetGroupTypeType,
+        "vpcIdentifier": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_RequiredListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targetGroupIdentifier": str,
+    },
+)
+_OptionalListTargetsRequestListTargetsPaginateTypeDef = TypedDict(
+    "_OptionalListTargetsRequestListTargetsPaginateTypeDef",
+    {
+        "targets": Sequence[TargetTypeDef],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTargetsRequestListTargetsPaginateTypeDef(
+    _RequiredListTargetsRequestListTargetsPaginateTypeDef,
+    _OptionalListTargetsRequestListTargetsPaginateTypeDef,
+):
+    pass
+
 ListListenersResponseTypeDef = TypedDict(
     "ListListenersResponseTypeDef",
     {
         "items": List[ListenerSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRulesResponseTypeDef = TypedDict(
     "ListRulesResponseTypeDef",
     {
         "items": List[RuleSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworkVpcAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkVpcAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkVpcAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServiceNetworksResponseTypeDef = TypedDict(
     "ListServiceNetworksResponseTypeDef",
     {
         "items": List[ServiceNetworkSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetGroupsResponseTypeDef = TypedDict(
     "ListTargetGroupsResponseTypeDef",
     {
         "items": List[TargetGroupSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTargetsResponseTypeDef = TypedDict(
     "ListTargetsResponseTypeDef",
     {
         "items": List[TargetSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredPathMatchTypeDef = TypedDict(
     "_RequiredPathMatchTypeDef",
     {
         "match": PathMatchTypeTypeDef,
@@ -1471,25 +1484,34 @@
     pass
 
 ListServiceNetworkServiceAssociationsResponseTypeDef = TypedDict(
     "ListServiceNetworkServiceAssociationsResponseTypeDef",
     {
         "items": List[ServiceNetworkServiceAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListServicesResponseTypeDef = TypedDict(
     "ListServicesResponseTypeDef",
     {
         "items": List[ServiceSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RuleActionOutputTypeDef = TypedDict(
+    "RuleActionOutputTypeDef",
+    {
+        "fixedResponse": FixedResponseActionTypeDef,
+        "forward": ForwardActionOutputTypeDef,
     },
+    total=False,
 )
 
 RuleActionTypeDef = TypedDict(
     "RuleActionTypeDef",
     {
         "fixedResponse": FixedResponseActionTypeDef,
         "forward": ForwardActionTypeDef,
@@ -1524,101 +1546,112 @@
     "UpdateTargetGroupRequestRequestTypeDef",
     {
         "healthCheck": HealthCheckConfigTypeDef,
         "targetGroupIdentifier": str,
     },
 )
 
-HttpMatchTypeDef = TypedDict(
-    "HttpMatchTypeDef",
+HttpMatchOutputTypeDef = TypedDict(
+    "HttpMatchOutputTypeDef",
     {
-        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "headerMatches": List[HeaderMatchTypeDef],
         "method": str,
         "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "name": str,
-        "protocol": ListenerProtocolType,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateListenerRequestRequestTypeDef",
+HttpMatchTypeDef = TypedDict(
+    "HttpMatchTypeDef",
     {
-        "clientToken": str,
-        "port": int,
-        "tags": Mapping[str, str],
+        "headerMatches": Sequence[HeaderMatchTypeDef],
+        "method": str,
+        "pathMatch": PathMatchTypeDef,
     },
     total=False,
 )
 
-class CreateListenerRequestRequestTypeDef(
-    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
-):
-    pass
-
 CreateListenerResponseTypeDef = TypedDict(
     "CreateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetListenerResponseTypeDef = TypedDict(
     "GetListenerResponseTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UpdateListenerRequestRequestTypeDef = TypedDict(
-    "UpdateListenerRequestRequestTypeDef",
-    {
-        "defaultAction": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "serviceIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateListenerResponseTypeDef = TypedDict(
     "UpdateListenerResponseTypeDef",
     {
         "arn": str,
-        "defaultAction": RuleActionTypeDef,
+        "defaultAction": RuleActionOutputTypeDef,
         "id": str,
         "name": str,
         "port": int,
         "protocol": ListenerProtocolType,
         "serviceArn": str,
         "serviceId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateListenerRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "name": str,
+        "protocol": ListenerProtocolType,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateListenerRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateListenerRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "port": int,
+        "tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateListenerRequestRequestTypeDef(
+    _RequiredCreateListenerRequestRequestTypeDef, _OptionalCreateListenerRequestRequestTypeDef
+):
+    pass
+
+RuleActionUnionTypeDef = Union[RuleActionTypeDef, RuleActionOutputTypeDef]
+UpdateListenerRequestRequestTypeDef = TypedDict(
+    "UpdateListenerRequestRequestTypeDef",
+    {
+        "defaultAction": RuleActionTypeDef,
+        "listenerIdentifier": str,
+        "serviceIdentifier": str,
     },
 )
 
 _RequiredCreateTargetGroupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTargetGroupRequestRequestTypeDef",
     {
         "name": str,
@@ -1645,15 +1678,15 @@
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTargetGroupResponseTypeDef = TypedDict(
     "GetTargetGroupResponseTypeDef",
     {
         "arn": str,
@@ -1663,107 +1696,130 @@
         "failureMessage": str,
         "id": str,
         "lastUpdatedAt": datetime,
         "name": str,
         "serviceArns": List[str],
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTargetGroupResponseTypeDef = TypedDict(
     "UpdateTargetGroupResponseTypeDef",
     {
         "arn": str,
         "config": TargetGroupConfigTypeDef,
         "id": str,
         "name": str,
         "status": TargetGroupStatusType,
         "type": TargetGroupTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RuleMatchTypeDef = TypedDict(
-    "RuleMatchTypeDef",
+RuleMatchOutputTypeDef = TypedDict(
+    "RuleMatchOutputTypeDef",
     {
-        "httpMatch": HttpMatchTypeDef,
+        "httpMatch": HttpMatchOutputTypeDef,
     },
     total=False,
 )
 
-_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateRuleRequestRequestTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "listenerIdentifier": str,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "serviceIdentifier": str,
-    },
-)
-_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateRuleRequestRequestTypeDef",
+RuleMatchTypeDef = TypedDict(
+    "RuleMatchTypeDef",
     {
-        "clientToken": str,
-        "tags": Mapping[str, str],
+        "httpMatch": HttpMatchTypeDef,
     },
     total=False,
 )
 
-class CreateRuleRequestRequestTypeDef(
-    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
-):
-    pass
-
 CreateRuleResponseTypeDef = TypedDict(
     "CreateRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRuleResponseTypeDef = TypedDict(
     "GetRuleResponseTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "createdAt": datetime,
         "id": str,
         "isDefault": bool,
         "lastUpdatedAt": datetime,
-        "match": RuleMatchTypeDef,
+        "match": RuleMatchOutputTypeDef,
         "name": str,
         "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RuleUpdateSuccessTypeDef = TypedDict(
     "RuleUpdateSuccessTypeDef",
     {
-        "action": RuleActionTypeDef,
+        "action": RuleActionOutputTypeDef,
         "arn": str,
         "id": str,
         "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+    },
+    total=False,
+)
+
+UpdateRuleResponseTypeDef = TypedDict(
+    "UpdateRuleResponseTypeDef",
+    {
+        "action": RuleActionOutputTypeDef,
+        "arn": str,
+        "id": str,
+        "isDefault": bool,
+        "match": RuleMatchOutputTypeDef,
+        "name": str,
+        "priority": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateRuleRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateRuleRequestRequestTypeDef",
+    {
+        "action": RuleActionTypeDef,
+        "listenerIdentifier": str,
         "match": RuleMatchTypeDef,
         "name": str,
         "priority": int,
+        "serviceIdentifier": str,
+    },
+)
+_OptionalCreateRuleRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateRuleRequestRequestTypeDef",
+    {
+        "clientToken": str,
+        "tags": Mapping[str, str],
     },
     total=False,
 )
 
+class CreateRuleRequestRequestTypeDef(
+    _RequiredCreateRuleRequestRequestTypeDef, _OptionalCreateRuleRequestRequestTypeDef
+):
+    pass
+
+RuleMatchUnionTypeDef = Union[RuleMatchTypeDef, RuleMatchOutputTypeDef]
 _RequiredRuleUpdateTypeDef = TypedDict(
     "_RequiredRuleUpdateTypeDef",
     {
         "ruleIdentifier": str,
     },
 )
 _OptionalRuleUpdateTypeDef = TypedDict(
@@ -1798,34 +1854,20 @@
 )
 
 class UpdateRuleRequestRequestTypeDef(
     _RequiredUpdateRuleRequestRequestTypeDef, _OptionalUpdateRuleRequestRequestTypeDef
 ):
     pass
 
-UpdateRuleResponseTypeDef = TypedDict(
-    "UpdateRuleResponseTypeDef",
-    {
-        "action": RuleActionTypeDef,
-        "arn": str,
-        "id": str,
-        "isDefault": bool,
-        "match": RuleMatchTypeDef,
-        "name": str,
-        "priority": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 BatchUpdateRuleResponseTypeDef = TypedDict(
     "BatchUpdateRuleResponseTypeDef",
     {
         "successful": List[RuleUpdateSuccessTypeDef],
         "unsuccessful": List[RuleUpdateFailureTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateRuleRequestRequestTypeDef = TypedDict(
     "BatchUpdateRuleRequestRequestTypeDef",
     {
         "listenerIdentifier": str,
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-vpc-lattice
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.VPCLattice 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore vpc-lattice type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore vpc-lattice type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-vpc-lattice"></a>
 
 # types-aiobotocore-vpc-lattice
 
 [![PyPI - types-aiobotocore-vpc-lattice](https://img.shields.io/pypi/v/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-vpc-lattice.svg?color=blue)](https://pypi.org/project/types-aiobotocore-vpc-lattice)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-vpc-lattice?color=blue)](https://pypistats.org/packages/types-aiobotocore-vpc-lattice)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-vpc-lattice)](https://pepy.tech/project/types-aiobotocore-vpc-lattice)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.VPCLattice 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/vpc-lattice.html#VPCLattice)
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
 [types-aiobotocore-vpc-lattice docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_vpc_lattice/).
 
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
@@ -354,161 +353,167 @@
 )
 
 
 def check_value(value: AuthPolicyStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_vpc_lattice.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_vpc_lattice.type_defs import (
     AccessLogSubscriptionSummaryTypeDef,
+    ResponseMetadataTypeDef,
     RuleUpdateFailureTypeDef,
     CreateAccessLogSubscriptionRequestRequestTypeDef,
-    CreateAccessLogSubscriptionResponseTypeDef,
     CreateServiceNetworkRequestRequestTypeDef,
-    CreateServiceNetworkResponseTypeDef,
     CreateServiceNetworkServiceAssociationRequestRequestTypeDef,
     DnsEntryTypeDef,
     CreateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    CreateServiceNetworkVpcAssociationResponseTypeDef,
     CreateServiceRequestRequestTypeDef,
     DeleteAccessLogSubscriptionRequestRequestTypeDef,
     DeleteAuthPolicyRequestRequestTypeDef,
     DeleteListenerRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteRuleRequestRequestTypeDef,
     DeleteServiceNetworkRequestRequestTypeDef,
     DeleteServiceNetworkServiceAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkServiceAssociationResponseTypeDef,
     DeleteServiceNetworkVpcAssociationRequestRequestTypeDef,
-    DeleteServiceNetworkVpcAssociationResponseTypeDef,
     DeleteServiceRequestRequestTypeDef,
-    DeleteServiceResponseTypeDef,
     DeleteTargetGroupRequestRequestTypeDef,
-    DeleteTargetGroupResponseTypeDef,
     TargetTypeDef,
     TargetFailureTypeDef,
     FixedResponseActionTypeDef,
     WeightedTargetGroupTypeDef,
     GetAccessLogSubscriptionRequestRequestTypeDef,
-    GetAccessLogSubscriptionResponseTypeDef,
     GetAuthPolicyRequestRequestTypeDef,
-    GetAuthPolicyResponseTypeDef,
     GetListenerRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRuleRequestRequestTypeDef,
     GetServiceNetworkRequestRequestTypeDef,
-    GetServiceNetworkResponseTypeDef,
     GetServiceNetworkServiceAssociationRequestRequestTypeDef,
     GetServiceNetworkVpcAssociationRequestRequestTypeDef,
-    GetServiceNetworkVpcAssociationResponseTypeDef,
     GetServiceRequestRequestTypeDef,
     GetTargetGroupRequestRequestTypeDef,
     HeaderMatchTypeTypeDef,
     MatcherTypeDef,
-    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccessLogSubscriptionsRequestRequestTypeDef,
-    ListListenersRequestListListenersPaginateTypeDef,
     ListListenersRequestRequestTypeDef,
     ListenerSummaryTypeDef,
-    ListRulesRequestListRulesPaginateTypeDef,
     ListRulesRequestRequestTypeDef,
     RuleSummaryTypeDef,
-    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
     ListServiceNetworkServiceAssociationsRequestRequestTypeDef,
-    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
     ListServiceNetworkVpcAssociationsRequestRequestTypeDef,
     ServiceNetworkVpcAssociationSummaryTypeDef,
-    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
     ListServiceNetworksRequestRequestTypeDef,
     ServiceNetworkSummaryTypeDef,
-    ListServicesRequestListServicesPaginateTypeDef,
     ListServicesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
     ListTargetGroupsRequestRequestTypeDef,
     TargetGroupSummaryTypeDef,
     TargetSummaryTypeDef,
-    PaginatorConfigTypeDef,
     PathMatchTypeTypeDef,
     PutAuthPolicyRequestRequestTypeDef,
-    PutAuthPolicyResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAccessLogSubscriptionRequestRequestTypeDef,
-    UpdateAccessLogSubscriptionResponseTypeDef,
     UpdateServiceNetworkRequestRequestTypeDef,
-    UpdateServiceNetworkResponseTypeDef,
     UpdateServiceNetworkVpcAssociationRequestRequestTypeDef,
-    UpdateServiceNetworkVpcAssociationResponseTypeDef,
     UpdateServiceRequestRequestTypeDef,
-    UpdateServiceResponseTypeDef,
+    CreateAccessLogSubscriptionResponseTypeDef,
+    CreateServiceNetworkResponseTypeDef,
+    CreateServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceNetworkServiceAssociationResponseTypeDef,
+    DeleteServiceNetworkVpcAssociationResponseTypeDef,
+    DeleteServiceResponseTypeDef,
+    DeleteTargetGroupResponseTypeDef,
+    GetAccessLogSubscriptionResponseTypeDef,
+    GetAuthPolicyResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetServiceNetworkResponseTypeDef,
+    GetServiceNetworkVpcAssociationResponseTypeDef,
     ListAccessLogSubscriptionsResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutAuthPolicyResponseTypeDef,
+    UpdateAccessLogSubscriptionResponseTypeDef,
+    UpdateServiceNetworkResponseTypeDef,
+    UpdateServiceNetworkVpcAssociationResponseTypeDef,
+    UpdateServiceResponseTypeDef,
     CreateServiceNetworkServiceAssociationResponseTypeDef,
     CreateServiceResponseTypeDef,
     GetServiceNetworkServiceAssociationResponseTypeDef,
     GetServiceResponseTypeDef,
     ServiceNetworkServiceAssociationSummaryTypeDef,
     ServiceSummaryTypeDef,
     DeregisterTargetsRequestRequestTypeDef,
-    ListTargetsRequestListTargetsPaginateTypeDef,
     ListTargetsRequestRequestTypeDef,
     RegisterTargetsRequestRequestTypeDef,
     DeregisterTargetsResponseTypeDef,
     RegisterTargetsResponseTypeDef,
+    ForwardActionOutputTypeDef,
     ForwardActionTypeDef,
     HeaderMatchTypeDef,
     HealthCheckConfigTypeDef,
+    ListAccessLogSubscriptionsRequestListAccessLogSubscriptionsPaginateTypeDef,
+    ListListenersRequestListListenersPaginateTypeDef,
+    ListRulesRequestListRulesPaginateTypeDef,
+    ListServiceNetworkServiceAssociationsRequestListServiceNetworkServiceAssociationsPaginateTypeDef,
+    ListServiceNetworkVpcAssociationsRequestListServiceNetworkVpcAssociationsPaginateTypeDef,
+    ListServiceNetworksRequestListServiceNetworksPaginateTypeDef,
+    ListServicesRequestListServicesPaginateTypeDef,
+    ListTargetGroupsRequestListTargetGroupsPaginateTypeDef,
+    ListTargetsRequestListTargetsPaginateTypeDef,
     ListListenersResponseTypeDef,
     ListRulesResponseTypeDef,
     ListServiceNetworkVpcAssociationsResponseTypeDef,
     ListServiceNetworksResponseTypeDef,
     ListTargetGroupsResponseTypeDef,
     ListTargetsResponseTypeDef,
     PathMatchTypeDef,
     ListServiceNetworkServiceAssociationsResponseTypeDef,
     ListServicesResponseTypeDef,
+    RuleActionOutputTypeDef,
     RuleActionTypeDef,
     TargetGroupConfigTypeDef,
     UpdateTargetGroupRequestRequestTypeDef,
+    HttpMatchOutputTypeDef,
     HttpMatchTypeDef,
-    CreateListenerRequestRequestTypeDef,
     CreateListenerResponseTypeDef,
     GetListenerResponseTypeDef,
-    UpdateListenerRequestRequestTypeDef,
     UpdateListenerResponseTypeDef,
+    CreateListenerRequestRequestTypeDef,
+    RuleActionUnionTypeDef,
+    UpdateListenerRequestRequestTypeDef,
     CreateTargetGroupRequestRequestTypeDef,
     CreateTargetGroupResponseTypeDef,
     GetTargetGroupResponseTypeDef,
     UpdateTargetGroupResponseTypeDef,
+    RuleMatchOutputTypeDef,
     RuleMatchTypeDef,
-    CreateRuleRequestRequestTypeDef,
     CreateRuleResponseTypeDef,
     GetRuleResponseTypeDef,
     RuleUpdateSuccessTypeDef,
+    UpdateRuleResponseTypeDef,
+    CreateRuleRequestRequestTypeDef,
+    RuleMatchUnionTypeDef,
     RuleUpdateTypeDef,
     UpdateRuleRequestRequestTypeDef,
-    UpdateRuleResponseTypeDef,
     BatchUpdateRuleResponseTypeDef,
     BatchUpdateRuleRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSubscriptionSummaryTypeDef:
+def get_value() -> AccessLogSubscriptionSummaryTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-vpc-lattice-2.5.2/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt` & `types-aiobotocore-vpc-lattice-2.5.2.post1/types_aiobotocore_vpc_lattice.egg-info/SOURCES.txt`

 * *Files identical despite different names*


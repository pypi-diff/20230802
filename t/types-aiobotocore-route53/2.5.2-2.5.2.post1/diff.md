# Comparing `tmp/types-aiobotocore-route53-2.5.2.tar.gz` & `tmp/types-aiobotocore-route53-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-2.5.2.tar", last modified: Sat Jul  8 01:44:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
```

## Comparing `types-aiobotocore-route53-2.5.2.tar` & `types-aiobotocore-route53-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.110793 types-aiobotocore-route53-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    23116 2023-07-08 01:44:13.110793 types-aiobotocore-route53-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21551 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:13.110793 types-aiobotocore-route53-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.110793 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    58365 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    58277 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10225 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-07-08 01:39:27.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    61142 2023-07-08 01:39:27.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:25.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-08 01:39:26.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.110793 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    23116 2023-07-08 01:44:12.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 01:44:12.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:12.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:12.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:12.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:44:12.000000 types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21641 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58375 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58287 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13017 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13015 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10219 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63226 2023-08-02 14:48:05.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63155 2023-08-02 14:48:05.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:01.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-08-02 14:48:04.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.521476 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    23159 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:54.000000 types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-2.5.2/LICENSE` & `types-aiobotocore-route53-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/PKG-INFO` & `types-aiobotocore-route53-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53"></a>
 
 # types-aiobotocore-route53
 
 [![PyPI - types-aiobotocore-route53](https://img.shields.io/pypi/v/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53)](https://pepy.tech/project/types-aiobotocore-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [types-aiobotocore-route53 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/).
 
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
@@ -385,31 +384,31 @@
 )
 
 
 def check_value(value: AccountLimitTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
+    ResponseMetadataTypeDef,
     AlarmIdentifierTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
@@ -438,83 +437,76 @@
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
-    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
-    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
     HostedZoneOwnerTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
-    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
-    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
+    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
+    GetHealthCheckCountResponseTypeDef,
+    GetHostedZoneCountResponseTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
+    TestDNSAnswerResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
@@ -550,41 +542,51 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
+    ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
+    HealthCheckConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
-    ChangeTypeDef,
     ListResourceRecordSetsResponseTypeDef,
+    ChangeTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountLimitTypeDef:
+def get_value() -> AccountLimitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-2.5.2/README.md` & `types-aiobotocore-route53-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-route53"></a>
 
 # types-aiobotocore-route53
 
 [![PyPI - types-aiobotocore-route53](https://img.shields.io/pypi/v/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53)](https://pepy.tech/project/types-aiobotocore-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [types-aiobotocore-route53 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/).
 
 See how it helps to find and fix potential bugs:
 
@@ -42,15 +42,15 @@
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
@@ -352,31 +352,31 @@
 )
 
 
 def check_value(value: AccountLimitTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
+    ResponseMetadataTypeDef,
     AlarmIdentifierTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
@@ -405,83 +405,76 @@
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
-    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
-    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
     HostedZoneOwnerTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
-    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
-    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
+    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
+    GetHealthCheckCountResponseTypeDef,
+    GetHostedZoneCountResponseTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
+    TestDNSAnswerResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
@@ -517,41 +510,51 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
+    ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
+    HealthCheckConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
-    ChangeTypeDef,
     ListResourceRecordSetsResponseTypeDef,
+    ChangeTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountLimitTypeDef:
+def get_value() -> AccountLimitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-2.5.2/setup.py` & `types-aiobotocore-route53-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_route53"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore route53 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore route53 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/"
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/__init__.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/__init__.pyi` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/__main__.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Route53 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Route53 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53\nOther"
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

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/client.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     GetHostedZoneResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyResponseTypeDef,
-    HealthCheckConfigTypeDef,
+    HealthCheckConfigUnionTypeDef,
     HostedZoneConfigTypeDef,
     ListCidrBlocksResponseTypeDef,
     ListCidrCollectionsResponseTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListGeoLocationsResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
@@ -303,15 +303,15 @@
         Creates a CIDR collection in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_cidr_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_cidr_collection)
         """
 
     async def create_health_check(
-        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigTypeDef
+        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigUnionTypeDef
     ) -> CreateHealthCheckResponseTypeDef:
         """
         Creates a new health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_health_check)
         """
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/client.pyi` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     GetHostedZoneResponseTypeDef,
     GetQueryLoggingConfigResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     GetReusableDelegationSetResponseTypeDef,
     GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceResponseTypeDef,
     GetTrafficPolicyResponseTypeDef,
-    HealthCheckConfigTypeDef,
+    HealthCheckConfigUnionTypeDef,
     HostedZoneConfigTypeDef,
     ListCidrBlocksResponseTypeDef,
     ListCidrCollectionsResponseTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListGeoLocationsResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
@@ -290,15 +290,15 @@
         """
         Creates a CIDR collection in the current Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_cidr_collection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_cidr_collection)
         """
     async def create_health_check(
-        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigTypeDef
+        self, *, CallerReference: str, HealthCheckConfig: HealthCheckConfigUnionTypeDef
     ) -> CreateHealthCheckResponseTypeDef:
         """
         Creates a new health check.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Client.create_health_check)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/client/#create_health_check)
         """
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/literals.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/literals.pyi` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/paginator.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,105 +80,105 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrblockspaginator)
         """
 
 
 class ListCidrCollectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCidrCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrcollectionspaginator)
         """
 
 
 class ListCidrLocationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrlocationspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCidrLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrlocationspaginator)
         """
 
 
 class ListHealthChecksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhealthcheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhealthcheckspaginator)
         """
 
 
 class ListHostedZonesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhostedzonespaginator)
     """
 
     def paginate(
-        self, *, DelegationSetId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DelegationSetId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhostedzonespaginator)
         """
 
 
 class ListQueryLoggingConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listqueryloggingconfigspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQueryLoggingConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listqueryloggingconfigspaginator)
         """
 
 
 class ListResourceRecordSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listresourcerecordsetspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceRecordSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listresourcerecordsetspaginator)
         """
 
 
@@ -189,13 +189,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/paginator.pyi` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -77,99 +77,99 @@
     """
 
     def paginate(
         self,
         *,
         CollectionId: str,
         LocationName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCidrBlocksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrBlocks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrblockspaginator)
         """
 
 class ListCidrCollectionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrcollectionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCidrCollectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrCollections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrcollectionspaginator)
         """
 
 class ListCidrLocationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrlocationspaginator)
     """
 
     def paginate(
-        self, *, CollectionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CollectionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCidrLocationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListCidrLocations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listcidrlocationspaginator)
         """
 
 class ListHealthChecksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhealthcheckspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHealthChecksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHealthChecks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhealthcheckspaginator)
         """
 
 class ListHostedZonesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhostedzonespaginator)
     """
 
     def paginate(
-        self, *, DelegationSetId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, DelegationSetId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHostedZonesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListHostedZones.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listhostedzonespaginator)
         """
 
 class ListQueryLoggingConfigsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listqueryloggingconfigspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQueryLoggingConfigsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListQueryLoggingConfigs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listqueryloggingconfigspaginator)
         """
 
 class ListResourceRecordSetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listresourcerecordsetspaginator)
     """
 
     def paginate(
-        self, *, HostedZoneId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, HostedZoneId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceRecordSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListResourceRecordSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listresourcerecordsetspaginator)
         """
 
 class ListVPCAssociationAuthorizationsPaginator(AioPaginator):
@@ -179,13 +179,13 @@
     """
 
     def paginate(
         self,
         *,
         HostedZoneId: str,
         MaxResults: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVPCAssociationAuthorizationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53.Paginator.ListVPCAssociationAuthorizations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/paginators/#listvpcassociationauthorizationspaginator)
         """
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/type_defs.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53.type_defs import AccountLimitTypeDef
 
-    data: AccountLimitTypeDef = {...}
+    data: AccountLimitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccountLimitTypeType,
     ChangeActionType,
     ChangeStatusType,
     CidrCollectionChangeActionType,
     CloudWatchRegionType,
@@ -45,19 +45,19 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
+    "ResponseMetadataTypeDef",
     "AlarmIdentifierTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
-    "ChangeCidrCollectionResponseTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
@@ -86,83 +86,76 @@
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
-    "GetCheckerIpRangesResponseTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
-    "GetHealthCheckCountResponseTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     "GetHealthCheckRequestRequestTypeDef",
     "GetHealthCheckStatusRequestRequestTypeDef",
-    "GetHostedZoneCountResponseTypeDef",
     "GetHostedZoneLimitRequestRequestTypeDef",
     "HostedZoneLimitTypeDef",
     "GetHostedZoneRequestRequestTypeDef",
     "GetQueryLoggingConfigRequestRequestTypeDef",
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
     "HostedZoneOwnerTypeDef",
-    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
-    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHealthChecksRequestRequestTypeDef",
     "ListHostedZonesByNameRequestRequestTypeDef",
     "ListHostedZonesByVPCRequestRequestTypeDef",
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListHostedZonesRequestRequestTypeDef",
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListQueryLoggingConfigsRequestRequestTypeDef",
-    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListResourceRecordSetsRequestRequestTypeDef",
     "ListReusableDelegationSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
-    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
-    "TestDNSAnswerResponseTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
-    "GetAccountLimitResponseTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
+    "ChangeCidrCollectionResponseTypeDef",
     "ChangeResourceRecordSetsResponseTypeDef",
     "DeactivateKeySigningKeyResponseTypeDef",
     "DeleteHostedZoneResponseTypeDef",
     "DeleteKeySigningKeyResponseTypeDef",
     "DisableHostedZoneDNSSECResponseTypeDef",
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     "EnableHostedZoneDNSSECResponseTypeDef",
+    "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
+    "GetCheckerIpRangesResponseTypeDef",
+    "GetHealthCheckCountResponseTypeDef",
+    "GetHostedZoneCountResponseTypeDef",
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    "TestDNSAnswerResponseTypeDef",
+    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
@@ -198,31 +191,41 @@
     "ListGeoLocationsResponseTypeDef",
     "GetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     "GetHostedZoneLimitResponseTypeDef",
     "GetReusableDelegationSetLimitResponseTypeDef",
     "HealthCheckObservationTypeDef",
     "HostedZoneTypeDef",
     "HostedZoneSummaryTypeDef",
+    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
+    "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
+    "HealthCheckConfigUnionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
-    "ChangeTypeDef",
     "ListResourceRecordSetsResponseTypeDef",
+    "ChangeTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -260,14 +263,25 @@
 )
 
 
 class ChangeInfoTypeDef(_RequiredChangeInfoTypeDef, _OptionalChangeInfoTypeDef):
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
+
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
@@ -295,22 +309,14 @@
     {
         "LocationName": str,
         "Action": CidrCollectionChangeActionType,
         "CidrList": Sequence[str],
     },
 )
 
-ChangeCidrCollectionResponseTypeDef = TypedDict(
-    "ChangeCidrCollectionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -699,22 +705,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-GetCheckerIpRangesResponseTypeDef = TypedDict(
-    "GetCheckerIpRangesResponseTypeDef",
-    {
-        "CheckerIpRanges": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDNSSECRequestRequestTypeDef = TypedDict(
     "GetDNSSECRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 
@@ -724,22 +722,14 @@
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
     total=False,
 )
 
-GetHealthCheckCountResponseTypeDef = TypedDict(
-    "GetHealthCheckCountResponseTypeDef",
-    {
-        "HealthCheckCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHealthCheckLastFailureReasonRequestRequestTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
@@ -753,22 +743,14 @@
 GetHealthCheckStatusRequestRequestTypeDef = TypedDict(
     "GetHealthCheckStatusRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
-GetHostedZoneCountResponseTypeDef = TypedDict(
-    "GetHostedZoneCountResponseTypeDef",
-    {
-        "HostedZoneCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHostedZoneLimitRequestRequestTypeDef = TypedDict(
     "GetHostedZoneLimitRequestRequestTypeDef",
     {
         "Type": HostedZoneLimitTypeType,
         "HostedZoneId": str,
     },
 )
@@ -814,22 +796,14 @@
 GetReusableDelegationSetRequestRequestTypeDef = TypedDict(
     "GetReusableDelegationSetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    {
-        "TrafficPolicyInstanceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrafficPolicyInstanceRequestRequestTypeDef = TypedDict(
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -864,37 +838,24 @@
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
 )
 
-_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LocationName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
-    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCidrBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrBlocksRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrBlocksRequestRequestTypeDef = TypedDict(
@@ -910,53 +871,23 @@
 
 class ListCidrBlocksRequestRequestTypeDef(
     _RequiredListCidrBlocksRequestRequestTypeDef, _OptionalListCidrBlocksRequestRequestTypeDef
 ):
     pass
 
 
-ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCidrCollectionsRequestRequestTypeDef = TypedDict(
     "ListCidrCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
-    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCidrLocationsRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrLocationsRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrLocationsRequestRequestTypeDef = TypedDict(
@@ -990,22 +921,14 @@
         "StartCountryCode": str,
         "StartSubdivisionCode": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHealthChecksRequestRequestTypeDef = TypedDict(
     "ListHealthChecksRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1041,74 +964,34 @@
 class ListHostedZonesByVPCRequestRequestTypeDef(
     _RequiredListHostedZonesByVPCRequestRequestTypeDef,
     _OptionalListHostedZonesByVPCRequestRequestTypeDef,
 ):
     pass
 
 
-ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    {
-        "DelegationSetId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHostedZonesRequestRequestTypeDef = TypedDict(
     "ListHostedZonesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "DelegationSetId": str,
     },
     total=False,
 )
 
-ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryLoggingConfigsRequestRequestTypeDef = TypedDict(
     "ListQueryLoggingConfigsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
-    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceRecordSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceRecordSetsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListResourceRecordSetsRequestRequestTypeDef = TypedDict(
@@ -1255,37 +1138,14 @@
 class ListTrafficPolicyVersionsRequestRequestTypeDef(
     _RequiredListTrafficPolicyVersionsRequestRequestTypeDef,
     _OptionalListTrafficPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "MaxResults": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
-    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -1301,42 +1161,21 @@
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
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
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
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
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
         "RecordType": RRTypeType,
     },
@@ -1354,27 +1193,14 @@
 
 class TestDNSAnswerRequestRequestTypeDef(
     _RequiredTestDNSAnswerRequestRequestTypeDef, _OptionalTestDNSAnswerRequestRequestTypeDef
 ):
     pass
 
 
-TestDNSAnswerResponseTypeDef = TypedDict(
-    "TestDNSAnswerResponseTypeDef",
-    {
-        "Nameserver": str,
-        "RecordName": str,
-        "RecordType": RRTypeType,
-        "RecordData": List[str],
-        "ResponseCode": str,
-        "Protocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHostedZoneCommentRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
@@ -1408,103 +1234,193 @@
         "Id": str,
         "TTL": int,
         "TrafficPolicyId": str,
         "TrafficPolicyVersion": int,
     },
 )
 
-GetAccountLimitResponseTypeDef = TypedDict(
-    "GetAccountLimitResponseTypeDef",
-    {
-        "Limit": AccountLimitTypeDef,
-        "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateKeySigningKeyResponseTypeDef = TypedDict(
     "ActivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateVPCWithHostedZoneResponseTypeDef = TypedDict(
     "AssociateVPCWithHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChangeCidrCollectionResponseTypeDef = TypedDict(
+    "ChangeCidrCollectionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeResourceRecordSetsResponseTypeDef = TypedDict(
     "ChangeResourceRecordSetsResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeactivateKeySigningKeyResponseTypeDef = TypedDict(
     "DeactivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteHostedZoneResponseTypeDef = TypedDict(
     "DeleteHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeySigningKeyResponseTypeDef = TypedDict(
     "DeleteKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "DisableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateVPCFromHostedZoneResponseTypeDef = TypedDict(
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "EnableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountLimitResponseTypeDef = TypedDict(
+    "GetAccountLimitResponseTypeDef",
+    {
+        "Limit": AccountLimitTypeDef,
+        "Count": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChangeResponseTypeDef = TypedDict(
     "GetChangeResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetCheckerIpRangesResponseTypeDef = TypedDict(
+    "GetCheckerIpRangesResponseTypeDef",
+    {
+        "CheckerIpRanges": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHealthCheckCountResponseTypeDef = TypedDict(
+    "GetHealthCheckCountResponseTypeDef",
+    {
+        "HealthCheckCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHostedZoneCountResponseTypeDef = TypedDict(
+    "GetHostedZoneCountResponseTypeDef",
+    {
+        "HostedZoneCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    {
+        "TrafficPolicyInstanceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestDNSAnswerResponseTypeDef = TypedDict(
+    "TestDNSAnswerResponseTypeDef",
+    {
+        "Nameserver": str,
+        "RecordName": str,
+        "RecordType": RRTypeType,
+        "RecordData": List[str],
+        "ResponseCode": str,
+        "Protocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckConfigOutputTypeDef",
+    {
+        "Type": HealthCheckTypeType,
+    },
+)
+_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckConfigOutputTypeDef",
+    {
+        "IPAddress": str,
+        "Port": int,
+        "ResourcePath": str,
+        "FullyQualifiedDomainName": str,
+        "SearchString": str,
+        "RequestInterval": int,
+        "FailureThreshold": int,
+        "MeasureLatency": bool,
+        "Inverted": bool,
+        "Disabled": bool,
+        "HealthThreshold": int,
+        "ChildHealthChecks": List[str],
+        "EnableSNI": bool,
+        "Regions": List[HealthCheckRegionType],
+        "AlarmIdentifier": AlarmIdentifierTypeDef,
+        "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
+        "RoutingControlArn": str,
+    },
+    total=False,
+)
+
+
+class HealthCheckConfigOutputTypeDef(
+    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
     },
 )
 _OptionalHealthCheckConfigTypeDef = TypedDict(
@@ -1606,15 +1522,15 @@
 )
 
 CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
@@ -1647,15 +1563,15 @@
 
 ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
     "ListVPCAssociationAuthorizationsResponseTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
@@ -1713,24 +1629,24 @@
 )
 
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCidrCollectionResponseTypeDef = TypedDict(
     "CreateCidrCollectionResponseTypeDef",
     {
         "Collection": CidrCollectionTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCloudWatchAlarmConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmConfigurationTypeDef",
     {
         "EvaluationPeriods": int,
@@ -1758,15 +1674,15 @@
 
 
 ListCidrCollectionsResponseTypeDef = TypedDict(
     "ListCidrCollectionsResponseTypeDef",
     {
         "NextToken": str,
         "CidrCollections": List[CollectionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostedZoneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHostedZoneRequestRequestTypeDef",
     {
         "Name": str,
@@ -1791,209 +1707,209 @@
 
 
 CreateReusableDelegationSetResponseTypeDef = TypedDict(
     "CreateReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetResponseTypeDef = TypedDict(
     "GetReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReusableDelegationSetsResponseTypeDef = TypedDict(
     "ListReusableDelegationSetsResponseTypeDef",
     {
         "DelegationSets": List[DelegationSetTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQueryLoggingConfigResponseTypeDef = TypedDict(
     "CreateQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryLoggingConfigResponseTypeDef = TypedDict(
     "GetQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueryLoggingConfigsResponseTypeDef = TypedDict(
     "ListQueryLoggingConfigsResponseTypeDef",
     {
         "QueryLoggingConfigs": List[QueryLoggingConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "CreateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "GetTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByHostedZoneResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByPolicyResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByPolicyResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyResponseTypeDef = TypedDict(
     "CreateTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyVersionResponseTypeDef = TypedDict(
     "CreateTrafficPolicyVersionResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyResponseTypeDef = TypedDict(
     "GetTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyVersionsResponseTypeDef = TypedDict(
     "ListTrafficPolicyVersionsResponseTypeDef",
     {
         "TrafficPolicies": List[TrafficPolicyTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyVersionMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyCommentResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyCommentResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDNSSECResponseTypeDef = TypedDict(
     "GetDNSSECResponseTypeDef",
     {
         "Status": DNSSECStatusTypeDef,
         "KeySigningKeys": List[KeySigningKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoLocationResponseTypeDef = TypedDict(
     "GetGeoLocationResponseTypeDef",
     {
         "GeoLocationDetails": GeoLocationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeoLocationsResponseTypeDef = TypedDict(
     "ListGeoLocationsResponseTypeDef",
     {
         "GeoLocationDetailsList": List[GeoLocationDetailsTypeDef],
         "IsTruncated": bool,
         "NextContinentCode": str,
         "NextCountryCode": str,
         "NextSubdivisionCode": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef = TypedDict(
     "_RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     {
         "Id": str,
@@ -2016,24 +1932,24 @@
 
 
 GetHostedZoneLimitResponseTypeDef = TypedDict(
     "GetHostedZoneLimitResponseTypeDef",
     {
         "Limit": HostedZoneLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetLimitResponseTypeDef = TypedDict(
     "GetReusableDelegationSetLimitResponseTypeDef",
     {
         "Limit": ReusableDelegationSetLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HealthCheckObservationTypeDef = TypedDict(
     "HealthCheckObservationTypeDef",
     {
         "Region": HealthCheckRegionType,
@@ -2071,34 +1987,191 @@
     {
         "HostedZoneId": str,
         "Name": str,
         "Owner": HostedZoneOwnerTypeDef,
     },
 )
 
+_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "LocationName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
+    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+):
+    pass
+
+
+ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
+    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+):
+    pass
+
+
+ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    {
+        "DelegationSetId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
+    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "MaxResults": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
+    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+):
+    pass
+
+
 ListCidrLocationsResponseTypeDef = TypedDict(
     "ListCidrLocationsResponseTypeDef",
     {
         "NextToken": str,
         "CidrLocations": List[LocationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPoliciesResponseTypeDef = TypedDict(
     "ListTrafficPoliciesResponseTypeDef",
     {
         "TrafficPolicySummaries": List[TrafficPolicySummaryTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredResourceRecordSetOutputTypeDef = TypedDict(
+    "_RequiredResourceRecordSetOutputTypeDef",
+    {
+        "Name": str,
+        "Type": RRTypeType,
+    },
+)
+_OptionalResourceRecordSetOutputTypeDef = TypedDict(
+    "_OptionalResourceRecordSetOutputTypeDef",
+    {
+        "SetIdentifier": str,
+        "Weight": int,
+        "Region": ResourceRecordSetRegionType,
+        "GeoLocation": GeoLocationTypeDef,
+        "Failover": ResourceRecordSetFailoverType,
+        "MultiValueAnswer": bool,
+        "TTL": int,
+        "ResourceRecords": List[ResourceRecordTypeDef],
+        "AliasTarget": AliasTargetTypeDef,
+        "HealthCheckId": str,
+        "TrafficPolicyInstanceId": str,
+        "CidrRoutingConfig": CidrRoutingConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ResourceRecordSetOutputTypeDef(
+    _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
+):
+    pass
+
+
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
         "Type": RRTypeType,
     },
 )
@@ -2132,36 +2205,37 @@
     "CreateHealthCheckRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
+HealthCheckConfigUnionTypeDef = Union[HealthCheckConfigTypeDef, HealthCheckConfigOutputTypeDef]
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourcesResponseTypeDef = TypedDict(
     "ListTagsForResourcesResponseTypeDef",
     {
         "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
         "HealthCheckVersion": int,
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "LinkedService": LinkedServiceTypeDef,
@@ -2175,147 +2249,147 @@
     pass
 
 
 GetHealthCheckLastFailureReasonResponseTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckStatusResponseTypeDef = TypedDict(
     "GetHealthCheckStatusResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPC": VPCTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "DNSName": str,
         "HostedZoneId": str,
         "IsTruncated": bool,
         "NextDNSName": str,
         "NextHostedZoneId": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesResponseTypeDef = TypedDict(
     "ListHostedZonesResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHostedZoneCommentResponseTypeDef = TypedDict(
     "UpdateHostedZoneCommentResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByVPCResponseTypeDef = TypedDict(
     "ListHostedZonesByVPCResponseTypeDef",
     {
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ChangeTypeDef = TypedDict(
-    "ChangeTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ResourceRecordSet": ResourceRecordSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceRecordSetsResponseTypeDef = TypedDict(
     "ListResourceRecordSetsResponseTypeDef",
     {
-        "ResourceRecordSets": List[ResourceRecordSetTypeDef],
+        "ResourceRecordSets": List[ResourceRecordSetOutputTypeDef],
         "IsTruncated": bool,
         "NextRecordName": str,
         "NextRecordType": RRTypeType,
         "NextRecordIdentifier": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChangeTypeDef = TypedDict(
+    "ChangeTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ResourceRecordSet": ResourceRecordSetTypeDef,
     },
 )
 
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckResponseTypeDef = TypedDict(
     "GetHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHealthChecksResponseTypeDef = TypedDict(
     "ListHealthChecksResponseTypeDef",
     {
         "HealthChecks": List[HealthCheckTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHealthCheckResponseTypeDef = TypedDict(
     "UpdateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChangeBatchTypeDef = TypedDict(
     "_RequiredChangeBatchTypeDef",
     {
         "Changes": Sequence[ChangeTypeDef],
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/type_defs.pyi` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53.type_defs import AccountLimitTypeDef
 
-    data: AccountLimitTypeDef = {...}
+    data: AccountLimitTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     AccountLimitTypeType,
     ChangeActionType,
     ChangeStatusType,
     CidrCollectionChangeActionType,
     CloudWatchRegionType,
@@ -44,19 +44,19 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountLimitTypeDef",
     "ActivateKeySigningKeyRequestRequestTypeDef",
     "ChangeInfoTypeDef",
+    "ResponseMetadataTypeDef",
     "AlarmIdentifierTypeDef",
     "AliasTargetTypeDef",
     "VPCTypeDef",
     "CidrCollectionChangeTypeDef",
-    "ChangeCidrCollectionResponseTypeDef",
     "TagTypeDef",
     "CidrBlockSummaryTypeDef",
     "CidrCollectionTypeDef",
     "CidrRoutingConfigTypeDef",
     "DimensionTypeDef",
     "CollectionSummaryTypeDef",
     "CreateCidrCollectionRequestRequestTypeDef",
@@ -85,83 +85,76 @@
     "DisableHostedZoneDNSSECRequestRequestTypeDef",
     "EnableHostedZoneDNSSECRequestRequestTypeDef",
     "GeoLocationDetailsTypeDef",
     "GeoLocationTypeDef",
     "GetAccountLimitRequestRequestTypeDef",
     "GetChangeRequestRequestTypeDef",
     "WaiterConfigTypeDef",
-    "GetCheckerIpRangesResponseTypeDef",
     "GetDNSSECRequestRequestTypeDef",
     "GetGeoLocationRequestRequestTypeDef",
-    "GetHealthCheckCountResponseTypeDef",
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     "GetHealthCheckRequestRequestTypeDef",
     "GetHealthCheckStatusRequestRequestTypeDef",
-    "GetHostedZoneCountResponseTypeDef",
     "GetHostedZoneLimitRequestRequestTypeDef",
     "HostedZoneLimitTypeDef",
     "GetHostedZoneRequestRequestTypeDef",
     "GetQueryLoggingConfigRequestRequestTypeDef",
     "GetReusableDelegationSetLimitRequestRequestTypeDef",
     "ReusableDelegationSetLimitTypeDef",
     "GetReusableDelegationSetRequestRequestTypeDef",
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     "GetTrafficPolicyRequestRequestTypeDef",
     "StatusReportTypeDef",
     "LinkedServiceTypeDef",
     "HostedZoneOwnerTypeDef",
-    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListCidrBlocksRequestRequestTypeDef",
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
     "ListCidrCollectionsRequestRequestTypeDef",
-    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
     "ListCidrLocationsRequestRequestTypeDef",
     "LocationSummaryTypeDef",
     "ListGeoLocationsRequestRequestTypeDef",
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
     "ListHealthChecksRequestRequestTypeDef",
     "ListHostedZonesByNameRequestRequestTypeDef",
     "ListHostedZonesByVPCRequestRequestTypeDef",
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
     "ListHostedZonesRequestRequestTypeDef",
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
     "ListQueryLoggingConfigsRequestRequestTypeDef",
-    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
     "ListResourceRecordSetsRequestRequestTypeDef",
     "ListReusableDelegationSetsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ListTagsForResourcesRequestRequestTypeDef",
     "ListTrafficPoliciesRequestRequestTypeDef",
     "TrafficPolicySummaryTypeDef",
     "ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef",
     "ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef",
     "ListTrafficPolicyInstancesRequestRequestTypeDef",
     "ListTrafficPolicyVersionsRequestRequestTypeDef",
-    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListVPCAssociationAuthorizationsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "TestDNSAnswerRequestRequestTypeDef",
-    "TestDNSAnswerResponseTypeDef",
     "UpdateHostedZoneCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyCommentRequestRequestTypeDef",
     "UpdateTrafficPolicyInstanceRequestRequestTypeDef",
-    "GetAccountLimitResponseTypeDef",
     "ActivateKeySigningKeyResponseTypeDef",
     "AssociateVPCWithHostedZoneResponseTypeDef",
+    "ChangeCidrCollectionResponseTypeDef",
     "ChangeResourceRecordSetsResponseTypeDef",
     "DeactivateKeySigningKeyResponseTypeDef",
     "DeleteHostedZoneResponseTypeDef",
     "DeleteKeySigningKeyResponseTypeDef",
     "DisableHostedZoneDNSSECResponseTypeDef",
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     "EnableHostedZoneDNSSECResponseTypeDef",
+    "GetAccountLimitResponseTypeDef",
     "GetChangeResponseTypeDef",
+    "GetCheckerIpRangesResponseTypeDef",
+    "GetHealthCheckCountResponseTypeDef",
+    "GetHostedZoneCountResponseTypeDef",
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    "TestDNSAnswerResponseTypeDef",
+    "HealthCheckConfigOutputTypeDef",
     "HealthCheckConfigTypeDef",
     "UpdateHealthCheckRequestRequestTypeDef",
     "AssociateVPCWithHostedZoneRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationRequestRequestTypeDef",
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     "DisassociateVPCFromHostedZoneRequestRequestTypeDef",
@@ -197,31 +190,41 @@
     "ListGeoLocationsResponseTypeDef",
     "GetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     "GetHostedZoneLimitResponseTypeDef",
     "GetReusableDelegationSetLimitResponseTypeDef",
     "HealthCheckObservationTypeDef",
     "HostedZoneTypeDef",
     "HostedZoneSummaryTypeDef",
+    "ListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    "ListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    "ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    "ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
     "ListCidrLocationsResponseTypeDef",
     "ListTrafficPoliciesResponseTypeDef",
+    "ResourceRecordSetOutputTypeDef",
     "ResourceRecordSetTypeDef",
     "CreateHealthCheckRequestRequestTypeDef",
+    "HealthCheckConfigUnionTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "ListTagsForResourcesResponseTypeDef",
     "HealthCheckTypeDef",
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     "GetHealthCheckStatusResponseTypeDef",
     "CreateHostedZoneResponseTypeDef",
     "GetHostedZoneResponseTypeDef",
     "ListHostedZonesByNameResponseTypeDef",
     "ListHostedZonesResponseTypeDef",
     "UpdateHostedZoneCommentResponseTypeDef",
     "ListHostedZonesByVPCResponseTypeDef",
-    "ChangeTypeDef",
     "ListResourceRecordSetsResponseTypeDef",
+    "ChangeTypeDef",
     "CreateHealthCheckResponseTypeDef",
     "GetHealthCheckResponseTypeDef",
     "ListHealthChecksResponseTypeDef",
     "UpdateHealthCheckResponseTypeDef",
     "ChangeBatchTypeDef",
     "ChangeResourceRecordSetsRequestRequestTypeDef",
 )
@@ -257,14 +260,25 @@
     },
     total=False,
 )
 
 class ChangeInfoTypeDef(_RequiredChangeInfoTypeDef, _OptionalChangeInfoTypeDef):
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
+
 AlarmIdentifierTypeDef = TypedDict(
     "AlarmIdentifierTypeDef",
     {
         "Region": CloudWatchRegionType,
         "Name": str,
     },
 )
@@ -292,22 +306,14 @@
     {
         "LocationName": str,
         "Action": CidrCollectionChangeActionType,
         "CidrList": Sequence[str],
     },
 )
 
-ChangeCidrCollectionResponseTypeDef = TypedDict(
-    "ChangeCidrCollectionResponseTypeDef",
-    {
-        "Id": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
     total=False,
@@ -686,22 +692,14 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-GetCheckerIpRangesResponseTypeDef = TypedDict(
-    "GetCheckerIpRangesResponseTypeDef",
-    {
-        "CheckerIpRanges": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDNSSECRequestRequestTypeDef = TypedDict(
     "GetDNSSECRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 
@@ -711,22 +709,14 @@
         "ContinentCode": str,
         "CountryCode": str,
         "SubdivisionCode": str,
     },
     total=False,
 )
 
-GetHealthCheckCountResponseTypeDef = TypedDict(
-    "GetHealthCheckCountResponseTypeDef",
-    {
-        "HealthCheckCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHealthCheckLastFailureReasonRequestRequestTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
@@ -740,22 +730,14 @@
 GetHealthCheckStatusRequestRequestTypeDef = TypedDict(
     "GetHealthCheckStatusRequestRequestTypeDef",
     {
         "HealthCheckId": str,
     },
 )
 
-GetHostedZoneCountResponseTypeDef = TypedDict(
-    "GetHostedZoneCountResponseTypeDef",
-    {
-        "HostedZoneCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetHostedZoneLimitRequestRequestTypeDef = TypedDict(
     "GetHostedZoneLimitRequestRequestTypeDef",
     {
         "Type": HostedZoneLimitTypeType,
         "HostedZoneId": str,
     },
 )
@@ -801,22 +783,14 @@
 GetReusableDelegationSetRequestRequestTypeDef = TypedDict(
     "GetReusableDelegationSetRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
-    "GetTrafficPolicyInstanceCountResponseTypeDef",
-    {
-        "TrafficPolicyInstanceCount": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetTrafficPolicyInstanceRequestRequestTypeDef = TypedDict(
     "GetTrafficPolicyInstanceRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
@@ -851,35 +825,24 @@
     {
         "OwningAccount": str,
         "OwningService": str,
     },
     total=False,
 )
 
-_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
-    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "LocationName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
-    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
-):
-    pass
-
 _RequiredListCidrBlocksRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrBlocksRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrBlocksRequestRequestTypeDef = TypedDict(
@@ -893,51 +856,23 @@
 )
 
 class ListCidrBlocksRequestRequestTypeDef(
     _RequiredListCidrBlocksRequestRequestTypeDef, _OptionalListCidrBlocksRequestRequestTypeDef
 ):
     pass
 
-ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
-    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCidrCollectionsRequestRequestTypeDef = TypedDict(
     "ListCidrCollectionsRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "CollectionId": str,
-    },
-)
-_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
-    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
-    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListCidrLocationsRequestRequestTypeDef = TypedDict(
     "_RequiredListCidrLocationsRequestRequestTypeDef",
     {
         "CollectionId": str,
     },
 )
 _OptionalListCidrLocationsRequestRequestTypeDef = TypedDict(
@@ -969,22 +904,14 @@
         "StartCountryCode": str,
         "StartSubdivisionCode": str,
         "MaxItems": str,
     },
     total=False,
 )
 
-ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
-    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHealthChecksRequestRequestTypeDef = TypedDict(
     "ListHealthChecksRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
     },
     total=False,
@@ -1018,72 +945,34 @@
 
 class ListHostedZonesByVPCRequestRequestTypeDef(
     _RequiredListHostedZonesByVPCRequestRequestTypeDef,
     _OptionalListHostedZonesByVPCRequestRequestTypeDef,
 ):
     pass
 
-ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
-    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
-    {
-        "DelegationSetId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHostedZonesRequestRequestTypeDef = TypedDict(
     "ListHostedZonesRequestRequestTypeDef",
     {
         "Marker": str,
         "MaxItems": str,
         "DelegationSetId": str,
     },
     total=False,
 )
 
-ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
-    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryLoggingConfigsRequestRequestTypeDef = TypedDict(
     "ListQueryLoggingConfigsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "MaxResults": str,
     },
     total=False,
 )
 
-_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
-    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
-    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceRecordSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceRecordSetsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListResourceRecordSetsRequestRequestTypeDef = TypedDict(
@@ -1222,35 +1111,14 @@
 
 class ListTrafficPolicyVersionsRequestRequestTypeDef(
     _RequiredListTrafficPolicyVersionsRequestRequestTypeDef,
     _OptionalListTrafficPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "HostedZoneId": str,
-    },
-)
-_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
-    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
-    {
-        "MaxResults": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
-    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
-):
-    pass
-
 _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
     "_RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef",
     {
         "HostedZoneId": str,
     },
 )
 _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef = TypedDict(
@@ -1264,42 +1132,21 @@
 
 class ListVPCAssociationAuthorizationsRequestRequestTypeDef(
     _RequiredListVPCAssociationAuthorizationsRequestRequestTypeDef,
     _OptionalListVPCAssociationAuthorizationsRequestRequestTypeDef,
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
 ResourceRecordTypeDef = TypedDict(
     "ResourceRecordTypeDef",
     {
         "Value": str,
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
 _RequiredTestDNSAnswerRequestRequestTypeDef = TypedDict(
     "_RequiredTestDNSAnswerRequestRequestTypeDef",
     {
         "HostedZoneId": str,
         "RecordName": str,
         "RecordType": RRTypeType,
     },
@@ -1315,27 +1162,14 @@
 )
 
 class TestDNSAnswerRequestRequestTypeDef(
     _RequiredTestDNSAnswerRequestRequestTypeDef, _OptionalTestDNSAnswerRequestRequestTypeDef
 ):
     pass
 
-TestDNSAnswerResponseTypeDef = TypedDict(
-    "TestDNSAnswerResponseTypeDef",
-    {
-        "Nameserver": str,
-        "RecordName": str,
-        "RecordType": RRTypeType,
-        "RecordData": List[str],
-        "ResponseCode": str,
-        "Protocol": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateHostedZoneCommentRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdateHostedZoneCommentRequestRequestTypeDef = TypedDict(
@@ -1367,102 +1201,190 @@
         "Id": str,
         "TTL": int,
         "TrafficPolicyId": str,
         "TrafficPolicyVersion": int,
     },
 )
 
-GetAccountLimitResponseTypeDef = TypedDict(
-    "GetAccountLimitResponseTypeDef",
-    {
-        "Limit": AccountLimitTypeDef,
-        "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ActivateKeySigningKeyResponseTypeDef = TypedDict(
     "ActivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateVPCWithHostedZoneResponseTypeDef = TypedDict(
     "AssociateVPCWithHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChangeCidrCollectionResponseTypeDef = TypedDict(
+    "ChangeCidrCollectionResponseTypeDef",
+    {
+        "Id": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeResourceRecordSetsResponseTypeDef = TypedDict(
     "ChangeResourceRecordSetsResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeactivateKeySigningKeyResponseTypeDef = TypedDict(
     "DeactivateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteHostedZoneResponseTypeDef = TypedDict(
     "DeleteHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteKeySigningKeyResponseTypeDef = TypedDict(
     "DeleteKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "DisableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateVPCFromHostedZoneResponseTypeDef = TypedDict(
     "DisassociateVPCFromHostedZoneResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 EnableHostedZoneDNSSECResponseTypeDef = TypedDict(
     "EnableHostedZoneDNSSECResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAccountLimitResponseTypeDef = TypedDict(
+    "GetAccountLimitResponseTypeDef",
+    {
+        "Limit": AccountLimitTypeDef,
+        "Count": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetChangeResponseTypeDef = TypedDict(
     "GetChangeResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCheckerIpRangesResponseTypeDef = TypedDict(
+    "GetCheckerIpRangesResponseTypeDef",
+    {
+        "CheckerIpRanges": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHealthCheckCountResponseTypeDef = TypedDict(
+    "GetHealthCheckCountResponseTypeDef",
+    {
+        "HealthCheckCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHostedZoneCountResponseTypeDef = TypedDict(
+    "GetHostedZoneCountResponseTypeDef",
+    {
+        "HostedZoneCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTrafficPolicyInstanceCountResponseTypeDef = TypedDict(
+    "GetTrafficPolicyInstanceCountResponseTypeDef",
+    {
+        "TrafficPolicyInstanceCount": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TestDNSAnswerResponseTypeDef = TypedDict(
+    "TestDNSAnswerResponseTypeDef",
+    {
+        "Nameserver": str,
+        "RecordName": str,
+        "RecordType": RRTypeType,
+        "RecordData": List[str],
+        "ResponseCode": str,
+        "Protocol": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredHealthCheckConfigOutputTypeDef = TypedDict(
+    "_RequiredHealthCheckConfigOutputTypeDef",
+    {
+        "Type": HealthCheckTypeType,
     },
 )
+_OptionalHealthCheckConfigOutputTypeDef = TypedDict(
+    "_OptionalHealthCheckConfigOutputTypeDef",
+    {
+        "IPAddress": str,
+        "Port": int,
+        "ResourcePath": str,
+        "FullyQualifiedDomainName": str,
+        "SearchString": str,
+        "RequestInterval": int,
+        "FailureThreshold": int,
+        "MeasureLatency": bool,
+        "Inverted": bool,
+        "Disabled": bool,
+        "HealthThreshold": int,
+        "ChildHealthChecks": List[str],
+        "EnableSNI": bool,
+        "Regions": List[HealthCheckRegionType],
+        "AlarmIdentifier": AlarmIdentifierTypeDef,
+        "InsufficientDataHealthStatus": InsufficientDataHealthStatusType,
+        "RoutingControlArn": str,
+    },
+    total=False,
+)
+
+class HealthCheckConfigOutputTypeDef(
+    _RequiredHealthCheckConfigOutputTypeDef, _OptionalHealthCheckConfigOutputTypeDef
+):
+    pass
 
 _RequiredHealthCheckConfigTypeDef = TypedDict(
     "_RequiredHealthCheckConfigTypeDef",
     {
         "Type": HealthCheckTypeType,
     },
 )
@@ -1559,15 +1481,15 @@
 )
 
 CreateVPCAssociationAuthorizationResponseTypeDef = TypedDict(
     "CreateVPCAssociationAuthorizationResponseTypeDef",
     {
         "HostedZoneId": str,
         "VPC": VPCTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVPCAssociationAuthorizationRequestRequestTypeDef = TypedDict(
     "DeleteVPCAssociationAuthorizationRequestRequestTypeDef",
     {
         "HostedZoneId": str,
@@ -1598,15 +1520,15 @@
 
 ListVPCAssociationAuthorizationsResponseTypeDef = TypedDict(
     "ListVPCAssociationAuthorizationsResponseTypeDef",
     {
         "HostedZoneId": str,
         "NextToken": str,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChangeCidrCollectionRequestRequestTypeDef = TypedDict(
     "_RequiredChangeCidrCollectionRequestRequestTypeDef",
     {
         "Id": str,
@@ -1660,24 +1582,24 @@
 )
 
 ListCidrBlocksResponseTypeDef = TypedDict(
     "ListCidrBlocksResponseTypeDef",
     {
         "NextToken": str,
         "CidrBlocks": List[CidrBlockSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateCidrCollectionResponseTypeDef = TypedDict(
     "CreateCidrCollectionResponseTypeDef",
     {
         "Collection": CidrCollectionTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCloudWatchAlarmConfigurationTypeDef = TypedDict(
     "_RequiredCloudWatchAlarmConfigurationTypeDef",
     {
         "EvaluationPeriods": int,
@@ -1703,15 +1625,15 @@
     pass
 
 ListCidrCollectionsResponseTypeDef = TypedDict(
     "ListCidrCollectionsResponseTypeDef",
     {
         "NextToken": str,
         "CidrCollections": List[CollectionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateHostedZoneRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHostedZoneRequestRequestTypeDef",
     {
         "Name": str,
@@ -1734,209 +1656,209 @@
     pass
 
 CreateReusableDelegationSetResponseTypeDef = TypedDict(
     "CreateReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetResponseTypeDef = TypedDict(
     "GetReusableDelegationSetResponseTypeDef",
     {
         "DelegationSet": DelegationSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListReusableDelegationSetsResponseTypeDef = TypedDict(
     "ListReusableDelegationSetsResponseTypeDef",
     {
         "DelegationSets": List[DelegationSetTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateKeySigningKeyResponseTypeDef = TypedDict(
     "CreateKeySigningKeyResponseTypeDef",
     {
         "ChangeInfo": ChangeInfoTypeDef,
         "KeySigningKey": KeySigningKeyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateQueryLoggingConfigResponseTypeDef = TypedDict(
     "CreateQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryLoggingConfigResponseTypeDef = TypedDict(
     "GetQueryLoggingConfigResponseTypeDef",
     {
         "QueryLoggingConfig": QueryLoggingConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListQueryLoggingConfigsResponseTypeDef = TypedDict(
     "ListQueryLoggingConfigsResponseTypeDef",
     {
         "QueryLoggingConfigs": List[QueryLoggingConfigTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "CreateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "GetTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByHostedZoneResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByHostedZoneResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesByPolicyResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesByPolicyResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyInstancesResponseTypeDef = TypedDict(
     "ListTrafficPolicyInstancesResponseTypeDef",
     {
         "TrafficPolicyInstances": List[TrafficPolicyInstanceTypeDef],
         "HostedZoneIdMarker": str,
         "TrafficPolicyInstanceNameMarker": str,
         "TrafficPolicyInstanceTypeMarker": RRTypeType,
         "IsTruncated": bool,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyInstanceResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyInstanceResponseTypeDef",
     {
         "TrafficPolicyInstance": TrafficPolicyInstanceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyResponseTypeDef = TypedDict(
     "CreateTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTrafficPolicyVersionResponseTypeDef = TypedDict(
     "CreateTrafficPolicyVersionResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTrafficPolicyResponseTypeDef = TypedDict(
     "GetTrafficPolicyResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPolicyVersionsResponseTypeDef = TypedDict(
     "ListTrafficPolicyVersionsResponseTypeDef",
     {
         "TrafficPolicies": List[TrafficPolicyTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyVersionMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTrafficPolicyCommentResponseTypeDef = TypedDict(
     "UpdateTrafficPolicyCommentResponseTypeDef",
     {
         "TrafficPolicy": TrafficPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDNSSECResponseTypeDef = TypedDict(
     "GetDNSSECResponseTypeDef",
     {
         "Status": DNSSECStatusTypeDef,
         "KeySigningKeys": List[KeySigningKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGeoLocationResponseTypeDef = TypedDict(
     "GetGeoLocationResponseTypeDef",
     {
         "GeoLocationDetails": GeoLocationDetailsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGeoLocationsResponseTypeDef = TypedDict(
     "ListGeoLocationsResponseTypeDef",
     {
         "GeoLocationDetailsList": List[GeoLocationDetailsTypeDef],
         "IsTruncated": bool,
         "NextContinentCode": str,
         "NextCountryCode": str,
         "NextSubdivisionCode": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef = TypedDict(
     "_RequiredGetChangeRequestResourceRecordSetsChangedWaitTypeDef",
     {
         "Id": str,
@@ -1957,24 +1879,24 @@
     pass
 
 GetHostedZoneLimitResponseTypeDef = TypedDict(
     "GetHostedZoneLimitResponseTypeDef",
     {
         "Limit": HostedZoneLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReusableDelegationSetLimitResponseTypeDef = TypedDict(
     "GetReusableDelegationSetLimitResponseTypeDef",
     {
         "Limit": ReusableDelegationSetLimitTypeDef,
         "Count": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HealthCheckObservationTypeDef = TypedDict(
     "HealthCheckObservationTypeDef",
     {
         "Region": HealthCheckRegionType,
@@ -2010,34 +1932,181 @@
     {
         "HostedZoneId": str,
         "Name": str,
         "Owner": HostedZoneOwnerTypeDef,
     },
 )
 
+_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef = TypedDict(
+    "_OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef",
+    {
+        "LocationName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCidrBlocksRequestListCidrBlocksPaginateTypeDef(
+    _RequiredListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    _OptionalListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+):
+    pass
+
+ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef = TypedDict(
+    "ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "CollectionId": str,
+    },
+)
+_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef = TypedDict(
+    "_OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListCidrLocationsRequestListCidrLocationsPaginateTypeDef(
+    _RequiredListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    _OptionalListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+):
+    pass
+
+ListHealthChecksRequestListHealthChecksPaginateTypeDef = TypedDict(
+    "ListHealthChecksRequestListHealthChecksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListHostedZonesRequestListHostedZonesPaginateTypeDef = TypedDict(
+    "ListHostedZonesRequestListHostedZonesPaginateTypeDef",
+    {
+        "DelegationSetId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef = TypedDict(
+    "ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef = TypedDict(
+    "_OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef(
+    _RequiredListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    _OptionalListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+):
+    pass
+
+_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "HostedZoneId": str,
+    },
+)
+_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef = TypedDict(
+    "_OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef",
+    {
+        "MaxResults": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef(
+    _RequiredListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+    _OptionalListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
+):
+    pass
+
 ListCidrLocationsResponseTypeDef = TypedDict(
     "ListCidrLocationsResponseTypeDef",
     {
         "NextToken": str,
         "CidrLocations": List[LocationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTrafficPoliciesResponseTypeDef = TypedDict(
     "ListTrafficPoliciesResponseTypeDef",
     {
         "TrafficPolicySummaries": List[TrafficPolicySummaryTypeDef],
         "IsTruncated": bool,
         "TrafficPolicyIdMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredResourceRecordSetOutputTypeDef = TypedDict(
+    "_RequiredResourceRecordSetOutputTypeDef",
+    {
+        "Name": str,
+        "Type": RRTypeType,
+    },
+)
+_OptionalResourceRecordSetOutputTypeDef = TypedDict(
+    "_OptionalResourceRecordSetOutputTypeDef",
+    {
+        "SetIdentifier": str,
+        "Weight": int,
+        "Region": ResourceRecordSetRegionType,
+        "GeoLocation": GeoLocationTypeDef,
+        "Failover": ResourceRecordSetFailoverType,
+        "MultiValueAnswer": bool,
+        "TTL": int,
+        "ResourceRecords": List[ResourceRecordTypeDef],
+        "AliasTarget": AliasTargetTypeDef,
+        "HealthCheckId": str,
+        "TrafficPolicyInstanceId": str,
+        "CidrRoutingConfig": CidrRoutingConfigTypeDef,
+    },
+    total=False,
+)
+
+class ResourceRecordSetOutputTypeDef(
+    _RequiredResourceRecordSetOutputTypeDef, _OptionalResourceRecordSetOutputTypeDef
+):
+    pass
+
 _RequiredResourceRecordSetTypeDef = TypedDict(
     "_RequiredResourceRecordSetTypeDef",
     {
         "Name": str,
         "Type": RRTypeType,
     },
 )
@@ -2069,36 +2138,37 @@
     "CreateHealthCheckRequestRequestTypeDef",
     {
         "CallerReference": str,
         "HealthCheckConfig": HealthCheckConfigTypeDef,
     },
 )
 
+HealthCheckConfigUnionTypeDef = Union[HealthCheckConfigTypeDef, HealthCheckConfigOutputTypeDef]
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceTagSet": ResourceTagSetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourcesResponseTypeDef = TypedDict(
     "ListTagsForResourcesResponseTypeDef",
     {
         "ResourceTagSets": List[ResourceTagSetTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredHealthCheckTypeDef = TypedDict(
     "_RequiredHealthCheckTypeDef",
     {
         "Id": str,
         "CallerReference": str,
-        "HealthCheckConfig": HealthCheckConfigTypeDef,
+        "HealthCheckConfig": HealthCheckConfigOutputTypeDef,
         "HealthCheckVersion": int,
     },
 )
 _OptionalHealthCheckTypeDef = TypedDict(
     "_OptionalHealthCheckTypeDef",
     {
         "LinkedService": LinkedServiceTypeDef,
@@ -2110,147 +2180,147 @@
 class HealthCheckTypeDef(_RequiredHealthCheckTypeDef, _OptionalHealthCheckTypeDef):
     pass
 
 GetHealthCheckLastFailureReasonResponseTypeDef = TypedDict(
     "GetHealthCheckLastFailureReasonResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckStatusResponseTypeDef = TypedDict(
     "GetHealthCheckStatusResponseTypeDef",
     {
         "HealthCheckObservations": List[HealthCheckObservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateHostedZoneResponseTypeDef = TypedDict(
     "CreateHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "ChangeInfo": ChangeInfoTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPC": VPCTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHostedZoneResponseTypeDef = TypedDict(
     "GetHostedZoneResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
         "DelegationSet": DelegationSetTypeDef,
         "VPCs": List[VPCTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByNameResponseTypeDef = TypedDict(
     "ListHostedZonesByNameResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "DNSName": str,
         "HostedZoneId": str,
         "IsTruncated": bool,
         "NextDNSName": str,
         "NextHostedZoneId": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesResponseTypeDef = TypedDict(
     "ListHostedZonesResponseTypeDef",
     {
         "HostedZones": List[HostedZoneTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHostedZoneCommentResponseTypeDef = TypedDict(
     "UpdateHostedZoneCommentResponseTypeDef",
     {
         "HostedZone": HostedZoneTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHostedZonesByVPCResponseTypeDef = TypedDict(
     "ListHostedZonesByVPCResponseTypeDef",
     {
         "HostedZoneSummaries": List[HostedZoneSummaryTypeDef],
         "MaxItems": str,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ChangeTypeDef = TypedDict(
-    "ChangeTypeDef",
-    {
-        "Action": ChangeActionType,
-        "ResourceRecordSet": ResourceRecordSetTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceRecordSetsResponseTypeDef = TypedDict(
     "ListResourceRecordSetsResponseTypeDef",
     {
-        "ResourceRecordSets": List[ResourceRecordSetTypeDef],
+        "ResourceRecordSets": List[ResourceRecordSetOutputTypeDef],
         "IsTruncated": bool,
         "NextRecordName": str,
         "NextRecordType": RRTypeType,
         "NextRecordIdentifier": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ChangeTypeDef = TypedDict(
+    "ChangeTypeDef",
+    {
+        "Action": ChangeActionType,
+        "ResourceRecordSet": ResourceRecordSetTypeDef,
     },
 )
 
 CreateHealthCheckResponseTypeDef = TypedDict(
     "CreateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
         "Location": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetHealthCheckResponseTypeDef = TypedDict(
     "GetHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListHealthChecksResponseTypeDef = TypedDict(
     "ListHealthChecksResponseTypeDef",
     {
         "HealthChecks": List[HealthCheckTypeDef],
         "Marker": str,
         "IsTruncated": bool,
         "NextMarker": str,
         "MaxItems": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateHealthCheckResponseTypeDef = TypedDict(
     "UpdateHealthCheckResponseTypeDef",
     {
         "HealthCheck": HealthCheckTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredChangeBatchTypeDef = TypedDict(
     "_RequiredChangeBatchTypeDef",
     {
         "Changes": Sequence[ChangeTypeDef],
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/waiter.py` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53/waiter.pyi` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/PKG-INFO` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53"></a>
 
 # types-aiobotocore-route53
 
 [![PyPI - types-aiobotocore-route53](https://img.shields.io/pypi/v/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53)](https://pepy.tech/project/types-aiobotocore-route53)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53.html#Route53)
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
 [types-aiobotocore-route53 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53/).
 
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
@@ -385,31 +384,31 @@
 )
 
 
 def check_value(value: AccountLimitTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_route53.type_defs import (
     AccountLimitTypeDef,
     ActivateKeySigningKeyRequestRequestTypeDef,
     ChangeInfoTypeDef,
+    ResponseMetadataTypeDef,
     AlarmIdentifierTypeDef,
     AliasTargetTypeDef,
     VPCTypeDef,
     CidrCollectionChangeTypeDef,
-    ChangeCidrCollectionResponseTypeDef,
     TagTypeDef,
     CidrBlockSummaryTypeDef,
     CidrCollectionTypeDef,
     CidrRoutingConfigTypeDef,
     DimensionTypeDef,
     CollectionSummaryTypeDef,
     CreateCidrCollectionRequestRequestTypeDef,
@@ -438,83 +437,76 @@
     DisableHostedZoneDNSSECRequestRequestTypeDef,
     EnableHostedZoneDNSSECRequestRequestTypeDef,
     GeoLocationDetailsTypeDef,
     GeoLocationTypeDef,
     GetAccountLimitRequestRequestTypeDef,
     GetChangeRequestRequestTypeDef,
     WaiterConfigTypeDef,
-    GetCheckerIpRangesResponseTypeDef,
     GetDNSSECRequestRequestTypeDef,
     GetGeoLocationRequestRequestTypeDef,
-    GetHealthCheckCountResponseTypeDef,
     GetHealthCheckLastFailureReasonRequestRequestTypeDef,
     GetHealthCheckRequestRequestTypeDef,
     GetHealthCheckStatusRequestRequestTypeDef,
-    GetHostedZoneCountResponseTypeDef,
     GetHostedZoneLimitRequestRequestTypeDef,
     HostedZoneLimitTypeDef,
     GetHostedZoneRequestRequestTypeDef,
     GetQueryLoggingConfigRequestRequestTypeDef,
     GetReusableDelegationSetLimitRequestRequestTypeDef,
     ReusableDelegationSetLimitTypeDef,
     GetReusableDelegationSetRequestRequestTypeDef,
-    GetTrafficPolicyInstanceCountResponseTypeDef,
     GetTrafficPolicyInstanceRequestRequestTypeDef,
     GetTrafficPolicyRequestRequestTypeDef,
     StatusReportTypeDef,
     LinkedServiceTypeDef,
     HostedZoneOwnerTypeDef,
-    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListCidrBlocksRequestRequestTypeDef,
-    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
     ListCidrCollectionsRequestRequestTypeDef,
-    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
     ListCidrLocationsRequestRequestTypeDef,
     LocationSummaryTypeDef,
     ListGeoLocationsRequestRequestTypeDef,
-    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
     ListHealthChecksRequestRequestTypeDef,
     ListHostedZonesByNameRequestRequestTypeDef,
     ListHostedZonesByVPCRequestRequestTypeDef,
-    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
     ListHostedZonesRequestRequestTypeDef,
-    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
     ListQueryLoggingConfigsRequestRequestTypeDef,
-    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
     ListResourceRecordSetsRequestRequestTypeDef,
     ListReusableDelegationSetsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ListTagsForResourcesRequestRequestTypeDef,
     ListTrafficPoliciesRequestRequestTypeDef,
     TrafficPolicySummaryTypeDef,
     ListTrafficPolicyInstancesByHostedZoneRequestRequestTypeDef,
     ListTrafficPolicyInstancesByPolicyRequestRequestTypeDef,
     ListTrafficPolicyInstancesRequestRequestTypeDef,
     ListTrafficPolicyVersionsRequestRequestTypeDef,
-    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListVPCAssociationAuthorizationsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ResourceRecordTypeDef,
-    ResponseMetadataTypeDef,
     TestDNSAnswerRequestRequestTypeDef,
-    TestDNSAnswerResponseTypeDef,
     UpdateHostedZoneCommentRequestRequestTypeDef,
     UpdateTrafficPolicyCommentRequestRequestTypeDef,
     UpdateTrafficPolicyInstanceRequestRequestTypeDef,
-    GetAccountLimitResponseTypeDef,
     ActivateKeySigningKeyResponseTypeDef,
     AssociateVPCWithHostedZoneResponseTypeDef,
+    ChangeCidrCollectionResponseTypeDef,
     ChangeResourceRecordSetsResponseTypeDef,
     DeactivateKeySigningKeyResponseTypeDef,
     DeleteHostedZoneResponseTypeDef,
     DeleteKeySigningKeyResponseTypeDef,
     DisableHostedZoneDNSSECResponseTypeDef,
     DisassociateVPCFromHostedZoneResponseTypeDef,
     EnableHostedZoneDNSSECResponseTypeDef,
+    GetAccountLimitResponseTypeDef,
     GetChangeResponseTypeDef,
+    GetCheckerIpRangesResponseTypeDef,
+    GetHealthCheckCountResponseTypeDef,
+    GetHostedZoneCountResponseTypeDef,
+    GetTrafficPolicyInstanceCountResponseTypeDef,
+    TestDNSAnswerResponseTypeDef,
+    HealthCheckConfigOutputTypeDef,
     HealthCheckConfigTypeDef,
     UpdateHealthCheckRequestRequestTypeDef,
     AssociateVPCWithHostedZoneRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationRequestRequestTypeDef,
     CreateVPCAssociationAuthorizationResponseTypeDef,
     DeleteVPCAssociationAuthorizationRequestRequestTypeDef,
     DisassociateVPCFromHostedZoneRequestRequestTypeDef,
@@ -550,41 +542,51 @@
     ListGeoLocationsResponseTypeDef,
     GetChangeRequestResourceRecordSetsChangedWaitTypeDef,
     GetHostedZoneLimitResponseTypeDef,
     GetReusableDelegationSetLimitResponseTypeDef,
     HealthCheckObservationTypeDef,
     HostedZoneTypeDef,
     HostedZoneSummaryTypeDef,
+    ListCidrBlocksRequestListCidrBlocksPaginateTypeDef,
+    ListCidrCollectionsRequestListCidrCollectionsPaginateTypeDef,
+    ListCidrLocationsRequestListCidrLocationsPaginateTypeDef,
+    ListHealthChecksRequestListHealthChecksPaginateTypeDef,
+    ListHostedZonesRequestListHostedZonesPaginateTypeDef,
+    ListQueryLoggingConfigsRequestListQueryLoggingConfigsPaginateTypeDef,
+    ListResourceRecordSetsRequestListResourceRecordSetsPaginateTypeDef,
+    ListVPCAssociationAuthorizationsRequestListVPCAssociationAuthorizationsPaginateTypeDef,
     ListCidrLocationsResponseTypeDef,
     ListTrafficPoliciesResponseTypeDef,
+    ResourceRecordSetOutputTypeDef,
     ResourceRecordSetTypeDef,
     CreateHealthCheckRequestRequestTypeDef,
+    HealthCheckConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTagsForResourcesResponseTypeDef,
     HealthCheckTypeDef,
     GetHealthCheckLastFailureReasonResponseTypeDef,
     GetHealthCheckStatusResponseTypeDef,
     CreateHostedZoneResponseTypeDef,
     GetHostedZoneResponseTypeDef,
     ListHostedZonesByNameResponseTypeDef,
     ListHostedZonesResponseTypeDef,
     UpdateHostedZoneCommentResponseTypeDef,
     ListHostedZonesByVPCResponseTypeDef,
-    ChangeTypeDef,
     ListResourceRecordSetsResponseTypeDef,
+    ChangeTypeDef,
     CreateHealthCheckResponseTypeDef,
     GetHealthCheckResponseTypeDef,
     ListHealthChecksResponseTypeDef,
     UpdateHealthCheckResponseTypeDef,
     ChangeBatchTypeDef,
     ChangeResourceRecordSetsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccountLimitTypeDef:
+def get_value() -> AccountLimitTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-2.5.2/types_aiobotocore_route53.egg-info/SOURCES.txt` & `types-aiobotocore-route53-2.5.2.post1/types_aiobotocore_route53.egg-info/SOURCES.txt`

 * *Files identical despite different names*


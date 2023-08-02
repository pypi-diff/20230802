# Comparing `tmp/types-aiobotocore-networkmanager-2.5.2.tar.gz` & `tmp/types-aiobotocore-networkmanager-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-networkmanager-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-networkmanager-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
```

## Comparing `types-aiobotocore-networkmanager-2.5.2.tar` & `types-aiobotocore-networkmanager-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.754603 types-aiobotocore-networkmanager-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-07-08 01:44:02.754603 types-aiobotocore-networkmanager-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27226 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.754603 types-aiobotocore-networkmanager-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.734603 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/
--rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73474 2023-07-08 01:35:46.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    73359 2023-07-08 01:35:46.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-07-08 01:35:46.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14631 2023-07-08 01:35:46.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    28579 2023-07-08 01:35:46.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    28555 2023-07-08 01:35:46.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    95886 2023-07-08 01:35:48.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    95769 2023-07-08 01:35:47.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:45.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.754603 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-07-08 01:44:02.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:02.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:02.000000 types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.349511 types-aiobotocore-networkmanager-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-08-02 14:52:43.345512 types-aiobotocore-networkmanager-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    27209 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.349511 types-aiobotocore-networkmanager-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.341512 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73474 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73359 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14633 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14631 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    28537 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28513 2023-08-02 14:44:04.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    95682 2023-08-02 14:44:06.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95565 2023-08-02 14:44:05.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:03.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.345512 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    28755 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:43.000000 types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/LICENSE` & `types-aiobotocore-networkmanager-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/PKG-INFO` & `types-aiobotocore-networkmanager-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-networkmanager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore networkmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore networkmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-networkmanager"></a>
 
 # types-aiobotocore-networkmanager
 
 [![PyPI - types-aiobotocore-networkmanager](https://img.shields.io/pypi/v/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-networkmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-networkmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NetworkManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
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
 [types-aiobotocore-networkmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/).
 
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
@@ -426,25 +425,26 @@
 )
 
 
 def check_value(value: AttachmentStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_networkmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_networkmanager.type_defs import (
     AWSLocationTypeDef,
     AcceptAttachmentRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AccountStatusTypeDef,
     AssociateConnectPeerRequestRequestTypeDef,
     ConnectPeerAssociationTypeDef,
     AssociateCustomerGatewayRequestRequestTypeDef,
     CustomerGatewayAssociationTypeDef,
     AssociateLinkRequestRequestTypeDef,
     LinkAssociationTypeDef,
@@ -473,95 +473,73 @@
     DeleteDeviceRequestRequestTypeDef,
     DeleteGlobalNetworkRequestRequestTypeDef,
     DeleteLinkRequestRequestTypeDef,
     DeletePeeringRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeregisterTransitGatewayRequestRequestTypeDef,
-    DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeGlobalNetworksRequestRequestTypeDef,
     DisassociateConnectPeerRequestRequestTypeDef,
     DisassociateCustomerGatewayRequestRequestTypeDef,
     DisassociateLinkRequestRequestTypeDef,
     DisassociateTransitGatewayConnectPeerRequestRequestTypeDef,
     ExecuteCoreNetworkChangeSetRequestRequestTypeDef,
     GetConnectAttachmentRequestRequestTypeDef,
-    GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
     GetConnectPeerAssociationsRequestRequestTypeDef,
     GetConnectPeerRequestRequestTypeDef,
-    GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
-    GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
     GetCoreNetworkChangeEventsRequestRequestTypeDef,
-    GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
     GetCoreNetworkChangeSetRequestRequestTypeDef,
     GetCoreNetworkPolicyRequestRequestTypeDef,
     GetCoreNetworkRequestRequestTypeDef,
-    GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
     GetCustomerGatewayAssociationsRequestRequestTypeDef,
-    GetDevicesRequestGetDevicesPaginateTypeDef,
     GetDevicesRequestRequestTypeDef,
-    GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
     GetLinkAssociationsRequestRequestTypeDef,
-    GetLinksRequestGetLinksPaginateTypeDef,
     GetLinksRequestRequestTypeDef,
-    GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
     GetNetworkResourceCountsRequestRequestTypeDef,
     NetworkResourceCountTypeDef,
-    GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
     GetNetworkResourceRelationshipsRequestRequestTypeDef,
     RelationshipTypeDef,
-    GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
     GetNetworkResourcesRequestRequestTypeDef,
-    GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
     GetNetworkTelemetryRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteAnalysisRequestRequestTypeDef,
     GetSiteToSiteVpnAttachmentRequestRequestTypeDef,
-    GetSitesRequestGetSitesPaginateTypeDef,
     GetSitesRequestRequestTypeDef,
-    GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
     GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
     GetTransitGatewayPeeringRequestRequestTypeDef,
-    GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
     GetTransitGatewayRegistrationsRequestRequestTypeDef,
     GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
     GetVpcAttachmentRequestRequestTypeDef,
-    ListAttachmentsRequestListAttachmentsPaginateTypeDef,
     ListAttachmentsRequestRequestTypeDef,
-    ListConnectPeersRequestListConnectPeersPaginateTypeDef,
     ListConnectPeersRequestRequestTypeDef,
-    ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
     ListCoreNetworkPolicyVersionsRequestRequestTypeDef,
-    ListCoreNetworksRequestListCoreNetworksPaginateTypeDef,
     ListCoreNetworksRequestRequestTypeDef,
     ListOrganizationServiceAccessStatusRequestRequestTypeDef,
-    ListPeeringsRequestListPeeringsPaginateTypeDef,
     ListPeeringsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NetworkResourceSummaryTypeDef,
     NetworkRouteDestinationTypeDef,
-    PaginatorConfigTypeDef,
     PutCoreNetworkPolicyRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterTransitGatewayRequestRequestTypeDef,
     RejectAttachmentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreCoreNetworkPolicyVersionRequestRequestTypeDef,
     RouteAnalysisCompletionTypeDef,
     RouteAnalysisEndpointOptionsSpecificationTypeDef,
     RouteAnalysisEndpointOptionsTypeDef,
     StartOrganizationServiceAccessUpdateRequestRequestTypeDef,
     TransitGatewayRegistrationStateReasonTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateCoreNetworkRequestRequestTypeDef,
     UpdateGlobalNetworkRequestRequestTypeDef,
     UpdateNetworkResourceMetadataRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     UpdateNetworkResourceMetadataResponseTypeDef,
     OrganizationStatusTypeDef,
     AssociateConnectPeerResponseTypeDef,
     DisassociateConnectPeerResponseTypeDef,
     GetConnectPeerAssociationsResponseTypeDef,
     AssociateCustomerGatewayResponseTypeDef,
     DisassociateCustomerGatewayResponseTypeDef,
@@ -604,14 +582,35 @@
     CreateSiteRequestRequestTypeDef,
     DeviceTypeDef,
     SiteTypeDef,
     UpdateDeviceRequestRequestTypeDef,
     UpdateSiteRequestRequestTypeDef,
     CreateVpcAttachmentRequestRequestTypeDef,
     UpdateVpcAttachmentRequestRequestTypeDef,
+    DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef,
+    GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+    GetConnectionsRequestGetConnectionsPaginateTypeDef,
+    GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+    GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+    GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+    GetDevicesRequestGetDevicesPaginateTypeDef,
+    GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+    GetLinksRequestGetLinksPaginateTypeDef,
+    GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+    GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+    GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+    GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+    GetSitesRequestGetSitesPaginateTypeDef,
+    GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+    GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+    ListAttachmentsRequestListAttachmentsPaginateTypeDef,
+    ListConnectPeersRequestListConnectPeersPaginateTypeDef,
+    ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+    ListCoreNetworksRequestListCoreNetworksPaginateTypeDef,
+    ListPeeringsRequestListPeeringsPaginateTypeDef,
     GetNetworkResourceCountsResponseTypeDef,
     GetNetworkResourceRelationshipsResponseTypeDef,
     PathComponentTypeDef,
     NetworkRouteTypeDef,
     StartRouteAnalysisRequestRequestTypeDef,
     TransitGatewayRegistrationTypeDef,
     ListOrganizationServiceAccessStatusResponseTypeDef,
@@ -685,15 +684,15 @@
     GetVpcAttachmentResponseTypeDef,
     UpdateVpcAttachmentResponseTypeDef,
     GetRouteAnalysisResponseTypeDef,
     StartRouteAnalysisResponseTypeDef,
 )
 
 
-def get_structure() -> AWSLocationTypeDef:
+def get_value() -> AWSLocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/README.md` & `types-aiobotocore-networkmanager-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-networkmanager"></a>
 
 # types-aiobotocore-networkmanager
 
 [![PyPI - types-aiobotocore-networkmanager](https://img.shields.io/pypi/v/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-networkmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-networkmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NetworkManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
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
 [types-aiobotocore-networkmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/).
 
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
@@ -393,25 +393,26 @@
 )
 
 
 def check_value(value: AttachmentStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_networkmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_networkmanager.type_defs import (
     AWSLocationTypeDef,
     AcceptAttachmentRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AccountStatusTypeDef,
     AssociateConnectPeerRequestRequestTypeDef,
     ConnectPeerAssociationTypeDef,
     AssociateCustomerGatewayRequestRequestTypeDef,
     CustomerGatewayAssociationTypeDef,
     AssociateLinkRequestRequestTypeDef,
     LinkAssociationTypeDef,
@@ -440,95 +441,73 @@
     DeleteDeviceRequestRequestTypeDef,
     DeleteGlobalNetworkRequestRequestTypeDef,
     DeleteLinkRequestRequestTypeDef,
     DeletePeeringRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeregisterTransitGatewayRequestRequestTypeDef,
-    DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeGlobalNetworksRequestRequestTypeDef,
     DisassociateConnectPeerRequestRequestTypeDef,
     DisassociateCustomerGatewayRequestRequestTypeDef,
     DisassociateLinkRequestRequestTypeDef,
     DisassociateTransitGatewayConnectPeerRequestRequestTypeDef,
     ExecuteCoreNetworkChangeSetRequestRequestTypeDef,
     GetConnectAttachmentRequestRequestTypeDef,
-    GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
     GetConnectPeerAssociationsRequestRequestTypeDef,
     GetConnectPeerRequestRequestTypeDef,
-    GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
-    GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
     GetCoreNetworkChangeEventsRequestRequestTypeDef,
-    GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
     GetCoreNetworkChangeSetRequestRequestTypeDef,
     GetCoreNetworkPolicyRequestRequestTypeDef,
     GetCoreNetworkRequestRequestTypeDef,
-    GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
     GetCustomerGatewayAssociationsRequestRequestTypeDef,
-    GetDevicesRequestGetDevicesPaginateTypeDef,
     GetDevicesRequestRequestTypeDef,
-    GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
     GetLinkAssociationsRequestRequestTypeDef,
-    GetLinksRequestGetLinksPaginateTypeDef,
     GetLinksRequestRequestTypeDef,
-    GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
     GetNetworkResourceCountsRequestRequestTypeDef,
     NetworkResourceCountTypeDef,
-    GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
     GetNetworkResourceRelationshipsRequestRequestTypeDef,
     RelationshipTypeDef,
-    GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
     GetNetworkResourcesRequestRequestTypeDef,
-    GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
     GetNetworkTelemetryRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteAnalysisRequestRequestTypeDef,
     GetSiteToSiteVpnAttachmentRequestRequestTypeDef,
-    GetSitesRequestGetSitesPaginateTypeDef,
     GetSitesRequestRequestTypeDef,
-    GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
     GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
     GetTransitGatewayPeeringRequestRequestTypeDef,
-    GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
     GetTransitGatewayRegistrationsRequestRequestTypeDef,
     GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
     GetVpcAttachmentRequestRequestTypeDef,
-    ListAttachmentsRequestListAttachmentsPaginateTypeDef,
     ListAttachmentsRequestRequestTypeDef,
-    ListConnectPeersRequestListConnectPeersPaginateTypeDef,
     ListConnectPeersRequestRequestTypeDef,
-    ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
     ListCoreNetworkPolicyVersionsRequestRequestTypeDef,
-    ListCoreNetworksRequestListCoreNetworksPaginateTypeDef,
     ListCoreNetworksRequestRequestTypeDef,
     ListOrganizationServiceAccessStatusRequestRequestTypeDef,
-    ListPeeringsRequestListPeeringsPaginateTypeDef,
     ListPeeringsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NetworkResourceSummaryTypeDef,
     NetworkRouteDestinationTypeDef,
-    PaginatorConfigTypeDef,
     PutCoreNetworkPolicyRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterTransitGatewayRequestRequestTypeDef,
     RejectAttachmentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreCoreNetworkPolicyVersionRequestRequestTypeDef,
     RouteAnalysisCompletionTypeDef,
     RouteAnalysisEndpointOptionsSpecificationTypeDef,
     RouteAnalysisEndpointOptionsTypeDef,
     StartOrganizationServiceAccessUpdateRequestRequestTypeDef,
     TransitGatewayRegistrationStateReasonTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateCoreNetworkRequestRequestTypeDef,
     UpdateGlobalNetworkRequestRequestTypeDef,
     UpdateNetworkResourceMetadataRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     UpdateNetworkResourceMetadataResponseTypeDef,
     OrganizationStatusTypeDef,
     AssociateConnectPeerResponseTypeDef,
     DisassociateConnectPeerResponseTypeDef,
     GetConnectPeerAssociationsResponseTypeDef,
     AssociateCustomerGatewayResponseTypeDef,
     DisassociateCustomerGatewayResponseTypeDef,
@@ -571,14 +550,35 @@
     CreateSiteRequestRequestTypeDef,
     DeviceTypeDef,
     SiteTypeDef,
     UpdateDeviceRequestRequestTypeDef,
     UpdateSiteRequestRequestTypeDef,
     CreateVpcAttachmentRequestRequestTypeDef,
     UpdateVpcAttachmentRequestRequestTypeDef,
+    DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef,
+    GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+    GetConnectionsRequestGetConnectionsPaginateTypeDef,
+    GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+    GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+    GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+    GetDevicesRequestGetDevicesPaginateTypeDef,
+    GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+    GetLinksRequestGetLinksPaginateTypeDef,
+    GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+    GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+    GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+    GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+    GetSitesRequestGetSitesPaginateTypeDef,
+    GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+    GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+    ListAttachmentsRequestListAttachmentsPaginateTypeDef,
+    ListConnectPeersRequestListConnectPeersPaginateTypeDef,
+    ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+    ListCoreNetworksRequestListCoreNetworksPaginateTypeDef,
+    ListPeeringsRequestListPeeringsPaginateTypeDef,
     GetNetworkResourceCountsResponseTypeDef,
     GetNetworkResourceRelationshipsResponseTypeDef,
     PathComponentTypeDef,
     NetworkRouteTypeDef,
     StartRouteAnalysisRequestRequestTypeDef,
     TransitGatewayRegistrationTypeDef,
     ListOrganizationServiceAccessStatusResponseTypeDef,
@@ -652,15 +652,15 @@
     GetVpcAttachmentResponseTypeDef,
     UpdateVpcAttachmentResponseTypeDef,
     GetRouteAnalysisResponseTypeDef,
     StartRouteAnalysisResponseTypeDef,
 )
 
 
-def get_structure() -> AWSLocationTypeDef:
+def get_value() -> AWSLocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/setup.py` & `types-aiobotocore-networkmanager-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-networkmanager",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_networkmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with"
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
-    keywords="aiobotocore networkmanager type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore networkmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_networkmanager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/"
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/__init__.py` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/__init__.pyi` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/__main__.py` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.NetworkManager 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.NetworkManager 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager\nOther"
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

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/client.py` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/client.pyi` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/literals.py` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/literals.pyi` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/paginator.py` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeGlobalNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.DescribeGlobalNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
         """
 
 
@@ -158,15 +158,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectPeerIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectpeerassociationspaginator)
         """
 
 
@@ -178,15 +178,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionIds: Sequence[str] = ...,
         DeviceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectionspaginator)
         """
 
 
@@ -197,15 +197,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCoreNetworkChangeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangeeventspaginator)
         """
 
 
@@ -216,15 +216,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCoreNetworkChangeSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangesetpaginator)
         """
 
 
@@ -235,15 +235,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         CustomerGatewayArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCustomerGatewayAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCustomerGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcustomergatewayassociationspaginator)
         """
 
 
@@ -255,15 +255,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceIds: Sequence[str] = ...,
         SiteId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getdevicespaginator)
         """
 
 
@@ -275,15 +275,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceId: str = ...,
         LinkId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLinkAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinkAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkassociationspaginator)
         """
 
 
@@ -297,15 +297,15 @@
         self,
         *,
         GlobalNetworkId: str,
         LinkIds: Sequence[str] = ...,
         SiteId: str = ...,
         Type: str = ...,
         Provider: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkspaginator)
         """
 
 
@@ -316,15 +316,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ResourceType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkResourceCountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceCounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcecountspaginator)
         """
 
 
@@ -340,15 +340,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkResourceRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceRelationships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcerelationshipspaginator)
         """
 
 
@@ -364,15 +364,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcespaginator)
         """
 
 
@@ -388,15 +388,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkTelemetryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkTelemetry.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworktelemetrypaginator)
         """
 
 
@@ -407,15 +407,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         SiteIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getsitespaginator)
         """
 
 
@@ -426,15 +426,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTransitGatewayConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayconnectpeerassociationspaginator)
         """
 
 
@@ -445,15 +445,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTransitGatewayRegistrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayRegistrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayregistrationspaginator)
         """
 
 
@@ -466,15 +466,15 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         AttachmentType: AttachmentTypeType = ...,
         EdgeLocation: str = ...,
         State: AttachmentStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listattachmentspaginator)
         """
 
 
@@ -485,45 +485,45 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         ConnectAttachmentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConnectPeersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListConnectPeers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listconnectpeerspaginator)
         """
 
 
 class ListCoreNetworkPolicyVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworkPolicyVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkpolicyversionspaginator)
     """
 
     def paginate(
-        self, *, CoreNetworkId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CoreNetworkId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoreNetworkPolicyVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworkPolicyVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkpolicyversionspaginator)
         """
 
 
 class ListCoreNetworksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoreNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkspaginator)
         """
 
 
@@ -536,13 +536,13 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         PeeringType: Literal["TRANSIT_GATEWAY"] = ...,
         EdgeLocation: str = ...,
         State: PeeringStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPeeringsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListPeerings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listpeeringspaginator)
         """
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/paginator.pyi` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -135,15 +135,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeGlobalNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.DescribeGlobalNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#describeglobalnetworkspaginator)
         """
 
 class GetConnectPeerAssociationsPaginator(AioPaginator):
@@ -153,15 +153,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectPeerIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectpeerassociationspaginator)
         """
 
 class GetConnectionsPaginator(AioPaginator):
@@ -172,15 +172,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ConnectionIds: Sequence[str] = ...,
         DeviceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetConnectionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetConnections.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getconnectionspaginator)
         """
 
 class GetCoreNetworkChangeEventsPaginator(AioPaginator):
@@ -190,15 +190,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCoreNetworkChangeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangeeventspaginator)
         """
 
 class GetCoreNetworkChangeSetPaginator(AioPaginator):
@@ -208,15 +208,15 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str,
         PolicyVersionId: int,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCoreNetworkChangeSetResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCoreNetworkChangeSet.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcorenetworkchangesetpaginator)
         """
 
 class GetCustomerGatewayAssociationsPaginator(AioPaginator):
@@ -226,15 +226,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         CustomerGatewayArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetCustomerGatewayAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetCustomerGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getcustomergatewayassociationspaginator)
         """
 
 class GetDevicesPaginator(AioPaginator):
@@ -245,15 +245,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceIds: Sequence[str] = ...,
         SiteId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDevicesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetDevices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getdevicespaginator)
         """
 
 class GetLinkAssociationsPaginator(AioPaginator):
@@ -264,15 +264,15 @@
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         DeviceId: str = ...,
         LinkId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLinkAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinkAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkassociationspaginator)
         """
 
 class GetLinksPaginator(AioPaginator):
@@ -285,15 +285,15 @@
         self,
         *,
         GlobalNetworkId: str,
         LinkIds: Sequence[str] = ...,
         SiteId: str = ...,
         Type: str = ...,
         Provider: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetLinksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getlinkspaginator)
         """
 
 class GetNetworkResourceCountsPaginator(AioPaginator):
@@ -303,15 +303,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         ResourceType: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkResourceCountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceCounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcecountspaginator)
         """
 
 class GetNetworkResourceRelationshipsPaginator(AioPaginator):
@@ -326,15 +326,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkResourceRelationshipsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResourceRelationships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcerelationshipspaginator)
         """
 
 class GetNetworkResourcesPaginator(AioPaginator):
@@ -349,15 +349,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkResourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworkresourcespaginator)
         """
 
 class GetNetworkTelemetryPaginator(AioPaginator):
@@ -372,15 +372,15 @@
         GlobalNetworkId: str,
         CoreNetworkId: str = ...,
         RegisteredGatewayArn: str = ...,
         AwsRegion: str = ...,
         AccountId: str = ...,
         ResourceType: str = ...,
         ResourceArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetNetworkTelemetryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetNetworkTelemetry.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getnetworktelemetrypaginator)
         """
 
 class GetSitesPaginator(AioPaginator):
@@ -390,15 +390,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         SiteIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetSitesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetSites.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#getsitespaginator)
         """
 
 class GetTransitGatewayConnectPeerAssociationsPaginator(AioPaginator):
@@ -408,15 +408,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayConnectPeerArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTransitGatewayConnectPeerAssociationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayConnectPeerAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayconnectpeerassociationspaginator)
         """
 
 class GetTransitGatewayRegistrationsPaginator(AioPaginator):
@@ -426,15 +426,15 @@
     """
 
     def paginate(
         self,
         *,
         GlobalNetworkId: str,
         TransitGatewayArns: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTransitGatewayRegistrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.GetTransitGatewayRegistrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#gettransitgatewayregistrationspaginator)
         """
 
 class ListAttachmentsPaginator(AioPaginator):
@@ -446,15 +446,15 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         AttachmentType: AttachmentTypeType = ...,
         EdgeLocation: str = ...,
         State: AttachmentStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachmentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listattachmentspaginator)
         """
 
 class ListConnectPeersPaginator(AioPaginator):
@@ -464,43 +464,43 @@
     """
 
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         ConnectAttachmentId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListConnectPeersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListConnectPeers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listconnectpeerspaginator)
         """
 
 class ListCoreNetworkPolicyVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworkPolicyVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkpolicyversionspaginator)
     """
 
     def paginate(
-        self, *, CoreNetworkId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CoreNetworkId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoreNetworkPolicyVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworkPolicyVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkpolicyversionspaginator)
         """
 
 class ListCoreNetworksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListCoreNetworksResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListCoreNetworks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listcorenetworkspaginator)
         """
 
 class ListPeeringsPaginator(AioPaginator):
@@ -512,13 +512,13 @@
     def paginate(
         self,
         *,
         CoreNetworkId: str = ...,
         PeeringType: Literal["TRANSIT_GATEWAY"] = ...,
         EdgeLocation: str = ...,
         State: PeeringStateType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPeeringsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager.Paginator.ListPeerings.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/paginators/#listpeeringspaginator)
         """
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/type_defs.py` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_networkmanager.type_defs import AWSLocationTypeDef
 
-    data: AWSLocationTypeDef = {...}
+    data: AWSLocationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -51,18 +51,18 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AWSLocationTypeDef",
     "AcceptAttachmentRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AccountStatusTypeDef",
     "AssociateConnectPeerRequestRequestTypeDef",
     "ConnectPeerAssociationTypeDef",
     "AssociateCustomerGatewayRequestRequestTypeDef",
     "CustomerGatewayAssociationTypeDef",
     "AssociateLinkRequestRequestTypeDef",
     "LinkAssociationTypeDef",
@@ -91,95 +91,73 @@
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteGlobalNetworkRequestRequestTypeDef",
     "DeleteLinkRequestRequestTypeDef",
     "DeletePeeringRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeregisterTransitGatewayRequestRequestTypeDef",
-    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeGlobalNetworksRequestRequestTypeDef",
     "DisassociateConnectPeerRequestRequestTypeDef",
     "DisassociateCustomerGatewayRequestRequestTypeDef",
     "DisassociateLinkRequestRequestTypeDef",
     "DisassociateTransitGatewayConnectPeerRequestRequestTypeDef",
     "ExecuteCoreNetworkChangeSetRequestRequestTypeDef",
     "GetConnectAttachmentRequestRequestTypeDef",
-    "GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
     "GetConnectPeerAssociationsRequestRequestTypeDef",
     "GetConnectPeerRequestRequestTypeDef",
-    "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     "GetConnectionsRequestRequestTypeDef",
-    "GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
     "GetCoreNetworkChangeEventsRequestRequestTypeDef",
-    "GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
     "GetCoreNetworkChangeSetRequestRequestTypeDef",
     "GetCoreNetworkPolicyRequestRequestTypeDef",
     "GetCoreNetworkRequestRequestTypeDef",
-    "GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
     "GetCustomerGatewayAssociationsRequestRequestTypeDef",
-    "GetDevicesRequestGetDevicesPaginateTypeDef",
     "GetDevicesRequestRequestTypeDef",
-    "GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
     "GetLinkAssociationsRequestRequestTypeDef",
-    "GetLinksRequestGetLinksPaginateTypeDef",
     "GetLinksRequestRequestTypeDef",
-    "GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
     "GetNetworkResourceCountsRequestRequestTypeDef",
     "NetworkResourceCountTypeDef",
-    "GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
     "GetNetworkResourceRelationshipsRequestRequestTypeDef",
     "RelationshipTypeDef",
-    "GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
     "GetNetworkResourcesRequestRequestTypeDef",
-    "GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
     "GetNetworkTelemetryRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRouteAnalysisRequestRequestTypeDef",
     "GetSiteToSiteVpnAttachmentRequestRequestTypeDef",
-    "GetSitesRequestGetSitesPaginateTypeDef",
     "GetSitesRequestRequestTypeDef",
-    "GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
     "GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef",
     "GetTransitGatewayPeeringRequestRequestTypeDef",
-    "GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
     "GetTransitGatewayRegistrationsRequestRequestTypeDef",
     "GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef",
     "GetVpcAttachmentRequestRequestTypeDef",
-    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
     "ListAttachmentsRequestRequestTypeDef",
-    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
     "ListConnectPeersRequestRequestTypeDef",
-    "ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
     "ListCoreNetworkPolicyVersionsRequestRequestTypeDef",
-    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
     "ListCoreNetworksRequestRequestTypeDef",
     "ListOrganizationServiceAccessStatusRequestRequestTypeDef",
-    "ListPeeringsRequestListPeeringsPaginateTypeDef",
     "ListPeeringsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NetworkResourceSummaryTypeDef",
     "NetworkRouteDestinationTypeDef",
-    "PaginatorConfigTypeDef",
     "PutCoreNetworkPolicyRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterTransitGatewayRequestRequestTypeDef",
     "RejectAttachmentRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreCoreNetworkPolicyVersionRequestRequestTypeDef",
     "RouteAnalysisCompletionTypeDef",
     "RouteAnalysisEndpointOptionsSpecificationTypeDef",
     "RouteAnalysisEndpointOptionsTypeDef",
     "StartOrganizationServiceAccessUpdateRequestRequestTypeDef",
     "TransitGatewayRegistrationStateReasonTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateCoreNetworkRequestRequestTypeDef",
     "UpdateGlobalNetworkRequestRequestTypeDef",
     "UpdateNetworkResourceMetadataRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "UpdateNetworkResourceMetadataResponseTypeDef",
     "OrganizationStatusTypeDef",
     "AssociateConnectPeerResponseTypeDef",
     "DisassociateConnectPeerResponseTypeDef",
     "GetConnectPeerAssociationsResponseTypeDef",
     "AssociateCustomerGatewayResponseTypeDef",
     "DisassociateCustomerGatewayResponseTypeDef",
@@ -222,14 +200,35 @@
     "CreateSiteRequestRequestTypeDef",
     "DeviceTypeDef",
     "SiteTypeDef",
     "UpdateDeviceRequestRequestTypeDef",
     "UpdateSiteRequestRequestTypeDef",
     "CreateVpcAttachmentRequestRequestTypeDef",
     "UpdateVpcAttachmentRequestRequestTypeDef",
+    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+    "GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
+    "GetConnectionsRequestGetConnectionsPaginateTypeDef",
+    "GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
+    "GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
+    "GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
+    "GetDevicesRequestGetDevicesPaginateTypeDef",
+    "GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
+    "GetLinksRequestGetLinksPaginateTypeDef",
+    "GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
+    "GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
+    "GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
+    "GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
+    "GetSitesRequestGetSitesPaginateTypeDef",
+    "GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
+    "GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
+    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
+    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
+    "ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
+    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
+    "ListPeeringsRequestListPeeringsPaginateTypeDef",
     "GetNetworkResourceCountsResponseTypeDef",
     "GetNetworkResourceRelationshipsResponseTypeDef",
     "PathComponentTypeDef",
     "NetworkRouteTypeDef",
     "StartRouteAnalysisRequestRequestTypeDef",
     "TransitGatewayRegistrationTypeDef",
     "ListOrganizationServiceAccessStatusResponseTypeDef",
@@ -318,14 +317,25 @@
 AcceptAttachmentRequestRequestTypeDef = TypedDict(
     "AcceptAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
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
 AccountStatusTypeDef = TypedDict(
     "AccountStatusTypeDef",
     {
         "AccountId": str,
         "SLRDeploymentStatus": str,
     },
     total=False,
@@ -343,22 +353,20 @@
     "_OptionalAssociateConnectPeerRequestRequestTypeDef",
     {
         "LinkId": str,
     },
     total=False,
 )
 
-
 class AssociateConnectPeerRequestRequestTypeDef(
     _RequiredAssociateConnectPeerRequestRequestTypeDef,
     _OptionalAssociateConnectPeerRequestRequestTypeDef,
 ):
     pass
 
-
 ConnectPeerAssociationTypeDef = TypedDict(
     "ConnectPeerAssociationTypeDef",
     {
         "ConnectPeerId": str,
         "GlobalNetworkId": str,
         "DeviceId": str,
         "LinkId": str,
@@ -379,22 +387,20 @@
     "_OptionalAssociateCustomerGatewayRequestRequestTypeDef",
     {
         "LinkId": str,
     },
     total=False,
 )
 
-
 class AssociateCustomerGatewayRequestRequestTypeDef(
     _RequiredAssociateCustomerGatewayRequestRequestTypeDef,
     _OptionalAssociateCustomerGatewayRequestRequestTypeDef,
 ):
     pass
 
-
 CustomerGatewayAssociationTypeDef = TypedDict(
     "CustomerGatewayAssociationTypeDef",
     {
         "CustomerGatewayArn": str,
         "GlobalNetworkId": str,
         "DeviceId": str,
         "LinkId": str,
@@ -435,22 +441,20 @@
     "_OptionalAssociateTransitGatewayConnectPeerRequestRequestTypeDef",
     {
         "LinkId": str,
     },
     total=False,
 )
 
-
 class AssociateTransitGatewayConnectPeerRequestRequestTypeDef(
     _RequiredAssociateTransitGatewayConnectPeerRequestRequestTypeDef,
     _OptionalAssociateTransitGatewayConnectPeerRequestRequestTypeDef,
 ):
     pass
 
-
 TransitGatewayConnectPeerAssociationTypeDef = TypedDict(
     "TransitGatewayConnectPeerAssociationTypeDef",
     {
         "TransitGatewayConnectPeerArn": str,
         "GlobalNetworkId": str,
         "DeviceId": str,
         "LinkId": str,
@@ -560,21 +564,19 @@
     "_OptionalCoreNetworkPolicyErrorTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
-
 class CoreNetworkPolicyErrorTypeDef(
     _RequiredCoreNetworkPolicyErrorTypeDef, _OptionalCoreNetworkPolicyErrorTypeDef
 ):
     pass
 
-
 CoreNetworkPolicyVersionTypeDef = TypedDict(
     "CoreNetworkPolicyVersionTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
         "Alias": CoreNetworkPolicyAliasType,
         "Description": str,
@@ -709,19 +711,20 @@
     "DeregisterTransitGatewayRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "TransitGatewayArn": str,
     },
 )
 
-DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef = TypedDict(
-    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "GlobalNetworkIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeGlobalNetworksRequestRequestTypeDef = TypedDict(
     "DescribeGlobalNetworksRequestRequestTypeDef",
     {
@@ -776,37 +779,14 @@
 GetConnectAttachmentRequestRequestTypeDef = TypedDict(
     "GetConnectAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
-_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
-    {
-        "ConnectPeerIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef(
-    _RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
-    _OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectPeerAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
@@ -815,53 +795,27 @@
         "ConnectPeerIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConnectPeerAssociationsRequestRequestTypeDef(
     _RequiredGetConnectPeerAssociationsRequestRequestTypeDef,
     _OptionalGetConnectPeerAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 GetConnectPeerRequestRequestTypeDef = TypedDict(
     "GetConnectPeerRequestRequestTypeDef",
     {
         "ConnectPeerId": str,
     },
 )
 
-_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
-    "_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
-    "_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef",
-    {
-        "ConnectionIds": Sequence[str],
-        "DeviceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetConnectionsRequestGetConnectionsPaginateTypeDef(
-    _RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef,
-    _OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetConnectionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetConnectionsRequestRequestTypeDef = TypedDict(
@@ -871,44 +825,19 @@
         "DeviceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetConnectionsRequestRequestTypeDef(
     _RequiredGetConnectionsRequestRequestTypeDef, _OptionalGetConnectionsRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
-    "_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "PolicyVersionId": int,
-    },
-)
-_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
-    "_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef(
-    _RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
-    _OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCoreNetworkChangeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCoreNetworkChangeEventsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
     },
 )
@@ -917,45 +846,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetCoreNetworkChangeEventsRequestRequestTypeDef(
     _RequiredGetCoreNetworkChangeEventsRequestRequestTypeDef,
     _OptionalGetCoreNetworkChangeEventsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "PolicyVersionId": int,
-    },
-)
-_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef(
-    _RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
-    _OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCoreNetworkChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredGetCoreNetworkChangeSetRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
     },
 )
@@ -964,22 +868,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetCoreNetworkChangeSetRequestRequestTypeDef(
     _RequiredGetCoreNetworkChangeSetRequestRequestTypeDef,
     _OptionalGetCoreNetworkChangeSetRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredGetCoreNetworkPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetCoreNetworkPolicyRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 _OptionalGetCoreNetworkPolicyRequestRequestTypeDef = TypedDict(
@@ -987,52 +889,27 @@
     {
         "PolicyVersionId": int,
         "Alias": CoreNetworkPolicyAliasType,
     },
     total=False,
 )
 
-
 class GetCoreNetworkPolicyRequestRequestTypeDef(
     _RequiredGetCoreNetworkPolicyRequestRequestTypeDef,
     _OptionalGetCoreNetworkPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 GetCoreNetworkRequestRequestTypeDef = TypedDict(
     "GetCoreNetworkRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 
-_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
-    {
-        "CustomerGatewayArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef(
-    _RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
-    _OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetCustomerGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCustomerGatewayAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetCustomerGatewayAssociationsRequestRequestTypeDef = TypedDict(
@@ -1041,46 +918,20 @@
         "CustomerGatewayArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetCustomerGatewayAssociationsRequestRequestTypeDef(
     _RequiredGetCustomerGatewayAssociationsRequestRequestTypeDef,
     _OptionalGetCustomerGatewayAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicesRequestGetDevicesPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicesRequestGetDevicesPaginateTypeDef",
-    {
-        "DeviceIds": Sequence[str],
-        "SiteId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDevicesRequestGetDevicesPaginateTypeDef(
-    _RequiredGetDevicesRequestGetDevicesPaginateTypeDef,
-    _OptionalGetDevicesRequestGetDevicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetDevicesRequestRequestTypeDef = TypedDict(
@@ -1090,45 +941,19 @@
         "SiteId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetDevicesRequestRequestTypeDef(
     _RequiredGetDevicesRequestRequestTypeDef, _OptionalGetDevicesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "LinkId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef(
-    _RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
-    _OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetLinkAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetLinkAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetLinkAssociationsRequestRequestTypeDef = TypedDict(
@@ -1138,47 +963,20 @@
         "LinkId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetLinkAssociationsRequestRequestTypeDef(
     _RequiredGetLinkAssociationsRequestRequestTypeDef,
     _OptionalGetLinkAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
-    "_RequiredGetLinksRequestGetLinksPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
-    "_OptionalGetLinksRequestGetLinksPaginateTypeDef",
-    {
-        "LinkIds": Sequence[str],
-        "SiteId": str,
-        "Type": str,
-        "Provider": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetLinksRequestGetLinksPaginateTypeDef(
-    _RequiredGetLinksRequestGetLinksPaginateTypeDef, _OptionalGetLinksRequestGetLinksPaginateTypeDef
-):
-    pass
-
-
 _RequiredGetLinksRequestRequestTypeDef = TypedDict(
     "_RequiredGetLinksRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetLinksRequestRequestTypeDef = TypedDict(
@@ -1190,44 +988,19 @@
         "Provider": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetLinksRequestRequestTypeDef(
     _RequiredGetLinksRequestRequestTypeDef, _OptionalGetLinksRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef(
-    _RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
-    _OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetNetworkResourceCountsRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkResourceCountsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetNetworkResourceCountsRequestRequestTypeDef = TypedDict(
@@ -1236,59 +1009,29 @@
         "ResourceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetNetworkResourceCountsRequestRequestTypeDef(
     _RequiredGetNetworkResourceCountsRequestRequestTypeDef,
     _OptionalGetNetworkResourceCountsRequestRequestTypeDef,
 ):
     pass
 
-
 NetworkResourceCountTypeDef = TypedDict(
     "NetworkResourceCountTypeDef",
     {
         "ResourceType": str,
         "Count": int,
     },
     total=False,
 )
 
-_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "RegisteredGatewayArn": str,
-        "AwsRegion": str,
-        "AccountId": str,
-        "ResourceType": str,
-        "ResourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef(
-    _RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
-    _OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetNetworkResourceRelationshipsRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkResourceRelationshipsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetNetworkResourceRelationshipsRequestRequestTypeDef = TypedDict(
@@ -1302,59 +1045,29 @@
         "ResourceArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetNetworkResourceRelationshipsRequestRequestTypeDef(
     _RequiredGetNetworkResourceRelationshipsRequestRequestTypeDef,
     _OptionalGetNetworkResourceRelationshipsRequestRequestTypeDef,
 ):
     pass
 
-
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "From": str,
         "To": str,
     },
     total=False,
 )
 
-_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "RegisteredGatewayArn": str,
-        "AwsRegion": str,
-        "AccountId": str,
-        "ResourceType": str,
-        "ResourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef(
-    _RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
-    _OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetNetworkResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkResourcesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetNetworkResourcesRequestRequestTypeDef = TypedDict(
@@ -1368,50 +1081,20 @@
         "ResourceArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetNetworkResourcesRequestRequestTypeDef(
     _RequiredGetNetworkResourcesRequestRequestTypeDef,
     _OptionalGetNetworkResourcesRequestRequestTypeDef,
 ):
     pass
 
-
-_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "RegisteredGatewayArn": str,
-        "AwsRegion": str,
-        "AccountId": str,
-        "ResourceType": str,
-        "ResourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef(
-    _RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
-    _OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetNetworkTelemetryRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkTelemetryRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetNetworkTelemetryRequestRequestTypeDef = TypedDict(
@@ -1425,37 +1108,27 @@
         "ResourceArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetNetworkTelemetryRequestRequestTypeDef(
     _RequiredGetNetworkTelemetryRequestRequestTypeDef,
     _OptionalGetNetworkTelemetryRequestRequestTypeDef,
 ):
     pass
 
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRouteAnalysisRequestRequestTypeDef = TypedDict(
     "GetRouteAnalysisRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "RouteAnalysisId": str,
     },
 )
@@ -1463,36 +1136,14 @@
 GetSiteToSiteVpnAttachmentRequestRequestTypeDef = TypedDict(
     "GetSiteToSiteVpnAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
-_RequiredGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
-    "_RequiredGetSitesRequestGetSitesPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
-    "_OptionalGetSitesRequestGetSitesPaginateTypeDef",
-    {
-        "SiteIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetSitesRequestGetSitesPaginateTypeDef(
-    _RequiredGetSitesRequestGetSitesPaginateTypeDef, _OptionalGetSitesRequestGetSitesPaginateTypeDef
-):
-    pass
-
-
 _RequiredGetSitesRequestRequestTypeDef = TypedDict(
     "_RequiredGetSitesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetSitesRequestRequestTypeDef = TypedDict(
@@ -1501,44 +1152,19 @@
         "SiteIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetSitesRequestRequestTypeDef(
     _RequiredGetSitesRequestRequestTypeDef, _OptionalGetSitesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
-    {
-        "TransitGatewayConnectPeerArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef(
-    _RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
-    _OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
@@ -1547,52 +1173,27 @@
         "TransitGatewayConnectPeerArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef(
     _RequiredGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
     _OptionalGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
 ):
     pass
 
-
 GetTransitGatewayPeeringRequestRequestTypeDef = TypedDict(
     "GetTransitGatewayPeeringRequestRequestTypeDef",
     {
         "PeeringId": str,
     },
 )
 
-_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
-    {
-        "TransitGatewayArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef(
-    _RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
-    _OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTransitGatewayRegistrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTransitGatewayRegistrationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetTransitGatewayRegistrationsRequestRequestTypeDef = TypedDict(
@@ -1601,108 +1202,58 @@
         "TransitGatewayArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetTransitGatewayRegistrationsRequestRequestTypeDef(
     _RequiredGetTransitGatewayRegistrationsRequestRequestTypeDef,
     _OptionalGetTransitGatewayRegistrationsRequestRequestTypeDef,
 ):
     pass
 
-
 GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef = TypedDict(
     "GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
 GetVpcAttachmentRequestRequestTypeDef = TypedDict(
     "GetVpcAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
-ListAttachmentsRequestListAttachmentsPaginateTypeDef = TypedDict(
-    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "AttachmentType": AttachmentTypeType,
-        "EdgeLocation": str,
-        "State": AttachmentStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAttachmentsRequestRequestTypeDef = TypedDict(
     "ListAttachmentsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "AttachmentType": AttachmentTypeType,
         "EdgeLocation": str,
         "State": AttachmentStateType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListConnectPeersRequestListConnectPeersPaginateTypeDef = TypedDict(
-    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "ConnectAttachmentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConnectPeersRequestRequestTypeDef = TypedDict(
     "ListConnectPeersRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "ConnectAttachmentId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
-        {
-            "CoreNetworkId": str,
-        },
-    )
-)
-_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-
-class ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef(
-    _RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
-    _OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListCoreNetworkPolicyVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCoreNetworkPolicyVersionsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 _OptionalListCoreNetworkPolicyVersionsRequestRequestTypeDef = TypedDict(
@@ -1710,30 +1261,20 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListCoreNetworkPolicyVersionsRequestRequestTypeDef(
     _RequiredListCoreNetworkPolicyVersionsRequestRequestTypeDef,
     _OptionalListCoreNetworkPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
-
-ListCoreNetworksRequestListCoreNetworksPaginateTypeDef = TypedDict(
-    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListCoreNetworksRequestRequestTypeDef = TypedDict(
     "ListCoreNetworksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1744,26 +1285,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPeeringsRequestListPeeringsPaginateTypeDef = TypedDict(
-    "ListPeeringsRequestListPeeringsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "PeeringType": Literal["TRANSIT_GATEWAY"],
-        "EdgeLocation": str,
-        "State": PeeringStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPeeringsRequestRequestTypeDef = TypedDict(
     "ListPeeringsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PeeringType": Literal["TRANSIT_GATEWAY"],
         "EdgeLocation": str,
         "State": PeeringStateType,
@@ -1802,24 +1331,14 @@
         "EdgeLocation": str,
         "ResourceType": str,
         "ResourceId": str,
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
 _RequiredPutCoreNetworkPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutCoreNetworkPolicyRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyDocument": str,
     },
 )
@@ -1829,22 +1348,20 @@
         "Description": str,
         "LatestVersionId": int,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class PutCoreNetworkPolicyRequestRequestTypeDef(
     _RequiredPutCoreNetworkPolicyRequestRequestTypeDef,
     _OptionalPutCoreNetworkPolicyRequestRequestTypeDef,
 ):
     pass
 
-
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyDocument": str,
         "ResourceArn": str,
     },
 )
@@ -1860,25 +1377,14 @@
 RejectAttachmentRequestRequestTypeDef = TypedDict(
     "RejectAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
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
 RestoreCoreNetworkPolicyVersionRequestRequestTypeDef = TypedDict(
     "RestoreCoreNetworkPolicyVersionRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
     },
 )
@@ -1949,79 +1455,81 @@
         "LinkId": str,
         "ConnectedLinkId": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateCoreNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCoreNetworkRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 _OptionalUpdateCoreNetworkRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCoreNetworkRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateCoreNetworkRequestRequestTypeDef(
     _RequiredUpdateCoreNetworkRequestRequestTypeDef, _OptionalUpdateCoreNetworkRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateGlobalNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalNetworkRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalUpdateGlobalNetworkRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGlobalNetworkRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateGlobalNetworkRequestRequestTypeDef(
     _RequiredUpdateGlobalNetworkRequestRequestTypeDef,
     _OptionalUpdateGlobalNetworkRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateNetworkResourceMetadataRequestRequestTypeDef = TypedDict(
     "UpdateNetworkResourceMetadataRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "ResourceArn": str,
         "Metadata": Mapping[str, str],
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateNetworkResourceMetadataResponseTypeDef = TypedDict(
     "UpdateNetworkResourceMetadataResponseTypeDef",
     {
         "ResourceArn": str,
         "Metadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrganizationStatusTypeDef = TypedDict(
     "OrganizationStatusTypeDef",
     {
         "OrganizationId": str,
@@ -2032,107 +1540,107 @@
     total=False,
 )
 
 AssociateConnectPeerResponseTypeDef = TypedDict(
     "AssociateConnectPeerResponseTypeDef",
     {
         "ConnectPeerAssociation": ConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateConnectPeerResponseTypeDef = TypedDict(
     "DisassociateConnectPeerResponseTypeDef",
     {
         "ConnectPeerAssociation": ConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectPeerAssociationsResponseTypeDef = TypedDict(
     "GetConnectPeerAssociationsResponseTypeDef",
     {
         "ConnectPeerAssociations": List[ConnectPeerAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateCustomerGatewayResponseTypeDef = TypedDict(
     "AssociateCustomerGatewayResponseTypeDef",
     {
         "CustomerGatewayAssociation": CustomerGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateCustomerGatewayResponseTypeDef = TypedDict(
     "DisassociateCustomerGatewayResponseTypeDef",
     {
         "CustomerGatewayAssociation": CustomerGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCustomerGatewayAssociationsResponseTypeDef = TypedDict(
     "GetCustomerGatewayAssociationsResponseTypeDef",
     {
         "CustomerGatewayAssociations": List[CustomerGatewayAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateLinkResponseTypeDef = TypedDict(
     "AssociateLinkResponseTypeDef",
     {
         "LinkAssociation": LinkAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateLinkResponseTypeDef = TypedDict(
     "DisassociateLinkResponseTypeDef",
     {
         "LinkAssociation": LinkAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLinkAssociationsResponseTypeDef = TypedDict(
     "GetLinkAssociationsResponseTypeDef",
     {
         "LinkAssociations": List[LinkAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateTransitGatewayConnectPeerResponseTypeDef = TypedDict(
     "AssociateTransitGatewayConnectPeerResponseTypeDef",
     {
         "TransitGatewayConnectPeerAssociation": TransitGatewayConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateTransitGatewayConnectPeerResponseTypeDef = TypedDict(
     "DisassociateTransitGatewayConnectPeerResponseTypeDef",
     {
         "TransitGatewayConnectPeerAssociation": TransitGatewayConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayConnectPeerAssociationsResponseTypeDef = TypedDict(
     "GetTransitGatewayConnectPeerAssociationsResponseTypeDef",
     {
         "TransitGatewayConnectPeerAssociations": List[TransitGatewayConnectPeerAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectPeerSummaryTypeDef = TypedDict(
     "ConnectPeerSummaryTypeDef",
     {
         "CoreNetworkId": str,
@@ -2193,21 +1701,19 @@
         "ConnectedLinkId": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateCoreNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCoreNetworkRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalCreateCoreNetworkRequestRequestTypeDef = TypedDict(
@@ -2217,21 +1723,19 @@
         "Tags": Sequence[TagTypeDef],
         "PolicyDocument": str,
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateCoreNetworkRequestRequestTypeDef(
     _RequiredCreateCoreNetworkRequestRequestTypeDef, _OptionalCreateCoreNetworkRequestRequestTypeDef
 ):
     pass
 
-
 CreateGlobalNetworkRequestRequestTypeDef = TypedDict(
     "CreateGlobalNetworkRequestRequestTypeDef",
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
@@ -2249,22 +1753,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateSiteToSiteVpnAttachmentRequestRequestTypeDef(
     _RequiredCreateSiteToSiteVpnAttachmentRequestRequestTypeDef,
     _OptionalCreateSiteToSiteVpnAttachmentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateTransitGatewayPeeringRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransitGatewayPeeringRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "TransitGatewayArn": str,
     },
 )
@@ -2273,22 +1775,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateTransitGatewayPeeringRequestRequestTypeDef(
     _RequiredCreateTransitGatewayPeeringRequestRequestTypeDef,
     _OptionalCreateTransitGatewayPeeringRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef",
     {
         "PeeringId": str,
         "TransitGatewayRouteTableArn": str,
     },
 )
@@ -2297,22 +1797,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef(
     _RequiredCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
     _OptionalCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
 ):
     pass
 
-
 GlobalNetworkTypeDef = TypedDict(
     "GlobalNetworkTypeDef",
     {
         "GlobalNetworkId": str,
         "GlobalNetworkArn": str,
         "Description": str,
         "CreatedAt": datetime,
@@ -2322,15 +1820,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "RegisteredGatewayArn": str,
@@ -2398,21 +1896,19 @@
         "Type": str,
         "Provider": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateLinkRequestRequestTypeDef(
     _RequiredCreateLinkRequestRequestTypeDef, _OptionalCreateLinkRequestRequestTypeDef
 ):
     pass
 
-
 LinkTypeDef = TypedDict(
     "LinkTypeDef",
     {
         "LinkId": str,
         "LinkArn": str,
         "GlobalNetworkId": str,
         "SiteId": str,
@@ -2441,21 +1937,19 @@
         "Type": str,
         "Bandwidth": BandwidthTypeDef,
         "Provider": str,
     },
     total=False,
 )
 
-
 class UpdateLinkRequestRequestTypeDef(
     _RequiredUpdateLinkRequestRequestTypeDef, _OptionalUpdateLinkRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateConnectPeerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectPeerRequestRequestTypeDef",
     {
         "ConnectAttachmentId": str,
         "PeerAddress": str,
         "InsideCidrBlocks": Sequence[str],
     },
@@ -2467,21 +1961,19 @@
         "BgpOptions": BgpOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateConnectPeerRequestRequestTypeDef(
     _RequiredCreateConnectPeerRequestRequestTypeDef, _OptionalCreateConnectPeerRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateConnectAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectAttachmentRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "EdgeLocation": str,
         "TransportAttachmentId": str,
         "Options": ConnectAttachmentOptionsTypeDef,
@@ -2492,22 +1984,20 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateConnectAttachmentRequestRequestTypeDef(
     _RequiredCreateConnectAttachmentRequestRequestTypeDef,
     _OptionalCreateConnectAttachmentRequestRequestTypeDef,
 ):
     pass
 
-
 ConnectPeerConfigurationTypeDef = TypedDict(
     "ConnectPeerConfigurationTypeDef",
     {
         "CoreNetworkAddress": str,
         "PeerAddress": str,
         "InsideCidrBlocks": List[str],
         "Protocol": Literal["GRE"],
@@ -2574,15 +2064,15 @@
 )
 
 ListCoreNetworkPolicyVersionsResponseTypeDef = TypedDict(
     "ListCoreNetworkPolicyVersionsResponseTypeDef",
     {
         "CoreNetworkPolicyVersions": List[CoreNetworkPolicyVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RouteTableIdentifierTypeDef = TypedDict(
     "RouteTableIdentifierTypeDef",
     {
         "TransitGatewayRouteTableArn": str,
@@ -2625,21 +2115,19 @@
         "Location": LocationTypeDef,
         "SiteId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDeviceRequestRequestTypeDef(
     _RequiredCreateDeviceRequestRequestTypeDef, _OptionalCreateDeviceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalCreateSiteRequestRequestTypeDef = TypedDict(
@@ -2648,21 +2136,19 @@
         "Description": str,
         "Location": LocationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
-
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "DeviceId": str,
         "DeviceArn": str,
         "GlobalNetworkId": str,
         "AWSLocation": AWSLocationTypeDef,
@@ -2713,21 +2199,19 @@
         "SerialNumber": str,
         "Location": LocationTypeDef,
         "SiteId": str,
     },
     total=False,
 )
 
-
 class UpdateDeviceRequestRequestTypeDef(
     _RequiredUpdateDeviceRequestRequestTypeDef, _OptionalUpdateDeviceRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "SiteId": str,
     },
 )
@@ -2736,21 +2220,19 @@
     {
         "Description": str,
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
-
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateVpcAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcAttachmentRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "VpcArn": str,
         "SubnetArns": Sequence[str],
     },
@@ -2761,22 +2243,20 @@
         "Options": VpcOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
-
 class CreateVpcAttachmentRequestRequestTypeDef(
     _RequiredCreateVpcAttachmentRequestRequestTypeDef,
     _OptionalCreateVpcAttachmentRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateVpcAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 _OptionalUpdateVpcAttachmentRequestRequestTypeDef = TypedDict(
@@ -2785,37 +2265,444 @@
         "AddSubnetArns": Sequence[str],
         "RemoveSubnetArns": Sequence[str],
         "Options": VpcOptionsTypeDef,
     },
     total=False,
 )
 
-
 class UpdateVpcAttachmentRequestRequestTypeDef(
     _RequiredUpdateVpcAttachmentRequestRequestTypeDef,
     _OptionalUpdateVpcAttachmentRequestRequestTypeDef,
 ):
     pass
 
+DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef = TypedDict(
+    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+    {
+        "GlobalNetworkIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
+    {
+        "ConnectPeerIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef(
+    _RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+    _OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef",
+    {
+        "ConnectionIds": Sequence[str],
+        "DeviceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetConnectionsRequestGetConnectionsPaginateTypeDef(
+    _RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef,
+    _OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
+    "_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "PolicyVersionId": int,
+    },
+)
+_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
+    "_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef(
+    _RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+    _OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "PolicyVersionId": int,
+    },
+)
+_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef(
+    _RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+    _OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+):
+    pass
+
+_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
+    {
+        "CustomerGatewayArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef(
+    _RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+    _OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicesRequestGetDevicesPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicesRequestGetDevicesPaginateTypeDef",
+    {
+        "DeviceIds": Sequence[str],
+        "SiteId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetDevicesRequestGetDevicesPaginateTypeDef(
+    _RequiredGetDevicesRequestGetDevicesPaginateTypeDef,
+    _OptionalGetDevicesRequestGetDevicesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "LinkId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef(
+    _RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+    _OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
+    "_RequiredGetLinksRequestGetLinksPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
+    "_OptionalGetLinksRequestGetLinksPaginateTypeDef",
+    {
+        "LinkIds": Sequence[str],
+        "SiteId": str,
+        "Type": str,
+        "Provider": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetLinksRequestGetLinksPaginateTypeDef(
+    _RequiredGetLinksRequestGetLinksPaginateTypeDef, _OptionalGetLinksRequestGetLinksPaginateTypeDef
+):
+    pass
+
+_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef(
+    _RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+    _OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "RegisteredGatewayArn": str,
+        "AwsRegion": str,
+        "AccountId": str,
+        "ResourceType": str,
+        "ResourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef(
+    _RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+    _OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "RegisteredGatewayArn": str,
+        "AwsRegion": str,
+        "AccountId": str,
+        "ResourceType": str,
+        "ResourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef(
+    _RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+    _OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "RegisteredGatewayArn": str,
+        "AwsRegion": str,
+        "AccountId": str,
+        "ResourceType": str,
+        "ResourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef(
+    _RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+    _OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+):
+    pass
+
+_RequiredGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
+    "_RequiredGetSitesRequestGetSitesPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
+    "_OptionalGetSitesRequestGetSitesPaginateTypeDef",
+    {
+        "SiteIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetSitesRequestGetSitesPaginateTypeDef(
+    _RequiredGetSitesRequestGetSitesPaginateTypeDef, _OptionalGetSitesRequestGetSitesPaginateTypeDef
+):
+    pass
+
+_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
+    {
+        "TransitGatewayConnectPeerArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef(
+    _RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+    _OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
+    {
+        "TransitGatewayArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef(
+    _RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+    _OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+):
+    pass
+
+ListAttachmentsRequestListAttachmentsPaginateTypeDef = TypedDict(
+    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "AttachmentType": AttachmentTypeType,
+        "EdgeLocation": str,
+        "State": AttachmentStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConnectPeersRequestListConnectPeersPaginateTypeDef = TypedDict(
+    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "ConnectAttachmentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
+        {
+            "CoreNetworkId": str,
+        },
+    )
+)
+_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+class ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef(
+    _RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+    _OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+):
+    pass
+
+ListCoreNetworksRequestListCoreNetworksPaginateTypeDef = TypedDict(
+    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPeeringsRequestListPeeringsPaginateTypeDef = TypedDict(
+    "ListPeeringsRequestListPeeringsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "PeeringType": Literal["TRANSIT_GATEWAY"],
+        "EdgeLocation": str,
+        "State": PeeringStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
 
 GetNetworkResourceCountsResponseTypeDef = TypedDict(
     "GetNetworkResourceCountsResponseTypeDef",
     {
         "NetworkResourceCounts": List[NetworkResourceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResourceRelationshipsResponseTypeDef = TypedDict(
     "GetNetworkResourceRelationshipsResponseTypeDef",
     {
         "Relationships": List[RelationshipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PathComponentTypeDef = TypedDict(
     "PathComponentTypeDef",
     {
         "Sequence": int,
@@ -2850,22 +2737,20 @@
     {
         "IncludeReturnPath": bool,
         "UseMiddleboxes": bool,
     },
     total=False,
 )
 
-
 class StartRouteAnalysisRequestRequestTypeDef(
     _RequiredStartRouteAnalysisRequestRequestTypeDef,
     _OptionalStartRouteAnalysisRequestRequestTypeDef,
 ):
     pass
 
-
 TransitGatewayRegistrationTypeDef = TypedDict(
     "TransitGatewayRegistrationTypeDef",
     {
         "GlobalNetworkId": str,
         "TransitGatewayArn": str,
         "State": TransitGatewayRegistrationStateReasonTypeDef,
     },
@@ -2873,133 +2758,133 @@
 )
 
 ListOrganizationServiceAccessStatusResponseTypeDef = TypedDict(
     "ListOrganizationServiceAccessStatusResponseTypeDef",
     {
         "OrganizationStatus": OrganizationStatusTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartOrganizationServiceAccessUpdateResponseTypeDef = TypedDict(
     "StartOrganizationServiceAccessUpdateResponseTypeDef",
     {
         "OrganizationStatus": OrganizationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectPeersResponseTypeDef = TypedDict(
     "ListConnectPeersResponseTypeDef",
     {
         "ConnectPeers": List[ConnectPeerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConnectionResponseTypeDef = TypedDict(
     "CreateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectionsResponseTypeDef = TypedDict(
     "GetConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionResponseTypeDef = TypedDict(
     "UpdateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoreNetworksResponseTypeDef = TypedDict(
     "ListCoreNetworksResponseTypeDef",
     {
         "CoreNetworks": List[CoreNetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalNetworkResponseTypeDef = TypedDict(
     "CreateGlobalNetworkResponseTypeDef",
     {
         "GlobalNetwork": GlobalNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalNetworkResponseTypeDef = TypedDict(
     "DeleteGlobalNetworkResponseTypeDef",
     {
         "GlobalNetwork": GlobalNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalNetworksResponseTypeDef = TypedDict(
     "DescribeGlobalNetworksResponseTypeDef",
     {
         "GlobalNetworks": List[GlobalNetworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalNetworkResponseTypeDef = TypedDict(
     "UpdateGlobalNetworkResponseTypeDef",
     {
         "GlobalNetwork": GlobalNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResourcesResponseTypeDef = TypedDict(
     "GetNetworkResourcesResponseTypeDef",
     {
         "NetworkResources": List[NetworkResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePeeringResponseTypeDef = TypedDict(
     "DeletePeeringResponseTypeDef",
     {
         "Peering": PeeringTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPeeringsResponseTypeDef = TypedDict(
     "ListPeeringsResponseTypeDef",
     {
         "Peerings": List[PeeringTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransitGatewayPeeringTypeDef = TypedDict(
     "TransitGatewayPeeringTypeDef",
     {
         "Peering": PeeringTypeDef,
@@ -3030,40 +2915,40 @@
     total=False,
 )
 
 CreateLinkResponseTypeDef = TypedDict(
     "CreateLinkResponseTypeDef",
     {
         "Link": LinkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLinkResponseTypeDef = TypedDict(
     "DeleteLinkResponseTypeDef",
     {
         "Link": LinkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLinksResponseTypeDef = TypedDict(
     "GetLinksResponseTypeDef",
     {
         "Links": List[LinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLinkResponseTypeDef = TypedDict(
     "UpdateLinkResponseTypeDef",
     {
         "Link": LinkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectPeerTypeDef = TypedDict(
     "ConnectPeerTypeDef",
     {
         "CoreNetworkId": str,
@@ -3079,65 +2964,65 @@
 )
 
 GetNetworkTelemetryResponseTypeDef = TypedDict(
     "GetNetworkTelemetryResponseTypeDef",
     {
         "NetworkTelemetry": List[NetworkTelemetryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkChangeEventsResponseTypeDef = TypedDict(
     "GetCoreNetworkChangeEventsResponseTypeDef",
     {
         "CoreNetworkChangeEvents": List[CoreNetworkChangeEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkChangeSetResponseTypeDef = TypedDict(
     "GetCoreNetworkChangeSetResponseTypeDef",
     {
         "CoreNetworkChanges": List[CoreNetworkChangeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCoreNetworkPolicyVersionResponseTypeDef = TypedDict(
     "DeleteCoreNetworkPolicyVersionResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkPolicyResponseTypeDef = TypedDict(
     "GetCoreNetworkPolicyResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutCoreNetworkPolicyResponseTypeDef = TypedDict(
     "PutCoreNetworkPolicyResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreCoreNetworkPolicyVersionResponseTypeDef = TypedDict(
     "RestoreCoreNetworkPolicyVersionResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetNetworkRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkRoutesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
@@ -3155,116 +3040,114 @@
         "States": Sequence[RouteStateType],
         "Types": Sequence[RouteTypeType],
         "DestinationFilters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
-
 class GetNetworkRoutesRequestRequestTypeDef(
     _RequiredGetNetworkRoutesRequestRequestTypeDef, _OptionalGetNetworkRoutesRequestRequestTypeDef
 ):
     pass
 
-
 CreateCoreNetworkResponseTypeDef = TypedDict(
     "CreateCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCoreNetworkResponseTypeDef = TypedDict(
     "DeleteCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkResponseTypeDef = TypedDict(
     "GetCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCoreNetworkResponseTypeDef = TypedDict(
     "UpdateCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDeviceResponseTypeDef = TypedDict(
     "CreateDeviceResponseTypeDef",
     {
         "Device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDeviceResponseTypeDef = TypedDict(
     "DeleteDeviceResponseTypeDef",
     {
         "Device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDevicesResponseTypeDef = TypedDict(
     "GetDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeviceResponseTypeDef = TypedDict(
     "UpdateDeviceResponseTypeDef",
     {
         "Device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSiteResponseTypeDef = TypedDict(
     "CreateSiteResponseTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSiteResponseTypeDef = TypedDict(
     "DeleteSiteResponseTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSitesResponseTypeDef = TypedDict(
     "GetSitesResponseTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteResponseTypeDef = TypedDict(
     "UpdateSiteResponseTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RouteAnalysisPathTypeDef = TypedDict(
     "RouteAnalysisPathTypeDef",
     {
         "CompletionStatus": RouteAnalysisCompletionTypeDef,
@@ -3277,64 +3160,64 @@
     "GetNetworkRoutesResponseTypeDef",
     {
         "RouteTableArn": str,
         "CoreNetworkSegmentEdge": CoreNetworkSegmentEdgeIdentifierTypeDef,
         "RouteTableType": RouteTableTypeType,
         "RouteTableTimestamp": datetime,
         "NetworkRoutes": List[NetworkRouteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterTransitGatewayResponseTypeDef = TypedDict(
     "DeregisterTransitGatewayResponseTypeDef",
     {
         "TransitGatewayRegistration": TransitGatewayRegistrationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayRegistrationsResponseTypeDef = TypedDict(
     "GetTransitGatewayRegistrationsResponseTypeDef",
     {
         "TransitGatewayRegistrations": List[TransitGatewayRegistrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTransitGatewayResponseTypeDef = TypedDict(
     "RegisterTransitGatewayResponseTypeDef",
     {
         "TransitGatewayRegistration": TransitGatewayRegistrationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitGatewayPeeringResponseTypeDef = TypedDict(
     "CreateTransitGatewayPeeringResponseTypeDef",
     {
         "TransitGatewayPeering": TransitGatewayPeeringTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayPeeringResponseTypeDef = TypedDict(
     "GetTransitGatewayPeeringResponseTypeDef",
     {
         "TransitGatewayPeering": TransitGatewayPeeringTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptAttachmentResponseTypeDef = TypedDict(
     "AcceptAttachmentResponseTypeDef",
     {
         "Attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectAttachmentTypeDef = TypedDict(
     "ConnectAttachmentTypeDef",
     {
         "Attachment": AttachmentTypeDef,
@@ -3344,32 +3227,32 @@
     total=False,
 )
 
 DeleteAttachmentResponseTypeDef = TypedDict(
     "DeleteAttachmentResponseTypeDef",
     {
         "Attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachmentsResponseTypeDef = TypedDict(
     "ListAttachmentsResponseTypeDef",
     {
         "Attachments": List[AttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectAttachmentResponseTypeDef = TypedDict(
     "RejectAttachmentResponseTypeDef",
     {
         "Attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SiteToSiteVpnAttachmentTypeDef = TypedDict(
     "SiteToSiteVpnAttachmentTypeDef",
     {
         "Attachment": AttachmentTypeDef,
@@ -3398,31 +3281,31 @@
     total=False,
 )
 
 CreateConnectPeerResponseTypeDef = TypedDict(
     "CreateConnectPeerResponseTypeDef",
     {
         "ConnectPeer": ConnectPeerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConnectPeerResponseTypeDef = TypedDict(
     "DeleteConnectPeerResponseTypeDef",
     {
         "ConnectPeer": ConnectPeerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectPeerResponseTypeDef = TypedDict(
     "GetConnectPeerResponseTypeDef",
     {
         "ConnectPeer": ConnectPeerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RouteAnalysisTypeDef = TypedDict(
     "RouteAnalysisTypeDef",
     {
         "GlobalNetworkId": str,
@@ -3440,90 +3323,90 @@
     total=False,
 )
 
 CreateConnectAttachmentResponseTypeDef = TypedDict(
     "CreateConnectAttachmentResponseTypeDef",
     {
         "ConnectAttachment": ConnectAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectAttachmentResponseTypeDef = TypedDict(
     "GetConnectAttachmentResponseTypeDef",
     {
         "ConnectAttachment": ConnectAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSiteToSiteVpnAttachmentResponseTypeDef = TypedDict(
     "CreateSiteToSiteVpnAttachmentResponseTypeDef",
     {
         "SiteToSiteVpnAttachment": SiteToSiteVpnAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteToSiteVpnAttachmentResponseTypeDef = TypedDict(
     "GetSiteToSiteVpnAttachmentResponseTypeDef",
     {
         "SiteToSiteVpnAttachment": SiteToSiteVpnAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitGatewayRouteTableAttachmentResponseTypeDef = TypedDict(
     "CreateTransitGatewayRouteTableAttachmentResponseTypeDef",
     {
         "TransitGatewayRouteTableAttachment": TransitGatewayRouteTableAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayRouteTableAttachmentResponseTypeDef = TypedDict(
     "GetTransitGatewayRouteTableAttachmentResponseTypeDef",
     {
         "TransitGatewayRouteTableAttachment": TransitGatewayRouteTableAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVpcAttachmentResponseTypeDef = TypedDict(
     "CreateVpcAttachmentResponseTypeDef",
     {
         "VpcAttachment": VpcAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcAttachmentResponseTypeDef = TypedDict(
     "GetVpcAttachmentResponseTypeDef",
     {
         "VpcAttachment": VpcAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcAttachmentResponseTypeDef = TypedDict(
     "UpdateVpcAttachmentResponseTypeDef",
     {
         "VpcAttachment": VpcAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteAnalysisResponseTypeDef = TypedDict(
     "GetRouteAnalysisResponseTypeDef",
     {
         "RouteAnalysis": RouteAnalysisTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRouteAnalysisResponseTypeDef = TypedDict(
     "StartRouteAnalysisResponseTypeDef",
     {
         "RouteAnalysis": RouteAnalysisTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager/type_defs.pyi` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_networkmanager.type_defs import AWSLocationTypeDef
 
-    data: AWSLocationTypeDef = {...}
+    data: AWSLocationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import (
@@ -51,17 +51,19 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AWSLocationTypeDef",
     "AcceptAttachmentRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "AccountStatusTypeDef",
     "AssociateConnectPeerRequestRequestTypeDef",
     "ConnectPeerAssociationTypeDef",
     "AssociateCustomerGatewayRequestRequestTypeDef",
     "CustomerGatewayAssociationTypeDef",
     "AssociateLinkRequestRequestTypeDef",
     "LinkAssociationTypeDef",
@@ -90,95 +92,73 @@
     "DeleteDeviceRequestRequestTypeDef",
     "DeleteGlobalNetworkRequestRequestTypeDef",
     "DeleteLinkRequestRequestTypeDef",
     "DeletePeeringRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSiteRequestRequestTypeDef",
     "DeregisterTransitGatewayRequestRequestTypeDef",
-    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeGlobalNetworksRequestRequestTypeDef",
     "DisassociateConnectPeerRequestRequestTypeDef",
     "DisassociateCustomerGatewayRequestRequestTypeDef",
     "DisassociateLinkRequestRequestTypeDef",
     "DisassociateTransitGatewayConnectPeerRequestRequestTypeDef",
     "ExecuteCoreNetworkChangeSetRequestRequestTypeDef",
     "GetConnectAttachmentRequestRequestTypeDef",
-    "GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
     "GetConnectPeerAssociationsRequestRequestTypeDef",
     "GetConnectPeerRequestRequestTypeDef",
-    "GetConnectionsRequestGetConnectionsPaginateTypeDef",
     "GetConnectionsRequestRequestTypeDef",
-    "GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
     "GetCoreNetworkChangeEventsRequestRequestTypeDef",
-    "GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
     "GetCoreNetworkChangeSetRequestRequestTypeDef",
     "GetCoreNetworkPolicyRequestRequestTypeDef",
     "GetCoreNetworkRequestRequestTypeDef",
-    "GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
     "GetCustomerGatewayAssociationsRequestRequestTypeDef",
-    "GetDevicesRequestGetDevicesPaginateTypeDef",
     "GetDevicesRequestRequestTypeDef",
-    "GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
     "GetLinkAssociationsRequestRequestTypeDef",
-    "GetLinksRequestGetLinksPaginateTypeDef",
     "GetLinksRequestRequestTypeDef",
-    "GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
     "GetNetworkResourceCountsRequestRequestTypeDef",
     "NetworkResourceCountTypeDef",
-    "GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
     "GetNetworkResourceRelationshipsRequestRequestTypeDef",
     "RelationshipTypeDef",
-    "GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
     "GetNetworkResourcesRequestRequestTypeDef",
-    "GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
     "GetNetworkTelemetryRequestRequestTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetRouteAnalysisRequestRequestTypeDef",
     "GetSiteToSiteVpnAttachmentRequestRequestTypeDef",
-    "GetSitesRequestGetSitesPaginateTypeDef",
     "GetSitesRequestRequestTypeDef",
-    "GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
     "GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef",
     "GetTransitGatewayPeeringRequestRequestTypeDef",
-    "GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
     "GetTransitGatewayRegistrationsRequestRequestTypeDef",
     "GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef",
     "GetVpcAttachmentRequestRequestTypeDef",
-    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
     "ListAttachmentsRequestRequestTypeDef",
-    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
     "ListConnectPeersRequestRequestTypeDef",
-    "ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
     "ListCoreNetworkPolicyVersionsRequestRequestTypeDef",
-    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
     "ListCoreNetworksRequestRequestTypeDef",
     "ListOrganizationServiceAccessStatusRequestRequestTypeDef",
-    "ListPeeringsRequestListPeeringsPaginateTypeDef",
     "ListPeeringsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "NetworkResourceSummaryTypeDef",
     "NetworkRouteDestinationTypeDef",
-    "PaginatorConfigTypeDef",
     "PutCoreNetworkPolicyRequestRequestTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
     "RegisterTransitGatewayRequestRequestTypeDef",
     "RejectAttachmentRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreCoreNetworkPolicyVersionRequestRequestTypeDef",
     "RouteAnalysisCompletionTypeDef",
     "RouteAnalysisEndpointOptionsSpecificationTypeDef",
     "RouteAnalysisEndpointOptionsTypeDef",
     "StartOrganizationServiceAccessUpdateRequestRequestTypeDef",
     "TransitGatewayRegistrationStateReasonTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateCoreNetworkRequestRequestTypeDef",
     "UpdateGlobalNetworkRequestRequestTypeDef",
     "UpdateNetworkResourceMetadataRequestRequestTypeDef",
+    "GetResourcePolicyResponseTypeDef",
     "UpdateNetworkResourceMetadataResponseTypeDef",
     "OrganizationStatusTypeDef",
     "AssociateConnectPeerResponseTypeDef",
     "DisassociateConnectPeerResponseTypeDef",
     "GetConnectPeerAssociationsResponseTypeDef",
     "AssociateCustomerGatewayResponseTypeDef",
     "DisassociateCustomerGatewayResponseTypeDef",
@@ -221,14 +201,35 @@
     "CreateSiteRequestRequestTypeDef",
     "DeviceTypeDef",
     "SiteTypeDef",
     "UpdateDeviceRequestRequestTypeDef",
     "UpdateSiteRequestRequestTypeDef",
     "CreateVpcAttachmentRequestRequestTypeDef",
     "UpdateVpcAttachmentRequestRequestTypeDef",
+    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+    "GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
+    "GetConnectionsRequestGetConnectionsPaginateTypeDef",
+    "GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
+    "GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
+    "GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
+    "GetDevicesRequestGetDevicesPaginateTypeDef",
+    "GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
+    "GetLinksRequestGetLinksPaginateTypeDef",
+    "GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
+    "GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
+    "GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
+    "GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
+    "GetSitesRequestGetSitesPaginateTypeDef",
+    "GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
+    "GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
+    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
+    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
+    "ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
+    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
+    "ListPeeringsRequestListPeeringsPaginateTypeDef",
     "GetNetworkResourceCountsResponseTypeDef",
     "GetNetworkResourceRelationshipsResponseTypeDef",
     "PathComponentTypeDef",
     "NetworkRouteTypeDef",
     "StartRouteAnalysisRequestRequestTypeDef",
     "TransitGatewayRegistrationTypeDef",
     "ListOrganizationServiceAccessStatusResponseTypeDef",
@@ -317,14 +318,25 @@
 AcceptAttachmentRequestRequestTypeDef = TypedDict(
     "AcceptAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
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
 AccountStatusTypeDef = TypedDict(
     "AccountStatusTypeDef",
     {
         "AccountId": str,
         "SLRDeploymentStatus": str,
     },
     total=False,
@@ -342,20 +354,22 @@
     "_OptionalAssociateConnectPeerRequestRequestTypeDef",
     {
         "LinkId": str,
     },
     total=False,
 )
 
+
 class AssociateConnectPeerRequestRequestTypeDef(
     _RequiredAssociateConnectPeerRequestRequestTypeDef,
     _OptionalAssociateConnectPeerRequestRequestTypeDef,
 ):
     pass
 
+
 ConnectPeerAssociationTypeDef = TypedDict(
     "ConnectPeerAssociationTypeDef",
     {
         "ConnectPeerId": str,
         "GlobalNetworkId": str,
         "DeviceId": str,
         "LinkId": str,
@@ -376,20 +390,22 @@
     "_OptionalAssociateCustomerGatewayRequestRequestTypeDef",
     {
         "LinkId": str,
     },
     total=False,
 )
 
+
 class AssociateCustomerGatewayRequestRequestTypeDef(
     _RequiredAssociateCustomerGatewayRequestRequestTypeDef,
     _OptionalAssociateCustomerGatewayRequestRequestTypeDef,
 ):
     pass
 
+
 CustomerGatewayAssociationTypeDef = TypedDict(
     "CustomerGatewayAssociationTypeDef",
     {
         "CustomerGatewayArn": str,
         "GlobalNetworkId": str,
         "DeviceId": str,
         "LinkId": str,
@@ -430,20 +446,22 @@
     "_OptionalAssociateTransitGatewayConnectPeerRequestRequestTypeDef",
     {
         "LinkId": str,
     },
     total=False,
 )
 
+
 class AssociateTransitGatewayConnectPeerRequestRequestTypeDef(
     _RequiredAssociateTransitGatewayConnectPeerRequestRequestTypeDef,
     _OptionalAssociateTransitGatewayConnectPeerRequestRequestTypeDef,
 ):
     pass
 
+
 TransitGatewayConnectPeerAssociationTypeDef = TypedDict(
     "TransitGatewayConnectPeerAssociationTypeDef",
     {
         "TransitGatewayConnectPeerArn": str,
         "GlobalNetworkId": str,
         "DeviceId": str,
         "LinkId": str,
@@ -553,19 +571,21 @@
     "_OptionalCoreNetworkPolicyErrorTypeDef",
     {
         "Path": str,
     },
     total=False,
 )
 
+
 class CoreNetworkPolicyErrorTypeDef(
     _RequiredCoreNetworkPolicyErrorTypeDef, _OptionalCoreNetworkPolicyErrorTypeDef
 ):
     pass
 
+
 CoreNetworkPolicyVersionTypeDef = TypedDict(
     "CoreNetworkPolicyVersionTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
         "Alias": CoreNetworkPolicyAliasType,
         "Description": str,
@@ -700,19 +720,20 @@
     "DeregisterTransitGatewayRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "TransitGatewayArn": str,
     },
 )
 
-DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef = TypedDict(
-    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "GlobalNetworkIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeGlobalNetworksRequestRequestTypeDef = TypedDict(
     "DescribeGlobalNetworksRequestRequestTypeDef",
     {
@@ -767,35 +788,14 @@
 GetConnectAttachmentRequestRequestTypeDef = TypedDict(
     "GetConnectAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
-_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
-    {
-        "ConnectPeerIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef(
-    _RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
-    _OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectPeerAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
@@ -804,49 +804,29 @@
         "ConnectPeerIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConnectPeerAssociationsRequestRequestTypeDef(
     _RequiredGetConnectPeerAssociationsRequestRequestTypeDef,
     _OptionalGetConnectPeerAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 GetConnectPeerRequestRequestTypeDef = TypedDict(
     "GetConnectPeerRequestRequestTypeDef",
     {
         "ConnectPeerId": str,
     },
 )
 
-_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
-    "_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
-    "_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef",
-    {
-        "ConnectionIds": Sequence[str],
-        "DeviceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetConnectionsRequestGetConnectionsPaginateTypeDef(
-    _RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef,
-    _OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetConnectionsRequestRequestTypeDef = TypedDict(
     "_RequiredGetConnectionsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetConnectionsRequestRequestTypeDef = TypedDict(
@@ -856,39 +836,20 @@
         "DeviceId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetConnectionsRequestRequestTypeDef(
     _RequiredGetConnectionsRequestRequestTypeDef, _OptionalGetConnectionsRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
-    "_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "PolicyVersionId": int,
-    },
-)
-_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
-    "_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef(
-    _RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
-    _OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetCoreNetworkChangeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCoreNetworkChangeEventsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
     },
@@ -898,40 +859,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetCoreNetworkChangeEventsRequestRequestTypeDef(
     _RequiredGetCoreNetworkChangeEventsRequestRequestTypeDef,
     _OptionalGetCoreNetworkChangeEventsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
-    "_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "PolicyVersionId": int,
-    },
-)
-_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
-    "_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef(
-    _RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
-    _OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
-):
-    pass
 
 _RequiredGetCoreNetworkChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredGetCoreNetworkChangeSetRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
     },
@@ -941,20 +883,22 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetCoreNetworkChangeSetRequestRequestTypeDef(
     _RequiredGetCoreNetworkChangeSetRequestRequestTypeDef,
     _OptionalGetCoreNetworkChangeSetRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredGetCoreNetworkPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredGetCoreNetworkPolicyRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 _OptionalGetCoreNetworkPolicyRequestRequestTypeDef = TypedDict(
@@ -962,48 +906,29 @@
     {
         "PolicyVersionId": int,
         "Alias": CoreNetworkPolicyAliasType,
     },
     total=False,
 )
 
+
 class GetCoreNetworkPolicyRequestRequestTypeDef(
     _RequiredGetCoreNetworkPolicyRequestRequestTypeDef,
     _OptionalGetCoreNetworkPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 GetCoreNetworkRequestRequestTypeDef = TypedDict(
     "GetCoreNetworkRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 
-_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
-    {
-        "CustomerGatewayArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef(
-    _RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
-    _OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetCustomerGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetCustomerGatewayAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetCustomerGatewayAssociationsRequestRequestTypeDef = TypedDict(
@@ -1012,41 +937,21 @@
         "CustomerGatewayArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetCustomerGatewayAssociationsRequestRequestTypeDef(
     _RequiredGetCustomerGatewayAssociationsRequestRequestTypeDef,
     _OptionalGetCustomerGatewayAssociationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
-    "_RequiredGetDevicesRequestGetDevicesPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
-    "_OptionalGetDevicesRequestGetDevicesPaginateTypeDef",
-    {
-        "DeviceIds": Sequence[str],
-        "SiteId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDevicesRequestGetDevicesPaginateTypeDef(
-    _RequiredGetDevicesRequestGetDevicesPaginateTypeDef,
-    _OptionalGetDevicesRequestGetDevicesPaginateTypeDef,
-):
-    pass
 
 _RequiredGetDevicesRequestRequestTypeDef = TypedDict(
     "_RequiredGetDevicesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
@@ -1057,40 +962,20 @@
         "SiteId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetDevicesRequestRequestTypeDef(
     _RequiredGetDevicesRequestRequestTypeDef, _OptionalGetDevicesRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
-    {
-        "DeviceId": str,
-        "LinkId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef(
-    _RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
-    _OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetLinkAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetLinkAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
@@ -1101,42 +986,21 @@
         "LinkId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetLinkAssociationsRequestRequestTypeDef(
     _RequiredGetLinkAssociationsRequestRequestTypeDef,
     _OptionalGetLinkAssociationsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
-    "_RequiredGetLinksRequestGetLinksPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
-    "_OptionalGetLinksRequestGetLinksPaginateTypeDef",
-    {
-        "LinkIds": Sequence[str],
-        "SiteId": str,
-        "Type": str,
-        "Provider": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetLinksRequestGetLinksPaginateTypeDef(
-    _RequiredGetLinksRequestGetLinksPaginateTypeDef, _OptionalGetLinksRequestGetLinksPaginateTypeDef
-):
-    pass
 
 _RequiredGetLinksRequestRequestTypeDef = TypedDict(
     "_RequiredGetLinksRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
@@ -1149,39 +1013,20 @@
         "Provider": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetLinksRequestRequestTypeDef(
     _RequiredGetLinksRequestRequestTypeDef, _OptionalGetLinksRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
-    {
-        "ResourceType": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef(
-    _RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
-    _OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetNetworkResourceCountsRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkResourceCountsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
@@ -1191,55 +1036,31 @@
         "ResourceType": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetNetworkResourceCountsRequestRequestTypeDef(
     _RequiredGetNetworkResourceCountsRequestRequestTypeDef,
     _OptionalGetNetworkResourceCountsRequestRequestTypeDef,
 ):
     pass
 
+
 NetworkResourceCountTypeDef = TypedDict(
     "NetworkResourceCountTypeDef",
     {
         "ResourceType": str,
         "Count": int,
     },
     total=False,
 )
 
-_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "RegisteredGatewayArn": str,
-        "AwsRegion": str,
-        "AccountId": str,
-        "ResourceType": str,
-        "ResourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef(
-    _RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
-    _OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetNetworkResourceRelationshipsRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkResourceRelationshipsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetNetworkResourceRelationshipsRequestRequestTypeDef = TypedDict(
@@ -1253,55 +1074,31 @@
         "ResourceArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetNetworkResourceRelationshipsRequestRequestTypeDef(
     _RequiredGetNetworkResourceRelationshipsRequestRequestTypeDef,
     _OptionalGetNetworkResourceRelationshipsRequestRequestTypeDef,
 ):
     pass
 
+
 RelationshipTypeDef = TypedDict(
     "RelationshipTypeDef",
     {
         "From": str,
         "To": str,
     },
     total=False,
 )
 
-_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "RegisteredGatewayArn": str,
-        "AwsRegion": str,
-        "AccountId": str,
-        "ResourceType": str,
-        "ResourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef(
-    _RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
-    _OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetNetworkResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkResourcesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetNetworkResourcesRequestRequestTypeDef = TypedDict(
@@ -1315,45 +1112,21 @@
         "ResourceArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetNetworkResourcesRequestRequestTypeDef(
     _RequiredGetNetworkResourcesRequestRequestTypeDef,
     _OptionalGetNetworkResourcesRequestRequestTypeDef,
 ):
     pass
 
-_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
-    "_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
-    "_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "RegisteredGatewayArn": str,
-        "AwsRegion": str,
-        "AccountId": str,
-        "ResourceType": str,
-        "ResourceArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef(
-    _RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
-    _OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
-):
-    pass
 
 _RequiredGetNetworkTelemetryRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkTelemetryRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
@@ -1368,35 +1141,29 @@
         "ResourceArn": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetNetworkTelemetryRequestRequestTypeDef(
     _RequiredGetNetworkTelemetryRequestRequestTypeDef,
     _OptionalGetNetworkTelemetryRequestRequestTypeDef,
 ):
     pass
 
+
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "PolicyDocument": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetRouteAnalysisRequestRequestTypeDef = TypedDict(
     "GetRouteAnalysisRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "RouteAnalysisId": str,
     },
 )
@@ -1404,34 +1171,14 @@
 GetSiteToSiteVpnAttachmentRequestRequestTypeDef = TypedDict(
     "GetSiteToSiteVpnAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
-_RequiredGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
-    "_RequiredGetSitesRequestGetSitesPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
-    "_OptionalGetSitesRequestGetSitesPaginateTypeDef",
-    {
-        "SiteIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetSitesRequestGetSitesPaginateTypeDef(
-    _RequiredGetSitesRequestGetSitesPaginateTypeDef, _OptionalGetSitesRequestGetSitesPaginateTypeDef
-):
-    pass
-
 _RequiredGetSitesRequestRequestTypeDef = TypedDict(
     "_RequiredGetSitesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetSitesRequestRequestTypeDef = TypedDict(
@@ -1440,39 +1187,20 @@
         "SiteIds": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetSitesRequestRequestTypeDef(
     _RequiredGetSitesRequestRequestTypeDef, _OptionalGetSitesRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
-    "_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
-    {
-        "TransitGatewayConnectPeerArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef(
-    _RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
-    _OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
@@ -1482,48 +1210,29 @@
         "TransitGatewayConnectPeerArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef(
     _RequiredGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
     _OptionalGetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
 ):
     pass
 
+
 GetTransitGatewayPeeringRequestRequestTypeDef = TypedDict(
     "GetTransitGatewayPeeringRequestRequestTypeDef",
     {
         "PeeringId": str,
     },
 )
 
-_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
-    {
-        "GlobalNetworkId": str,
-    },
-)
-_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
-    {
-        "TransitGatewayArns": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef(
-    _RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
-    _OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTransitGatewayRegistrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetTransitGatewayRegistrationsRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalGetTransitGatewayRegistrationsRequestRequestTypeDef = TypedDict(
@@ -1532,104 +1241,60 @@
         "TransitGatewayArns": Sequence[str],
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetTransitGatewayRegistrationsRequestRequestTypeDef(
     _RequiredGetTransitGatewayRegistrationsRequestRequestTypeDef,
     _OptionalGetTransitGatewayRegistrationsRequestRequestTypeDef,
 ):
     pass
 
+
 GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef = TypedDict(
     "GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
 GetVpcAttachmentRequestRequestTypeDef = TypedDict(
     "GetVpcAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 
-ListAttachmentsRequestListAttachmentsPaginateTypeDef = TypedDict(
-    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "AttachmentType": AttachmentTypeType,
-        "EdgeLocation": str,
-        "State": AttachmentStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListAttachmentsRequestRequestTypeDef = TypedDict(
     "ListAttachmentsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "AttachmentType": AttachmentTypeType,
         "EdgeLocation": str,
         "State": AttachmentStateType,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListConnectPeersRequestListConnectPeersPaginateTypeDef = TypedDict(
-    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "ConnectAttachmentId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListConnectPeersRequestRequestTypeDef = TypedDict(
     "ListConnectPeersRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "ConnectAttachmentId": str,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
-    TypedDict(
-        "_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
-        {
-            "CoreNetworkId": str,
-        },
-    )
-)
-_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
-    TypedDict(
-        "_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
-        {
-            "PaginationConfig": "PaginatorConfigTypeDef",
-        },
-        total=False,
-    )
-)
-
-class ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef(
-    _RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
-    _OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListCoreNetworkPolicyVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListCoreNetworkPolicyVersionsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 _OptionalListCoreNetworkPolicyVersionsRequestRequestTypeDef = TypedDict(
@@ -1637,27 +1302,21 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListCoreNetworkPolicyVersionsRequestRequestTypeDef(
     _RequiredListCoreNetworkPolicyVersionsRequestRequestTypeDef,
     _OptionalListCoreNetworkPolicyVersionsRequestRequestTypeDef,
 ):
     pass
 
-ListCoreNetworksRequestListCoreNetworksPaginateTypeDef = TypedDict(
-    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListCoreNetworksRequestRequestTypeDef = TypedDict(
     "ListCoreNetworksRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
@@ -1669,26 +1328,14 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListPeeringsRequestListPeeringsPaginateTypeDef = TypedDict(
-    "ListPeeringsRequestListPeeringsPaginateTypeDef",
-    {
-        "CoreNetworkId": str,
-        "PeeringType": Literal["TRANSIT_GATEWAY"],
-        "EdgeLocation": str,
-        "State": PeeringStateType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPeeringsRequestRequestTypeDef = TypedDict(
     "ListPeeringsRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PeeringType": Literal["TRANSIT_GATEWAY"],
         "EdgeLocation": str,
         "State": PeeringStateType,
@@ -1727,24 +1374,14 @@
         "EdgeLocation": str,
         "ResourceType": str,
         "ResourceId": str,
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
 _RequiredPutCoreNetworkPolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutCoreNetworkPolicyRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyDocument": str,
     },
 )
@@ -1754,20 +1391,22 @@
         "Description": str,
         "LatestVersionId": int,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class PutCoreNetworkPolicyRequestRequestTypeDef(
     _RequiredPutCoreNetworkPolicyRequestRequestTypeDef,
     _OptionalPutCoreNetworkPolicyRequestRequestTypeDef,
 ):
     pass
 
+
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "PolicyDocument": str,
         "ResourceArn": str,
     },
 )
@@ -1783,25 +1422,14 @@
 RejectAttachmentRequestRequestTypeDef = TypedDict(
     "RejectAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
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
 RestoreCoreNetworkPolicyVersionRequestRequestTypeDef = TypedDict(
     "RestoreCoreNetworkPolicyVersionRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "PolicyVersionId": int,
     },
 )
@@ -1872,73 +1500,87 @@
         "LinkId": str,
         "ConnectedLinkId": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateConnectionRequestRequestTypeDef(
     _RequiredUpdateConnectionRequestRequestTypeDef, _OptionalUpdateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateCoreNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateCoreNetworkRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
     },
 )
 _OptionalUpdateCoreNetworkRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateCoreNetworkRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateCoreNetworkRequestRequestTypeDef(
     _RequiredUpdateCoreNetworkRequestRequestTypeDef, _OptionalUpdateCoreNetworkRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateGlobalNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateGlobalNetworkRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalUpdateGlobalNetworkRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateGlobalNetworkRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateGlobalNetworkRequestRequestTypeDef(
     _RequiredUpdateGlobalNetworkRequestRequestTypeDef,
     _OptionalUpdateGlobalNetworkRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateNetworkResourceMetadataRequestRequestTypeDef = TypedDict(
     "UpdateNetworkResourceMetadataRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "ResourceArn": str,
         "Metadata": Mapping[str, str],
     },
 )
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "PolicyDocument": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateNetworkResourceMetadataResponseTypeDef = TypedDict(
     "UpdateNetworkResourceMetadataResponseTypeDef",
     {
         "ResourceArn": str,
         "Metadata": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OrganizationStatusTypeDef = TypedDict(
     "OrganizationStatusTypeDef",
     {
         "OrganizationId": str,
@@ -1949,107 +1591,107 @@
     total=False,
 )
 
 AssociateConnectPeerResponseTypeDef = TypedDict(
     "AssociateConnectPeerResponseTypeDef",
     {
         "ConnectPeerAssociation": ConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateConnectPeerResponseTypeDef = TypedDict(
     "DisassociateConnectPeerResponseTypeDef",
     {
         "ConnectPeerAssociation": ConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectPeerAssociationsResponseTypeDef = TypedDict(
     "GetConnectPeerAssociationsResponseTypeDef",
     {
         "ConnectPeerAssociations": List[ConnectPeerAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateCustomerGatewayResponseTypeDef = TypedDict(
     "AssociateCustomerGatewayResponseTypeDef",
     {
         "CustomerGatewayAssociation": CustomerGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateCustomerGatewayResponseTypeDef = TypedDict(
     "DisassociateCustomerGatewayResponseTypeDef",
     {
         "CustomerGatewayAssociation": CustomerGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCustomerGatewayAssociationsResponseTypeDef = TypedDict(
     "GetCustomerGatewayAssociationsResponseTypeDef",
     {
         "CustomerGatewayAssociations": List[CustomerGatewayAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateLinkResponseTypeDef = TypedDict(
     "AssociateLinkResponseTypeDef",
     {
         "LinkAssociation": LinkAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateLinkResponseTypeDef = TypedDict(
     "DisassociateLinkResponseTypeDef",
     {
         "LinkAssociation": LinkAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLinkAssociationsResponseTypeDef = TypedDict(
     "GetLinkAssociationsResponseTypeDef",
     {
         "LinkAssociations": List[LinkAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateTransitGatewayConnectPeerResponseTypeDef = TypedDict(
     "AssociateTransitGatewayConnectPeerResponseTypeDef",
     {
         "TransitGatewayConnectPeerAssociation": TransitGatewayConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateTransitGatewayConnectPeerResponseTypeDef = TypedDict(
     "DisassociateTransitGatewayConnectPeerResponseTypeDef",
     {
         "TransitGatewayConnectPeerAssociation": TransitGatewayConnectPeerAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayConnectPeerAssociationsResponseTypeDef = TypedDict(
     "GetTransitGatewayConnectPeerAssociationsResponseTypeDef",
     {
         "TransitGatewayConnectPeerAssociations": List[TransitGatewayConnectPeerAssociationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectPeerSummaryTypeDef = TypedDict(
     "ConnectPeerSummaryTypeDef",
     {
         "CoreNetworkId": str,
@@ -2110,19 +1752,21 @@
         "ConnectedLinkId": str,
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateConnectionRequestRequestTypeDef(
     _RequiredCreateConnectionRequestRequestTypeDef, _OptionalCreateConnectionRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateCoreNetworkRequestRequestTypeDef = TypedDict(
     "_RequiredCreateCoreNetworkRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalCreateCoreNetworkRequestRequestTypeDef = TypedDict(
@@ -2132,19 +1776,21 @@
         "Tags": Sequence[TagTypeDef],
         "PolicyDocument": str,
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateCoreNetworkRequestRequestTypeDef(
     _RequiredCreateCoreNetworkRequestRequestTypeDef, _OptionalCreateCoreNetworkRequestRequestTypeDef
 ):
     pass
 
+
 CreateGlobalNetworkRequestRequestTypeDef = TypedDict(
     "CreateGlobalNetworkRequestRequestTypeDef",
     {
         "Description": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
@@ -2162,20 +1808,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateSiteToSiteVpnAttachmentRequestRequestTypeDef(
     _RequiredCreateSiteToSiteVpnAttachmentRequestRequestTypeDef,
     _OptionalCreateSiteToSiteVpnAttachmentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateTransitGatewayPeeringRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransitGatewayPeeringRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "TransitGatewayArn": str,
     },
 )
@@ -2184,20 +1832,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateTransitGatewayPeeringRequestRequestTypeDef(
     _RequiredCreateTransitGatewayPeeringRequestRequestTypeDef,
     _OptionalCreateTransitGatewayPeeringRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef",
     {
         "PeeringId": str,
         "TransitGatewayRouteTableArn": str,
     },
 )
@@ -2206,20 +1856,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef(
     _RequiredCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
     _OptionalCreateTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
 ):
     pass
 
+
 GlobalNetworkTypeDef = TypedDict(
     "GlobalNetworkTypeDef",
     {
         "GlobalNetworkId": str,
         "GlobalNetworkArn": str,
         "Description": str,
         "CreatedAt": datetime,
@@ -2229,15 +1881,15 @@
     total=False,
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 NetworkResourceTypeDef = TypedDict(
     "NetworkResourceTypeDef",
     {
         "RegisteredGatewayArn": str,
@@ -2305,19 +1957,21 @@
         "Type": str,
         "Provider": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateLinkRequestRequestTypeDef(
     _RequiredCreateLinkRequestRequestTypeDef, _OptionalCreateLinkRequestRequestTypeDef
 ):
     pass
 
+
 LinkTypeDef = TypedDict(
     "LinkTypeDef",
     {
         "LinkId": str,
         "LinkArn": str,
         "GlobalNetworkId": str,
         "SiteId": str,
@@ -2346,19 +2000,21 @@
         "Type": str,
         "Bandwidth": BandwidthTypeDef,
         "Provider": str,
     },
     total=False,
 )
 
+
 class UpdateLinkRequestRequestTypeDef(
     _RequiredUpdateLinkRequestRequestTypeDef, _OptionalUpdateLinkRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateConnectPeerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectPeerRequestRequestTypeDef",
     {
         "ConnectAttachmentId": str,
         "PeerAddress": str,
         "InsideCidrBlocks": Sequence[str],
     },
@@ -2370,19 +2026,21 @@
         "BgpOptions": BgpOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateConnectPeerRequestRequestTypeDef(
     _RequiredCreateConnectPeerRequestRequestTypeDef, _OptionalCreateConnectPeerRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateConnectAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateConnectAttachmentRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "EdgeLocation": str,
         "TransportAttachmentId": str,
         "Options": ConnectAttachmentOptionsTypeDef,
@@ -2393,20 +2051,22 @@
     {
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateConnectAttachmentRequestRequestTypeDef(
     _RequiredCreateConnectAttachmentRequestRequestTypeDef,
     _OptionalCreateConnectAttachmentRequestRequestTypeDef,
 ):
     pass
 
+
 ConnectPeerConfigurationTypeDef = TypedDict(
     "ConnectPeerConfigurationTypeDef",
     {
         "CoreNetworkAddress": str,
         "PeerAddress": str,
         "InsideCidrBlocks": List[str],
         "Protocol": Literal["GRE"],
@@ -2473,15 +2133,15 @@
 )
 
 ListCoreNetworkPolicyVersionsResponseTypeDef = TypedDict(
     "ListCoreNetworkPolicyVersionsResponseTypeDef",
     {
         "CoreNetworkPolicyVersions": List[CoreNetworkPolicyVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RouteTableIdentifierTypeDef = TypedDict(
     "RouteTableIdentifierTypeDef",
     {
         "TransitGatewayRouteTableArn": str,
@@ -2524,19 +2184,21 @@
         "Location": LocationTypeDef,
         "SiteId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDeviceRequestRequestTypeDef(
     _RequiredCreateDeviceRequestRequestTypeDef, _OptionalCreateDeviceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSiteRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
     },
 )
 _OptionalCreateSiteRequestRequestTypeDef = TypedDict(
@@ -2545,19 +2207,21 @@
         "Description": str,
         "Location": LocationTypeDef,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateSiteRequestRequestTypeDef(
     _RequiredCreateSiteRequestRequestTypeDef, _OptionalCreateSiteRequestRequestTypeDef
 ):
     pass
 
+
 DeviceTypeDef = TypedDict(
     "DeviceTypeDef",
     {
         "DeviceId": str,
         "DeviceArn": str,
         "GlobalNetworkId": str,
         "AWSLocation": AWSLocationTypeDef,
@@ -2608,19 +2272,21 @@
         "SerialNumber": str,
         "Location": LocationTypeDef,
         "SiteId": str,
     },
     total=False,
 )
 
+
 class UpdateDeviceRequestRequestTypeDef(
     _RequiredUpdateDeviceRequestRequestTypeDef, _OptionalUpdateDeviceRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateSiteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSiteRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
         "SiteId": str,
     },
 )
@@ -2629,19 +2295,21 @@
     {
         "Description": str,
         "Location": LocationTypeDef,
     },
     total=False,
 )
 
+
 class UpdateSiteRequestRequestTypeDef(
     _RequiredUpdateSiteRequestRequestTypeDef, _OptionalUpdateSiteRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateVpcAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateVpcAttachmentRequestRequestTypeDef",
     {
         "CoreNetworkId": str,
         "VpcArn": str,
         "SubnetArns": Sequence[str],
     },
@@ -2652,20 +2320,22 @@
         "Options": VpcOptionsTypeDef,
         "Tags": Sequence[TagTypeDef],
         "ClientToken": str,
     },
     total=False,
 )
 
+
 class CreateVpcAttachmentRequestRequestTypeDef(
     _RequiredCreateVpcAttachmentRequestRequestTypeDef,
     _OptionalCreateVpcAttachmentRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateVpcAttachmentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
     },
 )
 _OptionalUpdateVpcAttachmentRequestRequestTypeDef = TypedDict(
@@ -2674,35 +2344,478 @@
         "AddSubnetArns": Sequence[str],
         "RemoveSubnetArns": Sequence[str],
         "Options": VpcOptionsTypeDef,
     },
     total=False,
 )
 
+
 class UpdateVpcAttachmentRequestRequestTypeDef(
     _RequiredUpdateVpcAttachmentRequestRequestTypeDef,
     _OptionalUpdateVpcAttachmentRequestRequestTypeDef,
 ):
     pass
 
+
+DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef = TypedDict(
+    "DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef",
+    {
+        "GlobalNetworkIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef",
+    {
+        "ConnectPeerIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef(
+    _RequiredGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+    _OptionalGetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
+    "_RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef = TypedDict(
+    "_OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef",
+    {
+        "ConnectionIds": Sequence[str],
+        "DeviceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetConnectionsRequestGetConnectionsPaginateTypeDef(
+    _RequiredGetConnectionsRequestGetConnectionsPaginateTypeDef,
+    _OptionalGetConnectionsRequestGetConnectionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
+    "_RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "PolicyVersionId": int,
+    },
+)
+_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef = TypedDict(
+    "_OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef(
+    _RequiredGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+    _OptionalGetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
+    "_RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "PolicyVersionId": int,
+    },
+)
+_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef = TypedDict(
+    "_OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef(
+    _RequiredGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+    _OptionalGetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef",
+    {
+        "CustomerGatewayArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef(
+    _RequiredGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+    _OptionalGetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
+    "_RequiredGetDevicesRequestGetDevicesPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetDevicesRequestGetDevicesPaginateTypeDef = TypedDict(
+    "_OptionalGetDevicesRequestGetDevicesPaginateTypeDef",
+    {
+        "DeviceIds": Sequence[str],
+        "SiteId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDevicesRequestGetDevicesPaginateTypeDef(
+    _RequiredGetDevicesRequestGetDevicesPaginateTypeDef,
+    _OptionalGetDevicesRequestGetDevicesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef",
+    {
+        "DeviceId": str,
+        "LinkId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef(
+    _RequiredGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+    _OptionalGetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
+    "_RequiredGetLinksRequestGetLinksPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetLinksRequestGetLinksPaginateTypeDef = TypedDict(
+    "_OptionalGetLinksRequestGetLinksPaginateTypeDef",
+    {
+        "LinkIds": Sequence[str],
+        "SiteId": str,
+        "Type": str,
+        "Provider": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetLinksRequestGetLinksPaginateTypeDef(
+    _RequiredGetLinksRequestGetLinksPaginateTypeDef, _OptionalGetLinksRequestGetLinksPaginateTypeDef
+):
+    pass
+
+
+_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef",
+    {
+        "ResourceType": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef(
+    _RequiredGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+    _OptionalGetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "RegisteredGatewayArn": str,
+        "AwsRegion": str,
+        "AccountId": str,
+        "ResourceType": str,
+        "ResourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef(
+    _RequiredGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+    _OptionalGetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "RegisteredGatewayArn": str,
+        "AwsRegion": str,
+        "AccountId": str,
+        "ResourceType": str,
+        "ResourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef(
+    _RequiredGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+    _OptionalGetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
+    "_RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef = TypedDict(
+    "_OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "RegisteredGatewayArn": str,
+        "AwsRegion": str,
+        "AccountId": str,
+        "ResourceType": str,
+        "ResourceArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef(
+    _RequiredGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+    _OptionalGetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
+    "_RequiredGetSitesRequestGetSitesPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetSitesRequestGetSitesPaginateTypeDef = TypedDict(
+    "_OptionalGetSitesRequestGetSitesPaginateTypeDef",
+    {
+        "SiteIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetSitesRequestGetSitesPaginateTypeDef(
+    _RequiredGetSitesRequestGetSitesPaginateTypeDef, _OptionalGetSitesRequestGetSitesPaginateTypeDef
+):
+    pass
+
+
+_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef = TypedDict(
+    "_OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef",
+    {
+        "TransitGatewayConnectPeerArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef(
+    _RequiredGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+    _OptionalGetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
+    {
+        "GlobalNetworkId": str,
+    },
+)
+_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef",
+    {
+        "TransitGatewayArns": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef(
+    _RequiredGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+    _OptionalGetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+):
+    pass
+
+
+ListAttachmentsRequestListAttachmentsPaginateTypeDef = TypedDict(
+    "ListAttachmentsRequestListAttachmentsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "AttachmentType": AttachmentTypeType,
+        "EdgeLocation": str,
+        "State": AttachmentStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListConnectPeersRequestListConnectPeersPaginateTypeDef = TypedDict(
+    "ListConnectPeersRequestListConnectPeersPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "ConnectAttachmentId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
+    TypedDict(
+        "_RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
+        {
+            "CoreNetworkId": str,
+        },
+    )
+)
+_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef = (
+    TypedDict(
+        "_OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef",
+        {
+            "PaginationConfig": PaginatorConfigTypeDef,
+        },
+        total=False,
+    )
+)
+
+
+class ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef(
+    _RequiredListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+    _OptionalListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+):
+    pass
+
+
+ListCoreNetworksRequestListCoreNetworksPaginateTypeDef = TypedDict(
+    "ListCoreNetworksRequestListCoreNetworksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPeeringsRequestListPeeringsPaginateTypeDef = TypedDict(
+    "ListPeeringsRequestListPeeringsPaginateTypeDef",
+    {
+        "CoreNetworkId": str,
+        "PeeringType": Literal["TRANSIT_GATEWAY"],
+        "EdgeLocation": str,
+        "State": PeeringStateType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 GetNetworkResourceCountsResponseTypeDef = TypedDict(
     "GetNetworkResourceCountsResponseTypeDef",
     {
         "NetworkResourceCounts": List[NetworkResourceCountTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResourceRelationshipsResponseTypeDef = TypedDict(
     "GetNetworkResourceRelationshipsResponseTypeDef",
     {
         "Relationships": List[RelationshipTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PathComponentTypeDef = TypedDict(
     "PathComponentTypeDef",
     {
         "Sequence": int,
@@ -2737,20 +2850,22 @@
     {
         "IncludeReturnPath": bool,
         "UseMiddleboxes": bool,
     },
     total=False,
 )
 
+
 class StartRouteAnalysisRequestRequestTypeDef(
     _RequiredStartRouteAnalysisRequestRequestTypeDef,
     _OptionalStartRouteAnalysisRequestRequestTypeDef,
 ):
     pass
 
+
 TransitGatewayRegistrationTypeDef = TypedDict(
     "TransitGatewayRegistrationTypeDef",
     {
         "GlobalNetworkId": str,
         "TransitGatewayArn": str,
         "State": TransitGatewayRegistrationStateReasonTypeDef,
     },
@@ -2758,133 +2873,133 @@
 )
 
 ListOrganizationServiceAccessStatusResponseTypeDef = TypedDict(
     "ListOrganizationServiceAccessStatusResponseTypeDef",
     {
         "OrganizationStatus": OrganizationStatusTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartOrganizationServiceAccessUpdateResponseTypeDef = TypedDict(
     "StartOrganizationServiceAccessUpdateResponseTypeDef",
     {
         "OrganizationStatus": OrganizationStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListConnectPeersResponseTypeDef = TypedDict(
     "ListConnectPeersResponseTypeDef",
     {
         "ConnectPeers": List[ConnectPeerSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateConnectionResponseTypeDef = TypedDict(
     "CreateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConnectionResponseTypeDef = TypedDict(
     "DeleteConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectionsResponseTypeDef = TypedDict(
     "GetConnectionsResponseTypeDef",
     {
         "Connections": List[ConnectionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateConnectionResponseTypeDef = TypedDict(
     "UpdateConnectionResponseTypeDef",
     {
         "Connection": ConnectionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCoreNetworksResponseTypeDef = TypedDict(
     "ListCoreNetworksResponseTypeDef",
     {
         "CoreNetworks": List[CoreNetworkSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGlobalNetworkResponseTypeDef = TypedDict(
     "CreateGlobalNetworkResponseTypeDef",
     {
         "GlobalNetwork": GlobalNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGlobalNetworkResponseTypeDef = TypedDict(
     "DeleteGlobalNetworkResponseTypeDef",
     {
         "GlobalNetwork": GlobalNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGlobalNetworksResponseTypeDef = TypedDict(
     "DescribeGlobalNetworksResponseTypeDef",
     {
         "GlobalNetworks": List[GlobalNetworkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGlobalNetworkResponseTypeDef = TypedDict(
     "UpdateGlobalNetworkResponseTypeDef",
     {
         "GlobalNetwork": GlobalNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNetworkResourcesResponseTypeDef = TypedDict(
     "GetNetworkResourcesResponseTypeDef",
     {
         "NetworkResources": List[NetworkResourceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeletePeeringResponseTypeDef = TypedDict(
     "DeletePeeringResponseTypeDef",
     {
         "Peering": PeeringTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPeeringsResponseTypeDef = TypedDict(
     "ListPeeringsResponseTypeDef",
     {
         "Peerings": List[PeeringTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TransitGatewayPeeringTypeDef = TypedDict(
     "TransitGatewayPeeringTypeDef",
     {
         "Peering": PeeringTypeDef,
@@ -2915,40 +3030,40 @@
     total=False,
 )
 
 CreateLinkResponseTypeDef = TypedDict(
     "CreateLinkResponseTypeDef",
     {
         "Link": LinkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteLinkResponseTypeDef = TypedDict(
     "DeleteLinkResponseTypeDef",
     {
         "Link": LinkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetLinksResponseTypeDef = TypedDict(
     "GetLinksResponseTypeDef",
     {
         "Links": List[LinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLinkResponseTypeDef = TypedDict(
     "UpdateLinkResponseTypeDef",
     {
         "Link": LinkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectPeerTypeDef = TypedDict(
     "ConnectPeerTypeDef",
     {
         "CoreNetworkId": str,
@@ -2964,65 +3079,65 @@
 )
 
 GetNetworkTelemetryResponseTypeDef = TypedDict(
     "GetNetworkTelemetryResponseTypeDef",
     {
         "NetworkTelemetry": List[NetworkTelemetryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkChangeEventsResponseTypeDef = TypedDict(
     "GetCoreNetworkChangeEventsResponseTypeDef",
     {
         "CoreNetworkChangeEvents": List[CoreNetworkChangeEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkChangeSetResponseTypeDef = TypedDict(
     "GetCoreNetworkChangeSetResponseTypeDef",
     {
         "CoreNetworkChanges": List[CoreNetworkChangeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCoreNetworkPolicyVersionResponseTypeDef = TypedDict(
     "DeleteCoreNetworkPolicyVersionResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkPolicyResponseTypeDef = TypedDict(
     "GetCoreNetworkPolicyResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutCoreNetworkPolicyResponseTypeDef = TypedDict(
     "PutCoreNetworkPolicyResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreCoreNetworkPolicyVersionResponseTypeDef = TypedDict(
     "RestoreCoreNetworkPolicyVersionResponseTypeDef",
     {
         "CoreNetworkPolicy": CoreNetworkPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetNetworkRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetNetworkRoutesRequestRequestTypeDef",
     {
         "GlobalNetworkId": str,
@@ -3040,114 +3155,116 @@
         "States": Sequence[RouteStateType],
         "Types": Sequence[RouteTypeType],
         "DestinationFilters": Mapping[str, Sequence[str]],
     },
     total=False,
 )
 
+
 class GetNetworkRoutesRequestRequestTypeDef(
     _RequiredGetNetworkRoutesRequestRequestTypeDef, _OptionalGetNetworkRoutesRequestRequestTypeDef
 ):
     pass
 
+
 CreateCoreNetworkResponseTypeDef = TypedDict(
     "CreateCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteCoreNetworkResponseTypeDef = TypedDict(
     "DeleteCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCoreNetworkResponseTypeDef = TypedDict(
     "GetCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateCoreNetworkResponseTypeDef = TypedDict(
     "UpdateCoreNetworkResponseTypeDef",
     {
         "CoreNetwork": CoreNetworkTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDeviceResponseTypeDef = TypedDict(
     "CreateDeviceResponseTypeDef",
     {
         "Device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDeviceResponseTypeDef = TypedDict(
     "DeleteDeviceResponseTypeDef",
     {
         "Device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDevicesResponseTypeDef = TypedDict(
     "GetDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDeviceResponseTypeDef = TypedDict(
     "UpdateDeviceResponseTypeDef",
     {
         "Device": DeviceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSiteResponseTypeDef = TypedDict(
     "CreateSiteResponseTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteSiteResponseTypeDef = TypedDict(
     "DeleteSiteResponseTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSitesResponseTypeDef = TypedDict(
     "GetSitesResponseTypeDef",
     {
         "Sites": List[SiteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSiteResponseTypeDef = TypedDict(
     "UpdateSiteResponseTypeDef",
     {
         "Site": SiteTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RouteAnalysisPathTypeDef = TypedDict(
     "RouteAnalysisPathTypeDef",
     {
         "CompletionStatus": RouteAnalysisCompletionTypeDef,
@@ -3160,64 +3277,64 @@
     "GetNetworkRoutesResponseTypeDef",
     {
         "RouteTableArn": str,
         "CoreNetworkSegmentEdge": CoreNetworkSegmentEdgeIdentifierTypeDef,
         "RouteTableType": RouteTableTypeType,
         "RouteTableTimestamp": datetime,
         "NetworkRoutes": List[NetworkRouteTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeregisterTransitGatewayResponseTypeDef = TypedDict(
     "DeregisterTransitGatewayResponseTypeDef",
     {
         "TransitGatewayRegistration": TransitGatewayRegistrationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayRegistrationsResponseTypeDef = TypedDict(
     "GetTransitGatewayRegistrationsResponseTypeDef",
     {
         "TransitGatewayRegistrations": List[TransitGatewayRegistrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RegisterTransitGatewayResponseTypeDef = TypedDict(
     "RegisterTransitGatewayResponseTypeDef",
     {
         "TransitGatewayRegistration": TransitGatewayRegistrationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitGatewayPeeringResponseTypeDef = TypedDict(
     "CreateTransitGatewayPeeringResponseTypeDef",
     {
         "TransitGatewayPeering": TransitGatewayPeeringTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayPeeringResponseTypeDef = TypedDict(
     "GetTransitGatewayPeeringResponseTypeDef",
     {
         "TransitGatewayPeering": TransitGatewayPeeringTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptAttachmentResponseTypeDef = TypedDict(
     "AcceptAttachmentResponseTypeDef",
     {
         "Attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectAttachmentTypeDef = TypedDict(
     "ConnectAttachmentTypeDef",
     {
         "Attachment": AttachmentTypeDef,
@@ -3227,32 +3344,32 @@
     total=False,
 )
 
 DeleteAttachmentResponseTypeDef = TypedDict(
     "DeleteAttachmentResponseTypeDef",
     {
         "Attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListAttachmentsResponseTypeDef = TypedDict(
     "ListAttachmentsResponseTypeDef",
     {
         "Attachments": List[AttachmentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RejectAttachmentResponseTypeDef = TypedDict(
     "RejectAttachmentResponseTypeDef",
     {
         "Attachment": AttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SiteToSiteVpnAttachmentTypeDef = TypedDict(
     "SiteToSiteVpnAttachmentTypeDef",
     {
         "Attachment": AttachmentTypeDef,
@@ -3281,31 +3398,31 @@
     total=False,
 )
 
 CreateConnectPeerResponseTypeDef = TypedDict(
     "CreateConnectPeerResponseTypeDef",
     {
         "ConnectPeer": ConnectPeerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteConnectPeerResponseTypeDef = TypedDict(
     "DeleteConnectPeerResponseTypeDef",
     {
         "ConnectPeer": ConnectPeerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectPeerResponseTypeDef = TypedDict(
     "GetConnectPeerResponseTypeDef",
     {
         "ConnectPeer": ConnectPeerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RouteAnalysisTypeDef = TypedDict(
     "RouteAnalysisTypeDef",
     {
         "GlobalNetworkId": str,
@@ -3323,90 +3440,90 @@
     total=False,
 )
 
 CreateConnectAttachmentResponseTypeDef = TypedDict(
     "CreateConnectAttachmentResponseTypeDef",
     {
         "ConnectAttachment": ConnectAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetConnectAttachmentResponseTypeDef = TypedDict(
     "GetConnectAttachmentResponseTypeDef",
     {
         "ConnectAttachment": ConnectAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateSiteToSiteVpnAttachmentResponseTypeDef = TypedDict(
     "CreateSiteToSiteVpnAttachmentResponseTypeDef",
     {
         "SiteToSiteVpnAttachment": SiteToSiteVpnAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSiteToSiteVpnAttachmentResponseTypeDef = TypedDict(
     "GetSiteToSiteVpnAttachmentResponseTypeDef",
     {
         "SiteToSiteVpnAttachment": SiteToSiteVpnAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitGatewayRouteTableAttachmentResponseTypeDef = TypedDict(
     "CreateTransitGatewayRouteTableAttachmentResponseTypeDef",
     {
         "TransitGatewayRouteTableAttachment": TransitGatewayRouteTableAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTransitGatewayRouteTableAttachmentResponseTypeDef = TypedDict(
     "GetTransitGatewayRouteTableAttachmentResponseTypeDef",
     {
         "TransitGatewayRouteTableAttachment": TransitGatewayRouteTableAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVpcAttachmentResponseTypeDef = TypedDict(
     "CreateVpcAttachmentResponseTypeDef",
     {
         "VpcAttachment": VpcAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcAttachmentResponseTypeDef = TypedDict(
     "GetVpcAttachmentResponseTypeDef",
     {
         "VpcAttachment": VpcAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVpcAttachmentResponseTypeDef = TypedDict(
     "UpdateVpcAttachmentResponseTypeDef",
     {
         "VpcAttachment": VpcAttachmentTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteAnalysisResponseTypeDef = TypedDict(
     "GetRouteAnalysisResponseTypeDef",
     {
         "RouteAnalysis": RouteAnalysisTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartRouteAnalysisResponseTypeDef = TypedDict(
     "StartRouteAnalysisResponseTypeDef",
     {
         "RouteAnalysis": RouteAnalysisTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/PKG-INFO` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-networkmanager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.NetworkManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore networkmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore networkmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-networkmanager"></a>
 
 # types-aiobotocore-networkmanager
 
 [![PyPI - types-aiobotocore-networkmanager](https://img.shields.io/pypi/v/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-networkmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-networkmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-networkmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-networkmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-networkmanager)](https://pepy.tech/project/types-aiobotocore-networkmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.NetworkManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/networkmanager.html#NetworkManager)
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
 [types-aiobotocore-networkmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_networkmanager/).
 
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
@@ -426,25 +425,26 @@
 )
 
 
 def check_value(value: AttachmentStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_networkmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_networkmanager.type_defs import (
     AWSLocationTypeDef,
     AcceptAttachmentRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     AccountStatusTypeDef,
     AssociateConnectPeerRequestRequestTypeDef,
     ConnectPeerAssociationTypeDef,
     AssociateCustomerGatewayRequestRequestTypeDef,
     CustomerGatewayAssociationTypeDef,
     AssociateLinkRequestRequestTypeDef,
     LinkAssociationTypeDef,
@@ -473,95 +473,73 @@
     DeleteDeviceRequestRequestTypeDef,
     DeleteGlobalNetworkRequestRequestTypeDef,
     DeleteLinkRequestRequestTypeDef,
     DeletePeeringRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSiteRequestRequestTypeDef,
     DeregisterTransitGatewayRequestRequestTypeDef,
-    DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeGlobalNetworksRequestRequestTypeDef,
     DisassociateConnectPeerRequestRequestTypeDef,
     DisassociateCustomerGatewayRequestRequestTypeDef,
     DisassociateLinkRequestRequestTypeDef,
     DisassociateTransitGatewayConnectPeerRequestRequestTypeDef,
     ExecuteCoreNetworkChangeSetRequestRequestTypeDef,
     GetConnectAttachmentRequestRequestTypeDef,
-    GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
     GetConnectPeerAssociationsRequestRequestTypeDef,
     GetConnectPeerRequestRequestTypeDef,
-    GetConnectionsRequestGetConnectionsPaginateTypeDef,
     GetConnectionsRequestRequestTypeDef,
-    GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
     GetCoreNetworkChangeEventsRequestRequestTypeDef,
-    GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
     GetCoreNetworkChangeSetRequestRequestTypeDef,
     GetCoreNetworkPolicyRequestRequestTypeDef,
     GetCoreNetworkRequestRequestTypeDef,
-    GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
     GetCustomerGatewayAssociationsRequestRequestTypeDef,
-    GetDevicesRequestGetDevicesPaginateTypeDef,
     GetDevicesRequestRequestTypeDef,
-    GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
     GetLinkAssociationsRequestRequestTypeDef,
-    GetLinksRequestGetLinksPaginateTypeDef,
     GetLinksRequestRequestTypeDef,
-    GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
     GetNetworkResourceCountsRequestRequestTypeDef,
     NetworkResourceCountTypeDef,
-    GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
     GetNetworkResourceRelationshipsRequestRequestTypeDef,
     RelationshipTypeDef,
-    GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
     GetNetworkResourcesRequestRequestTypeDef,
-    GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
     GetNetworkTelemetryRequestRequestTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetRouteAnalysisRequestRequestTypeDef,
     GetSiteToSiteVpnAttachmentRequestRequestTypeDef,
-    GetSitesRequestGetSitesPaginateTypeDef,
     GetSitesRequestRequestTypeDef,
-    GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
     GetTransitGatewayConnectPeerAssociationsRequestRequestTypeDef,
     GetTransitGatewayPeeringRequestRequestTypeDef,
-    GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
     GetTransitGatewayRegistrationsRequestRequestTypeDef,
     GetTransitGatewayRouteTableAttachmentRequestRequestTypeDef,
     GetVpcAttachmentRequestRequestTypeDef,
-    ListAttachmentsRequestListAttachmentsPaginateTypeDef,
     ListAttachmentsRequestRequestTypeDef,
-    ListConnectPeersRequestListConnectPeersPaginateTypeDef,
     ListConnectPeersRequestRequestTypeDef,
-    ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
     ListCoreNetworkPolicyVersionsRequestRequestTypeDef,
-    ListCoreNetworksRequestListCoreNetworksPaginateTypeDef,
     ListCoreNetworksRequestRequestTypeDef,
     ListOrganizationServiceAccessStatusRequestRequestTypeDef,
-    ListPeeringsRequestListPeeringsPaginateTypeDef,
     ListPeeringsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     NetworkResourceSummaryTypeDef,
     NetworkRouteDestinationTypeDef,
-    PaginatorConfigTypeDef,
     PutCoreNetworkPolicyRequestRequestTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
     RegisterTransitGatewayRequestRequestTypeDef,
     RejectAttachmentRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreCoreNetworkPolicyVersionRequestRequestTypeDef,
     RouteAnalysisCompletionTypeDef,
     RouteAnalysisEndpointOptionsSpecificationTypeDef,
     RouteAnalysisEndpointOptionsTypeDef,
     StartOrganizationServiceAccessUpdateRequestRequestTypeDef,
     TransitGatewayRegistrationStateReasonTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateCoreNetworkRequestRequestTypeDef,
     UpdateGlobalNetworkRequestRequestTypeDef,
     UpdateNetworkResourceMetadataRequestRequestTypeDef,
+    GetResourcePolicyResponseTypeDef,
     UpdateNetworkResourceMetadataResponseTypeDef,
     OrganizationStatusTypeDef,
     AssociateConnectPeerResponseTypeDef,
     DisassociateConnectPeerResponseTypeDef,
     GetConnectPeerAssociationsResponseTypeDef,
     AssociateCustomerGatewayResponseTypeDef,
     DisassociateCustomerGatewayResponseTypeDef,
@@ -604,14 +582,35 @@
     CreateSiteRequestRequestTypeDef,
     DeviceTypeDef,
     SiteTypeDef,
     UpdateDeviceRequestRequestTypeDef,
     UpdateSiteRequestRequestTypeDef,
     CreateVpcAttachmentRequestRequestTypeDef,
     UpdateVpcAttachmentRequestRequestTypeDef,
+    DescribeGlobalNetworksRequestDescribeGlobalNetworksPaginateTypeDef,
+    GetConnectPeerAssociationsRequestGetConnectPeerAssociationsPaginateTypeDef,
+    GetConnectionsRequestGetConnectionsPaginateTypeDef,
+    GetCoreNetworkChangeEventsRequestGetCoreNetworkChangeEventsPaginateTypeDef,
+    GetCoreNetworkChangeSetRequestGetCoreNetworkChangeSetPaginateTypeDef,
+    GetCustomerGatewayAssociationsRequestGetCustomerGatewayAssociationsPaginateTypeDef,
+    GetDevicesRequestGetDevicesPaginateTypeDef,
+    GetLinkAssociationsRequestGetLinkAssociationsPaginateTypeDef,
+    GetLinksRequestGetLinksPaginateTypeDef,
+    GetNetworkResourceCountsRequestGetNetworkResourceCountsPaginateTypeDef,
+    GetNetworkResourceRelationshipsRequestGetNetworkResourceRelationshipsPaginateTypeDef,
+    GetNetworkResourcesRequestGetNetworkResourcesPaginateTypeDef,
+    GetNetworkTelemetryRequestGetNetworkTelemetryPaginateTypeDef,
+    GetSitesRequestGetSitesPaginateTypeDef,
+    GetTransitGatewayConnectPeerAssociationsRequestGetTransitGatewayConnectPeerAssociationsPaginateTypeDef,
+    GetTransitGatewayRegistrationsRequestGetTransitGatewayRegistrationsPaginateTypeDef,
+    ListAttachmentsRequestListAttachmentsPaginateTypeDef,
+    ListConnectPeersRequestListConnectPeersPaginateTypeDef,
+    ListCoreNetworkPolicyVersionsRequestListCoreNetworkPolicyVersionsPaginateTypeDef,
+    ListCoreNetworksRequestListCoreNetworksPaginateTypeDef,
+    ListPeeringsRequestListPeeringsPaginateTypeDef,
     GetNetworkResourceCountsResponseTypeDef,
     GetNetworkResourceRelationshipsResponseTypeDef,
     PathComponentTypeDef,
     NetworkRouteTypeDef,
     StartRouteAnalysisRequestRequestTypeDef,
     TransitGatewayRegistrationTypeDef,
     ListOrganizationServiceAccessStatusResponseTypeDef,
@@ -685,15 +684,15 @@
     GetVpcAttachmentResponseTypeDef,
     UpdateVpcAttachmentResponseTypeDef,
     GetRouteAnalysisResponseTypeDef,
     StartRouteAnalysisResponseTypeDef,
 )
 
 
-def get_structure() -> AWSLocationTypeDef:
+def get_value() -> AWSLocationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-networkmanager-2.5.2/types_aiobotocore_networkmanager.egg-info/SOURCES.txt` & `types-aiobotocore-networkmanager-2.5.2.post1/types_aiobotocore_networkmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


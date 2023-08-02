# Comparing `tmp/types-aiobotocore-directconnect-2.5.2.tar.gz` & `tmp/types-aiobotocore-directconnect-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-directconnect-2.5.2.tar", last modified: Sat Jul  8 01:43:30 2023, max compression
+gzip compressed data, was "types-aiobotocore-directconnect-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:10 2023, max compression
```

## Comparing `types-aiobotocore-directconnect-2.5.2.tar` & `types-aiobotocore-directconnect-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.830003 types-aiobotocore-directconnect-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-07-08 01:43:30.830003 types-aiobotocore-directconnect-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19033 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:30.830003 types-aiobotocore-directconnect-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.826003 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    49897 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49822 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-07-08 01:28:46.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-07-08 01:28:45.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-07-08 01:28:45.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-07-08 01:28:45.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    55049 2023-07-08 01:28:47.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    55002 2023-07-08 01:28:46.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:44.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:30.830003 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20622 2023-07-08 01:43:30.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:43:30.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:30.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:30.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:30.000000 types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18976 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.037606 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49705 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49630 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10823 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10821 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5363 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    54831 2023-08-02 14:36:25.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54784 2023-08-02 14:36:25.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:24.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:10.045606 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20518 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:09.000000 types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-directconnect-2.5.2/LICENSE` & `types-aiobotocore-directconnect-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2/PKG-INFO` & `types-aiobotocore-directconnect-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-directconnect
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DirectConnect 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DirectConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore directconnect type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore directconnect type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-directconnect"></a>
 
 # types-aiobotocore-directconnect
 
 [![PyPI - types-aiobotocore-directconnect](https://img.shields.io/pypi/v/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-directconnect?color=blue)](https://pypistats.org/packages/types-aiobotocore-directconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-directconnect)](https://pepy.tech/project/types-aiobotocore-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DirectConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [types-aiobotocore-directconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/).
 
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
@@ -335,128 +334,128 @@
 )
 
 
 def check_value(value: AddressFamilyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_directconnect.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
+    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
-    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
-    LoaResponseMetadataTypeDef,
     LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
+    DeleteInterconnectResponseTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
+    LoaResponseTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
     ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
     DirectConnectGatewayAssociationProposalTypeDef,
     DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfaceTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
@@ -465,15 +464,15 @@
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
@@ -484,15 +483,15 @@
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
     VirtualInterfacesTypeDef,
     LagsTypeDef,
 )
 
 
-def get_structure() -> RouteFilterPrefixTypeDef:
+def get_value() -> RouteFilterPrefixTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-directconnect-2.5.2/README.md` & `types-aiobotocore-directconnect-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-directconnect"></a>
 
 # types-aiobotocore-directconnect
 
 [![PyPI - types-aiobotocore-directconnect](https://img.shields.io/pypi/v/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-directconnect?color=blue)](https://pypistats.org/packages/types-aiobotocore-directconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-directconnect)](https://pepy.tech/project/types-aiobotocore-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DirectConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [types-aiobotocore-directconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/).
 
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
@@ -302,128 +302,128 @@
 )
 
 
 def check_value(value: AddressFamilyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_directconnect.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
+    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
-    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
-    LoaResponseMetadataTypeDef,
     LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
+    DeleteInterconnectResponseTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
+    LoaResponseTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
     ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
     DirectConnectGatewayAssociationProposalTypeDef,
     DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfaceTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
@@ -432,15 +432,15 @@
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
@@ -451,15 +451,15 @@
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
     VirtualInterfacesTypeDef,
     LagsTypeDef,
 )
 
 
-def get_structure() -> RouteFilterPrefixTypeDef:
+def get_value() -> RouteFilterPrefixTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-directconnect-2.5.2/setup.py` & `types-aiobotocore-directconnect-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-directconnect",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_directconnect"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DirectConnect 2.5.2 service generated with"
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
-    keywords="aiobotocore directconnect type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore directconnect type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_directconnect": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/"
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/__init__.py` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/__init__.pyi` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/__main__.py` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DirectConnect 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DirectConnect 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect\nOther"
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

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/client.py` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     AllocateTransitVirtualInterfaceResultTypeDef,
     AssociateMacSecKeyResponseTypeDef,
     ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionsTypeDef,
     CreateBGPPeerResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
@@ -53,20 +53,20 @@
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagsTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
-    LoaResponseMetadataTypeDef,
+    LoaResponseTypeDef,
     LocationsTypeDef,
     NewBGPPeerTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
@@ -74,43 +74,39 @@
     RouteFilterPrefixTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     TagTypeDef,
     UpdateDirectConnectGatewayAssociationResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     VirtualGatewaysTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfacesTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("DirectConnectClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DirectConnectClientException: Type[BotocoreClientError]
     DirectConnectServerException: Type[BotocoreClientError]
     DuplicateTagKeysException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class DirectConnectClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/)
     """
 
     meta: ClientMeta
@@ -119,15 +115,14 @@
     def exceptions(self) -> Exceptions:
         """
         DirectConnectClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#exceptions)
         """
-
     async def accept_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         proposalId: str,
         associatedGatewayOwnerAccount: str,
         overrideAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
@@ -135,249 +130,229 @@
         """
         Accepts a proposal request to attach a virtual private gateway or transit
         gateway to a Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.accept_direct_connect_gateway_association_proposal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#accept_direct_connect_gateway_association_proposal)
         """
-
     async def allocate_connection_on_interconnect(
         self,
         *,
         bandwidth: str,
         connectionName: str,
         ownerAccount: str,
         interconnectId: str,
         vlan: int
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_connection_on_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_connection_on_interconnect)
         """
-
     async def allocate_hosted_connection(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         bandwidth: str,
         connectionName: str,
         vlan: int,
         tags: Sequence[TagTypeDef] = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a hosted connection on the specified interconnect or a link aggregation
         group (LAG) of interconnects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_hosted_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_hosted_connection)
         """
-
     async def allocate_private_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a private virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_private_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_private_virtual_interface)
         """
-
     async def allocate_public_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a public virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_public_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_public_virtual_interface)
         """
-
     async def allocate_transit_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef
     ) -> AllocateTransitVirtualInterfaceResultTypeDef:
         """
         Provisions a transit virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_transit_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_transit_virtual_interface)
         """
-
     async def associate_connection_with_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates an existing connection with a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_connection_with_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_connection_with_lag)
         """
-
     async def associate_hosted_connection(
         self, *, connectionId: str, parentConnectionId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates a hosted connection and its virtual interfaces with a link
         aggregation group (LAG) or interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_hosted_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_hosted_connection)
         """
-
     async def associate_mac_sec_key(
         self, *, connectionId: str, secretARN: str = ..., ckn: str = ..., cak: str = ...
     ) -> AssociateMacSecKeyResponseTypeDef:
         """
         Associates a MAC Security (MACsec) Connection Key Name (CKN)/ Connectivity
         Association Key (CAK) pair with an Direct Connect dedicated connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_mac_sec_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_mac_sec_key)
         """
-
     async def associate_virtual_interface(
         self, *, virtualInterfaceId: str, connectionId: str
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Associates a virtual interface with a specified link aggregation group (LAG) or
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_virtual_interface)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#close)
         """
-
     async def confirm_connection(self, *, connectionId: str) -> ConfirmConnectionResponseTypeDef:
         """
         Confirms the creation of the specified hosted connection on an interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_connection)
         """
-
     async def confirm_customer_agreement(
         self, *, agreementName: str = ...
     ) -> ConfirmCustomerAgreementResponseTypeDef:
         """
         The confirmation of the terms of agreement when creating the connection/link
         aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_customer_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_customer_agreement)
         """
-
     async def confirm_private_virtual_interface(
         self,
         *,
         virtualInterfaceId: str,
         virtualGatewayId: str = ...,
         directConnectGatewayId: str = ...
     ) -> ConfirmPrivateVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a private virtual interface created by another Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_private_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_private_virtual_interface)
         """
-
     async def confirm_public_virtual_interface(
         self, *, virtualInterfaceId: str
     ) -> ConfirmPublicVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a public virtual interface created by another Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_public_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_public_virtual_interface)
         """
-
     async def confirm_transit_virtual_interface(
         self, *, virtualInterfaceId: str, directConnectGatewayId: str
     ) -> ConfirmTransitVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a transit virtual interface created by another Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_transit_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_transit_virtual_interface)
         """
-
     async def create_bgp_peer(
         self, *, virtualInterfaceId: str = ..., newBGPPeer: NewBGPPeerTypeDef = ...
     ) -> CreateBGPPeerResponseTypeDef:
         """
         Creates a BGP peer on the specified virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_bgp_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_bgp_peer)
         """
-
     async def create_connection(
         self,
         *,
         location: str,
         bandwidth: str,
         connectionName: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a connection between a customer network and a specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_connection)
         """
-
     async def create_direct_connect_gateway(
         self, *, directConnectGatewayName: str, amazonSideAsn: int = ...
     ) -> CreateDirectConnectGatewayResultTypeDef:
         """
         Creates a Direct Connect gateway, which is an intermediate object that enables
         you to connect a set of virtual interfaces and virtual private gateways.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway)
         """
-
     async def create_direct_connect_gateway_association(
         self,
         *,
         directConnectGatewayId: str,
         gatewayId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
         virtualGatewayId: str = ...
@@ -385,15 +360,14 @@
         """
         Creates an association between a Direct Connect gateway and a virtual private
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway_association)
         """
-
     async def create_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         directConnectGatewayOwnerAccount: str,
         gatewayId: str,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
@@ -402,85 +376,79 @@
         """
         Creates a proposal to associate the specified virtual private gateway or transit
         gateway with the specified Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association_proposal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway_association_proposal)
         """
-
     async def create_interconnect(
         self,
         *,
         interconnectName: str,
         bandwidth: str,
         location: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...
-    ) -> InterconnectResponseMetadataTypeDef:
+    ) -> InterconnectResponseTypeDef:
         """
         Creates an interconnect between an Direct Connect Partner's network and a
         specific Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_interconnect)
         """
-
     async def create_lag(
         self,
         *,
         numberOfConnections: int,
         location: str,
         connectionsBandwidth: str,
         lagName: str,
         connectionId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         childConnectionTags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Creates a link aggregation group (LAG) with the specified number of bundled
         physical dedicated connections between the customer network and a specific
         Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_lag)
         """
-
     async def create_private_virtual_interface(
         self, *, connectionId: str, newPrivateVirtualInterface: NewPrivateVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a private virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_private_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_private_virtual_interface)
         """
-
     async def create_public_virtual_interface(
         self, *, connectionId: str, newPublicVirtualInterface: NewPublicVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a public virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_public_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_public_virtual_interface)
         """
-
     async def create_transit_virtual_interface(
         self, *, connectionId: str, newTransitVirtualInterface: NewTransitVirtualInterfaceTypeDef
     ) -> CreateTransitVirtualInterfaceResultTypeDef:
         """
         Creates a transit virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_transit_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_transit_virtual_interface)
         """
-
     async def delete_bgp_peer(
         self,
         *,
         virtualInterfaceId: str = ...,
         asn: int = ...,
         customerAddress: str = ...,
         bgpPeerId: str = ...
@@ -488,128 +456,116 @@
         """
         Deletes the specified BGP peer on the specified virtual interface with the
         specified customer address and ASN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_bgp_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_bgp_peer)
         """
-
-    async def delete_connection(self, *, connectionId: str) -> ConnectionResponseMetadataTypeDef:
+    async def delete_connection(self, *, connectionId: str) -> ConnectionResponseTypeDef:
         """
         Deletes the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_connection)
         """
-
     async def delete_direct_connect_gateway(
         self, *, directConnectGatewayId: str
     ) -> DeleteDirectConnectGatewayResultTypeDef:
         """
         Deletes the specified Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_direct_connect_gateway)
         """
-
     async def delete_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...
     ) -> DeleteDirectConnectGatewayAssociationResultTypeDef:
         """
         Deletes the association between the specified Direct Connect gateway and virtual
         private gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_direct_connect_gateway_association)
         """
-
     async def delete_direct_connect_gateway_association_proposal(
         self, *, proposalId: str
     ) -> DeleteDirectConnectGatewayAssociationProposalResultTypeDef:
         """
         Deletes the association proposal request between the specified Direct Connect
         gateway and virtual private gateway or transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway_association_proposal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_direct_connect_gateway_association_proposal)
         """
-
     async def delete_interconnect(
         self, *, interconnectId: str
     ) -> DeleteInterconnectResponseTypeDef:
         """
         Deletes the specified interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_interconnect)
         """
-
-    async def delete_lag(self, *, lagId: str) -> LagResponseMetadataTypeDef:
+    async def delete_lag(self, *, lagId: str) -> LagResponseTypeDef:
         """
         Deletes the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_lag)
         """
-
     async def delete_virtual_interface(
         self, *, virtualInterfaceId: str
     ) -> DeleteVirtualInterfaceResponseTypeDef:
         """
         Deletes a virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_virtual_interface)
         """
-
     async def describe_connection_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
     ) -> DescribeConnectionLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connection_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connection_loa)
         """
-
     async def describe_connections(self, *, connectionId: str = ...) -> ConnectionsTypeDef:
         """
         Displays the specified connection or all connections in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connections)
         """
-
     async def describe_connections_on_interconnect(
         self, *, interconnectId: str
     ) -> ConnectionsTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connections_on_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connections_on_interconnect)
         """
-
     async def describe_customer_metadata(self) -> DescribeCustomerMetadataResponseTypeDef:
         """
         Get and view a list of customer agreements, along with their signed status and
         whether the customer is an NNIPartner, NNIPartnerV2, or a nonPartner.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_customer_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_customer_metadata)
         """
-
     async def describe_direct_connect_gateway_association_proposals(
         self,
         *,
         directConnectGatewayId: str = ...,
         proposalId: str = ...,
         associatedGatewayId: str = ...,
         maxResults: int = ...,
@@ -618,15 +574,14 @@
         """
         Describes one or more association proposals for connection between a virtual
         private gateway or transit gateway and a Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_association_proposals)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_association_proposals)
         """
-
     async def describe_direct_connect_gateway_associations(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         maxResults: int = ...,
@@ -636,15 +591,14 @@
         """
         Lists the associations between your Direct Connect gateways and virtual private
         gateways and transit gateways.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_associations)
         """
-
     async def describe_direct_connect_gateway_attachments(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
@@ -652,160 +606,145 @@
         """
         Lists the attachments between your Direct Connect gateways and virtual
         interfaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_attachments)
         """
-
     async def describe_direct_connect_gateways(
         self, *, directConnectGatewayId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeDirectConnectGatewaysResultTypeDef:
         """
         Lists all your Direct Connect gateways or only the specified Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateways)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateways)
         """
-
     async def describe_hosted_connections(self, *, connectionId: str) -> ConnectionsTypeDef:
         """
         Lists the hosted connections that have been provisioned on the specified
         interconnect or link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_hosted_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_hosted_connections)
         """
-
     async def describe_interconnect_loa(
         self,
         *,
         interconnectId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
     ) -> DescribeInterconnectLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_interconnect_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_interconnect_loa)
         """
-
     async def describe_interconnects(self, *, interconnectId: str = ...) -> InterconnectsTypeDef:
         """
         Lists the interconnects owned by the Amazon Web Services account or only the
         specified interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_interconnects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_interconnects)
         """
-
     async def describe_lags(self, *, lagId: str = ...) -> LagsTypeDef:
         """
         Describes all your link aggregation groups (LAG) or the specified LAG.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_lags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_lags)
         """
-
     async def describe_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
-    ) -> LoaResponseMetadataTypeDef:
+    ) -> LoaResponseTypeDef:
         """
         Gets the LOA-CFA for a connection, interconnect, or link aggregation group
         (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_loa)
         """
-
     async def describe_locations(self) -> LocationsTypeDef:
         """
         Lists the Direct Connect locations in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_locations)
         """
-
     async def describe_router_configuration(
         self, *, virtualInterfaceId: str, routerTypeIdentifier: str = ...
     ) -> DescribeRouterConfigurationResponseTypeDef:
         """
         Details about the router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_router_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_router_configuration)
         """
-
     async def describe_tags(self, *, resourceArns: Sequence[str]) -> DescribeTagsResponseTypeDef:
         """
         Describes the tags associated with the specified Direct Connect resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_tags)
         """
-
     async def describe_virtual_gateways(self) -> VirtualGatewaysTypeDef:
         """
         Lists the virtual private gateways owned by the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_virtual_gateways)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_virtual_gateways)
         """
-
     async def describe_virtual_interfaces(
         self, *, connectionId: str = ..., virtualInterfaceId: str = ...
     ) -> VirtualInterfacesTypeDef:
         """
         Displays all virtual interfaces for an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_virtual_interfaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_virtual_interfaces)
         """
-
     async def disassociate_connection_from_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Disassociates a connection from a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.disassociate_connection_from_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#disassociate_connection_from_lag)
         """
-
     async def disassociate_mac_sec_key(
         self, *, connectionId: str, secretARN: str
     ) -> DisassociateMacSecKeyResponseTypeDef:
         """
         Removes the association between a MAC Security (MACsec) security key and an
         Direct Connect dedicated connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.disassociate_mac_sec_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#disassociate_mac_sec_key)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#generate_presigned_url)
         """
-
     async def list_virtual_interface_test_history(
         self,
         *,
         testId: str = ...,
         virtualInterfaceId: str = ...,
         bgpPeers: Sequence[str] = ...,
         status: str = ...,
@@ -814,15 +753,14 @@
     ) -> ListVirtualInterfaceTestHistoryResponseTypeDef:
         """
         Lists the virtual interface failover test history.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.list_virtual_interface_test_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#list_virtual_interface_test_history)
         """
-
     async def start_bgp_failover_test(
         self,
         *,
         virtualInterfaceId: str,
         bgpPeers: Sequence[str] = ...,
         testDurationInMinutes: int = ...
     ) -> StartBgpFailoverTestResponseTypeDef:
@@ -830,131 +768,118 @@
         Starts the virtual interface failover test that verifies your configuration
         meets your resiliency requirements by placing the BGP peering session in the
         DOWN state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.start_bgp_failover_test)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#start_bgp_failover_test)
         """
-
     async def stop_bgp_failover_test(
         self, *, virtualInterfaceId: str
     ) -> StopBgpFailoverTestResponseTypeDef:
         """
         Stops the virtual interface failover test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.stop_bgp_failover_test)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#stop_bgp_failover_test)
         """
-
     async def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified Direct Connect resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from the specified Direct Connect resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#untag_resource)
         """
-
     async def update_connection(
         self, *, connectionId: str, connectionName: str = ..., encryptionMode: str = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Updates the Direct Connect dedicated connection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_connection)
         """
-
     async def update_direct_connect_gateway(
         self, *, directConnectGatewayId: str, newDirectConnectGatewayName: str
     ) -> UpdateDirectConnectGatewayResponseTypeDef:
         """
         Updates the name of a current Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_direct_connect_gateway)
         """
-
     async def update_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
         removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
     ) -> UpdateDirectConnectGatewayAssociationResultTypeDef:
         """
         Updates the specified attributes of the Direct Connect gateway association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_direct_connect_gateway_association)
         """
-
     async def update_lag(
         self, *, lagId: str, lagName: str = ..., minimumLinks: int = ..., encryptionMode: str = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Updates the attributes of the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_lag)
         """
-
     async def update_virtual_interface_attributes(
         self,
         *,
         virtualInterfaceId: str,
         mtu: int = ...,
         enableSiteLink: bool = ...,
         virtualInterfaceName: str = ...
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Updates the specified attributes of the specified virtual private interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_virtual_interface_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_virtual_interface_attributes)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_direct_connect_gateway_associations"]
     ) -> DescribeDirectConnectGatewayAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_direct_connect_gateway_attachments"]
     ) -> DescribeDirectConnectGatewayAttachmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_direct_connect_gateways"]
     ) -> DescribeDirectConnectGatewaysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "DirectConnectClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/)
         """
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/client.pyi` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     AllocateTransitVirtualInterfaceResultTypeDef,
     AssociateMacSecKeyResponseTypeDef,
     ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionsTypeDef,
     CreateBGPPeerResponseTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
@@ -53,20 +53,20 @@
     DescribeDirectConnectGatewayAssociationsResultTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagsTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
-    LoaResponseMetadataTypeDef,
+    LoaResponseTypeDef,
     LocationsTypeDef,
     NewBGPPeerTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
@@ -74,39 +74,43 @@
     RouteFilterPrefixTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     TagTypeDef,
     UpdateDirectConnectGatewayAssociationResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     VirtualGatewaysTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfacesTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("DirectConnectClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     DirectConnectClientException: Type[BotocoreClientError]
     DirectConnectServerException: Type[BotocoreClientError]
     DuplicateTagKeysException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class DirectConnectClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/)
     """
 
     meta: ClientMeta
@@ -115,14 +119,15 @@
     def exceptions(self) -> Exceptions:
         """
         DirectConnectClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#exceptions)
         """
+
     async def accept_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         proposalId: str,
         associatedGatewayOwnerAccount: str,
         overrideAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
@@ -130,229 +135,249 @@
         """
         Accepts a proposal request to attach a virtual private gateway or transit
         gateway to a Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.accept_direct_connect_gateway_association_proposal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#accept_direct_connect_gateway_association_proposal)
         """
+
     async def allocate_connection_on_interconnect(
         self,
         *,
         bandwidth: str,
         connectionName: str,
         ownerAccount: str,
         interconnectId: str,
         vlan: int
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_connection_on_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_connection_on_interconnect)
         """
+
     async def allocate_hosted_connection(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         bandwidth: str,
         connectionName: str,
         vlan: int,
         tags: Sequence[TagTypeDef] = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a hosted connection on the specified interconnect or a link aggregation
         group (LAG) of interconnects.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_hosted_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_hosted_connection)
         """
+
     async def allocate_private_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPrivateVirtualInterfaceAllocation: NewPrivateVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a private virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_private_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_private_virtual_interface)
         """
+
     async def allocate_public_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newPublicVirtualInterfaceAllocation: NewPublicVirtualInterfaceAllocationTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Provisions a public virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_public_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_public_virtual_interface)
         """
+
     async def allocate_transit_virtual_interface(
         self,
         *,
         connectionId: str,
         ownerAccount: str,
         newTransitVirtualInterfaceAllocation: NewTransitVirtualInterfaceAllocationTypeDef
     ) -> AllocateTransitVirtualInterfaceResultTypeDef:
         """
         Provisions a transit virtual interface to be owned by the specified Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.allocate_transit_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#allocate_transit_virtual_interface)
         """
+
     async def associate_connection_with_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates an existing connection with a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_connection_with_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_connection_with_lag)
         """
+
     async def associate_hosted_connection(
         self, *, connectionId: str, parentConnectionId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Associates a hosted connection and its virtual interfaces with a link
         aggregation group (LAG) or interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_hosted_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_hosted_connection)
         """
+
     async def associate_mac_sec_key(
         self, *, connectionId: str, secretARN: str = ..., ckn: str = ..., cak: str = ...
     ) -> AssociateMacSecKeyResponseTypeDef:
         """
         Associates a MAC Security (MACsec) Connection Key Name (CKN)/ Connectivity
         Association Key (CAK) pair with an Direct Connect dedicated connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_mac_sec_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_mac_sec_key)
         """
+
     async def associate_virtual_interface(
         self, *, virtualInterfaceId: str, connectionId: str
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Associates a virtual interface with a specified link aggregation group (LAG) or
         connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.associate_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#associate_virtual_interface)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#close)
         """
+
     async def confirm_connection(self, *, connectionId: str) -> ConfirmConnectionResponseTypeDef:
         """
         Confirms the creation of the specified hosted connection on an interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_connection)
         """
+
     async def confirm_customer_agreement(
         self, *, agreementName: str = ...
     ) -> ConfirmCustomerAgreementResponseTypeDef:
         """
         The confirmation of the terms of agreement when creating the connection/link
         aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_customer_agreement)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_customer_agreement)
         """
+
     async def confirm_private_virtual_interface(
         self,
         *,
         virtualInterfaceId: str,
         virtualGatewayId: str = ...,
         directConnectGatewayId: str = ...
     ) -> ConfirmPrivateVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a private virtual interface created by another Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_private_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_private_virtual_interface)
         """
+
     async def confirm_public_virtual_interface(
         self, *, virtualInterfaceId: str
     ) -> ConfirmPublicVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a public virtual interface created by another Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_public_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_public_virtual_interface)
         """
+
     async def confirm_transit_virtual_interface(
         self, *, virtualInterfaceId: str, directConnectGatewayId: str
     ) -> ConfirmTransitVirtualInterfaceResponseTypeDef:
         """
         Accepts ownership of a transit virtual interface created by another Amazon Web
         Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.confirm_transit_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#confirm_transit_virtual_interface)
         """
+
     async def create_bgp_peer(
         self, *, virtualInterfaceId: str = ..., newBGPPeer: NewBGPPeerTypeDef = ...
     ) -> CreateBGPPeerResponseTypeDef:
         """
         Creates a BGP peer on the specified virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_bgp_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_bgp_peer)
         """
+
     async def create_connection(
         self,
         *,
         location: str,
         bandwidth: str,
         connectionName: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Creates a connection between a customer network and a specific Direct Connect
         location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_connection)
         """
+
     async def create_direct_connect_gateway(
         self, *, directConnectGatewayName: str, amazonSideAsn: int = ...
     ) -> CreateDirectConnectGatewayResultTypeDef:
         """
         Creates a Direct Connect gateway, which is an intermediate object that enables
         you to connect a set of virtual interfaces and virtual private gateways.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway)
         """
+
     async def create_direct_connect_gateway_association(
         self,
         *,
         directConnectGatewayId: str,
         gatewayId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
         virtualGatewayId: str = ...
@@ -360,14 +385,15 @@
         """
         Creates an association between a Direct Connect gateway and a virtual private
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway_association)
         """
+
     async def create_direct_connect_gateway_association_proposal(
         self,
         *,
         directConnectGatewayId: str,
         directConnectGatewayOwnerAccount: str,
         gatewayId: str,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
@@ -376,79 +402,85 @@
         """
         Creates a proposal to associate the specified virtual private gateway or transit
         gateway with the specified Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_direct_connect_gateway_association_proposal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_direct_connect_gateway_association_proposal)
         """
+
     async def create_interconnect(
         self,
         *,
         interconnectName: str,
         bandwidth: str,
         location: str,
         lagId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         providerName: str = ...
-    ) -> InterconnectResponseMetadataTypeDef:
+    ) -> InterconnectResponseTypeDef:
         """
         Creates an interconnect between an Direct Connect Partner's network and a
         specific Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_interconnect)
         """
+
     async def create_lag(
         self,
         *,
         numberOfConnections: int,
         location: str,
         connectionsBandwidth: str,
         lagName: str,
         connectionId: str = ...,
         tags: Sequence[TagTypeDef] = ...,
         childConnectionTags: Sequence[TagTypeDef] = ...,
         providerName: str = ...,
         requestMACSec: bool = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Creates a link aggregation group (LAG) with the specified number of bundled
         physical dedicated connections between the customer network and a specific
         Direct Connect location.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_lag)
         """
+
     async def create_private_virtual_interface(
         self, *, connectionId: str, newPrivateVirtualInterface: NewPrivateVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a private virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_private_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_private_virtual_interface)
         """
+
     async def create_public_virtual_interface(
         self, *, connectionId: str, newPublicVirtualInterface: NewPublicVirtualInterfaceTypeDef
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Creates a public virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_public_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_public_virtual_interface)
         """
+
     async def create_transit_virtual_interface(
         self, *, connectionId: str, newTransitVirtualInterface: NewTransitVirtualInterfaceTypeDef
     ) -> CreateTransitVirtualInterfaceResultTypeDef:
         """
         Creates a transit virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.create_transit_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#create_transit_virtual_interface)
         """
+
     async def delete_bgp_peer(
         self,
         *,
         virtualInterfaceId: str = ...,
         asn: int = ...,
         customerAddress: str = ...,
         bgpPeerId: str = ...
@@ -456,116 +488,128 @@
         """
         Deletes the specified BGP peer on the specified virtual interface with the
         specified customer address and ASN.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_bgp_peer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_bgp_peer)
         """
-    async def delete_connection(self, *, connectionId: str) -> ConnectionResponseMetadataTypeDef:
+
+    async def delete_connection(self, *, connectionId: str) -> ConnectionResponseTypeDef:
         """
         Deletes the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_connection)
         """
+
     async def delete_direct_connect_gateway(
         self, *, directConnectGatewayId: str
     ) -> DeleteDirectConnectGatewayResultTypeDef:
         """
         Deletes the specified Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_direct_connect_gateway)
         """
+
     async def delete_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...
     ) -> DeleteDirectConnectGatewayAssociationResultTypeDef:
         """
         Deletes the association between the specified Direct Connect gateway and virtual
         private gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_direct_connect_gateway_association)
         """
+
     async def delete_direct_connect_gateway_association_proposal(
         self, *, proposalId: str
     ) -> DeleteDirectConnectGatewayAssociationProposalResultTypeDef:
         """
         Deletes the association proposal request between the specified Direct Connect
         gateway and virtual private gateway or transit gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_direct_connect_gateway_association_proposal)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_direct_connect_gateway_association_proposal)
         """
+
     async def delete_interconnect(
         self, *, interconnectId: str
     ) -> DeleteInterconnectResponseTypeDef:
         """
         Deletes the specified interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_interconnect)
         """
-    async def delete_lag(self, *, lagId: str) -> LagResponseMetadataTypeDef:
+
+    async def delete_lag(self, *, lagId: str) -> LagResponseTypeDef:
         """
         Deletes the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_lag)
         """
+
     async def delete_virtual_interface(
         self, *, virtualInterfaceId: str
     ) -> DeleteVirtualInterfaceResponseTypeDef:
         """
         Deletes a virtual interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.delete_virtual_interface)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#delete_virtual_interface)
         """
+
     async def describe_connection_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
     ) -> DescribeConnectionLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connection_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connection_loa)
         """
+
     async def describe_connections(self, *, connectionId: str = ...) -> ConnectionsTypeDef:
         """
         Displays the specified connection or all connections in this Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connections)
         """
+
     async def describe_connections_on_interconnect(
         self, *, interconnectId: str
     ) -> ConnectionsTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_connections_on_interconnect)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_connections_on_interconnect)
         """
+
     async def describe_customer_metadata(self) -> DescribeCustomerMetadataResponseTypeDef:
         """
         Get and view a list of customer agreements, along with their signed status and
         whether the customer is an NNIPartner, NNIPartnerV2, or a nonPartner.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_customer_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_customer_metadata)
         """
+
     async def describe_direct_connect_gateway_association_proposals(
         self,
         *,
         directConnectGatewayId: str = ...,
         proposalId: str = ...,
         associatedGatewayId: str = ...,
         maxResults: int = ...,
@@ -574,14 +618,15 @@
         """
         Describes one or more association proposals for connection between a virtual
         private gateway or transit gateway and a Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_association_proposals)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_association_proposals)
         """
+
     async def describe_direct_connect_gateway_associations(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         maxResults: int = ...,
@@ -591,14 +636,15 @@
         """
         Lists the associations between your Direct Connect gateways and virtual private
         gateways and transit gateways.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_associations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_associations)
         """
+
     async def describe_direct_connect_gateway_attachments(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
         maxResults: int = ...,
         nextToken: str = ...
@@ -606,145 +652,160 @@
         """
         Lists the attachments between your Direct Connect gateways and virtual
         interfaces.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateway_attachments)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateway_attachments)
         """
+
     async def describe_direct_connect_gateways(
         self, *, directConnectGatewayId: str = ..., maxResults: int = ..., nextToken: str = ...
     ) -> DescribeDirectConnectGatewaysResultTypeDef:
         """
         Lists all your Direct Connect gateways or only the specified Direct Connect
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_direct_connect_gateways)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_direct_connect_gateways)
         """
+
     async def describe_hosted_connections(self, *, connectionId: str) -> ConnectionsTypeDef:
         """
         Lists the hosted connections that have been provisioned on the specified
         interconnect or link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_hosted_connections)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_hosted_connections)
         """
+
     async def describe_interconnect_loa(
         self,
         *,
         interconnectId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
     ) -> DescribeInterconnectLoaResponseTypeDef:
         """
         Deprecated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_interconnect_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_interconnect_loa)
         """
+
     async def describe_interconnects(self, *, interconnectId: str = ...) -> InterconnectsTypeDef:
         """
         Lists the interconnects owned by the Amazon Web Services account or only the
         specified interconnect.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_interconnects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_interconnects)
         """
+
     async def describe_lags(self, *, lagId: str = ...) -> LagsTypeDef:
         """
         Describes all your link aggregation groups (LAG) or the specified LAG.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_lags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_lags)
         """
+
     async def describe_loa(
         self,
         *,
         connectionId: str,
         providerName: str = ...,
         loaContentType: Literal["application/pdf"] = ...
-    ) -> LoaResponseMetadataTypeDef:
+    ) -> LoaResponseTypeDef:
         """
         Gets the LOA-CFA for a connection, interconnect, or link aggregation group
         (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_loa)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_loa)
         """
+
     async def describe_locations(self) -> LocationsTypeDef:
         """
         Lists the Direct Connect locations in the current Amazon Web Services Region.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_locations)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_locations)
         """
+
     async def describe_router_configuration(
         self, *, virtualInterfaceId: str, routerTypeIdentifier: str = ...
     ) -> DescribeRouterConfigurationResponseTypeDef:
         """
         Details about the router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_router_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_router_configuration)
         """
+
     async def describe_tags(self, *, resourceArns: Sequence[str]) -> DescribeTagsResponseTypeDef:
         """
         Describes the tags associated with the specified Direct Connect resources.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_tags)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_tags)
         """
+
     async def describe_virtual_gateways(self) -> VirtualGatewaysTypeDef:
         """
         Lists the virtual private gateways owned by the Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_virtual_gateways)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_virtual_gateways)
         """
+
     async def describe_virtual_interfaces(
         self, *, connectionId: str = ..., virtualInterfaceId: str = ...
     ) -> VirtualInterfacesTypeDef:
         """
         Displays all virtual interfaces for an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.describe_virtual_interfaces)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#describe_virtual_interfaces)
         """
+
     async def disassociate_connection_from_lag(
         self, *, connectionId: str, lagId: str
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Disassociates a connection from a link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.disassociate_connection_from_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#disassociate_connection_from_lag)
         """
+
     async def disassociate_mac_sec_key(
         self, *, connectionId: str, secretARN: str
     ) -> DisassociateMacSecKeyResponseTypeDef:
         """
         Removes the association between a MAC Security (MACsec) security key and an
         Direct Connect dedicated connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.disassociate_mac_sec_key)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#disassociate_mac_sec_key)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#generate_presigned_url)
         """
+
     async def list_virtual_interface_test_history(
         self,
         *,
         testId: str = ...,
         virtualInterfaceId: str = ...,
         bgpPeers: Sequence[str] = ...,
         status: str = ...,
@@ -753,14 +814,15 @@
     ) -> ListVirtualInterfaceTestHistoryResponseTypeDef:
         """
         Lists the virtual interface failover test history.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.list_virtual_interface_test_history)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#list_virtual_interface_test_history)
         """
+
     async def start_bgp_failover_test(
         self,
         *,
         virtualInterfaceId: str,
         bgpPeers: Sequence[str] = ...,
         testDurationInMinutes: int = ...
     ) -> StartBgpFailoverTestResponseTypeDef:
@@ -768,118 +830,131 @@
         Starts the virtual interface failover test that verifies your configuration
         meets your resiliency requirements by placing the BGP peering session in the
         DOWN state.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.start_bgp_failover_test)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#start_bgp_failover_test)
         """
+
     async def stop_bgp_failover_test(
         self, *, virtualInterfaceId: str
     ) -> StopBgpFailoverTestResponseTypeDef:
         """
         Stops the virtual interface failover test.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.stop_bgp_failover_test)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#stop_bgp_failover_test)
         """
+
     async def tag_resource(self, *, resourceArn: str, tags: Sequence[TagTypeDef]) -> Dict[str, Any]:
         """
         Adds the specified tags to the specified Direct Connect resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Removes one or more tags from the specified Direct Connect resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#untag_resource)
         """
+
     async def update_connection(
         self, *, connectionId: str, connectionName: str = ..., encryptionMode: str = ...
-    ) -> ConnectionResponseMetadataTypeDef:
+    ) -> ConnectionResponseTypeDef:
         """
         Updates the Direct Connect dedicated connection configuration.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_connection)
         """
+
     async def update_direct_connect_gateway(
         self, *, directConnectGatewayId: str, newDirectConnectGatewayName: str
     ) -> UpdateDirectConnectGatewayResponseTypeDef:
         """
         Updates the name of a current Direct Connect gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_direct_connect_gateway)
         """
+
     async def update_direct_connect_gateway_association(
         self,
         *,
         associationId: str = ...,
         addAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...,
         removeAllowedPrefixesToDirectConnectGateway: Sequence[RouteFilterPrefixTypeDef] = ...
     ) -> UpdateDirectConnectGatewayAssociationResultTypeDef:
         """
         Updates the specified attributes of the Direct Connect gateway association.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_direct_connect_gateway_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_direct_connect_gateway_association)
         """
+
     async def update_lag(
         self, *, lagId: str, lagName: str = ..., minimumLinks: int = ..., encryptionMode: str = ...
-    ) -> LagResponseMetadataTypeDef:
+    ) -> LagResponseTypeDef:
         """
         Updates the attributes of the specified link aggregation group (LAG).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_lag)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_lag)
         """
+
     async def update_virtual_interface_attributes(
         self,
         *,
         virtualInterfaceId: str,
         mtu: int = ...,
         enableSiteLink: bool = ...,
         virtualInterfaceName: str = ...
-    ) -> VirtualInterfaceResponseMetadataTypeDef:
+    ) -> VirtualInterfaceResponseTypeDef:
         """
         Updates the specified attributes of the specified virtual private interface.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.update_virtual_interface_attributes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#update_virtual_interface_attributes)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_direct_connect_gateway_associations"]
     ) -> DescribeDirectConnectGatewayAssociationsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_direct_connect_gateway_attachments"]
     ) -> DescribeDirectConnectGatewayAttachmentsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["describe_direct_connect_gateways"]
     ) -> DescribeDirectConnectGatewaysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "DirectConnectClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/client/)
         """
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/literals.py` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/literals.pyi` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/paginator.py` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
 
@@ -81,28 +81,28 @@
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
 
 class DescribeDirectConnectGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
-        self, *, directConnectGatewayId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, directConnectGatewayId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectConnectGatewaysResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayspaginator)
         """
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/paginator.pyi` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     def paginate(
         self,
         *,
         associationId: str = ...,
         associatedGatewayId: str = ...,
         directConnectGatewayId: str = ...,
         virtualGatewayId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectConnectGatewayAssociationsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAssociations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayassociationspaginator)
         """
 
 class DescribeDirectConnectGatewayAttachmentsPaginator(AioPaginator):
@@ -77,27 +77,27 @@
     """
 
     def paginate(
         self,
         *,
         directConnectGatewayId: str = ...,
         virtualInterfaceId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectConnectGatewayAttachmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGatewayAttachments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayattachmentspaginator)
         """
 
 class DescribeDirectConnectGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayspaginator)
     """
 
     def paginate(
-        self, *, directConnectGatewayId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, directConnectGatewayId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeDirectConnectGatewaysResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect.Paginator.DescribeDirectConnectGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/paginators/#describedirectconnectgatewayspaginator)
         """
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/type_defs.py` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_directconnect.type_defs import RouteFilterPrefixTypeDef
 
-    data: RouteFilterPrefixTypeDef = {...}
+    data: RouteFilterPrefixTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -41,118 +41,118 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "RouteFilterPrefixTypeDef",
+    "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
     "AssociateMacSecKeyRequestRequestTypeDef",
     "MacSecKeyTypeDef",
     "AssociateVirtualInterfaceRequestRequestTypeDef",
     "AssociatedGatewayTypeDef",
     "BGPPeerTypeDef",
     "ConfirmConnectionRequestRequestTypeDef",
-    "ConfirmConnectionResponseTypeDef",
     "ConfirmCustomerAgreementRequestRequestTypeDef",
-    "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationRequestRequestTypeDef",
     "DeleteDirectConnectGatewayRequestRequestTypeDef",
     "DeleteInterconnectRequestRequestTypeDef",
-    "DeleteInterconnectResponseTypeDef",
     "DeleteLagRequestRequestTypeDef",
     "DeleteVirtualInterfaceRequestRequestTypeDef",
-    "DeleteVirtualInterfaceResponseTypeDef",
     "DescribeConnectionLoaRequestRequestTypeDef",
     "LoaTypeDef",
     "DescribeConnectionsOnInterconnectRequestRequestTypeDef",
     "DescribeConnectionsRequestRequestTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     "DirectConnectGatewayAttachmentTypeDef",
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     "DescribeHostedConnectionsRequestRequestTypeDef",
     "DescribeInterconnectLoaRequestRequestTypeDef",
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
-    "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartBgpFailoverTestRequestRequestTypeDef",
     "StopBgpFailoverTestRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     "UpdateLagRequestRequestTypeDef",
     "UpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     "VirtualGatewayTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
+    "ConfirmConnectionResponseTypeDef",
+    "ConfirmCustomerAgreementResponseTypeDef",
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    "DeleteInterconnectResponseTypeDef",
+    "DeleteVirtualInterfaceResponseTypeDef",
+    "LoaResponseTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
-    "InterconnectResponseMetadataTypeDef",
+    "InterconnectResponseTypeDef",
     "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
     "NewPrivateVirtualInterfaceTypeDef",
     "NewPublicVirtualInterfaceAllocationTypeDef",
     "NewPublicVirtualInterfaceTypeDef",
     "NewTransitVirtualInterfaceAllocationTypeDef",
     "NewTransitVirtualInterfaceTypeDef",
     "ResourceTagTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateMacSecKeyResponseTypeDef",
-    "ConnectionResponseMetadataTypeDef",
+    "ConnectionResponseTypeDef",
     "ConnectionTypeDef",
     "DisassociateMacSecKeyResponseTypeDef",
     "DirectConnectGatewayAssociationProposalTypeDef",
     "DirectConnectGatewayAssociationTypeDef",
-    "VirtualInterfaceResponseMetadataTypeDef",
+    "VirtualInterfaceResponseTypeDef",
     "VirtualInterfaceTypeDef",
     "CreateBGPPeerRequestRequestTypeDef",
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
@@ -161,15 +161,15 @@
     "CreatePrivateVirtualInterfaceRequestRequestTypeDef",
     "AllocatePublicVirtualInterfaceRequestRequestTypeDef",
     "CreatePublicVirtualInterfaceRequestRequestTypeDef",
     "AllocateTransitVirtualInterfaceRequestRequestTypeDef",
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ConnectionsTypeDef",
-    "LagResponseMetadataTypeDef",
+    "LagResponseTypeDef",
     "LagTypeDef",
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
@@ -187,14 +187,25 @@
     "RouteFilterPrefixTypeDef",
     {
         "cidr": str,
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
 AllocateConnectionOnInterconnectRequestRequestTypeDef = TypedDict(
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     {
         "bandwidth": str,
         "connectionName": str,
         "ownerAccount": str,
         "interconnectId": str,
@@ -311,38 +322,22 @@
 ConfirmConnectionRequestRequestTypeDef = TypedDict(
     "ConfirmConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 
-ConfirmConnectionResponseTypeDef = TypedDict(
-    "ConfirmConnectionResponseTypeDef",
-    {
-        "connectionState": ConnectionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmCustomerAgreementRequestRequestTypeDef = TypedDict(
     "ConfirmCustomerAgreementRequestRequestTypeDef",
     {
         "agreementName": str,
     },
     total=False,
 )
 
-ConfirmCustomerAgreementResponseTypeDef = TypedDict(
-    "ConfirmCustomerAgreementResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
@@ -358,53 +353,29 @@
 class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(
     _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
 ):
     pass
 
 
-ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmPublicVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmTransitVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
         "directConnectGatewayId": str,
     },
 )
 
-ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -502,44 +473,28 @@
 DeleteInterconnectRequestRequestTypeDef = TypedDict(
     "DeleteInterconnectRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
 )
 
-DeleteInterconnectResponseTypeDef = TypedDict(
-    "DeleteInterconnectResponseTypeDef",
-    {
-        "interconnectState": InterconnectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLagRequestRequestTypeDef = TypedDict(
     "DeleteLagRequestRequestTypeDef",
     {
         "lagId": str,
     },
 )
 
 DeleteVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-DeleteVirtualInterfaceResponseTypeDef = TypedDict(
-    "DeleteVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectionLoaRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 _OptionalDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
@@ -591,22 +546,20 @@
         "associatedGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "associationId": str,
-        "associatedGatewayId": str,
-        "directConnectGatewayId": str,
-        "virtualGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
     {
@@ -616,24 +569,14 @@
         "maxResults": int,
         "nextToken": str,
         "virtualGatewayId": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "virtualInterfaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "virtualInterfaceId": str,
         "maxResults": int,
         "nextToken": str,
@@ -651,23 +594,14 @@
         "attachmentState": DirectConnectGatewayAttachmentStateType,
         "attachmentType": DirectConnectGatewayAttachmentTypeType,
         "stateChangeError": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewaysRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -833,57 +767,27 @@
         "testDurationInMinutes": int,
         "startTime": datetime,
         "endTime": datetime,
     },
     total=False,
 )
 
-LoaResponseMetadataTypeDef = TypedDict(
-    "LoaResponseMetadataTypeDef",
-    {
-        "loaContent": bytes,
-        "loaContentType": Literal["application/pdf"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "locationCode": str,
         "locationName": str,
         "region": str,
         "availablePortSpeeds": List[str],
         "availableProviders": List[str],
         "availableMacSecPortSpeeds": List[str],
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
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
@@ -1083,14 +987,79 @@
         "associationId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
+ConfirmConnectionResponseTypeDef = TypedDict(
+    "ConfirmConnectionResponseTypeDef",
+    {
+        "connectionState": ConnectionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmCustomerAgreementResponseTypeDef = TypedDict(
+    "ConfirmCustomerAgreementResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInterconnectResponseTypeDef = TypedDict(
+    "DeleteInterconnectResponseTypeDef",
+    {
+        "interconnectState": InterconnectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVirtualInterfaceResponseTypeDef = TypedDict(
+    "DeleteVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoaResponseTypeDef = TypedDict(
+    "LoaResponseTypeDef",
+    {
+        "loaContent": bytes,
+        "loaContentType": Literal["application/pdf"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAllocateHostedConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAllocateHostedConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "bandwidth": str,
         "connectionName": str,
@@ -1189,16 +1158,16 @@
 
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
 
-InterconnectResponseMetadataTypeDef = TypedDict(
-    "InterconnectResponseMetadataTypeDef",
+InterconnectResponseTypeDef = TypedDict(
+    "InterconnectResponseTypeDef",
     {
         "interconnectId": str,
         "interconnectName": str,
         "interconnectState": InterconnectStateType,
         "region": str,
         "location": str,
         "bandwidth": str,
@@ -1207,15 +1176,15 @@
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InterconnectTypeDef = TypedDict(
     "InterconnectTypeDef",
     {
         "interconnectId": str,
@@ -1406,20 +1375,20 @@
 )
 
 AssociateMacSecKeyResponseTypeDef = TypedDict(
     "AssociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConnectionResponseMetadataTypeDef = TypedDict(
-    "ConnectionResponseMetadataTypeDef",
+ConnectionResponseTypeDef = TypedDict(
+    "ConnectionResponseTypeDef",
     {
         "ownerAccount": str,
         "connectionId": str,
         "connectionName": str,
         "connectionState": ConnectionStateType,
         "region": str,
         "location": str,
@@ -1435,15 +1404,15 @@
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ownerAccount": str,
@@ -1473,15 +1442,15 @@
 )
 
 DisassociateMacSecKeyResponseTypeDef = TypedDict(
     "DisassociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
     "DirectConnectGatewayAssociationProposalTypeDef",
     {
         "proposalId": str,
@@ -1508,16 +1477,16 @@
         "virtualGatewayId": str,
         "virtualGatewayRegion": str,
         "virtualGatewayOwnerAccount": str,
     },
     total=False,
 )
 
-VirtualInterfaceResponseMetadataTypeDef = TypedDict(
-    "VirtualInterfaceResponseMetadataTypeDef",
+VirtualInterfaceResponseTypeDef = TypedDict(
+    "VirtualInterfaceResponseTypeDef",
     {
         "ownerAccount": str,
         "virtualInterfaceId": str,
         "location": str,
         "connectionId": str,
         "virtualInterfaceType": str,
         "virtualInterfaceName": str,
@@ -1537,15 +1506,15 @@
         "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
         "bgpPeers": List[BGPPeerTypeDef],
         "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "tags": List[TagTypeDef],
         "siteLinkEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualInterfaceTypeDef = TypedDict(
     "VirtualInterfaceTypeDef",
     {
         "ownerAccount": str,
@@ -1587,134 +1556,165 @@
     total=False,
 )
 
 CreateDirectConnectGatewayResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewaysResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysResultTypeDef",
     {
         "directConnectGateways": List[DirectConnectGatewayTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayResponseTypeDef = TypedDict(
     "UpdateDirectConnectGatewayResponseTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomerMetadataResponseTypeDef = TypedDict(
     "DescribeCustomerMetadataResponseTypeDef",
     {
         "agreements": List[CustomerAgreementTypeDef],
         "nniPartnerType": NniPartnerTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionLoaResponseTypeDef = TypedDict(
     "DescribeConnectionLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInterconnectLoaResponseTypeDef = TypedDict(
     "DescribeInterconnectLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    {
+        "associationId": str,
+        "associatedGatewayId": str,
+        "directConnectGatewayId": str,
+        "virtualGatewayId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "virtualInterfaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     {
         "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouterConfigurationResponseTypeDef = TypedDict(
     "DescribeRouterConfigurationResponseTypeDef",
     {
         "customerRouterConfig": str,
         "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
         "virtualInterfaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBgpFailoverTestResponseTypeDef = TypedDict(
     "StartBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBgpFailoverTestResponseTypeDef = TypedDict(
     "StopBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LocationsTypeDef = TypedDict(
     "LocationsTypeDef",
     {
         "locations": List[LocationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualGatewaysTypeDef = TypedDict(
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InterconnectsTypeDef = TypedDict(
     "InterconnectsTypeDef",
     {
         "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
@@ -1765,28 +1765,28 @@
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LagResponseMetadataTypeDef = TypedDict(
-    "LagResponseMetadataTypeDef",
+LagResponseTypeDef = TypedDict(
+    "LagResponseTypeDef",
     {
         "connectionsBandwidth": str,
         "numberOfConnections": int,
         "lagId": str,
         "ownerAccount": str,
         "lagName": str,
         "lagState": LagStateType,
@@ -1801,15 +1801,15 @@
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagTypeDef = TypedDict(
     "LagTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1837,118 +1837,118 @@
     total=False,
 )
 
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationProposalsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     {
         "directConnectGatewayAssociationProposals": List[
             DirectConnectGatewayAssociationProposalTypeDef
         ],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
     {
         "directConnectGatewayAssociations": List[DirectConnectGatewayAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "AllocateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBGPPeerResponseTypeDef = TypedDict(
     "CreateBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "CreateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBGPPeerResponseTypeDef = TypedDict(
     "DeleteBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualInterfacesTypeDef = TypedDict(
     "VirtualInterfacesTypeDef",
     {
         "virtualInterfaces": List[VirtualInterfaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagsTypeDef = TypedDict(
     "LagsTypeDef",
     {
         "lags": List[LagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect/type_defs.pyi` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_directconnect.type_defs import RouteFilterPrefixTypeDef
 
-    data: RouteFilterPrefixTypeDef = {...}
+    data: RouteFilterPrefixTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -40,118 +40,118 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "RouteFilterPrefixTypeDef",
+    "ResponseMetadataTypeDef",
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     "TagTypeDef",
     "AssociateConnectionWithLagRequestRequestTypeDef",
     "AssociateHostedConnectionRequestRequestTypeDef",
     "AssociateMacSecKeyRequestRequestTypeDef",
     "MacSecKeyTypeDef",
     "AssociateVirtualInterfaceRequestRequestTypeDef",
     "AssociatedGatewayTypeDef",
     "BGPPeerTypeDef",
     "ConfirmConnectionRequestRequestTypeDef",
-    "ConfirmConnectionResponseTypeDef",
     "ConfirmCustomerAgreementRequestRequestTypeDef",
-    "ConfirmCustomerAgreementResponseTypeDef",
     "ConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
     "NewBGPPeerTypeDef",
     "CreateDirectConnectGatewayRequestRequestTypeDef",
     "DirectConnectGatewayTypeDef",
     "CustomerAgreementTypeDef",
     "DeleteBGPPeerRequestRequestTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "DeleteDirectConnectGatewayAssociationRequestRequestTypeDef",
     "DeleteDirectConnectGatewayRequestRequestTypeDef",
     "DeleteInterconnectRequestRequestTypeDef",
-    "DeleteInterconnectResponseTypeDef",
     "DeleteLagRequestRequestTypeDef",
     "DeleteVirtualInterfaceRequestRequestTypeDef",
-    "DeleteVirtualInterfaceResponseTypeDef",
     "DescribeConnectionLoaRequestRequestTypeDef",
     "LoaTypeDef",
     "DescribeConnectionsOnInterconnectRequestRequestTypeDef",
     "DescribeConnectionsRequestRequestTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     "DirectConnectGatewayAttachmentTypeDef",
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     "DescribeHostedConnectionsRequestRequestTypeDef",
     "DescribeInterconnectLoaRequestRequestTypeDef",
     "DescribeInterconnectsRequestRequestTypeDef",
     "DescribeLagsRequestRequestTypeDef",
     "DescribeLoaRequestRequestTypeDef",
     "DescribeRouterConfigurationRequestRequestTypeDef",
     "RouterTypeTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DescribeVirtualInterfacesRequestRequestTypeDef",
     "DisassociateConnectionFromLagRequestRequestTypeDef",
     "DisassociateMacSecKeyRequestRequestTypeDef",
     "ListVirtualInterfaceTestHistoryRequestRequestTypeDef",
     "VirtualInterfaceTestHistoryTypeDef",
-    "LoaResponseMetadataTypeDef",
     "LocationTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "StartBgpFailoverTestRequestRequestTypeDef",
     "StopBgpFailoverTestRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateConnectionRequestRequestTypeDef",
     "UpdateDirectConnectGatewayRequestRequestTypeDef",
     "UpdateLagRequestRequestTypeDef",
     "UpdateVirtualInterfaceAttributesRequestRequestTypeDef",
     "VirtualGatewayTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef",
     "CreateDirectConnectGatewayAssociationRequestRequestTypeDef",
     "UpdateDirectConnectGatewayAssociationRequestRequestTypeDef",
+    "ConfirmConnectionResponseTypeDef",
+    "ConfirmCustomerAgreementResponseTypeDef",
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    "DeleteInterconnectResponseTypeDef",
+    "DeleteVirtualInterfaceResponseTypeDef",
+    "LoaResponseTypeDef",
     "AllocateHostedConnectionRequestRequestTypeDef",
     "CreateConnectionRequestRequestTypeDef",
     "CreateInterconnectRequestRequestTypeDef",
     "CreateLagRequestRequestTypeDef",
-    "InterconnectResponseMetadataTypeDef",
+    "InterconnectResponseTypeDef",
     "InterconnectTypeDef",
     "NewPrivateVirtualInterfaceAllocationTypeDef",
     "NewPrivateVirtualInterfaceTypeDef",
     "NewPublicVirtualInterfaceAllocationTypeDef",
     "NewPublicVirtualInterfaceTypeDef",
     "NewTransitVirtualInterfaceAllocationTypeDef",
     "NewTransitVirtualInterfaceTypeDef",
     "ResourceTagTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssociateMacSecKeyResponseTypeDef",
-    "ConnectionResponseMetadataTypeDef",
+    "ConnectionResponseTypeDef",
     "ConnectionTypeDef",
     "DisassociateMacSecKeyResponseTypeDef",
     "DirectConnectGatewayAssociationProposalTypeDef",
     "DirectConnectGatewayAssociationTypeDef",
-    "VirtualInterfaceResponseMetadataTypeDef",
+    "VirtualInterfaceResponseTypeDef",
     "VirtualInterfaceTypeDef",
     "CreateBGPPeerRequestRequestTypeDef",
     "CreateDirectConnectGatewayResultTypeDef",
     "DeleteDirectConnectGatewayResultTypeDef",
     "DescribeDirectConnectGatewaysResultTypeDef",
     "UpdateDirectConnectGatewayResponseTypeDef",
     "DescribeCustomerMetadataResponseTypeDef",
     "DescribeConnectionLoaResponseTypeDef",
     "DescribeInterconnectLoaResponseTypeDef",
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     "DescribeRouterConfigurationResponseTypeDef",
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     "StartBgpFailoverTestResponseTypeDef",
     "StopBgpFailoverTestResponseTypeDef",
     "LocationsTypeDef",
     "VirtualGatewaysTypeDef",
@@ -160,15 +160,15 @@
     "CreatePrivateVirtualInterfaceRequestRequestTypeDef",
     "AllocatePublicVirtualInterfaceRequestRequestTypeDef",
     "CreatePublicVirtualInterfaceRequestRequestTypeDef",
     "AllocateTransitVirtualInterfaceRequestRequestTypeDef",
     "CreateTransitVirtualInterfaceRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ConnectionsTypeDef",
-    "LagResponseMetadataTypeDef",
+    "LagResponseTypeDef",
     "LagTypeDef",
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
@@ -186,14 +186,25 @@
     "RouteFilterPrefixTypeDef",
     {
         "cidr": str,
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
 AllocateConnectionOnInterconnectRequestRequestTypeDef = TypedDict(
     "AllocateConnectionOnInterconnectRequestRequestTypeDef",
     {
         "bandwidth": str,
         "connectionName": str,
         "ownerAccount": str,
         "interconnectId": str,
@@ -306,38 +317,22 @@
 ConfirmConnectionRequestRequestTypeDef = TypedDict(
     "ConfirmConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 
-ConfirmConnectionResponseTypeDef = TypedDict(
-    "ConfirmConnectionResponseTypeDef",
-    {
-        "connectionState": ConnectionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmCustomerAgreementRequestRequestTypeDef = TypedDict(
     "ConfirmCustomerAgreementRequestRequestTypeDef",
     {
         "agreementName": str,
     },
     total=False,
 )
 
-ConfirmCustomerAgreementResponseTypeDef = TypedDict(
-    "ConfirmCustomerAgreementResponseTypeDef",
-    {
-        "status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "_RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
@@ -351,53 +346,29 @@
 
 class ConfirmPrivateVirtualInterfaceRequestRequestTypeDef(
     _RequiredConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
     _OptionalConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
 ):
     pass
 
-ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmPublicVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmPublicVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmPublicVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ConfirmTransitVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "ConfirmTransitVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
         "directConnectGatewayId": str,
     },
 )
 
-ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
-    "ConfirmTransitVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 NewBGPPeerTypeDef = TypedDict(
     "NewBGPPeerTypeDef",
     {
         "asn": int,
         "authKey": str,
         "addressFamily": AddressFamilyType,
         "amazonAddress": str,
@@ -493,44 +464,28 @@
 DeleteInterconnectRequestRequestTypeDef = TypedDict(
     "DeleteInterconnectRequestRequestTypeDef",
     {
         "interconnectId": str,
     },
 )
 
-DeleteInterconnectResponseTypeDef = TypedDict(
-    "DeleteInterconnectResponseTypeDef",
-    {
-        "interconnectState": InterconnectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLagRequestRequestTypeDef = TypedDict(
     "DeleteLagRequestRequestTypeDef",
     {
         "lagId": str,
     },
 )
 
 DeleteVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "DeleteVirtualInterfaceRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 
-DeleteVirtualInterfaceResponseTypeDef = TypedDict(
-    "DeleteVirtualInterfaceResponseTypeDef",
-    {
-        "virtualInterfaceState": VirtualInterfaceStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeConnectionLoaRequestRequestTypeDef",
     {
         "connectionId": str,
     },
 )
 _OptionalDescribeConnectionLoaRequestRequestTypeDef = TypedDict(
@@ -580,22 +535,20 @@
         "associatedGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "associationId": str,
-        "associatedGatewayId": str,
-        "directConnectGatewayId": str,
-        "virtualGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef",
     {
@@ -605,24 +558,14 @@
         "maxResults": int,
         "nextToken": str,
         "virtualGatewayId": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "virtualInterfaceId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "virtualInterfaceId": str,
         "maxResults": int,
         "nextToken": str,
@@ -640,23 +583,14 @@
         "attachmentState": DirectConnectGatewayAttachmentStateType,
         "attachmentType": DirectConnectGatewayAttachmentTypeType,
         "stateChangeError": str,
     },
     total=False,
 )
 
-DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
-    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
-    {
-        "directConnectGatewayId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeDirectConnectGatewaysRequestRequestTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysRequestRequestTypeDef",
     {
         "directConnectGatewayId": str,
         "maxResults": int,
         "nextToken": str,
     },
@@ -816,57 +750,27 @@
         "testDurationInMinutes": int,
         "startTime": datetime,
         "endTime": datetime,
     },
     total=False,
 )
 
-LoaResponseMetadataTypeDef = TypedDict(
-    "LoaResponseMetadataTypeDef",
-    {
-        "loaContent": bytes,
-        "loaContentType": Literal["application/pdf"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LocationTypeDef = TypedDict(
     "LocationTypeDef",
     {
         "locationCode": str,
         "locationName": str,
         "region": str,
         "availablePortSpeeds": List[str],
         "availableProviders": List[str],
         "availableMacSecPortSpeeds": List[str],
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
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
     "_RequiredStartBgpFailoverTestRequestRequestTypeDef",
     {
         "virtualInterfaceId": str,
     },
 )
 _OptionalStartBgpFailoverTestRequestRequestTypeDef = TypedDict(
@@ -1052,14 +956,79 @@
         "associationId": str,
         "addAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
         "removeAllowedPrefixesToDirectConnectGateway": Sequence[RouteFilterPrefixTypeDef],
     },
     total=False,
 )
 
+ConfirmConnectionResponseTypeDef = TypedDict(
+    "ConfirmConnectionResponseTypeDef",
+    {
+        "connectionState": ConnectionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmCustomerAgreementResponseTypeDef = TypedDict(
+    "ConfirmCustomerAgreementResponseTypeDef",
+    {
+        "status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPrivateVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPrivateVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmPublicVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmPublicVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmTransitVirtualInterfaceResponseTypeDef = TypedDict(
+    "ConfirmTransitVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteInterconnectResponseTypeDef = TypedDict(
+    "DeleteInterconnectResponseTypeDef",
+    {
+        "interconnectState": InterconnectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteVirtualInterfaceResponseTypeDef = TypedDict(
+    "DeleteVirtualInterfaceResponseTypeDef",
+    {
+        "virtualInterfaceState": VirtualInterfaceStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+LoaResponseTypeDef = TypedDict(
+    "LoaResponseTypeDef",
+    {
+        "loaContent": bytes,
+        "loaContentType": Literal["application/pdf"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredAllocateHostedConnectionRequestRequestTypeDef = TypedDict(
     "_RequiredAllocateHostedConnectionRequestRequestTypeDef",
     {
         "connectionId": str,
         "ownerAccount": str,
         "bandwidth": str,
         "connectionName": str,
@@ -1150,16 +1119,16 @@
 )
 
 class CreateLagRequestRequestTypeDef(
     _RequiredCreateLagRequestRequestTypeDef, _OptionalCreateLagRequestRequestTypeDef
 ):
     pass
 
-InterconnectResponseMetadataTypeDef = TypedDict(
-    "InterconnectResponseMetadataTypeDef",
+InterconnectResponseTypeDef = TypedDict(
+    "InterconnectResponseTypeDef",
     {
         "interconnectId": str,
         "interconnectName": str,
         "interconnectState": InterconnectStateType,
         "region": str,
         "location": str,
         "bandwidth": str,
@@ -1168,15 +1137,15 @@
         "awsDevice": str,
         "jumboFrameCapable": bool,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InterconnectTypeDef = TypedDict(
     "InterconnectTypeDef",
     {
         "interconnectId": str,
@@ -1359,20 +1328,20 @@
 )
 
 AssociateMacSecKeyResponseTypeDef = TypedDict(
     "AssociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ConnectionResponseMetadataTypeDef = TypedDict(
-    "ConnectionResponseMetadataTypeDef",
+ConnectionResponseTypeDef = TypedDict(
+    "ConnectionResponseTypeDef",
     {
         "ownerAccount": str,
         "connectionId": str,
         "connectionName": str,
         "connectionState": ConnectionStateType,
         "region": str,
         "location": str,
@@ -1388,15 +1357,15 @@
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "portEncryptionStatus": str,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionTypeDef = TypedDict(
     "ConnectionTypeDef",
     {
         "ownerAccount": str,
@@ -1426,15 +1395,15 @@
 )
 
 DisassociateMacSecKeyResponseTypeDef = TypedDict(
     "DisassociateMacSecKeyResponseTypeDef",
     {
         "connectionId": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DirectConnectGatewayAssociationProposalTypeDef = TypedDict(
     "DirectConnectGatewayAssociationProposalTypeDef",
     {
         "proposalId": str,
@@ -1461,16 +1430,16 @@
         "virtualGatewayId": str,
         "virtualGatewayRegion": str,
         "virtualGatewayOwnerAccount": str,
     },
     total=False,
 )
 
-VirtualInterfaceResponseMetadataTypeDef = TypedDict(
-    "VirtualInterfaceResponseMetadataTypeDef",
+VirtualInterfaceResponseTypeDef = TypedDict(
+    "VirtualInterfaceResponseTypeDef",
     {
         "ownerAccount": str,
         "virtualInterfaceId": str,
         "location": str,
         "connectionId": str,
         "virtualInterfaceType": str,
         "virtualInterfaceName": str,
@@ -1490,15 +1459,15 @@
         "routeFilterPrefixes": List[RouteFilterPrefixTypeDef],
         "bgpPeers": List[BGPPeerTypeDef],
         "region": str,
         "awsDeviceV2": str,
         "awsLogicalDeviceId": str,
         "tags": List[TagTypeDef],
         "siteLinkEnabled": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualInterfaceTypeDef = TypedDict(
     "VirtualInterfaceTypeDef",
     {
         "ownerAccount": str,
@@ -1540,134 +1509,165 @@
     total=False,
 )
 
 CreateDirectConnectGatewayResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayResultTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewaysResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewaysResultTypeDef",
     {
         "directConnectGateways": List[DirectConnectGatewayTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayResponseTypeDef = TypedDict(
     "UpdateDirectConnectGatewayResponseTypeDef",
     {
         "directConnectGateway": DirectConnectGatewayTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeCustomerMetadataResponseTypeDef = TypedDict(
     "DescribeCustomerMetadataResponseTypeDef",
     {
         "agreements": List[CustomerAgreementTypeDef],
         "nniPartnerType": NniPartnerTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeConnectionLoaResponseTypeDef = TypedDict(
     "DescribeConnectionLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeInterconnectLoaResponseTypeDef = TypedDict(
     "DescribeInterconnectLoaResponseTypeDef",
     {
         "loa": LoaTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef",
+    {
+        "associationId": str,
+        "associatedGatewayId": str,
+        "directConnectGatewayId": str,
+        "virtualGatewayId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "virtualInterfaceId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef = TypedDict(
+    "DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef",
+    {
+        "directConnectGatewayId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeDirectConnectGatewayAttachmentsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAttachmentsResultTypeDef",
     {
         "directConnectGatewayAttachments": List[DirectConnectGatewayAttachmentTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouterConfigurationResponseTypeDef = TypedDict(
     "DescribeRouterConfigurationResponseTypeDef",
     {
         "customerRouterConfig": str,
         "router": RouterTypeTypeDef,
         "virtualInterfaceId": str,
         "virtualInterfaceName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualInterfaceTestHistoryResponseTypeDef = TypedDict(
     "ListVirtualInterfaceTestHistoryResponseTypeDef",
     {
         "virtualInterfaceTestHistory": List[VirtualInterfaceTestHistoryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartBgpFailoverTestResponseTypeDef = TypedDict(
     "StartBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopBgpFailoverTestResponseTypeDef = TypedDict(
     "StopBgpFailoverTestResponseTypeDef",
     {
         "virtualInterfaceTest": VirtualInterfaceTestHistoryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LocationsTypeDef = TypedDict(
     "LocationsTypeDef",
     {
         "locations": List[LocationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualGatewaysTypeDef = TypedDict(
     "VirtualGatewaysTypeDef",
     {
         "virtualGateways": List[VirtualGatewayTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InterconnectsTypeDef = TypedDict(
     "InterconnectsTypeDef",
     {
         "interconnects": List[InterconnectTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocatePrivateVirtualInterfaceRequestRequestTypeDef = TypedDict(
     "AllocatePrivateVirtualInterfaceRequestRequestTypeDef",
     {
         "connectionId": str,
@@ -1718,28 +1718,28 @@
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "resourceTags": List[ResourceTagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ConnectionsTypeDef = TypedDict(
     "ConnectionsTypeDef",
     {
         "connections": List[ConnectionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-LagResponseMetadataTypeDef = TypedDict(
-    "LagResponseMetadataTypeDef",
+LagResponseTypeDef = TypedDict(
+    "LagResponseTypeDef",
     {
         "connectionsBandwidth": str,
         "numberOfConnections": int,
         "lagId": str,
         "ownerAccount": str,
         "lagName": str,
         "lagState": LagStateType,
@@ -1754,15 +1754,15 @@
         "jumboFrameCapable": bool,
         "hasLogicalRedundancy": HasLogicalRedundancyType,
         "tags": List[TagTypeDef],
         "providerName": str,
         "macSecCapable": bool,
         "encryptionMode": str,
         "macSecKeys": List[MacSecKeyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagTypeDef = TypedDict(
     "LagTypeDef",
     {
         "connectionsBandwidth": str,
@@ -1790,118 +1790,118 @@
     total=False,
 )
 
 CreateDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociationProposal": DirectConnectGatewayAssociationProposalTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationProposalsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationProposalsResultTypeDef",
     {
         "directConnectGatewayAssociationProposals": List[
             DirectConnectGatewayAssociationProposalTypeDef
         ],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AcceptDirectConnectGatewayAssociationProposalResultTypeDef = TypedDict(
     "AcceptDirectConnectGatewayAssociationProposalResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "CreateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "DeleteDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDirectConnectGatewayAssociationsResultTypeDef = TypedDict(
     "DescribeDirectConnectGatewayAssociationsResultTypeDef",
     {
         "directConnectGatewayAssociations": List[DirectConnectGatewayAssociationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDirectConnectGatewayAssociationResultTypeDef = TypedDict(
     "UpdateDirectConnectGatewayAssociationResultTypeDef",
     {
         "directConnectGatewayAssociation": DirectConnectGatewayAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AllocateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "AllocateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateBGPPeerResponseTypeDef = TypedDict(
     "CreateBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTransitVirtualInterfaceResultTypeDef = TypedDict(
     "CreateTransitVirtualInterfaceResultTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteBGPPeerResponseTypeDef = TypedDict(
     "DeleteBGPPeerResponseTypeDef",
     {
         "virtualInterface": VirtualInterfaceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 VirtualInterfacesTypeDef = TypedDict(
     "VirtualInterfacesTypeDef",
     {
         "virtualInterfaces": List[VirtualInterfaceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LagsTypeDef = TypedDict(
     "LagsTypeDef",
     {
         "lags": List[LagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/PKG-INFO` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-directconnect
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DirectConnect 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DirectConnect 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore directconnect type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore directconnect type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-directconnect"></a>
 
 # types-aiobotocore-directconnect
 
 [![PyPI - types-aiobotocore-directconnect](https://img.shields.io/pypi/v/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-directconnect.svg?color=blue)](https://pypi.org/project/types-aiobotocore-directconnect)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-directconnect?color=blue)](https://pypistats.org/packages/types-aiobotocore-directconnect)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-directconnect)](https://pepy.tech/project/types-aiobotocore-directconnect)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DirectConnect 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/directconnect.html#DirectConnect)
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
 [types-aiobotocore-directconnect docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_directconnect/).
 
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
@@ -335,128 +334,128 @@
 )
 
 
 def check_value(value: AddressFamilyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_directconnect.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_directconnect.type_defs import (
     RouteFilterPrefixTypeDef,
+    ResponseMetadataTypeDef,
     AllocateConnectionOnInterconnectRequestRequestTypeDef,
     TagTypeDef,
     AssociateConnectionWithLagRequestRequestTypeDef,
     AssociateHostedConnectionRequestRequestTypeDef,
     AssociateMacSecKeyRequestRequestTypeDef,
     MacSecKeyTypeDef,
     AssociateVirtualInterfaceRequestRequestTypeDef,
     AssociatedGatewayTypeDef,
     BGPPeerTypeDef,
     ConfirmConnectionRequestRequestTypeDef,
-    ConfirmConnectionResponseTypeDef,
     ConfirmCustomerAgreementRequestRequestTypeDef,
-    ConfirmCustomerAgreementResponseTypeDef,
     ConfirmPrivateVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPrivateVirtualInterfaceResponseTypeDef,
     ConfirmPublicVirtualInterfaceRequestRequestTypeDef,
-    ConfirmPublicVirtualInterfaceResponseTypeDef,
     ConfirmTransitVirtualInterfaceRequestRequestTypeDef,
-    ConfirmTransitVirtualInterfaceResponseTypeDef,
     NewBGPPeerTypeDef,
     CreateDirectConnectGatewayRequestRequestTypeDef,
     DirectConnectGatewayTypeDef,
     CustomerAgreementTypeDef,
     DeleteBGPPeerRequestRequestTypeDef,
     DeleteConnectionRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     DeleteDirectConnectGatewayAssociationRequestRequestTypeDef,
     DeleteDirectConnectGatewayRequestRequestTypeDef,
     DeleteInterconnectRequestRequestTypeDef,
-    DeleteInterconnectResponseTypeDef,
     DeleteLagRequestRequestTypeDef,
     DeleteVirtualInterfaceRequestRequestTypeDef,
-    DeleteVirtualInterfaceResponseTypeDef,
     DescribeConnectionLoaRequestRequestTypeDef,
     LoaTypeDef,
     DescribeConnectionsOnInterconnectRequestRequestTypeDef,
     DescribeConnectionsRequestRequestTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeDirectConnectGatewayAssociationsRequestRequestTypeDef,
-    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsRequestRequestTypeDef,
     DirectConnectGatewayAttachmentTypeDef,
-    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewaysRequestRequestTypeDef,
     DescribeHostedConnectionsRequestRequestTypeDef,
     DescribeInterconnectLoaRequestRequestTypeDef,
     DescribeInterconnectsRequestRequestTypeDef,
     DescribeLagsRequestRequestTypeDef,
     DescribeLoaRequestRequestTypeDef,
     DescribeRouterConfigurationRequestRequestTypeDef,
     RouterTypeTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DescribeVirtualInterfacesRequestRequestTypeDef,
     DisassociateConnectionFromLagRequestRequestTypeDef,
     DisassociateMacSecKeyRequestRequestTypeDef,
     ListVirtualInterfaceTestHistoryRequestRequestTypeDef,
     VirtualInterfaceTestHistoryTypeDef,
-    LoaResponseMetadataTypeDef,
     LocationTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     StartBgpFailoverTestRequestRequestTypeDef,
     StopBgpFailoverTestRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateConnectionRequestRequestTypeDef,
     UpdateDirectConnectGatewayRequestRequestTypeDef,
     UpdateLagRequestRequestTypeDef,
     UpdateVirtualInterfaceAttributesRequestRequestTypeDef,
     VirtualGatewayTypeDef,
     AcceptDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationProposalRequestRequestTypeDef,
     CreateDirectConnectGatewayAssociationRequestRequestTypeDef,
     UpdateDirectConnectGatewayAssociationRequestRequestTypeDef,
+    ConfirmConnectionResponseTypeDef,
+    ConfirmCustomerAgreementResponseTypeDef,
+    ConfirmPrivateVirtualInterfaceResponseTypeDef,
+    ConfirmPublicVirtualInterfaceResponseTypeDef,
+    ConfirmTransitVirtualInterfaceResponseTypeDef,
+    DeleteInterconnectResponseTypeDef,
+    DeleteVirtualInterfaceResponseTypeDef,
+    LoaResponseTypeDef,
     AllocateHostedConnectionRequestRequestTypeDef,
     CreateConnectionRequestRequestTypeDef,
     CreateInterconnectRequestRequestTypeDef,
     CreateLagRequestRequestTypeDef,
-    InterconnectResponseMetadataTypeDef,
+    InterconnectResponseTypeDef,
     InterconnectTypeDef,
     NewPrivateVirtualInterfaceAllocationTypeDef,
     NewPrivateVirtualInterfaceTypeDef,
     NewPublicVirtualInterfaceAllocationTypeDef,
     NewPublicVirtualInterfaceTypeDef,
     NewTransitVirtualInterfaceAllocationTypeDef,
     NewTransitVirtualInterfaceTypeDef,
     ResourceTagTypeDef,
     TagResourceRequestRequestTypeDef,
     AssociateMacSecKeyResponseTypeDef,
-    ConnectionResponseMetadataTypeDef,
+    ConnectionResponseTypeDef,
     ConnectionTypeDef,
     DisassociateMacSecKeyResponseTypeDef,
     DirectConnectGatewayAssociationProposalTypeDef,
     DirectConnectGatewayAssociationTypeDef,
-    VirtualInterfaceResponseMetadataTypeDef,
+    VirtualInterfaceResponseTypeDef,
     VirtualInterfaceTypeDef,
     CreateBGPPeerRequestRequestTypeDef,
     CreateDirectConnectGatewayResultTypeDef,
     DeleteDirectConnectGatewayResultTypeDef,
     DescribeDirectConnectGatewaysResultTypeDef,
     UpdateDirectConnectGatewayResponseTypeDef,
     DescribeCustomerMetadataResponseTypeDef,
     DescribeConnectionLoaResponseTypeDef,
     DescribeInterconnectLoaResponseTypeDef,
+    DescribeDirectConnectGatewayAssociationsRequestDescribeDirectConnectGatewayAssociationsPaginateTypeDef,
+    DescribeDirectConnectGatewayAttachmentsRequestDescribeDirectConnectGatewayAttachmentsPaginateTypeDef,
+    DescribeDirectConnectGatewaysRequestDescribeDirectConnectGatewaysPaginateTypeDef,
     DescribeDirectConnectGatewayAttachmentsResultTypeDef,
     DescribeRouterConfigurationResponseTypeDef,
     ListVirtualInterfaceTestHistoryResponseTypeDef,
     StartBgpFailoverTestResponseTypeDef,
     StopBgpFailoverTestResponseTypeDef,
     LocationsTypeDef,
     VirtualGatewaysTypeDef,
@@ -465,15 +464,15 @@
     CreatePrivateVirtualInterfaceRequestRequestTypeDef,
     AllocatePublicVirtualInterfaceRequestRequestTypeDef,
     CreatePublicVirtualInterfaceRequestRequestTypeDef,
     AllocateTransitVirtualInterfaceRequestRequestTypeDef,
     CreateTransitVirtualInterfaceRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ConnectionsTypeDef,
-    LagResponseMetadataTypeDef,
+    LagResponseTypeDef,
     LagTypeDef,
     CreateDirectConnectGatewayAssociationProposalResultTypeDef,
     DeleteDirectConnectGatewayAssociationProposalResultTypeDef,
     DescribeDirectConnectGatewayAssociationProposalsResultTypeDef,
     AcceptDirectConnectGatewayAssociationProposalResultTypeDef,
     CreateDirectConnectGatewayAssociationResultTypeDef,
     DeleteDirectConnectGatewayAssociationResultTypeDef,
@@ -484,15 +483,15 @@
     CreateTransitVirtualInterfaceResultTypeDef,
     DeleteBGPPeerResponseTypeDef,
     VirtualInterfacesTypeDef,
     LagsTypeDef,
 )
 
 
-def get_structure() -> RouteFilterPrefixTypeDef:
+def get_value() -> RouteFilterPrefixTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-directconnect-2.5.2/types_aiobotocore_directconnect.egg-info/SOURCES.txt` & `types-aiobotocore-directconnect-2.5.2.post1/types_aiobotocore_directconnect.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-appmesh-2.5.2.tar.gz` & `tmp/types-aiobotocore-appmesh-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appmesh-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-appmesh-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
```

## Comparing `types-aiobotocore-appmesh-2.5.2.tar` & `types-aiobotocore-appmesh-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.629695 types-aiobotocore-appmesh-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-07-08 01:43:14.621695 types-aiobotocore-appmesh-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    21267 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.629695 types-aiobotocore-appmesh-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.621695 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32306 2023-07-08 01:25:52.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    32251 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-08 01:25:52.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-07-08 01:25:52.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-07-08 01:25:52.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-07-08 01:25:52.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    80506 2023-07-08 01:25:54.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    80355 2023-07-08 01:25:53.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:51.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.621695 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    22832 2023-07-08 01:43:14.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:14.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:14.000000 types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.809654 types-aiobotocore-appmesh-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-08-02 14:51:52.805654 types-aiobotocore-appmesh-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23329 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.809654 types-aiobotocore-appmesh-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.801654 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32381 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32326 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9937 2023-08-02 14:33:18.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   100998 2023-08-02 14:33:20.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100807 2023-08-02 14:33:19.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:17.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.805654 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24847 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:52.000000 types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appmesh-2.5.2/LICENSE` & `types-aiobotocore-appmesh-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2/PKG-INFO` & `types-aiobotocore-appmesh-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appmesh
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appmesh type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appmesh type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appmesh"></a>
 
 # types-aiobotocore-appmesh
 
 [![PyPI - types-aiobotocore-appmesh](https://img.shields.io/pypi/v/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appmesh?color=blue)](https://pypistats.org/packages/types-aiobotocore-appmesh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppMesh 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [types-aiobotocore-appmesh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/).
 
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
@@ -359,27 +358,28 @@
 )
 
 
 def check_value(value: DefaultGatewayRouteRewriteType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appmesh.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
@@ -403,209 +403,263 @@
     WeightedTargetTypeDef,
     HealthCheckPolicyTypeDef,
     HttpPathMatchTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
     QueryParameterMatchTypeDef,
     JsonFormatRefTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
+    PortMappingTypeDef,
     ListenerTlsAcmCertificateTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
-    PortMappingTypeDef,
     MeshStatusTypeDef,
     MeshServiceDiscoveryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
+    SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
     TcpRouteMatchTypeDef,
+    TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
+    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    VirtualGatewayPortMappingTypeDef,
+    VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
+    AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
     ClientTlsCertificateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    GrpcRetryPolicyOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
+    HttpRetryPolicyOutputTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
     GatewayRouteTargetTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
+    GrpcRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
+    HttpRouteActionOutputTypeDef,
     HttpRouteActionTypeDef,
+    TcpRouteActionOutputTypeDef,
     TcpRouteActionTypeDef,
     HttpGatewayRouteRewriteTypeDef,
     HttpQueryParameterTypeDef,
+    LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
+    VirtualRouterListenerTypeDef,
     ListenerTlsCertificateTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
-    VirtualRouterListenerTypeDef,
     MeshSpecTypeDef,
+    SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
+    TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
     VirtualNodeConnectionPoolTypeDef,
     VirtualServiceProviderTypeDef,
+    ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
     ListenerTimeoutTypeDef,
     GrpcGatewayRouteActionTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
+    TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
     HttpGatewayRouteActionTypeDef,
+    FileAccessLogOutputTypeDef,
+    VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
     CreateMeshInputRequestTypeDef,
     MeshDataTypeDef,
     UpdateMeshInputRequestTypeDef,
+    ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
+    TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
+    VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
+    VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
     VirtualServiceSpecTypeDef,
+    GrpcGatewayRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
+    GrpcRouteMatchOutputTypeDef,
     GrpcRouteMatchTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
     HttpGatewayRouteMatchTypeDef,
+    HttpRouteMatchOutputTypeDef,
     HttpRouteMatchTypeDef,
+    AccessLogOutputTypeDef,
+    VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
+    VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
-    VirtualRouterDataTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
+    ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
+    ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
+    VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
+    VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
     VirtualServiceDataTypeDef,
+    GrpcGatewayRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
+    GrpcRouteOutputTypeDef,
     GrpcRouteTypeDef,
+    HttpGatewayRouteOutputTypeDef,
     HttpGatewayRouteTypeDef,
+    HttpRouteOutputTypeDef,
     HttpRouteTypeDef,
+    LoggingOutputTypeDef,
+    VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
+    ListenerOutputTypeDef,
     ListenerTypeDef,
+    ClientPolicyOutputTypeDef,
     ClientPolicyTypeDef,
+    VirtualGatewayListenerOutputTypeDef,
     VirtualGatewayListenerTypeDef,
+    VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
+    BackendDefaultsOutputTypeDef,
+    VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
+    VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
-    CreateGatewayRouteInputRequestTypeDef,
     GatewayRouteDataTypeDef,
+    CreateGatewayRouteInputRequestTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
-    CreateRouteInputRequestTypeDef,
     RouteDataTypeDef,
+    CreateRouteInputRequestTypeDef,
+    RouteSpecUnionTypeDef,
     UpdateRouteInputRequestTypeDef,
+    BackendOutputTypeDef,
     BackendTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
     DescribeGatewayRouteOutputTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     CreateRouteOutputTypeDef,
     DeleteRouteOutputTypeDef,
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
-    VirtualGatewayDataTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
-    VirtualNodeDataTypeDef,
+    VirtualNodeSpecUnionTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_value() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appmesh-2.5.2/README.md` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-appmesh
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore appmesh type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appmesh"></a>
 
 # types-aiobotocore-appmesh
 
 [![PyPI - types-aiobotocore-appmesh](https://img.shields.io/pypi/v/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appmesh?color=blue)](https://pypistats.org/packages/types-aiobotocore-appmesh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppMesh 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [types-aiobotocore-appmesh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/).
 
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
@@ -326,27 +358,28 @@
 )
 
 
 def check_value(value: DefaultGatewayRouteRewriteType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appmesh.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
@@ -370,209 +403,263 @@
     WeightedTargetTypeDef,
     HealthCheckPolicyTypeDef,
     HttpPathMatchTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
     QueryParameterMatchTypeDef,
     JsonFormatRefTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
+    PortMappingTypeDef,
     ListenerTlsAcmCertificateTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
-    PortMappingTypeDef,
     MeshStatusTypeDef,
     MeshServiceDiscoveryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
+    SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
     TcpRouteMatchTypeDef,
+    TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
+    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    VirtualGatewayPortMappingTypeDef,
+    VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
+    AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
     ClientTlsCertificateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    GrpcRetryPolicyOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
+    HttpRetryPolicyOutputTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
     GatewayRouteTargetTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
+    GrpcRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
+    HttpRouteActionOutputTypeDef,
     HttpRouteActionTypeDef,
+    TcpRouteActionOutputTypeDef,
     TcpRouteActionTypeDef,
     HttpGatewayRouteRewriteTypeDef,
     HttpQueryParameterTypeDef,
+    LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
+    VirtualRouterListenerTypeDef,
     ListenerTlsCertificateTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
-    VirtualRouterListenerTypeDef,
     MeshSpecTypeDef,
+    SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
+    TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
     VirtualNodeConnectionPoolTypeDef,
     VirtualServiceProviderTypeDef,
+    ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
     ListenerTimeoutTypeDef,
     GrpcGatewayRouteActionTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
+    TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
     HttpGatewayRouteActionTypeDef,
+    FileAccessLogOutputTypeDef,
+    VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
     CreateMeshInputRequestTypeDef,
     MeshDataTypeDef,
     UpdateMeshInputRequestTypeDef,
+    ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
+    TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
+    VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
+    VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
     VirtualServiceSpecTypeDef,
+    GrpcGatewayRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
+    GrpcRouteMatchOutputTypeDef,
     GrpcRouteMatchTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
     HttpGatewayRouteMatchTypeDef,
+    HttpRouteMatchOutputTypeDef,
     HttpRouteMatchTypeDef,
+    AccessLogOutputTypeDef,
+    VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
+    VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
-    VirtualRouterDataTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
+    ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
+    ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
+    VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
+    VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
     VirtualServiceDataTypeDef,
+    GrpcGatewayRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
+    GrpcRouteOutputTypeDef,
     GrpcRouteTypeDef,
+    HttpGatewayRouteOutputTypeDef,
     HttpGatewayRouteTypeDef,
+    HttpRouteOutputTypeDef,
     HttpRouteTypeDef,
+    LoggingOutputTypeDef,
+    VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
+    ListenerOutputTypeDef,
     ListenerTypeDef,
+    ClientPolicyOutputTypeDef,
     ClientPolicyTypeDef,
+    VirtualGatewayListenerOutputTypeDef,
     VirtualGatewayListenerTypeDef,
+    VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
+    BackendDefaultsOutputTypeDef,
+    VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
+    VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
-    CreateGatewayRouteInputRequestTypeDef,
     GatewayRouteDataTypeDef,
+    CreateGatewayRouteInputRequestTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
-    CreateRouteInputRequestTypeDef,
     RouteDataTypeDef,
+    CreateRouteInputRequestTypeDef,
+    RouteSpecUnionTypeDef,
     UpdateRouteInputRequestTypeDef,
+    BackendOutputTypeDef,
     BackendTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
     DescribeGatewayRouteOutputTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     CreateRouteOutputTypeDef,
     DeleteRouteOutputTypeDef,
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
-    VirtualGatewayDataTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
-    VirtualNodeDataTypeDef,
+    VirtualNodeSpecUnionTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_value() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appmesh-2.5.2/setup.py` & `types-aiobotocore-appmesh-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appmesh",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_appmesh"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore appmesh type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore appmesh type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appmesh": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/"
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/__init__.py` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/__init__.pyi` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/__main__.py` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppMesh 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AppMesh 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh\nOther"
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

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/client.py` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -48,70 +48,66 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
-    GatewayRouteSpecTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
-    RouteSpecTypeDef,
+    RouteSpecUnionTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
-    VirtualGatewaySpecTypeDef,
-    VirtualNodeSpecTypeDef,
-    VirtualRouterSpecTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeSpecUnionTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AppMeshClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
-
 class AppMeshClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/)
     """
 
     meta: ClientMeta
@@ -120,133 +116,124 @@
     def exceptions(self) -> Exceptions:
         """
         AppMeshClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#close)
         """
-
     async def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_gateway_route)
         """
-
     async def create_mesh(
         self,
         *,
         meshName: str,
         clientToken: str = ...,
         spec: MeshSpecTypeDef = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateMeshOutputTypeDef:
         """
         Creates a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_mesh)
         """
-
     async def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_route)
         """
-
     async def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_gateway)
         """
-
     async def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_node)
         """
-
     async def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_router)
         """
-
     async def create_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -255,167 +242,151 @@
     ) -> CreateVirtualServiceOutputTypeDef:
         """
         Creates a virtual service within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_service)
         """
-
     async def delete_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteGatewayRouteOutputTypeDef:
         """
         Deletes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_gateway_route)
         """
-
     async def delete_mesh(self, *, meshName: str) -> DeleteMeshOutputTypeDef:
         """
         Deletes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_mesh)
         """
-
     async def delete_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteRouteOutputTypeDef:
         """
         Deletes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_route)
         """
-
     async def delete_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteVirtualGatewayOutputTypeDef:
         """
         Deletes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_gateway)
         """
-
     async def delete_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DeleteVirtualNodeOutputTypeDef:
         """
         Deletes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_node)
         """
-
     async def delete_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteVirtualRouterOutputTypeDef:
         """
         Deletes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_router)
         """
-
     async def delete_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DeleteVirtualServiceOutputTypeDef:
         """
         Deletes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_service)
         """
-
     async def describe_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeGatewayRouteOutputTypeDef:
         """
         Describes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_gateway_route)
         """
-
     async def describe_mesh(
         self, *, meshName: str, meshOwner: str = ...
     ) -> DescribeMeshOutputTypeDef:
         """
         Describes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_mesh)
         """
-
     async def describe_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeRouteOutputTypeDef:
         """
         Describes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_route)
         """
-
     async def describe_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeVirtualGatewayOutputTypeDef:
         """
         Describes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_gateway)
         """
-
     async def describe_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DescribeVirtualNodeOutputTypeDef:
         """
         Describes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_node)
         """
-
     async def describe_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeVirtualRouterOutputTypeDef:
         """
         Describes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_router)
         """
-
     async def describe_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DescribeVirtualServiceOutputTypeDef:
         """
         Describes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_service)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#generate_presigned_url)
         """
-
     async def list_gateway_routes(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -424,25 +395,23 @@
         """
         Returns a list of existing gateway routes that are associated to a virtual
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_gateway_routes)
         """
-
     async def list_meshes(
         self, *, limit: int = ..., nextToken: str = ...
     ) -> ListMeshesOutputTypeDef:
         """
         Returns a list of existing service meshes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_meshes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_meshes)
         """
-
     async def list_routes(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -450,176 +419,162 @@
     ) -> ListRoutesOutputTypeDef:
         """
         Returns a list of existing routes in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_routes)
         """
-
     async def list_tags_for_resource(
         self, *, resourceArn: str, limit: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         List the tags for an App Mesh resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_tags_for_resource)
         """
-
     async def list_virtual_gateways(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualGatewaysOutputTypeDef:
         """
         Returns a list of existing virtual gateways in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_gateways)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_gateways)
         """
-
     async def list_virtual_nodes(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualNodesOutputTypeDef:
         """
         Returns a list of existing virtual nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_nodes)
         """
-
     async def list_virtual_routers(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualRoutersOutputTypeDef:
         """
         Returns a list of existing virtual routers in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_routers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_routers)
         """
-
     async def list_virtual_services(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualServicesOutputTypeDef:
         """
         Returns a list of existing virtual services in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_services)
         """
-
     async def tag_resource(
         self, *, resourceArn: str, tags: Sequence[TagRefTypeDef]
     ) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#tag_resource)
         """
-
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#untag_resource)
         """
-
     async def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_gateway_route)
         """
-
     async def update_mesh(
         self, *, meshName: str, clientToken: str = ..., spec: MeshSpecTypeDef = ...
     ) -> UpdateMeshOutputTypeDef:
         """
         Updates an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_mesh)
         """
-
     async def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_route)
         """
-
     async def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_gateway)
         """
-
     async def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_node)
         """
-
     async def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_router)
         """
-
     async def update_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -627,87 +582,77 @@
     ) -> UpdateVirtualServiceOutputTypeDef:
         """
         Updates an existing virtual service in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_service)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_gateway_routes"]
     ) -> ListGatewayRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_meshes"]) -> ListMeshesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_gateways"]
     ) -> ListVirtualGatewaysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_nodes"]
     ) -> ListVirtualNodesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_routers"]
     ) -> ListVirtualRoutersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_services"]
     ) -> ListVirtualServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "AppMeshClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/)
         """
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/client.pyi` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -48,66 +48,70 @@
     DescribeGatewayRouteOutputTypeDef,
     DescribeMeshOutputTypeDef,
     DescribeRouteOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
-    GatewayRouteSpecTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     ListGatewayRoutesOutputTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
     MeshSpecTypeDef,
-    RouteSpecTypeDef,
+    RouteSpecUnionTypeDef,
     TagRefTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     UpdateMeshOutputTypeDef,
     UpdateRouteOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
-    VirtualGatewaySpecTypeDef,
-    VirtualNodeSpecTypeDef,
-    VirtualRouterSpecTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeSpecUnionTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     VirtualServiceSpecTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AppMeshClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     BadRequestException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     ForbiddenException: Type[BotocoreClientError]
     InternalServerErrorException: Type[BotocoreClientError]
     LimitExceededException: Type[BotocoreClientError]
     NotFoundException: Type[BotocoreClientError]
     ResourceInUseException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     TooManyRequestsException: Type[BotocoreClientError]
     TooManyTagsException: Type[BotocoreClientError]
 
+
 class AppMeshClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/)
     """
 
     meta: ClientMeta
@@ -116,124 +120,133 @@
     def exceptions(self) -> Exceptions:
         """
         AppMeshClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#close)
         """
+
     async def create_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateGatewayRouteOutputTypeDef:
         """
         Creates a gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_gateway_route)
         """
+
     async def create_mesh(
         self,
         *,
         meshName: str,
         clientToken: str = ...,
         spec: MeshSpecTypeDef = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateMeshOutputTypeDef:
         """
         Creates a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_mesh)
         """
+
     async def create_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateRouteOutputTypeDef:
         """
         Creates a route that is associated with a virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_route)
         """
+
     async def create_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualGatewayOutputTypeDef:
         """
         Creates a virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_gateway)
         """
+
     async def create_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualNodeOutputTypeDef:
         """
         Creates a virtual node within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_node)
         """
+
     async def create_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...,
         tags: Sequence[TagRefTypeDef] = ...
     ) -> CreateVirtualRouterOutputTypeDef:
         """
         Creates a virtual router within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_router)
         """
+
     async def create_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -242,151 +255,167 @@
     ) -> CreateVirtualServiceOutputTypeDef:
         """
         Creates a virtual service within a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.create_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#create_virtual_service)
         """
+
     async def delete_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteGatewayRouteOutputTypeDef:
         """
         Deletes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_gateway_route)
         """
+
     async def delete_mesh(self, *, meshName: str) -> DeleteMeshOutputTypeDef:
         """
         Deletes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_mesh)
         """
+
     async def delete_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteRouteOutputTypeDef:
         """
         Deletes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_route)
         """
+
     async def delete_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DeleteVirtualGatewayOutputTypeDef:
         """
         Deletes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_gateway)
         """
+
     async def delete_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DeleteVirtualNodeOutputTypeDef:
         """
         Deletes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_node)
         """
+
     async def delete_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DeleteVirtualRouterOutputTypeDef:
         """
         Deletes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_router)
         """
+
     async def delete_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DeleteVirtualServiceOutputTypeDef:
         """
         Deletes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.delete_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#delete_virtual_service)
         """
+
     async def describe_gateway_route(
         self, *, gatewayRouteName: str, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeGatewayRouteOutputTypeDef:
         """
         Describes an existing gateway route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_gateway_route)
         """
+
     async def describe_mesh(
         self, *, meshName: str, meshOwner: str = ...
     ) -> DescribeMeshOutputTypeDef:
         """
         Describes an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_mesh)
         """
+
     async def describe_route(
         self, *, meshName: str, routeName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeRouteOutputTypeDef:
         """
         Describes an existing route.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_route)
         """
+
     async def describe_virtual_gateway(
         self, *, meshName: str, virtualGatewayName: str, meshOwner: str = ...
     ) -> DescribeVirtualGatewayOutputTypeDef:
         """
         Describes an existing virtual gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_gateway)
         """
+
     async def describe_virtual_node(
         self, *, meshName: str, virtualNodeName: str, meshOwner: str = ...
     ) -> DescribeVirtualNodeOutputTypeDef:
         """
         Describes an existing virtual node.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_node)
         """
+
     async def describe_virtual_router(
         self, *, meshName: str, virtualRouterName: str, meshOwner: str = ...
     ) -> DescribeVirtualRouterOutputTypeDef:
         """
         Describes an existing virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_router)
         """
+
     async def describe_virtual_service(
         self, *, meshName: str, virtualServiceName: str, meshOwner: str = ...
     ) -> DescribeVirtualServiceOutputTypeDef:
         """
         Describes an existing virtual service.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.describe_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#describe_virtual_service)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#generate_presigned_url)
         """
+
     async def list_gateway_routes(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -395,23 +424,25 @@
         """
         Returns a list of existing gateway routes that are associated to a virtual
         gateway.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_gateway_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_gateway_routes)
         """
+
     async def list_meshes(
         self, *, limit: int = ..., nextToken: str = ...
     ) -> ListMeshesOutputTypeDef:
         """
         Returns a list of existing service meshes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_meshes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_meshes)
         """
+
     async def list_routes(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         limit: int = ...,
         meshOwner: str = ...,
@@ -419,162 +450,176 @@
     ) -> ListRoutesOutputTypeDef:
         """
         Returns a list of existing routes in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_routes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_routes)
         """
+
     async def list_tags_for_resource(
         self, *, resourceArn: str, limit: int = ..., nextToken: str = ...
     ) -> ListTagsForResourceOutputTypeDef:
         """
         List the tags for an App Mesh resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_tags_for_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_tags_for_resource)
         """
+
     async def list_virtual_gateways(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualGatewaysOutputTypeDef:
         """
         Returns a list of existing virtual gateways in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_gateways)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_gateways)
         """
+
     async def list_virtual_nodes(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualNodesOutputTypeDef:
         """
         Returns a list of existing virtual nodes.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_nodes)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_nodes)
         """
+
     async def list_virtual_routers(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualRoutersOutputTypeDef:
         """
         Returns a list of existing virtual routers in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_routers)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_routers)
         """
+
     async def list_virtual_services(
         self, *, meshName: str, limit: int = ..., meshOwner: str = ..., nextToken: str = ...
     ) -> ListVirtualServicesOutputTypeDef:
         """
         Returns a list of existing virtual services in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.list_virtual_services)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#list_virtual_services)
         """
+
     async def tag_resource(
         self, *, resourceArn: str, tags: Sequence[TagRefTypeDef]
     ) -> Dict[str, Any]:
         """
         Associates the specified tags to a resource with the specified `resourceArn`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.tag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#tag_resource)
         """
+
     async def untag_resource(self, *, resourceArn: str, tagKeys: Sequence[str]) -> Dict[str, Any]:
         """
         Deletes specified tags from a resource.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.untag_resource)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#untag_resource)
         """
+
     async def update_gateway_route(
         self,
         *,
         gatewayRouteName: str,
         meshName: str,
-        spec: GatewayRouteSpecTypeDef,
+        spec: GatewayRouteSpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateGatewayRouteOutputTypeDef:
         """
         Updates an existing gateway route that is associated to a specified virtual
         gateway in a service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_gateway_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_gateway_route)
         """
+
     async def update_mesh(
         self, *, meshName: str, clientToken: str = ..., spec: MeshSpecTypeDef = ...
     ) -> UpdateMeshOutputTypeDef:
         """
         Updates an existing service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_mesh)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_mesh)
         """
+
     async def update_route(
         self,
         *,
         meshName: str,
         routeName: str,
-        spec: RouteSpecTypeDef,
+        spec: RouteSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateRouteOutputTypeDef:
         """
         Updates an existing route for a specified service mesh and virtual router.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_route)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_route)
         """
+
     async def update_virtual_gateway(
         self,
         *,
         meshName: str,
-        spec: VirtualGatewaySpecTypeDef,
+        spec: VirtualGatewaySpecUnionTypeDef,
         virtualGatewayName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualGatewayOutputTypeDef:
         """
         Updates an existing virtual gateway in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_gateway)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_gateway)
         """
+
     async def update_virtual_node(
         self,
         *,
         meshName: str,
-        spec: VirtualNodeSpecTypeDef,
+        spec: VirtualNodeSpecUnionTypeDef,
         virtualNodeName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualNodeOutputTypeDef:
         """
         Updates an existing virtual node in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_node)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_node)
         """
+
     async def update_virtual_router(
         self,
         *,
         meshName: str,
-        spec: VirtualRouterSpecTypeDef,
+        spec: VirtualRouterSpecUnionTypeDef,
         virtualRouterName: str,
         clientToken: str = ...,
         meshOwner: str = ...
     ) -> UpdateVirtualRouterOutputTypeDef:
         """
         Updates an existing virtual router in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_router)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_router)
         """
+
     async def update_virtual_service(
         self,
         *,
         meshName: str,
         spec: VirtualServiceSpecTypeDef,
         virtualServiceName: str,
         clientToken: str = ...,
@@ -582,77 +627,87 @@
     ) -> UpdateVirtualServiceOutputTypeDef:
         """
         Updates an existing virtual service in a specified service mesh.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.update_virtual_service)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#update_virtual_service)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_gateway_routes"]
     ) -> ListGatewayRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_meshes"]) -> ListMeshesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(self, operation_name: Literal["list_routes"]) -> ListRoutesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_tags_for_resource"]
     ) -> ListTagsForResourcePaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_gateways"]
     ) -> ListVirtualGatewaysPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_nodes"]
     ) -> ListVirtualNodesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_routers"]
     ) -> ListVirtualRoutersPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     @overload
     def get_paginator(
         self, operation_name: Literal["list_virtual_services"]
     ) -> ListVirtualServicesPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "AppMeshClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/client/)
         """
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/literals.py` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/literals.pyi` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/paginator.py` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,30 +81,30 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listgatewayroutespaginator)
         """
 
 
 class ListMeshesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listmeshespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMeshesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listmeshespaginator)
         """
 
 
@@ -116,104 +116,88 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listroutespaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listtagsforresourcepaginator)
         """
 
 
 class ListVirtualGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualgatewayspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualgatewayspaginator)
         """
 
 
 class ListVirtualNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualnodespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualNodesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualnodespaginator)
         """
 
 
 class ListVirtualRoutersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualrouterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualRoutersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualrouterspaginator)
         """
 
 
 class ListVirtualServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualservicespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualservicespaginator)
         """
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/paginator.pyi` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -78,29 +78,29 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualGatewayName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGatewayRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListGatewayRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listgatewayroutespaginator)
         """
 
 class ListMeshesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listmeshespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMeshesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListMeshes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listmeshespaginator)
         """
 
 class ListRoutesPaginator(AioPaginator):
@@ -111,99 +111,83 @@
 
     def paginate(
         self,
         *,
         meshName: str,
         virtualRouterName: str,
         meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoutesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listroutespaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, resourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, resourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listtagsforresourcepaginator)
         """
 
 class ListVirtualGatewaysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualgatewayspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualGatewaysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualGateways.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualgatewayspaginator)
         """
 
 class ListVirtualNodesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualnodespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualNodesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualNodes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualnodespaginator)
         """
 
 class ListVirtualRoutersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualrouterspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualRoutersOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualRouters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualrouterspaginator)
         """
 
 class ListVirtualServicesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualservicespaginator)
     """
 
     def paginate(
-        self,
-        *,
-        meshName: str,
-        meshOwner: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, meshName: str, meshOwner: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListVirtualServicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh.Paginator.ListVirtualServices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/paginators/#listvirtualservicespaginator)
         """
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/type_defs.py` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
-    data: AwsCloudMapInstanceAttributeTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     DefaultGatewayRouteRewriteType,
     DnsResponseTypeType,
     DurationUnitType,
     EgressFilterTypeType,
     GatewayRouteStatusCodeType,
@@ -42,20 +42,20 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AwsCloudMapInstanceAttributeTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
     "DeleteVirtualNodeInputRequestTypeDef",
     "DeleteVirtualRouterInputRequestTypeDef",
     "DeleteVirtualServiceInputRequestTypeDef",
@@ -79,197 +79,251 @@
     "WeightedTargetTypeDef",
     "HealthCheckPolicyTypeDef",
     "HttpPathMatchTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
     "QueryParameterMatchTypeDef",
     "JsonFormatRefTypeDef",
-    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
-    "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
-    "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
-    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
-    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
-    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
+    "PortMappingTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
-    "PortMappingTypeDef",
     "MeshStatusTypeDef",
     "MeshServiceDiscoveryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
+    "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
     "TcpRouteMatchTypeDef",
+    "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
+    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
-    "VirtualGatewayPortMappingTypeDef",
+    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
+    "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
     "ClientTlsCertificateTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "GrpcRetryPolicyOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
+    "HttpRetryPolicyOutputTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
     "GatewayRouteTargetTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
+    "GrpcRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
+    "HttpRouteActionOutputTypeDef",
     "HttpRouteActionTypeDef",
+    "TcpRouteActionOutputTypeDef",
     "TcpRouteActionTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
     "HttpQueryParameterTypeDef",
+    "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
+    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    "ListRoutesInputListRoutesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
+    "VirtualRouterListenerTypeDef",
     "ListenerTlsCertificateTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
-    "VirtualRouterListenerTypeDef",
     "MeshSpecTypeDef",
+    "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
+    "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
+    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
     "VirtualServiceProviderTypeDef",
+    "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
     "ListenerTimeoutTypeDef",
     "GrpcGatewayRouteActionTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
+    "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
     "HttpGatewayRouteActionTypeDef",
+    "FileAccessLogOutputTypeDef",
+    "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
+    "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
     "CreateMeshInputRequestTypeDef",
     "MeshDataTypeDef",
     "UpdateMeshInputRequestTypeDef",
+    "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
+    "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
+    "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
+    "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
     "VirtualServiceSpecTypeDef",
+    "GrpcGatewayRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
+    "GrpcRouteMatchOutputTypeDef",
     "GrpcRouteMatchTypeDef",
+    "HttpGatewayRouteMatchOutputTypeDef",
     "HttpGatewayRouteMatchTypeDef",
+    "HttpRouteMatchOutputTypeDef",
     "HttpRouteMatchTypeDef",
+    "AccessLogOutputTypeDef",
+    "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
+    "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
-    "VirtualRouterDataTypeDef",
+    "VirtualRouterSpecUnionTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
+    "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
+    "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
+    "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
+    "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
     "VirtualServiceDataTypeDef",
+    "GrpcGatewayRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
+    "GrpcRouteOutputTypeDef",
     "GrpcRouteTypeDef",
+    "HttpGatewayRouteOutputTypeDef",
     "HttpGatewayRouteTypeDef",
+    "HttpRouteOutputTypeDef",
     "HttpRouteTypeDef",
+    "LoggingOutputTypeDef",
+    "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
     "DescribeVirtualRouterOutputTypeDef",
     "UpdateVirtualRouterOutputTypeDef",
+    "ListenerOutputTypeDef",
     "ListenerTypeDef",
+    "ClientPolicyOutputTypeDef",
     "ClientPolicyTypeDef",
+    "VirtualGatewayListenerOutputTypeDef",
     "VirtualGatewayListenerTypeDef",
+    "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
+    "GatewayRouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
+    "RouteSpecOutputTypeDef",
     "RouteSpecTypeDef",
+    "BackendDefaultsOutputTypeDef",
+    "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
+    "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
-    "CreateGatewayRouteInputRequestTypeDef",
     "GatewayRouteDataTypeDef",
+    "CreateGatewayRouteInputRequestTypeDef",
+    "GatewayRouteSpecUnionTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
-    "CreateRouteInputRequestTypeDef",
     "RouteDataTypeDef",
+    "CreateRouteInputRequestTypeDef",
+    "RouteSpecUnionTypeDef",
     "UpdateRouteInputRequestTypeDef",
+    "BackendOutputTypeDef",
     "BackendTypeDef",
+    "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
     "DescribeGatewayRouteOutputTypeDef",
     "UpdateGatewayRouteOutputTypeDef",
     "CreateRouteOutputTypeDef",
     "DeleteRouteOutputTypeDef",
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
+    "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
+    "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
-    "VirtualGatewayDataTypeDef",
+    "VirtualGatewaySpecUnionTypeDef",
+    "VirtualNodeDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
-    "VirtualNodeDataTypeDef",
+    "VirtualNodeSpecUnionTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
@@ -303,14 +357,25 @@
     "TagRefTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredDeleteGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDeleteGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -319,21 +384,19 @@
     "_OptionalDeleteGatewayRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteGatewayRouteInputRequestTypeDef(
     _RequiredDeleteGatewayRouteInputRequestTypeDef, _OptionalDeleteGatewayRouteInputRequestTypeDef
 ):
     pass
 
-
 DeleteMeshInputRequestTypeDef = TypedDict(
     "DeleteMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 
@@ -349,21 +412,19 @@
     "_OptionalDeleteRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteRouteInputRequestTypeDef(
     _RequiredDeleteRouteInputRequestTypeDef, _OptionalDeleteRouteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -371,22 +432,20 @@
     "_OptionalDeleteVirtualGatewayInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualGatewayInputRequestTypeDef(
     _RequiredDeleteVirtualGatewayInputRequestTypeDef,
     _OptionalDeleteVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDeleteVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "virtualNodeName": str,
     },
 )
@@ -394,21 +453,19 @@
     "_OptionalDeleteVirtualNodeInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualNodeInputRequestTypeDef(
     _RequiredDeleteVirtualNodeInputRequestTypeDef, _OptionalDeleteVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -416,21 +473,19 @@
     "_OptionalDeleteVirtualRouterInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualRouterInputRequestTypeDef(
     _RequiredDeleteVirtualRouterInputRequestTypeDef, _OptionalDeleteVirtualRouterInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDeleteVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "virtualServiceName": str,
     },
 )
@@ -438,22 +493,20 @@
     "_OptionalDeleteVirtualServiceInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DeleteVirtualServiceInputRequestTypeDef(
     _RequiredDeleteVirtualServiceInputRequestTypeDef,
     _OptionalDeleteVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDescribeGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -462,43 +515,39 @@
     "_OptionalDescribeGatewayRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeGatewayRouteInputRequestTypeDef(
     _RequiredDescribeGatewayRouteInputRequestTypeDef,
     _OptionalDescribeGatewayRouteInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeMeshInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalDescribeMeshInputRequestTypeDef = TypedDict(
     "_OptionalDescribeMeshInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeMeshInputRequestTypeDef(
     _RequiredDescribeMeshInputRequestTypeDef, _OptionalDescribeMeshInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeRouteInputRequestTypeDef = TypedDict(
     "_RequiredDescribeRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "virtualRouterName": str,
     },
@@ -507,21 +556,19 @@
     "_OptionalDescribeRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeRouteInputRequestTypeDef(
     _RequiredDescribeRouteInputRequestTypeDef, _OptionalDescribeRouteInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -529,22 +576,20 @@
     "_OptionalDescribeVirtualGatewayInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualGatewayInputRequestTypeDef(
     _RequiredDescribeVirtualGatewayInputRequestTypeDef,
     _OptionalDescribeVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "virtualNodeName": str,
     },
 )
@@ -552,21 +597,19 @@
     "_OptionalDescribeVirtualNodeInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualNodeInputRequestTypeDef(
     _RequiredDescribeVirtualNodeInputRequestTypeDef, _OptionalDescribeVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
 _RequiredDescribeVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -574,22 +617,20 @@
     "_OptionalDescribeVirtualRouterInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualRouterInputRequestTypeDef(
     _RequiredDescribeVirtualRouterInputRequestTypeDef,
     _OptionalDescribeVirtualRouterInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDescribeVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "virtualServiceName": str,
     },
 )
@@ -597,22 +638,20 @@
     "_OptionalDescribeVirtualServiceInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class DescribeVirtualServiceInputRequestTypeDef(
     _RequiredDescribeVirtualServiceInputRequestTypeDef,
     _OptionalDescribeVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredDnsServiceDiscoveryTypeDef = TypedDict(
     "_RequiredDnsServiceDiscoveryTypeDef",
     {
         "hostname": str,
     },
 )
 _OptionalDnsServiceDiscoveryTypeDef = TypedDict(
@@ -620,21 +659,19 @@
     {
         "ipPreference": IpPreferenceType,
         "responseType": DnsResponseTypeType,
     },
     total=False,
 )
 
-
 class DnsServiceDiscoveryTypeDef(
     _RequiredDnsServiceDiscoveryTypeDef, _OptionalDnsServiceDiscoveryTypeDef
 ):
     pass
 
-
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "unit": DurationUnitType,
         "value": int,
     },
     total=False,
@@ -725,19 +762,17 @@
     "_OptionalWeightedTargetTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
-
 class WeightedTargetTypeDef(_RequiredWeightedTargetTypeDef, _OptionalWeightedTargetTypeDef):
     pass
 
-
 _RequiredHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": PortProtocolType,
         "timeoutMillis": int,
@@ -749,21 +784,19 @@
     {
         "path": str,
         "port": int,
     },
     total=False,
 )
 
-
 class HealthCheckPolicyTypeDef(
     _RequiredHealthCheckPolicyTypeDef, _OptionalHealthCheckPolicyTypeDef
 ):
     pass
 
-
 HttpPathMatchTypeDef = TypedDict(
     "HttpPathMatchTypeDef",
     {
         "exact": str,
         "regex": str,
     },
     total=False,
@@ -798,38 +831,24 @@
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualGatewayName": str,
-    },
-)
-_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
-    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -839,29 +858,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
-
-ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListMeshesInputRequestTypeDef = TypedDict(
     "ListMeshesInputRequestTypeDef",
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
@@ -876,38 +885,14 @@
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
     },
 )
 
-_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualRouterName": str,
-    },
-)
-_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListRoutesInputListRoutesPaginateTypeDef(
-    _RequiredListRoutesInputListRoutesPaginateTypeDef,
-    _OptionalListRoutesInputListRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -917,21 +902,19 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListRoutesInputRequestTypeDef(
     _RequiredListRoutesInputRequestTypeDef, _OptionalListRoutesInputRequestTypeDef
 ):
     pass
 
-
 RouteRefTypeDef = TypedDict(
     "RouteRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
@@ -939,36 +922,14 @@
         "resourceOwner": str,
         "routeName": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -976,44 +937,19 @@
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-
-_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
-    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualGatewaysInputRequestTypeDef = TypedDict(
@@ -1022,58 +958,33 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualGatewaysInputRequestTypeDef(
     _RequiredListVirtualGatewaysInputRequestTypeDef, _OptionalListVirtualGatewaysInputRequestTypeDef
 ):
     pass
 
-
 VirtualGatewayRefTypeDef = TypedDict(
     "VirtualGatewayRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
-_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
-    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -1082,58 +993,33 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualNodesInputRequestTypeDef(
     _RequiredListVirtualNodesInputRequestTypeDef, _OptionalListVirtualNodesInputRequestTypeDef
 ):
     pass
 
-
 VirtualNodeRefTypeDef = TypedDict(
     "VirtualNodeRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualNodeName": str,
     },
 )
 
-_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
-    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -1142,58 +1028,33 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualRoutersInputRequestTypeDef(
     _RequiredListVirtualRoutersInputRequestTypeDef, _OptionalListVirtualRoutersInputRequestTypeDef
 ):
     pass
 
-
 VirtualRouterRefTypeDef = TypedDict(
     "VirtualRouterRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
-    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1202,35 +1063,41 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
-
 class ListVirtualServicesInputRequestTypeDef(
     _RequiredListVirtualServicesInputRequestTypeDef, _OptionalListVirtualServicesInputRequestTypeDef
 ):
     pass
 
-
 VirtualServiceRefTypeDef = TypedDict(
     "VirtualServiceRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
+    {
+        "port": int,
+        "protocol": PortProtocolType,
+    },
+)
+
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1244,22 +1111,14 @@
 TlsValidationContextSdsTrustTypeDef = TypedDict(
     "TlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": PortProtocolType,
-    },
-)
-
 MeshStatusTypeDef = TypedDict(
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
@@ -1268,39 +1127,25 @@
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
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
+RouteStatusTypeDef = TypedDict(
+    "RouteStatusTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "status": RouteStatusCodeType,
     },
 )
 
-RouteStatusTypeDef = TypedDict(
-    "RouteStatusTypeDef",
+SubjectAlternativeNameMatchersOutputTypeDef = TypedDict(
+    "SubjectAlternativeNameMatchersOutputTypeDef",
     {
-        "status": RouteStatusCodeType,
+        "exact": List[str],
     },
 )
 
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
@@ -1311,14 +1156,21 @@
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
+TlsValidationContextAcmTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextAcmTrustOutputTypeDef",
+    {
+        "certificateAuthorityArns": List[str],
+    },
+)
+
 TlsValidationContextAcmTrustTypeDef = TypedDict(
     "TlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
@@ -1369,22 +1221,20 @@
     "_OptionalVirtualGatewayHttpConnectionPoolTypeDef",
     {
         "maxPendingRequests": int,
     },
     total=False,
 )
 
-
 class VirtualGatewayHttpConnectionPoolTypeDef(
     _RequiredVirtualGatewayHttpConnectionPoolTypeDef,
     _OptionalVirtualGatewayHttpConnectionPoolTypeDef,
 ):
     pass
 
-
 VirtualGatewayStatusTypeDef = TypedDict(
     "VirtualGatewayStatusTypeDef",
     {
         "status": VirtualGatewayStatusCodeType,
     },
 )
 
@@ -1403,20 +1253,26 @@
     {
         "path": str,
         "port": int,
     },
     total=False,
 )
 
-
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
+VirtualGatewayPortMappingTypeDef = TypedDict(
+    "VirtualGatewayPortMappingTypeDef",
+    {
+        "port": int,
+        "protocol": VirtualGatewayPortProtocolType,
+    },
+)
 
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
@@ -1431,19 +1287,18 @@
 VirtualGatewayTlsValidationContextSdsTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayPortMappingTypeDef = TypedDict(
-    "VirtualGatewayPortMappingTypeDef",
+VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     {
-        "port": int,
-        "protocol": VirtualGatewayPortProtocolType,
+        "certificateAuthorityArns": List[str],
     },
 )
 
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
@@ -1474,21 +1329,19 @@
     "_OptionalVirtualNodeHttpConnectionPoolTypeDef",
     {
         "maxPendingRequests": int,
     },
     total=False,
 )
 
-
 class VirtualNodeHttpConnectionPoolTypeDef(
     _RequiredVirtualNodeHttpConnectionPoolTypeDef, _OptionalVirtualNodeHttpConnectionPoolTypeDef
 ):
     pass
 
-
 VirtualNodeTcpConnectionPoolTypeDef = TypedDict(
     "VirtualNodeTcpConnectionPoolTypeDef",
     {
         "maxConnections": int,
     },
 )
 
@@ -1523,14 +1376,36 @@
 VirtualServiceStatusTypeDef = TypedDict(
     "VirtualServiceStatusTypeDef",
     {
         "status": VirtualServiceStatusCodeType,
     },
 )
 
+_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
+    "_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef",
+    {
+        "namespaceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
+    "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
+    {
+        "attributes": List[AwsCloudMapInstanceAttributeTypeDef],
+        "ipPreference": IpPreferenceType,
+    },
+    total=False,
+)
+
+class AwsCloudMapServiceDiscoveryOutputTypeDef(
+    _RequiredAwsCloudMapServiceDiscoveryOutputTypeDef,
+    _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef,
+):
+    pass
+
 _RequiredAwsCloudMapServiceDiscoveryTypeDef = TypedDict(
     "_RequiredAwsCloudMapServiceDiscoveryTypeDef",
     {
         "namespaceName": str,
         "serviceName": str,
     },
 )
@@ -1539,47 +1414,67 @@
     {
         "attributes": Sequence[AwsCloudMapInstanceAttributeTypeDef],
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
 
-
 class AwsCloudMapServiceDiscoveryTypeDef(
     _RequiredAwsCloudMapServiceDiscoveryTypeDef, _OptionalAwsCloudMapServiceDiscoveryTypeDef
 ):
     pass
 
-
 ClientTlsCertificateTypeDef = TypedDict(
     "ClientTlsCertificateTypeDef",
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagRefTypeDef],
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+_RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredGrpcRetryPolicyOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagRefTypeDef],
+        "maxRetries": int,
+        "perRetryTimeout": DurationTypeDef,
+    },
+)
+_OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalGrpcRetryPolicyOutputTypeDef",
+    {
+        "grpcRetryEvents": List[GrpcRetryPolicyEventType],
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
     },
+    total=False,
 )
 
+class GrpcRetryPolicyOutputTypeDef(
+    _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
+):
+    pass
+
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1589,28 +1484,47 @@
         "grpcRetryEvents": Sequence[GrpcRetryPolicyEventType],
         "httpRetryEvents": Sequence[str],
         "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
-
 class GrpcRetryPolicyTypeDef(_RequiredGrpcRetryPolicyTypeDef, _OptionalGrpcRetryPolicyTypeDef):
     pass
 
-
 GrpcTimeoutTypeDef = TypedDict(
     "GrpcTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
 )
 
+_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredHttpRetryPolicyOutputTypeDef",
+    {
+        "maxRetries": int,
+        "perRetryTimeout": DurationTypeDef,
+    },
+)
+_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalHttpRetryPolicyOutputTypeDef",
+    {
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
+    },
+    total=False,
+)
+
+class HttpRetryPolicyOutputTypeDef(
+    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
+):
+    pass
+
 _RequiredHttpRetryPolicyTypeDef = TypedDict(
     "_RequiredHttpRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1619,19 +1533,17 @@
     {
         "httpRetryEvents": Sequence[str],
         "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
-
 class HttpRetryPolicyTypeDef(_RequiredHttpRetryPolicyTypeDef, _OptionalHttpRetryPolicyTypeDef):
     pass
 
-
 HttpTimeoutTypeDef = TypedDict(
     "HttpTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
@@ -1664,15 +1576,15 @@
 )
 
 ListGatewayRoutesOutputTypeDef = TypedDict(
     "ListGatewayRoutesOutputTypeDef",
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
@@ -1682,21 +1594,19 @@
     "_OptionalGatewayRouteTargetTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
-
 class GatewayRouteTargetTypeDef(
     _RequiredGatewayRouteTargetTypeDef, _OptionalGatewayRouteTargetTypeDef
 ):
     pass
 
-
 GrpcMetadataMatchMethodTypeDef = TypedDict(
     "GrpcMetadataMatchMethodTypeDef",
     {
         "exact": str,
         "prefix": str,
         "range": MatchRangeTypeDef,
         "regex": str,
@@ -1725,28 +1635,49 @@
         "range": MatchRangeTypeDef,
         "regex": str,
         "suffix": str,
     },
     total=False,
 )
 
+GrpcRouteActionOutputTypeDef = TypedDict(
+    "GrpcRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetTypeDef],
+    },
+)
+
 GrpcRouteActionTypeDef = TypedDict(
     "GrpcRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
+HttpRouteActionOutputTypeDef = TypedDict(
+    "HttpRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetTypeDef],
+    },
+)
+
 HttpRouteActionTypeDef = TypedDict(
     "HttpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
+TcpRouteActionOutputTypeDef = TypedDict(
+    "TcpRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetTypeDef],
+    },
+)
+
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
@@ -1770,81 +1701,251 @@
     "_OptionalHttpQueryParameterTypeDef",
     {
         "match": QueryParameterMatchTypeDef,
     },
     total=False,
 )
 
-
 class HttpQueryParameterTypeDef(
     _RequiredHttpQueryParameterTypeDef, _OptionalHttpQueryParameterTypeDef
 ):
     pass
 
+LoggingFormatOutputTypeDef = TypedDict(
+    "LoggingFormatOutputTypeDef",
+    {
+        "json": List[JsonFormatRefTypeDef],
+        "text": str,
+    },
+    total=False,
+)
 
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
+_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualGatewayName": str,
+    },
+)
+_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
+    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+):
+    pass
+
+ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualRouterName": str,
+    },
+)
+_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListRoutesInputListRoutesPaginateTypeDef(
+    _RequiredListRoutesInputListRoutesPaginateTypeDef,
+    _OptionalListRoutesInputListRoutesPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
+    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
+    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
+    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+):
+    pass
+
+_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
+    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+):
+    pass
+
 ListMeshesOutputTypeDef = TypedDict(
     "ListMeshesOutputTypeDef",
     {
         "meshes": List[MeshRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutesOutputTypeDef = TypedDict(
     "ListRoutesOutputTypeDef",
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualNodesOutputTypeDef = TypedDict(
     "ListVirtualNodesOutputTypeDef",
     {
         "nextToken": str,
         "virtualNodes": List[VirtualNodeRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualRoutersOutputTypeDef = TypedDict(
     "ListVirtualRoutersOutputTypeDef",
     {
         "nextToken": str,
         "virtualRouters": List[VirtualRouterRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualServicesOutputTypeDef = TypedDict(
     "ListVirtualServicesOutputTypeDef",
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VirtualRouterListenerTypeDef = TypedDict(
+    "VirtualRouterListenerTypeDef",
+    {
+        "portMapping": PortMappingTypeDef,
     },
 )
 
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
@@ -1859,37 +1960,47 @@
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualRouterListenerTypeDef = TypedDict(
-    "VirtualRouterListenerTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+SubjectAlternativeNamesOutputTypeDef = TypedDict(
+    "SubjectAlternativeNamesOutputTypeDef",
+    {
+        "match": SubjectAlternativeNameMatchersOutputTypeDef,
+    },
+)
+
 SubjectAlternativeNamesTypeDef = TypedDict(
     "SubjectAlternativeNamesTypeDef",
     {
         "match": SubjectAlternativeNameMatchersTypeDef,
     },
 )
 
+TlsValidationContextTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextTrustOutputTypeDef",
+    {
+        "acm": TlsValidationContextAcmTrustOutputTypeDef,
+        "file": TlsValidationContextFileTrustTypeDef,
+        "sds": TlsValidationContextSdsTrustTypeDef,
+    },
+    total=False,
+)
+
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
@@ -1930,14 +2041,24 @@
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
+    {
+        "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
+        "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
+        "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
@@ -1960,14 +2081,23 @@
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
+ServiceDiscoveryOutputTypeDef = TypedDict(
+    "ServiceDiscoveryOutputTypeDef",
+    {
+        "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
+        "dns": DnsServiceDiscoveryTypeDef,
+    },
+    total=False,
+)
+
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
@@ -1994,21 +2124,19 @@
     "_OptionalGrpcGatewayRouteActionTypeDef",
     {
         "rewrite": GrpcGatewayRouteRewriteTypeDef,
     },
     total=False,
 )
 
-
 class GrpcGatewayRouteActionTypeDef(
     _RequiredGrpcGatewayRouteActionTypeDef, _OptionalGrpcGatewayRouteActionTypeDef
 ):
     pass
 
-
 _RequiredGrpcGatewayRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcGatewayRouteMetadataTypeDef = TypedDict(
@@ -2016,21 +2144,19 @@
     {
         "invert": bool,
         "match": GrpcMetadataMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class GrpcGatewayRouteMetadataTypeDef(
     _RequiredGrpcGatewayRouteMetadataTypeDef, _OptionalGrpcGatewayRouteMetadataTypeDef
 ):
     pass
 
-
 _RequiredGrpcRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcRouteMetadataTypeDef = TypedDict(
@@ -2038,21 +2164,19 @@
     {
         "invert": bool,
         "match": GrpcRouteMetadataMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class GrpcRouteMetadataTypeDef(
     _RequiredGrpcRouteMetadataTypeDef, _OptionalGrpcRouteMetadataTypeDef
 ):
     pass
 
-
 _RequiredHttpGatewayRouteHeaderTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteHeaderTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpGatewayRouteHeaderTypeDef = TypedDict(
@@ -2060,21 +2184,19 @@
     {
         "invert": bool,
         "match": HeaderMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class HttpGatewayRouteHeaderTypeDef(
     _RequiredHttpGatewayRouteHeaderTypeDef, _OptionalHttpGatewayRouteHeaderTypeDef
 ):
     pass
 
-
 _RequiredHttpRouteHeaderTypeDef = TypedDict(
     "_RequiredHttpRouteHeaderTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpRouteHeaderTypeDef = TypedDict(
@@ -2082,18 +2204,34 @@
     {
         "invert": bool,
         "match": HeaderMatchMethodTypeDef,
     },
     total=False,
 )
 
-
 class HttpRouteHeaderTypeDef(_RequiredHttpRouteHeaderTypeDef, _OptionalHttpRouteHeaderTypeDef):
     pass
 
+_RequiredTcpRouteOutputTypeDef = TypedDict(
+    "_RequiredTcpRouteOutputTypeDef",
+    {
+        "action": TcpRouteActionOutputTypeDef,
+    },
+)
+_OptionalTcpRouteOutputTypeDef = TypedDict(
+    "_OptionalTcpRouteOutputTypeDef",
+    {
+        "match": TcpRouteMatchTypeDef,
+        "timeout": TcpTimeoutTypeDef,
+    },
+    total=False,
+)
+
+class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
+    pass
 
 _RequiredTcpRouteTypeDef = TypedDict(
     "_RequiredTcpRouteTypeDef",
     {
         "action": TcpRouteActionTypeDef,
     },
 )
@@ -2102,39 +2240,74 @@
     {
         "match": TcpRouteMatchTypeDef,
         "timeout": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
-
 class TcpRouteTypeDef(_RequiredTcpRouteTypeDef, _OptionalTcpRouteTypeDef):
     pass
 
-
 _RequiredHttpGatewayRouteActionTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalHttpGatewayRouteActionTypeDef = TypedDict(
     "_OptionalHttpGatewayRouteActionTypeDef",
     {
         "rewrite": HttpGatewayRouteRewriteTypeDef,
     },
     total=False,
 )
 
-
 class HttpGatewayRouteActionTypeDef(
     _RequiredHttpGatewayRouteActionTypeDef, _OptionalHttpGatewayRouteActionTypeDef
 ):
     pass
 
+_RequiredFileAccessLogOutputTypeDef = TypedDict(
+    "_RequiredFileAccessLogOutputTypeDef",
+    {
+        "path": str,
+    },
+)
+_OptionalFileAccessLogOutputTypeDef = TypedDict(
+    "_OptionalFileAccessLogOutputTypeDef",
+    {
+        "format": LoggingFormatOutputTypeDef,
+    },
+    total=False,
+)
+
+class FileAccessLogOutputTypeDef(
+    _RequiredFileAccessLogOutputTypeDef, _OptionalFileAccessLogOutputTypeDef
+):
+    pass
+
+_RequiredVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayFileAccessLogOutputTypeDef",
+    {
+        "path": str,
+    },
+)
+_OptionalVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayFileAccessLogOutputTypeDef",
+    {
+        "format": LoggingFormatOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayFileAccessLogOutputTypeDef(
+    _RequiredVirtualGatewayFileAccessLogOutputTypeDef,
+    _OptionalVirtualGatewayFileAccessLogOutputTypeDef,
+):
+    pass
 
 _RequiredFileAccessLogTypeDef = TypedDict(
     "_RequiredFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
@@ -2142,39 +2315,43 @@
     "_OptionalFileAccessLogTypeDef",
     {
         "format": LoggingFormatTypeDef,
     },
     total=False,
 )
 
-
 class FileAccessLogTypeDef(_RequiredFileAccessLogTypeDef, _OptionalFileAccessLogTypeDef):
     pass
 
-
 _RequiredVirtualGatewayFileAccessLogTypeDef = TypedDict(
     "_RequiredVirtualGatewayFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
 _OptionalVirtualGatewayFileAccessLogTypeDef = TypedDict(
     "_OptionalVirtualGatewayFileAccessLogTypeDef",
     {
         "format": LoggingFormatTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayFileAccessLogTypeDef(
     _RequiredVirtualGatewayFileAccessLogTypeDef, _OptionalVirtualGatewayFileAccessLogTypeDef
 ):
     pass
 
+VirtualRouterSpecOutputTypeDef = TypedDict(
+    "VirtualRouterSpecOutputTypeDef",
+    {
+        "listeners": List[VirtualRouterListenerTypeDef],
+    },
+    total=False,
+)
 
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
@@ -2192,21 +2369,19 @@
         "clientToken": str,
         "spec": MeshSpecTypeDef,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateMeshInputRequestTypeDef(
     _RequiredCreateMeshInputRequestTypeDef, _OptionalCreateMeshInputRequestTypeDef
 ):
     pass
 
-
 MeshDataTypeDef = TypedDict(
     "MeshDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
         "spec": MeshSpecTypeDef,
         "status": MeshStatusTypeDef,
@@ -2224,20 +2399,38 @@
     {
         "clientToken": str,
         "spec": MeshSpecTypeDef,
     },
     total=False,
 )
 
-
 class UpdateMeshInputRequestTypeDef(
     _RequiredUpdateMeshInputRequestTypeDef, _OptionalUpdateMeshInputRequestTypeDef
 ):
     pass
 
+_RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredListenerTlsValidationContextOutputTypeDef",
+    {
+        "trust": ListenerTlsValidationContextTrustTypeDef,
+    },
+)
+_OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalListenerTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class ListenerTlsValidationContextOutputTypeDef(
+    _RequiredListenerTlsValidationContextOutputTypeDef,
+    _OptionalListenerTlsValidationContextOutputTypeDef,
+):
+    pass
 
 _RequiredListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextTypeDef",
     {
         "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
@@ -2245,20 +2438,37 @@
     "_OptionalListenerTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class ListenerTlsValidationContextTypeDef(
     _RequiredListenerTlsValidationContextTypeDef, _OptionalListenerTlsValidationContextTypeDef
 ):
     pass
 
+_RequiredTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredTlsValidationContextOutputTypeDef",
+    {
+        "trust": TlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class TlsValidationContextOutputTypeDef(
+    _RequiredTlsValidationContextOutputTypeDef, _OptionalTlsValidationContextOutputTypeDef
+):
+    pass
 
 _RequiredTlsValidationContextTypeDef = TypedDict(
     "_RequiredTlsValidationContextTypeDef",
     {
         "trust": TlsValidationContextTrustTypeDef,
     },
 )
@@ -2266,20 +2476,38 @@
     "_OptionalTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class TlsValidationContextTypeDef(
     _RequiredTlsValidationContextTypeDef, _OptionalTlsValidationContextTypeDef
 ):
     pass
 
+_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
+    {
+        "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    },
+)
+_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayListenerTlsValidationContextOutputTypeDef(
+    _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef,
+    _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef,
+):
+    pass
 
 _RequiredVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
@@ -2287,21 +2515,39 @@
     "_OptionalVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayListenerTlsValidationContextTypeDef(
     _RequiredVirtualGatewayListenerTlsValidationContextTypeDef,
     _OptionalVirtualGatewayListenerTlsValidationContextTypeDef,
 ):
     pass
 
+_RequiredVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayTlsValidationContextOutputTypeDef",
+    {
+        "trust": VirtualGatewayTlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayTlsValidationContextOutputTypeDef(
+    _RequiredVirtualGatewayTlsValidationContextOutputTypeDef,
+    _OptionalVirtualGatewayTlsValidationContextOutputTypeDef,
+):
+    pass
 
 _RequiredVirtualGatewayTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayTlsValidationContextTrustTypeDef,
     },
 )
@@ -2309,80 +2555,144 @@
     "_OptionalVirtualGatewayTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayTlsValidationContextTypeDef(
     _RequiredVirtualGatewayTlsValidationContextTypeDef,
     _OptionalVirtualGatewayTlsValidationContextTypeDef,
 ):
     pass
 
-
 VirtualServiceSpecTypeDef = TypedDict(
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
+GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteMatchOutputTypeDef",
+    {
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "metadata": List[GrpcGatewayRouteMetadataTypeDef],
+        "port": int,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 GrpcGatewayRouteMatchTypeDef = TypedDict(
     "GrpcGatewayRouteMatchTypeDef",
     {
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
+GrpcRouteMatchOutputTypeDef = TypedDict(
+    "GrpcRouteMatchOutputTypeDef",
+    {
+        "metadata": List[GrpcRouteMetadataTypeDef],
+        "methodName": str,
+        "port": int,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 GrpcRouteMatchTypeDef = TypedDict(
     "GrpcRouteMatchTypeDef",
     {
         "metadata": Sequence[GrpcRouteMetadataTypeDef],
         "methodName": str,
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
+HttpGatewayRouteMatchOutputTypeDef = TypedDict(
+    "HttpGatewayRouteMatchOutputTypeDef",
+    {
+        "headers": List[HttpGatewayRouteHeaderTypeDef],
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
+        "port": int,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterTypeDef],
+    },
+    total=False,
+)
+
 HttpGatewayRouteMatchTypeDef = TypedDict(
     "HttpGatewayRouteMatchTypeDef",
     {
         "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
+HttpRouteMatchOutputTypeDef = TypedDict(
+    "HttpRouteMatchOutputTypeDef",
+    {
+        "headers": List[HttpRouteHeaderTypeDef],
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
+        "port": int,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterTypeDef],
+        "scheme": HttpSchemeType,
+    },
+    total=False,
+)
+
 HttpRouteMatchTypeDef = TypedDict(
     "HttpRouteMatchTypeDef",
     {
         "headers": Sequence[HttpRouteHeaderTypeDef],
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
         "scheme": HttpSchemeType,
     },
     total=False,
 )
 
+AccessLogOutputTypeDef = TypedDict(
+    "AccessLogOutputTypeDef",
+    {
+        "file": FileAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
+VirtualGatewayAccessLogOutputTypeDef = TypedDict(
+    "VirtualGatewayAccessLogOutputTypeDef",
+    {
+        "file": VirtualGatewayFileAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
 AccessLogTypeDef = TypedDict(
     "AccessLogTypeDef",
     {
         "file": FileAccessLogTypeDef,
     },
     total=False,
 )
@@ -2391,14 +2701,25 @@
     "VirtualGatewayAccessLogTypeDef",
     {
         "file": VirtualGatewayFileAccessLogTypeDef,
     },
     total=False,
 )
 
+VirtualRouterDataTypeDef = TypedDict(
+    "VirtualRouterDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualRouterSpecOutputTypeDef,
+        "status": VirtualRouterStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2409,21 +2730,19 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualRouterInputRequestTypeDef(
     _RequiredCreateVirtualRouterInputRequestTypeDef, _OptionalCreateVirtualRouterInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2433,63 +2752,71 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
-
-VirtualRouterDataTypeDef = TypedDict(
-    "VirtualRouterDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualRouterSpecTypeDef,
-        "status": VirtualRouterStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
+VirtualRouterSpecUnionTypeDef = Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef]
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMeshOutputTypeDef = TypedDict(
     "DeleteMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMeshOutputTypeDef = TypedDict(
     "DescribeMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMeshOutputTypeDef = TypedDict(
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListenerTlsOutputTypeDef = TypedDict(
+    "_RequiredListenerTlsOutputTypeDef",
+    {
+        "certificate": ListenerTlsCertificateTypeDef,
+        "mode": ListenerTlsModeType,
     },
 )
+_OptionalListenerTlsOutputTypeDef = TypedDict(
+    "_OptionalListenerTlsOutputTypeDef",
+    {
+        "validation": ListenerTlsValidationContextOutputTypeDef,
+    },
+    total=False,
+)
+
+class ListenerTlsOutputTypeDef(
+    _RequiredListenerTlsOutputTypeDef, _OptionalListenerTlsOutputTypeDef
+):
+    pass
 
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
@@ -2498,18 +2825,37 @@
     "_OptionalListenerTlsTypeDef",
     {
         "validation": ListenerTlsValidationContextTypeDef,
     },
     total=False,
 )
 
-
 class ListenerTlsTypeDef(_RequiredListenerTlsTypeDef, _OptionalListenerTlsTypeDef):
     pass
 
+_RequiredClientPolicyTlsOutputTypeDef = TypedDict(
+    "_RequiredClientPolicyTlsOutputTypeDef",
+    {
+        "validation": TlsValidationContextOutputTypeDef,
+    },
+)
+_OptionalClientPolicyTlsOutputTypeDef = TypedDict(
+    "_OptionalClientPolicyTlsOutputTypeDef",
+    {
+        "certificate": ClientTlsCertificateTypeDef,
+        "enforce": bool,
+        "ports": List[int],
+    },
+    total=False,
+)
+
+class ClientPolicyTlsOutputTypeDef(
+    _RequiredClientPolicyTlsOutputTypeDef, _OptionalClientPolicyTlsOutputTypeDef
+):
+    pass
 
 _RequiredClientPolicyTlsTypeDef = TypedDict(
     "_RequiredClientPolicyTlsTypeDef",
     {
         "validation": TlsValidationContextTypeDef,
     },
 )
@@ -2519,18 +2865,36 @@
         "certificate": ClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": Sequence[int],
     },
     total=False,
 )
 
-
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
+_RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
+    {
+        "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
+        "mode": VirtualGatewayListenerTlsModeType,
+    },
+)
+_OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
+    {
+        "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayListenerTlsOutputTypeDef(
+    _RequiredVirtualGatewayListenerTlsOutputTypeDef, _OptionalVirtualGatewayListenerTlsOutputTypeDef
+):
+    pass
 
 _RequiredVirtualGatewayListenerTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsTypeDef",
     {
         "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
@@ -2539,20 +2903,40 @@
     "_OptionalVirtualGatewayListenerTlsTypeDef",
     {
         "validation": VirtualGatewayListenerTlsValidationContextTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayListenerTlsTypeDef(
     _RequiredVirtualGatewayListenerTlsTypeDef, _OptionalVirtualGatewayListenerTlsTypeDef
 ):
     pass
 
+_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef",
+    {
+        "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
+    {
+        "certificate": VirtualGatewayClientTlsCertificateTypeDef,
+        "enforce": bool,
+        "ports": List[int],
+    },
+    total=False,
+)
+
+class VirtualGatewayClientPolicyTlsOutputTypeDef(
+    _RequiredVirtualGatewayClientPolicyTlsOutputTypeDef,
+    _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef,
+):
+    pass
 
 _RequiredVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayClientPolicyTlsTypeDef",
     {
         "validation": VirtualGatewayTlsValidationContextTypeDef,
     },
 )
@@ -2562,21 +2946,19 @@
         "certificate": VirtualGatewayClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": Sequence[int],
     },
     total=False,
 )
 
-
 class VirtualGatewayClientPolicyTlsTypeDef(
     _RequiredVirtualGatewayClientPolicyTlsTypeDef, _OptionalVirtualGatewayClientPolicyTlsTypeDef
 ):
     pass
 
-
 _RequiredCreateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -2587,22 +2969,20 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualServiceInputRequestTypeDef(
     _RequiredCreateVirtualServiceInputRequestTypeDef,
     _OptionalCreateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -2612,41 +2992,66 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualServiceInputRequestTypeDef(
     _RequiredUpdateVirtualServiceInputRequestTypeDef,
     _OptionalUpdateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
-
 VirtualServiceDataTypeDef = TypedDict(
     "VirtualServiceDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
         "spec": VirtualServiceSpecTypeDef,
         "status": VirtualServiceStatusTypeDef,
         "virtualServiceName": str,
     },
 )
 
+GrpcGatewayRouteOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteOutputTypeDef",
+    {
+        "action": GrpcGatewayRouteActionTypeDef,
+        "match": GrpcGatewayRouteMatchOutputTypeDef,
+    },
+)
+
 GrpcGatewayRouteTypeDef = TypedDict(
     "GrpcGatewayRouteTypeDef",
     {
         "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchTypeDef,
     },
 )
 
+_RequiredGrpcRouteOutputTypeDef = TypedDict(
+    "_RequiredGrpcRouteOutputTypeDef",
+    {
+        "action": GrpcRouteActionOutputTypeDef,
+        "match": GrpcRouteMatchOutputTypeDef,
+    },
+)
+_OptionalGrpcRouteOutputTypeDef = TypedDict(
+    "_OptionalGrpcRouteOutputTypeDef",
+    {
+        "retryPolicy": GrpcRetryPolicyOutputTypeDef,
+        "timeout": GrpcTimeoutTypeDef,
+    },
+    total=False,
+)
+
+class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
+    pass
+
 _RequiredGrpcRouteTypeDef = TypedDict(
     "_RequiredGrpcRouteTypeDef",
     {
         "action": GrpcRouteActionTypeDef,
         "match": GrpcRouteMatchTypeDef,
     },
 )
@@ -2655,27 +3060,52 @@
     {
         "retryPolicy": GrpcRetryPolicyTypeDef,
         "timeout": GrpcTimeoutTypeDef,
     },
     total=False,
 )
 
-
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
+HttpGatewayRouteOutputTypeDef = TypedDict(
+    "HttpGatewayRouteOutputTypeDef",
+    {
+        "action": HttpGatewayRouteActionTypeDef,
+        "match": HttpGatewayRouteMatchOutputTypeDef,
+    },
+)
 
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
 
+_RequiredHttpRouteOutputTypeDef = TypedDict(
+    "_RequiredHttpRouteOutputTypeDef",
+    {
+        "action": HttpRouteActionOutputTypeDef,
+        "match": HttpRouteMatchOutputTypeDef,
+    },
+)
+_OptionalHttpRouteOutputTypeDef = TypedDict(
+    "_OptionalHttpRouteOutputTypeDef",
+    {
+        "retryPolicy": HttpRetryPolicyOutputTypeDef,
+        "timeout": HttpTimeoutTypeDef,
+    },
+    total=False,
+)
+
+class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
+    pass
+
 _RequiredHttpRouteTypeDef = TypedDict(
     "_RequiredHttpRouteTypeDef",
     {
         "action": HttpRouteActionTypeDef,
         "match": HttpRouteMatchTypeDef,
     },
 )
@@ -2684,18 +3114,32 @@
     {
         "retryPolicy": HttpRetryPolicyTypeDef,
         "timeout": HttpTimeoutTypeDef,
     },
     total=False,
 )
 
-
 class HttpRouteTypeDef(_RequiredHttpRouteTypeDef, _OptionalHttpRouteTypeDef):
     pass
 
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "accessLog": AccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
+VirtualGatewayLoggingOutputTypeDef = TypedDict(
+    "VirtualGatewayLoggingOutputTypeDef",
+    {
+        "accessLog": VirtualGatewayAccessLogOutputTypeDef,
+    },
+    total=False,
+)
 
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "accessLog": AccessLogTypeDef,
     },
     total=False,
@@ -2709,42 +3153,63 @@
     total=False,
 )
 
 CreateVirtualRouterOutputTypeDef = TypedDict(
     "CreateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualRouterOutputTypeDef = TypedDict(
     "DeleteVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualRouterOutputTypeDef = TypedDict(
     "DescribeVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualRouterOutputTypeDef = TypedDict(
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListenerOutputTypeDef = TypedDict(
+    "_RequiredListenerOutputTypeDef",
+    {
+        "portMapping": PortMappingTypeDef,
+    },
+)
+_OptionalListenerOutputTypeDef = TypedDict(
+    "_OptionalListenerOutputTypeDef",
+    {
+        "connectionPool": VirtualNodeConnectionPoolTypeDef,
+        "healthCheck": HealthCheckPolicyTypeDef,
+        "outlierDetection": OutlierDetectionTypeDef,
+        "timeout": ListenerTimeoutTypeDef,
+        "tls": ListenerTlsOutputTypeDef,
     },
+    total=False,
 )
 
+class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
+    pass
+
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerTypeDef = TypedDict(
@@ -2755,27 +3220,54 @@
         "outlierDetection": OutlierDetectionTypeDef,
         "timeout": ListenerTimeoutTypeDef,
         "tls": ListenerTlsTypeDef,
     },
     total=False,
 )
 
-
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
+ClientPolicyOutputTypeDef = TypedDict(
+    "ClientPolicyOutputTypeDef",
+    {
+        "tls": ClientPolicyTlsOutputTypeDef,
+    },
+    total=False,
+)
 
 ClientPolicyTypeDef = TypedDict(
     "ClientPolicyTypeDef",
     {
         "tls": ClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
+_RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerOutputTypeDef",
+    {
+        "portMapping": VirtualGatewayPortMappingTypeDef,
+    },
+)
+_OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerOutputTypeDef",
+    {
+        "connectionPool": VirtualGatewayConnectionPoolTypeDef,
+        "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
+        "tls": VirtualGatewayListenerTlsOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewayListenerOutputTypeDef(
+    _RequiredVirtualGatewayListenerOutputTypeDef, _OptionalVirtualGatewayListenerOutputTypeDef
+):
+    pass
+
 _RequiredVirtualGatewayListenerTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTypeDef",
     {
         "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTypeDef = TypedDict(
@@ -2784,84 +3276,140 @@
         "connectionPool": VirtualGatewayConnectionPoolTypeDef,
         "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
         "tls": VirtualGatewayListenerTlsTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewayListenerTypeDef(
     _RequiredVirtualGatewayListenerTypeDef, _OptionalVirtualGatewayListenerTypeDef
 ):
     pass
 
+VirtualGatewayClientPolicyOutputTypeDef = TypedDict(
+    "VirtualGatewayClientPolicyOutputTypeDef",
+    {
+        "tls": VirtualGatewayClientPolicyTlsOutputTypeDef,
+    },
+    total=False,
+)
 
 VirtualGatewayClientPolicyTypeDef = TypedDict(
     "VirtualGatewayClientPolicyTypeDef",
     {
         "tls": VirtualGatewayClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
 CreateVirtualServiceOutputTypeDef = TypedDict(
     "CreateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualServiceOutputTypeDef = TypedDict(
     "DeleteVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualServiceOutputTypeDef = TypedDict(
     "DescribeVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualServiceOutputTypeDef = TypedDict(
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GatewayRouteSpecOutputTypeDef = TypedDict(
+    "GatewayRouteSpecOutputTypeDef",
+    {
+        "grpcRoute": GrpcGatewayRouteOutputTypeDef,
+        "http2Route": HttpGatewayRouteOutputTypeDef,
+        "httpRoute": HttpGatewayRouteOutputTypeDef,
+        "priority": int,
+    },
+    total=False,
+)
+
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
         "http2Route": HttpGatewayRouteTypeDef,
         "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
     },
     total=False,
 )
 
+RouteSpecOutputTypeDef = TypedDict(
+    "RouteSpecOutputTypeDef",
+    {
+        "grpcRoute": GrpcRouteOutputTypeDef,
+        "http2Route": HttpRouteOutputTypeDef,
+        "httpRoute": HttpRouteOutputTypeDef,
+        "priority": int,
+        "tcpRoute": TcpRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 RouteSpecTypeDef = TypedDict(
     "RouteSpecTypeDef",
     {
         "grpcRoute": GrpcRouteTypeDef,
         "http2Route": HttpRouteTypeDef,
         "httpRoute": HttpRouteTypeDef,
         "priority": int,
         "tcpRoute": TcpRouteTypeDef,
     },
     total=False,
 )
 
+BackendDefaultsOutputTypeDef = TypedDict(
+    "BackendDefaultsOutputTypeDef",
+    {
+        "clientPolicy": ClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredVirtualServiceBackendOutputTypeDef = TypedDict(
+    "_RequiredVirtualServiceBackendOutputTypeDef",
+    {
+        "virtualServiceName": str,
+    },
+)
+_OptionalVirtualServiceBackendOutputTypeDef = TypedDict(
+    "_OptionalVirtualServiceBackendOutputTypeDef",
+    {
+        "clientPolicy": ClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualServiceBackendOutputTypeDef(
+    _RequiredVirtualServiceBackendOutputTypeDef, _OptionalVirtualServiceBackendOutputTypeDef
+):
+    pass
+
 BackendDefaultsTypeDef = TypedDict(
     "BackendDefaultsTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
@@ -2876,29 +3424,47 @@
     "_OptionalVirtualServiceBackendTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
 
-
 class VirtualServiceBackendTypeDef(
     _RequiredVirtualServiceBackendTypeDef, _OptionalVirtualServiceBackendTypeDef
 ):
     pass
 
+VirtualGatewayBackendDefaultsOutputTypeDef = TypedDict(
+    "VirtualGatewayBackendDefaultsOutputTypeDef",
+    {
+        "clientPolicy": VirtualGatewayClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
 
 VirtualGatewayBackendDefaultsTypeDef = TypedDict(
     "VirtualGatewayBackendDefaultsTypeDef",
     {
         "clientPolicy": VirtualGatewayClientPolicyTypeDef,
     },
     total=False,
 )
 
+GatewayRouteDataTypeDef = TypedDict(
+    "GatewayRouteDataTypeDef",
+    {
+        "gatewayRouteName": str,
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": GatewayRouteSpecOutputTypeDef,
+        "status": GatewayRouteStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -2910,33 +3476,20 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
-
-GatewayRouteDataTypeDef = TypedDict(
-    "GatewayRouteDataTypeDef",
-    {
-        "gatewayRouteName": str,
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": GatewayRouteSpecTypeDef,
-        "status": GatewayRouteStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
-
+GatewayRouteSpecUnionTypeDef = Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef]
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -2947,20 +3500,30 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecOutputTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
 
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
@@ -2973,33 +3536,20 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
-
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
-
+RouteSpecUnionTypeDef = Union[RouteSpecTypeDef, RouteSpecOutputTypeDef]
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -3010,29 +3560,55 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateRouteInputRequestTypeDef(
     _RequiredUpdateRouteInputRequestTypeDef, _OptionalUpdateRouteInputRequestTypeDef
 ):
     pass
 
+BackendOutputTypeDef = TypedDict(
+    "BackendOutputTypeDef",
+    {
+        "virtualService": VirtualServiceBackendOutputTypeDef,
+    },
+    total=False,
+)
 
 BackendTypeDef = TypedDict(
     "BackendTypeDef",
     {
         "virtualService": VirtualServiceBackendTypeDef,
     },
     total=False,
 )
 
+_RequiredVirtualGatewaySpecOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewaySpecOutputTypeDef",
+    {
+        "listeners": List[VirtualGatewayListenerOutputTypeDef],
+    },
+)
+_OptionalVirtualGatewaySpecOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewaySpecOutputTypeDef",
+    {
+        "backendDefaults": VirtualGatewayBackendDefaultsOutputTypeDef,
+        "logging": VirtualGatewayLoggingOutputTypeDef,
+    },
+    total=False,
+)
+
+class VirtualGatewaySpecOutputTypeDef(
+    _RequiredVirtualGatewaySpecOutputTypeDef, _OptionalVirtualGatewaySpecOutputTypeDef
+):
+    pass
+
 _RequiredVirtualGatewaySpecTypeDef = TypedDict(
     "_RequiredVirtualGatewaySpecTypeDef",
     {
         "listeners": Sequence[VirtualGatewayListenerTypeDef],
     },
 )
 _OptionalVirtualGatewaySpecTypeDef = TypedDict(
@@ -3040,97 +3616,118 @@
     {
         "backendDefaults": VirtualGatewayBackendDefaultsTypeDef,
         "logging": VirtualGatewayLoggingTypeDef,
     },
     total=False,
 )
 
-
 class VirtualGatewaySpecTypeDef(
     _RequiredVirtualGatewaySpecTypeDef, _OptionalVirtualGatewaySpecTypeDef
 ):
     pass
 
-
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGatewayRouteOutputTypeDef = TypedDict(
     "DeleteGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGatewayRouteOutputTypeDef = TypedDict(
     "DescribeGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGatewayRouteOutputTypeDef = TypedDict(
     "UpdateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteOutputTypeDef = TypedDict(
     "CreateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRouteOutputTypeDef = TypedDict(
     "DeleteRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouteOutputTypeDef = TypedDict(
     "DescribeRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteOutputTypeDef = TypedDict(
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VirtualNodeSpecOutputTypeDef = TypedDict(
+    "VirtualNodeSpecOutputTypeDef",
+    {
+        "backendDefaults": BackendDefaultsOutputTypeDef,
+        "backends": List[BackendOutputTypeDef],
+        "listeners": List[ListenerOutputTypeDef],
+        "logging": LoggingOutputTypeDef,
+        "serviceDiscovery": ServiceDiscoveryOutputTypeDef,
     },
+    total=False,
 )
 
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
         "backends": Sequence[BackendTypeDef],
         "listeners": Sequence[ListenerTypeDef],
         "logging": LoggingTypeDef,
         "serviceDiscovery": ServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayDataTypeDef = TypedDict(
+    "VirtualGatewayDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualGatewaySpecOutputTypeDef,
+        "status": VirtualGatewayStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredCreateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3141,22 +3738,20 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualGatewayInputRequestTypeDef(
     _RequiredCreateVirtualGatewayInputRequestTypeDef,
     _OptionalCreateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
 _RequiredUpdateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3166,30 +3761,29 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-
-VirtualGatewayDataTypeDef = TypedDict(
-    "VirtualGatewayDataTypeDef",
+VirtualGatewaySpecUnionTypeDef = Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef]
+VirtualNodeDataTypeDef = TypedDict(
+    "VirtualNodeDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualGatewaySpecTypeDef,
-        "status": VirtualGatewayStatusTypeDef,
-        "virtualGatewayName": str,
+        "spec": VirtualNodeSpecOutputTypeDef,
+        "status": VirtualNodeStatusTypeDef,
+        "virtualNodeName": str,
     },
 )
 
 _RequiredCreateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
@@ -3203,21 +3797,19 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
-
 class CreateVirtualNodeInputRequestTypeDef(
     _RequiredCreateVirtualNodeInputRequestTypeDef, _OptionalCreateVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualNodeSpecTypeDef,
         "virtualNodeName": str,
     },
@@ -3227,88 +3819,76 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
-
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
-
-VirtualNodeDataTypeDef = TypedDict(
-    "VirtualNodeDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualNodeSpecTypeDef,
-        "status": VirtualNodeStatusTypeDef,
-        "virtualNodeName": str,
-    },
-)
-
+VirtualNodeSpecUnionTypeDef = Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef]
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualGatewayOutputTypeDef = TypedDict(
     "DeleteVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualGatewayOutputTypeDef = TypedDict(
     "DescribeVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualGatewayOutputTypeDef = TypedDict(
     "UpdateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVirtualNodeOutputTypeDef = TypedDict(
     "CreateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualNodeOutputTypeDef = TypedDict(
     "DeleteVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualNodeOutputTypeDef = TypedDict(
     "DescribeVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualNodeOutputTypeDef = TypedDict(
     "UpdateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh/type_defs.pyi` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appmesh.type_defs import AwsCloudMapInstanceAttributeTypeDef
 
-    data: AwsCloudMapInstanceAttributeTypeDef = {...}
+    data: AwsCloudMapInstanceAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     DefaultGatewayRouteRewriteType,
     DnsResponseTypeType,
     DurationUnitType,
     EgressFilterTypeType,
     GatewayRouteStatusCodeType,
@@ -42,19 +42,21 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AwsCloudMapInstanceAttributeTypeDef",
     "ListenerTlsFileCertificateTypeDef",
     "ListenerTlsSdsCertificateTypeDef",
     "TagRefTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteGatewayRouteInputRequestTypeDef",
     "DeleteMeshInputRequestTypeDef",
     "DeleteRouteInputRequestTypeDef",
     "DeleteVirtualGatewayInputRequestTypeDef",
     "DeleteVirtualNodeInputRequestTypeDef",
     "DeleteVirtualRouterInputRequestTypeDef",
     "DeleteVirtualServiceInputRequestTypeDef",
@@ -78,197 +80,251 @@
     "WeightedTargetTypeDef",
     "HealthCheckPolicyTypeDef",
     "HttpPathMatchTypeDef",
     "HttpGatewayRoutePathRewriteTypeDef",
     "HttpGatewayRoutePrefixRewriteTypeDef",
     "QueryParameterMatchTypeDef",
     "JsonFormatRefTypeDef",
-    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListGatewayRoutesInputRequestTypeDef",
-    "ListMeshesInputListMeshesPaginateTypeDef",
     "ListMeshesInputRequestTypeDef",
     "MeshRefTypeDef",
-    "ListRoutesInputListRoutesPaginateTypeDef",
     "ListRoutesInputRequestTypeDef",
     "RouteRefTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
     "ListVirtualGatewaysInputRequestTypeDef",
     "VirtualGatewayRefTypeDef",
-    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
     "ListVirtualNodesInputRequestTypeDef",
     "VirtualNodeRefTypeDef",
-    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
     "ListVirtualRoutersInputRequestTypeDef",
     "VirtualRouterRefTypeDef",
-    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListVirtualServicesInputRequestTypeDef",
     "VirtualServiceRefTypeDef",
+    "PortMappingTypeDef",
     "ListenerTlsAcmCertificateTypeDef",
     "TlsValidationContextFileTrustTypeDef",
     "TlsValidationContextSdsTrustTypeDef",
-    "PortMappingTypeDef",
     "MeshStatusTypeDef",
     "MeshServiceDiscoveryTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RouteStatusTypeDef",
+    "SubjectAlternativeNameMatchersOutputTypeDef",
     "SubjectAlternativeNameMatchersTypeDef",
     "TcpRouteMatchTypeDef",
+    "TlsValidationContextAcmTrustOutputTypeDef",
     "TlsValidationContextAcmTrustTypeDef",
     "UntagResourceInputRequestTypeDef",
     "VirtualGatewayListenerTlsFileCertificateTypeDef",
     "VirtualGatewayListenerTlsSdsCertificateTypeDef",
     "VirtualGatewayGrpcConnectionPoolTypeDef",
     "VirtualGatewayHttp2ConnectionPoolTypeDef",
     "VirtualGatewayHttpConnectionPoolTypeDef",
     "VirtualGatewayStatusTypeDef",
     "VirtualGatewayHealthCheckPolicyTypeDef",
+    "VirtualGatewayPortMappingTypeDef",
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     "VirtualGatewayTlsValidationContextFileTrustTypeDef",
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
-    "VirtualGatewayPortMappingTypeDef",
+    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     "VirtualNodeGrpcConnectionPoolTypeDef",
     "VirtualNodeHttp2ConnectionPoolTypeDef",
     "VirtualNodeHttpConnectionPoolTypeDef",
     "VirtualNodeTcpConnectionPoolTypeDef",
     "VirtualNodeStatusTypeDef",
     "VirtualNodeServiceProviderTypeDef",
     "VirtualRouterStatusTypeDef",
     "VirtualRouterServiceProviderTypeDef",
     "VirtualServiceStatusTypeDef",
+    "AwsCloudMapServiceDiscoveryOutputTypeDef",
     "AwsCloudMapServiceDiscoveryTypeDef",
     "ClientTlsCertificateTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "GrpcRetryPolicyOutputTypeDef",
     "GrpcRetryPolicyTypeDef",
     "GrpcTimeoutTypeDef",
+    "HttpRetryPolicyOutputTypeDef",
     "HttpRetryPolicyTypeDef",
     "HttpTimeoutTypeDef",
     "OutlierDetectionTypeDef",
     "TcpTimeoutTypeDef",
     "GrpcGatewayRouteRewriteTypeDef",
     "ListGatewayRoutesOutputTypeDef",
     "GatewayRouteTargetTypeDef",
     "GrpcMetadataMatchMethodTypeDef",
     "GrpcRouteMetadataMatchMethodTypeDef",
     "HeaderMatchMethodTypeDef",
+    "GrpcRouteActionOutputTypeDef",
     "GrpcRouteActionTypeDef",
+    "HttpRouteActionOutputTypeDef",
     "HttpRouteActionTypeDef",
+    "TcpRouteActionOutputTypeDef",
     "TcpRouteActionTypeDef",
     "HttpGatewayRouteRewriteTypeDef",
     "HttpQueryParameterTypeDef",
+    "LoggingFormatOutputTypeDef",
     "LoggingFormatTypeDef",
+    "ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    "ListRoutesInputListRoutesPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    "ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    "ListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    "ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    "ListVirtualServicesInputListVirtualServicesPaginateTypeDef",
     "ListMeshesOutputTypeDef",
     "ListRoutesOutputTypeDef",
     "ListVirtualGatewaysOutputTypeDef",
     "ListVirtualNodesOutputTypeDef",
     "ListVirtualRoutersOutputTypeDef",
     "ListVirtualServicesOutputTypeDef",
+    "VirtualRouterListenerTypeDef",
     "ListenerTlsCertificateTypeDef",
     "ListenerTlsValidationContextTrustTypeDef",
-    "VirtualRouterListenerTypeDef",
     "MeshSpecTypeDef",
+    "SubjectAlternativeNamesOutputTypeDef",
     "SubjectAlternativeNamesTypeDef",
+    "TlsValidationContextTrustOutputTypeDef",
     "TlsValidationContextTrustTypeDef",
     "VirtualGatewayClientTlsCertificateTypeDef",
     "VirtualGatewayConnectionPoolTypeDef",
     "VirtualGatewayListenerTlsCertificateTypeDef",
     "VirtualGatewayListenerTlsValidationContextTrustTypeDef",
+    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     "VirtualNodeConnectionPoolTypeDef",
     "VirtualServiceProviderTypeDef",
+    "ServiceDiscoveryOutputTypeDef",
     "ServiceDiscoveryTypeDef",
     "ListenerTimeoutTypeDef",
     "GrpcGatewayRouteActionTypeDef",
     "GrpcGatewayRouteMetadataTypeDef",
     "GrpcRouteMetadataTypeDef",
     "HttpGatewayRouteHeaderTypeDef",
     "HttpRouteHeaderTypeDef",
+    "TcpRouteOutputTypeDef",
     "TcpRouteTypeDef",
     "HttpGatewayRouteActionTypeDef",
+    "FileAccessLogOutputTypeDef",
+    "VirtualGatewayFileAccessLogOutputTypeDef",
     "FileAccessLogTypeDef",
     "VirtualGatewayFileAccessLogTypeDef",
+    "VirtualRouterSpecOutputTypeDef",
     "VirtualRouterSpecTypeDef",
     "CreateMeshInputRequestTypeDef",
     "MeshDataTypeDef",
     "UpdateMeshInputRequestTypeDef",
+    "ListenerTlsValidationContextOutputTypeDef",
     "ListenerTlsValidationContextTypeDef",
+    "TlsValidationContextOutputTypeDef",
     "TlsValidationContextTypeDef",
+    "VirtualGatewayListenerTlsValidationContextOutputTypeDef",
     "VirtualGatewayListenerTlsValidationContextTypeDef",
+    "VirtualGatewayTlsValidationContextOutputTypeDef",
     "VirtualGatewayTlsValidationContextTypeDef",
     "VirtualServiceSpecTypeDef",
+    "GrpcGatewayRouteMatchOutputTypeDef",
     "GrpcGatewayRouteMatchTypeDef",
+    "GrpcRouteMatchOutputTypeDef",
     "GrpcRouteMatchTypeDef",
+    "HttpGatewayRouteMatchOutputTypeDef",
     "HttpGatewayRouteMatchTypeDef",
+    "HttpRouteMatchOutputTypeDef",
     "HttpRouteMatchTypeDef",
+    "AccessLogOutputTypeDef",
+    "VirtualGatewayAccessLogOutputTypeDef",
     "AccessLogTypeDef",
     "VirtualGatewayAccessLogTypeDef",
+    "VirtualRouterDataTypeDef",
     "CreateVirtualRouterInputRequestTypeDef",
     "UpdateVirtualRouterInputRequestTypeDef",
-    "VirtualRouterDataTypeDef",
+    "VirtualRouterSpecUnionTypeDef",
     "CreateMeshOutputTypeDef",
     "DeleteMeshOutputTypeDef",
     "DescribeMeshOutputTypeDef",
     "UpdateMeshOutputTypeDef",
+    "ListenerTlsOutputTypeDef",
     "ListenerTlsTypeDef",
+    "ClientPolicyTlsOutputTypeDef",
     "ClientPolicyTlsTypeDef",
+    "VirtualGatewayListenerTlsOutputTypeDef",
     "VirtualGatewayListenerTlsTypeDef",
+    "VirtualGatewayClientPolicyTlsOutputTypeDef",
     "VirtualGatewayClientPolicyTlsTypeDef",
     "CreateVirtualServiceInputRequestTypeDef",
     "UpdateVirtualServiceInputRequestTypeDef",
     "VirtualServiceDataTypeDef",
+    "GrpcGatewayRouteOutputTypeDef",
     "GrpcGatewayRouteTypeDef",
+    "GrpcRouteOutputTypeDef",
     "GrpcRouteTypeDef",
+    "HttpGatewayRouteOutputTypeDef",
     "HttpGatewayRouteTypeDef",
+    "HttpRouteOutputTypeDef",
     "HttpRouteTypeDef",
+    "LoggingOutputTypeDef",
+    "VirtualGatewayLoggingOutputTypeDef",
     "LoggingTypeDef",
     "VirtualGatewayLoggingTypeDef",
     "CreateVirtualRouterOutputTypeDef",
     "DeleteVirtualRouterOutputTypeDef",
     "DescribeVirtualRouterOutputTypeDef",
     "UpdateVirtualRouterOutputTypeDef",
+    "ListenerOutputTypeDef",
     "ListenerTypeDef",
+    "ClientPolicyOutputTypeDef",
     "ClientPolicyTypeDef",
+    "VirtualGatewayListenerOutputTypeDef",
     "VirtualGatewayListenerTypeDef",
+    "VirtualGatewayClientPolicyOutputTypeDef",
     "VirtualGatewayClientPolicyTypeDef",
     "CreateVirtualServiceOutputTypeDef",
     "DeleteVirtualServiceOutputTypeDef",
     "DescribeVirtualServiceOutputTypeDef",
     "UpdateVirtualServiceOutputTypeDef",
+    "GatewayRouteSpecOutputTypeDef",
     "GatewayRouteSpecTypeDef",
+    "RouteSpecOutputTypeDef",
     "RouteSpecTypeDef",
+    "BackendDefaultsOutputTypeDef",
+    "VirtualServiceBackendOutputTypeDef",
     "BackendDefaultsTypeDef",
     "VirtualServiceBackendTypeDef",
+    "VirtualGatewayBackendDefaultsOutputTypeDef",
     "VirtualGatewayBackendDefaultsTypeDef",
-    "CreateGatewayRouteInputRequestTypeDef",
     "GatewayRouteDataTypeDef",
+    "CreateGatewayRouteInputRequestTypeDef",
+    "GatewayRouteSpecUnionTypeDef",
     "UpdateGatewayRouteInputRequestTypeDef",
-    "CreateRouteInputRequestTypeDef",
     "RouteDataTypeDef",
+    "CreateRouteInputRequestTypeDef",
+    "RouteSpecUnionTypeDef",
     "UpdateRouteInputRequestTypeDef",
+    "BackendOutputTypeDef",
     "BackendTypeDef",
+    "VirtualGatewaySpecOutputTypeDef",
     "VirtualGatewaySpecTypeDef",
     "CreateGatewayRouteOutputTypeDef",
     "DeleteGatewayRouteOutputTypeDef",
     "DescribeGatewayRouteOutputTypeDef",
     "UpdateGatewayRouteOutputTypeDef",
     "CreateRouteOutputTypeDef",
     "DeleteRouteOutputTypeDef",
     "DescribeRouteOutputTypeDef",
     "UpdateRouteOutputTypeDef",
+    "VirtualNodeSpecOutputTypeDef",
     "VirtualNodeSpecTypeDef",
+    "VirtualGatewayDataTypeDef",
     "CreateVirtualGatewayInputRequestTypeDef",
     "UpdateVirtualGatewayInputRequestTypeDef",
-    "VirtualGatewayDataTypeDef",
+    "VirtualGatewaySpecUnionTypeDef",
+    "VirtualNodeDataTypeDef",
     "CreateVirtualNodeInputRequestTypeDef",
     "UpdateVirtualNodeInputRequestTypeDef",
-    "VirtualNodeDataTypeDef",
+    "VirtualNodeSpecUnionTypeDef",
     "CreateVirtualGatewayOutputTypeDef",
     "DeleteVirtualGatewayOutputTypeDef",
     "DescribeVirtualGatewayOutputTypeDef",
     "UpdateVirtualGatewayOutputTypeDef",
     "CreateVirtualNodeOutputTypeDef",
     "DeleteVirtualNodeOutputTypeDef",
     "DescribeVirtualNodeOutputTypeDef",
@@ -302,14 +358,25 @@
     "TagRefTypeDef",
     {
         "key": str,
         "value": str,
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
 _RequiredDeleteGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDeleteGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -318,19 +385,21 @@
     "_OptionalDeleteGatewayRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DeleteGatewayRouteInputRequestTypeDef(
     _RequiredDeleteGatewayRouteInputRequestTypeDef, _OptionalDeleteGatewayRouteInputRequestTypeDef
 ):
     pass
 
+
 DeleteMeshInputRequestTypeDef = TypedDict(
     "DeleteMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 
@@ -346,19 +415,21 @@
     "_OptionalDeleteRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DeleteRouteInputRequestTypeDef(
     _RequiredDeleteRouteInputRequestTypeDef, _OptionalDeleteRouteInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -366,20 +437,22 @@
     "_OptionalDeleteVirtualGatewayInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DeleteVirtualGatewayInputRequestTypeDef(
     _RequiredDeleteVirtualGatewayInputRequestTypeDef,
     _OptionalDeleteVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDeleteVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "virtualNodeName": str,
     },
 )
@@ -387,19 +460,21 @@
     "_OptionalDeleteVirtualNodeInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DeleteVirtualNodeInputRequestTypeDef(
     _RequiredDeleteVirtualNodeInputRequestTypeDef, _OptionalDeleteVirtualNodeInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -407,19 +482,21 @@
     "_OptionalDeleteVirtualRouterInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DeleteVirtualRouterInputRequestTypeDef(
     _RequiredDeleteVirtualRouterInputRequestTypeDef, _OptionalDeleteVirtualRouterInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDeleteVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredDeleteVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "virtualServiceName": str,
     },
 )
@@ -427,20 +504,22 @@
     "_OptionalDeleteVirtualServiceInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DeleteVirtualServiceInputRequestTypeDef(
     _RequiredDeleteVirtualServiceInputRequestTypeDef,
     _OptionalDeleteVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredDescribeGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "virtualGatewayName": str,
     },
@@ -449,39 +528,43 @@
     "_OptionalDescribeGatewayRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeGatewayRouteInputRequestTypeDef(
     _RequiredDescribeGatewayRouteInputRequestTypeDef,
     _OptionalDescribeGatewayRouteInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeMeshInputRequestTypeDef = TypedDict(
     "_RequiredDescribeMeshInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalDescribeMeshInputRequestTypeDef = TypedDict(
     "_OptionalDescribeMeshInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeMeshInputRequestTypeDef(
     _RequiredDescribeMeshInputRequestTypeDef, _OptionalDescribeMeshInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeRouteInputRequestTypeDef = TypedDict(
     "_RequiredDescribeRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "virtualRouterName": str,
     },
@@ -490,19 +573,21 @@
     "_OptionalDescribeRouteInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeRouteInputRequestTypeDef(
     _RequiredDescribeRouteInputRequestTypeDef, _OptionalDescribeRouteInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -510,20 +595,22 @@
     "_OptionalDescribeVirtualGatewayInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeVirtualGatewayInputRequestTypeDef(
     _RequiredDescribeVirtualGatewayInputRequestTypeDef,
     _OptionalDescribeVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "virtualNodeName": str,
     },
 )
@@ -531,19 +618,21 @@
     "_OptionalDescribeVirtualNodeInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeVirtualNodeInputRequestTypeDef(
     _RequiredDescribeVirtualNodeInputRequestTypeDef, _OptionalDescribeVirtualNodeInputRequestTypeDef
 ):
     pass
 
+
 _RequiredDescribeVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -551,20 +640,22 @@
     "_OptionalDescribeVirtualRouterInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeVirtualRouterInputRequestTypeDef(
     _RequiredDescribeVirtualRouterInputRequestTypeDef,
     _OptionalDescribeVirtualRouterInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDescribeVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredDescribeVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "virtualServiceName": str,
     },
 )
@@ -572,20 +663,22 @@
     "_OptionalDescribeVirtualServiceInputRequestTypeDef",
     {
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class DescribeVirtualServiceInputRequestTypeDef(
     _RequiredDescribeVirtualServiceInputRequestTypeDef,
     _OptionalDescribeVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredDnsServiceDiscoveryTypeDef = TypedDict(
     "_RequiredDnsServiceDiscoveryTypeDef",
     {
         "hostname": str,
     },
 )
 _OptionalDnsServiceDiscoveryTypeDef = TypedDict(
@@ -593,19 +686,21 @@
     {
         "ipPreference": IpPreferenceType,
         "responseType": DnsResponseTypeType,
     },
     total=False,
 )
 
+
 class DnsServiceDiscoveryTypeDef(
     _RequiredDnsServiceDiscoveryTypeDef, _OptionalDnsServiceDiscoveryTypeDef
 ):
     pass
 
+
 DurationTypeDef = TypedDict(
     "DurationTypeDef",
     {
         "unit": DurationUnitType,
         "value": int,
     },
     total=False,
@@ -696,17 +791,19 @@
     "_OptionalWeightedTargetTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
+
 class WeightedTargetTypeDef(_RequiredWeightedTargetTypeDef, _OptionalWeightedTargetTypeDef):
     pass
 
+
 _RequiredHealthCheckPolicyTypeDef = TypedDict(
     "_RequiredHealthCheckPolicyTypeDef",
     {
         "healthyThreshold": int,
         "intervalMillis": int,
         "protocol": PortProtocolType,
         "timeoutMillis": int,
@@ -718,19 +815,21 @@
     {
         "path": str,
         "port": int,
     },
     total=False,
 )
 
+
 class HealthCheckPolicyTypeDef(
     _RequiredHealthCheckPolicyTypeDef, _OptionalHealthCheckPolicyTypeDef
 ):
     pass
 
+
 HttpPathMatchTypeDef = TypedDict(
     "HttpPathMatchTypeDef",
     {
         "exact": str,
         "regex": str,
     },
     total=False,
@@ -765,36 +864,24 @@
     "JsonFormatRefTypeDef",
     {
         "key": str,
         "value": str,
     },
 )
 
-_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualGatewayName": str,
-    },
-)
-_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
-    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredListGatewayRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListGatewayRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualGatewayName": str,
     },
 )
@@ -804,26 +891,20 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListGatewayRoutesInputRequestTypeDef(
     _RequiredListGatewayRoutesInputRequestTypeDef, _OptionalListGatewayRoutesInputRequestTypeDef
 ):
     pass
 
-ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
-    "ListMeshesInputListMeshesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
 
 ListMeshesInputRequestTypeDef = TypedDict(
     "ListMeshesInputRequestTypeDef",
     {
         "limit": int,
         "nextToken": str,
     },
@@ -839,36 +920,14 @@
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
     },
 )
 
-_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshName": str,
-        "virtualRouterName": str,
-    },
-)
-_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
-    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListRoutesInputListRoutesPaginateTypeDef(
-    _RequiredListRoutesInputListRoutesPaginateTypeDef,
-    _OptionalListRoutesInputListRoutesPaginateTypeDef,
-):
-    pass
-
 _RequiredListRoutesInputRequestTypeDef = TypedDict(
     "_RequiredListRoutesInputRequestTypeDef",
     {
         "meshName": str,
         "virtualRouterName": str,
     },
 )
@@ -878,19 +937,21 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListRoutesInputRequestTypeDef(
     _RequiredListRoutesInputRequestTypeDef, _OptionalListRoutesInputRequestTypeDef
 ):
     pass
 
+
 RouteRefTypeDef = TypedDict(
     "RouteRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
@@ -898,34 +959,14 @@
         "resourceOwner": str,
         "routeName": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "resourceArn": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -933,39 +974,20 @@
     {
         "limit": int,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
-    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
-):
-    pass
 
 _RequiredListVirtualGatewaysInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualGatewaysInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
@@ -975,54 +997,35 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListVirtualGatewaysInputRequestTypeDef(
     _RequiredListVirtualGatewaysInputRequestTypeDef, _OptionalListVirtualGatewaysInputRequestTypeDef
 ):
     pass
 
+
 VirtualGatewayRefTypeDef = TypedDict(
     "VirtualGatewayRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualGatewayName": str,
     },
 )
 
-_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
-    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualNodesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualNodesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualNodesInputRequestTypeDef = TypedDict(
@@ -1031,54 +1034,35 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListVirtualNodesInputRequestTypeDef(
     _RequiredListVirtualNodesInputRequestTypeDef, _OptionalListVirtualNodesInputRequestTypeDef
 ):
     pass
 
+
 VirtualNodeRefTypeDef = TypedDict(
     "VirtualNodeRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualNodeName": str,
     },
 )
 
-_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
-    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualRoutersInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualRoutersInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualRoutersInputRequestTypeDef = TypedDict(
@@ -1087,54 +1071,35 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListVirtualRoutersInputRequestTypeDef(
     _RequiredListVirtualRoutersInputRequestTypeDef, _OptionalListVirtualRoutersInputRequestTypeDef
 ):
     pass
 
+
 VirtualRouterRefTypeDef = TypedDict(
     "VirtualRouterRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualRouterName": str,
     },
 )
 
-_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshName": str,
-    },
-)
-_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
-    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
-    {
-        "meshOwner": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
-    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
-):
-    pass
-
 _RequiredListVirtualServicesInputRequestTypeDef = TypedDict(
     "_RequiredListVirtualServicesInputRequestTypeDef",
     {
         "meshName": str,
     },
 )
 _OptionalListVirtualServicesInputRequestTypeDef = TypedDict(
@@ -1143,33 +1108,43 @@
         "limit": int,
         "meshOwner": str,
         "nextToken": str,
     },
     total=False,
 )
 
+
 class ListVirtualServicesInputRequestTypeDef(
     _RequiredListVirtualServicesInputRequestTypeDef, _OptionalListVirtualServicesInputRequestTypeDef
 ):
     pass
 
+
 VirtualServiceRefTypeDef = TypedDict(
     "VirtualServiceRefTypeDef",
     {
         "arn": str,
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
         "meshName": str,
         "meshOwner": str,
         "resourceOwner": str,
         "version": int,
         "virtualServiceName": str,
     },
 )
 
+PortMappingTypeDef = TypedDict(
+    "PortMappingTypeDef",
+    {
+        "port": int,
+        "protocol": PortProtocolType,
+    },
+)
+
 ListenerTlsAcmCertificateTypeDef = TypedDict(
     "ListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1183,22 +1158,14 @@
 TlsValidationContextSdsTrustTypeDef = TypedDict(
     "TlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-PortMappingTypeDef = TypedDict(
-    "PortMappingTypeDef",
-    {
-        "port": int,
-        "protocol": PortProtocolType,
-    },
-)
-
 MeshStatusTypeDef = TypedDict(
     "MeshStatusTypeDef",
     {
         "status": MeshStatusCodeType,
     },
     total=False,
 )
@@ -1207,39 +1174,25 @@
     "MeshServiceDiscoveryTypeDef",
     {
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+RouteStatusTypeDef = TypedDict(
+    "RouteStatusTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "status": RouteStatusCodeType,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+SubjectAlternativeNameMatchersOutputTypeDef = TypedDict(
+    "SubjectAlternativeNameMatchersOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-RouteStatusTypeDef = TypedDict(
-    "RouteStatusTypeDef",
-    {
-        "status": RouteStatusCodeType,
+        "exact": List[str],
     },
 )
 
 SubjectAlternativeNameMatchersTypeDef = TypedDict(
     "SubjectAlternativeNameMatchersTypeDef",
     {
         "exact": Sequence[str],
@@ -1250,14 +1203,21 @@
     "TcpRouteMatchTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
+TlsValidationContextAcmTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextAcmTrustOutputTypeDef",
+    {
+        "certificateAuthorityArns": List[str],
+    },
+)
+
 TlsValidationContextAcmTrustTypeDef = TypedDict(
     "TlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
     },
 )
 
@@ -1308,20 +1268,22 @@
     "_OptionalVirtualGatewayHttpConnectionPoolTypeDef",
     {
         "maxPendingRequests": int,
     },
     total=False,
 )
 
+
 class VirtualGatewayHttpConnectionPoolTypeDef(
     _RequiredVirtualGatewayHttpConnectionPoolTypeDef,
     _OptionalVirtualGatewayHttpConnectionPoolTypeDef,
 ):
     pass
 
+
 VirtualGatewayStatusTypeDef = TypedDict(
     "VirtualGatewayStatusTypeDef",
     {
         "status": VirtualGatewayStatusCodeType,
     },
 )
 
@@ -1340,19 +1302,29 @@
     {
         "path": str,
         "port": int,
     },
     total=False,
 )
 
+
 class VirtualGatewayHealthCheckPolicyTypeDef(
     _RequiredVirtualGatewayHealthCheckPolicyTypeDef, _OptionalVirtualGatewayHealthCheckPolicyTypeDef
 ):
     pass
 
+
+VirtualGatewayPortMappingTypeDef = TypedDict(
+    "VirtualGatewayPortMappingTypeDef",
+    {
+        "port": int,
+        "protocol": VirtualGatewayPortProtocolType,
+    },
+)
+
 VirtualGatewayListenerTlsAcmCertificateTypeDef = TypedDict(
     "VirtualGatewayListenerTlsAcmCertificateTypeDef",
     {
         "certificateArn": str,
     },
 )
 
@@ -1366,19 +1338,18 @@
 VirtualGatewayTlsValidationContextSdsTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextSdsTrustTypeDef",
     {
         "secretName": str,
     },
 )
 
-VirtualGatewayPortMappingTypeDef = TypedDict(
-    "VirtualGatewayPortMappingTypeDef",
+VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef",
     {
-        "port": int,
-        "protocol": VirtualGatewayPortProtocolType,
+        "certificateAuthorityArns": List[str],
     },
 )
 
 VirtualGatewayTlsValidationContextAcmTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextAcmTrustTypeDef",
     {
         "certificateAuthorityArns": Sequence[str],
@@ -1409,19 +1380,21 @@
     "_OptionalVirtualNodeHttpConnectionPoolTypeDef",
     {
         "maxPendingRequests": int,
     },
     total=False,
 )
 
+
 class VirtualNodeHttpConnectionPoolTypeDef(
     _RequiredVirtualNodeHttpConnectionPoolTypeDef, _OptionalVirtualNodeHttpConnectionPoolTypeDef
 ):
     pass
 
+
 VirtualNodeTcpConnectionPoolTypeDef = TypedDict(
     "VirtualNodeTcpConnectionPoolTypeDef",
     {
         "maxConnections": int,
     },
 )
 
@@ -1456,14 +1429,38 @@
 VirtualServiceStatusTypeDef = TypedDict(
     "VirtualServiceStatusTypeDef",
     {
         "status": VirtualServiceStatusCodeType,
     },
 )
 
+_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
+    "_RequiredAwsCloudMapServiceDiscoveryOutputTypeDef",
+    {
+        "namespaceName": str,
+        "serviceName": str,
+    },
+)
+_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef = TypedDict(
+    "_OptionalAwsCloudMapServiceDiscoveryOutputTypeDef",
+    {
+        "attributes": List[AwsCloudMapInstanceAttributeTypeDef],
+        "ipPreference": IpPreferenceType,
+    },
+    total=False,
+)
+
+
+class AwsCloudMapServiceDiscoveryOutputTypeDef(
+    _RequiredAwsCloudMapServiceDiscoveryOutputTypeDef,
+    _OptionalAwsCloudMapServiceDiscoveryOutputTypeDef,
+):
+    pass
+
+
 _RequiredAwsCloudMapServiceDiscoveryTypeDef = TypedDict(
     "_RequiredAwsCloudMapServiceDiscoveryTypeDef",
     {
         "namespaceName": str,
         "serviceName": str,
     },
 )
@@ -1472,44 +1469,70 @@
     {
         "attributes": Sequence[AwsCloudMapInstanceAttributeTypeDef],
         "ipPreference": IpPreferenceType,
     },
     total=False,
 )
 
+
 class AwsCloudMapServiceDiscoveryTypeDef(
     _RequiredAwsCloudMapServiceDiscoveryTypeDef, _OptionalAwsCloudMapServiceDiscoveryTypeDef
 ):
     pass
 
+
 ClientTlsCertificateTypeDef = TypedDict(
     "ClientTlsCertificateTypeDef",
     {
         "file": ListenerTlsFileCertificateTypeDef,
         "sds": ListenerTlsSdsCertificateTypeDef,
     },
     total=False,
 )
 
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tags": Sequence[TagRefTypeDef],
+    },
+)
+
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "nextToken": str,
         "tags": List[TagRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+_RequiredGrpcRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredGrpcRetryPolicyOutputTypeDef",
     {
-        "resourceArn": str,
-        "tags": Sequence[TagRefTypeDef],
+        "maxRetries": int,
+        "perRetryTimeout": DurationTypeDef,
     },
 )
+_OptionalGrpcRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalGrpcRetryPolicyOutputTypeDef",
+    {
+        "grpcRetryEvents": List[GrpcRetryPolicyEventType],
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
+    },
+    total=False,
+)
+
+
+class GrpcRetryPolicyOutputTypeDef(
+    _RequiredGrpcRetryPolicyOutputTypeDef, _OptionalGrpcRetryPolicyOutputTypeDef
+):
+    pass
+
 
 _RequiredGrpcRetryPolicyTypeDef = TypedDict(
     "_RequiredGrpcRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
@@ -1520,26 +1543,51 @@
         "grpcRetryEvents": Sequence[GrpcRetryPolicyEventType],
         "httpRetryEvents": Sequence[str],
         "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
+
 class GrpcRetryPolicyTypeDef(_RequiredGrpcRetryPolicyTypeDef, _OptionalGrpcRetryPolicyTypeDef):
     pass
 
+
 GrpcTimeoutTypeDef = TypedDict(
     "GrpcTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
 )
 
+_RequiredHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_RequiredHttpRetryPolicyOutputTypeDef",
+    {
+        "maxRetries": int,
+        "perRetryTimeout": DurationTypeDef,
+    },
+)
+_OptionalHttpRetryPolicyOutputTypeDef = TypedDict(
+    "_OptionalHttpRetryPolicyOutputTypeDef",
+    {
+        "httpRetryEvents": List[str],
+        "tcpRetryEvents": List[Literal["connection-error"]],
+    },
+    total=False,
+)
+
+
+class HttpRetryPolicyOutputTypeDef(
+    _RequiredHttpRetryPolicyOutputTypeDef, _OptionalHttpRetryPolicyOutputTypeDef
+):
+    pass
+
+
 _RequiredHttpRetryPolicyTypeDef = TypedDict(
     "_RequiredHttpRetryPolicyTypeDef",
     {
         "maxRetries": int,
         "perRetryTimeout": DurationTypeDef,
     },
 )
@@ -1548,17 +1596,19 @@
     {
         "httpRetryEvents": Sequence[str],
         "tcpRetryEvents": Sequence[Literal["connection-error"]],
     },
     total=False,
 )
 
+
 class HttpRetryPolicyTypeDef(_RequiredHttpRetryPolicyTypeDef, _OptionalHttpRetryPolicyTypeDef):
     pass
 
+
 HttpTimeoutTypeDef = TypedDict(
     "HttpTimeoutTypeDef",
     {
         "idle": DurationTypeDef,
         "perRequest": DurationTypeDef,
     },
     total=False,
@@ -1591,15 +1641,15 @@
 )
 
 ListGatewayRoutesOutputTypeDef = TypedDict(
     "ListGatewayRoutesOutputTypeDef",
     {
         "gatewayRoutes": List[GatewayRouteRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGatewayRouteTargetTypeDef = TypedDict(
     "_RequiredGatewayRouteTargetTypeDef",
     {
         "virtualService": GatewayRouteVirtualServiceTypeDef,
@@ -1609,19 +1659,21 @@
     "_OptionalGatewayRouteTargetTypeDef",
     {
         "port": int,
     },
     total=False,
 )
 
+
 class GatewayRouteTargetTypeDef(
     _RequiredGatewayRouteTargetTypeDef, _OptionalGatewayRouteTargetTypeDef
 ):
     pass
 
+
 GrpcMetadataMatchMethodTypeDef = TypedDict(
     "GrpcMetadataMatchMethodTypeDef",
     {
         "exact": str,
         "prefix": str,
         "range": MatchRangeTypeDef,
         "regex": str,
@@ -1650,28 +1702,49 @@
         "range": MatchRangeTypeDef,
         "regex": str,
         "suffix": str,
     },
     total=False,
 )
 
+GrpcRouteActionOutputTypeDef = TypedDict(
+    "GrpcRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetTypeDef],
+    },
+)
+
 GrpcRouteActionTypeDef = TypedDict(
     "GrpcRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
+HttpRouteActionOutputTypeDef = TypedDict(
+    "HttpRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetTypeDef],
+    },
+)
+
 HttpRouteActionTypeDef = TypedDict(
     "HttpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
+TcpRouteActionOutputTypeDef = TypedDict(
+    "TcpRouteActionOutputTypeDef",
+    {
+        "weightedTargets": List[WeightedTargetTypeDef],
+    },
+)
+
 TcpRouteActionTypeDef = TypedDict(
     "TcpRouteActionTypeDef",
     {
         "weightedTargets": Sequence[WeightedTargetTypeDef],
     },
 )
 
@@ -1695,79 +1768,267 @@
     "_OptionalHttpQueryParameterTypeDef",
     {
         "match": QueryParameterMatchTypeDef,
     },
     total=False,
 )
 
+
 class HttpQueryParameterTypeDef(
     _RequiredHttpQueryParameterTypeDef, _OptionalHttpQueryParameterTypeDef
 ):
     pass
 
+
+LoggingFormatOutputTypeDef = TypedDict(
+    "LoggingFormatOutputTypeDef",
+    {
+        "json": List[JsonFormatRefTypeDef],
+        "text": str,
+    },
+    total=False,
+)
+
 LoggingFormatTypeDef = TypedDict(
     "LoggingFormatTypeDef",
     {
         "json": Sequence[JsonFormatRefTypeDef],
         "text": str,
     },
     total=False,
 )
 
+_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualGatewayName": str,
+    },
+)
+_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef(
+    _RequiredListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    _OptionalListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+):
+    pass
+
+
+ListMeshesInputListMeshesPaginateTypeDef = TypedDict(
+    "ListMeshesInputListMeshesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_RequiredListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshName": str,
+        "virtualRouterName": str,
+    },
+)
+_OptionalListRoutesInputListRoutesPaginateTypeDef = TypedDict(
+    "_OptionalListRoutesInputListRoutesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListRoutesInputListRoutesPaginateTypeDef(
+    _RequiredListRoutesInputListRoutesPaginateTypeDef,
+    _OptionalListRoutesInputListRoutesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "resourceArn": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef(
+    _RequiredListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    _OptionalListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualNodesInputListVirtualNodesPaginateTypeDef(
+    _RequiredListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    _OptionalListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef(
+    _RequiredListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    _OptionalListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshName": str,
+    },
+)
+_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef = TypedDict(
+    "_OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef",
+    {
+        "meshOwner": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListVirtualServicesInputListVirtualServicesPaginateTypeDef(
+    _RequiredListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+    _OptionalListVirtualServicesInputListVirtualServicesPaginateTypeDef,
+):
+    pass
+
+
 ListMeshesOutputTypeDef = TypedDict(
     "ListMeshesOutputTypeDef",
     {
         "meshes": List[MeshRefTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListRoutesOutputTypeDef = TypedDict(
     "ListRoutesOutputTypeDef",
     {
         "nextToken": str,
         "routes": List[RouteRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualGatewaysOutputTypeDef = TypedDict(
     "ListVirtualGatewaysOutputTypeDef",
     {
         "nextToken": str,
         "virtualGateways": List[VirtualGatewayRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualNodesOutputTypeDef = TypedDict(
     "ListVirtualNodesOutputTypeDef",
     {
         "nextToken": str,
         "virtualNodes": List[VirtualNodeRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualRoutersOutputTypeDef = TypedDict(
     "ListVirtualRoutersOutputTypeDef",
     {
         "nextToken": str,
         "virtualRouters": List[VirtualRouterRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListVirtualServicesOutputTypeDef = TypedDict(
     "ListVirtualServicesOutputTypeDef",
     {
         "nextToken": str,
         "virtualServices": List[VirtualServiceRefTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VirtualRouterListenerTypeDef = TypedDict(
+    "VirtualRouterListenerTypeDef",
+    {
+        "portMapping": PortMappingTypeDef,
     },
 )
 
 ListenerTlsCertificateTypeDef = TypedDict(
     "ListenerTlsCertificateTypeDef",
     {
         "acm": ListenerTlsAcmCertificateTypeDef,
@@ -1782,37 +2043,47 @@
     {
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
-VirtualRouterListenerTypeDef = TypedDict(
-    "VirtualRouterListenerTypeDef",
-    {
-        "portMapping": PortMappingTypeDef,
-    },
-)
-
 MeshSpecTypeDef = TypedDict(
     "MeshSpecTypeDef",
     {
         "egressFilter": EgressFilterTypeDef,
         "serviceDiscovery": MeshServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+SubjectAlternativeNamesOutputTypeDef = TypedDict(
+    "SubjectAlternativeNamesOutputTypeDef",
+    {
+        "match": SubjectAlternativeNameMatchersOutputTypeDef,
+    },
+)
+
 SubjectAlternativeNamesTypeDef = TypedDict(
     "SubjectAlternativeNamesTypeDef",
     {
         "match": SubjectAlternativeNameMatchersTypeDef,
     },
 )
 
+TlsValidationContextTrustOutputTypeDef = TypedDict(
+    "TlsValidationContextTrustOutputTypeDef",
+    {
+        "acm": TlsValidationContextAcmTrustOutputTypeDef,
+        "file": TlsValidationContextFileTrustTypeDef,
+        "sds": TlsValidationContextSdsTrustTypeDef,
+    },
+    total=False,
+)
+
 TlsValidationContextTrustTypeDef = TypedDict(
     "TlsValidationContextTrustTypeDef",
     {
         "acm": TlsValidationContextAcmTrustTypeDef,
         "file": TlsValidationContextFileTrustTypeDef,
         "sds": TlsValidationContextSdsTrustTypeDef,
     },
@@ -1853,14 +2124,24 @@
     {
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayTlsValidationContextTrustOutputTypeDef = TypedDict(
+    "VirtualGatewayTlsValidationContextTrustOutputTypeDef",
+    {
+        "acm": VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
+        "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
+        "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayTlsValidationContextTrustTypeDef = TypedDict(
     "VirtualGatewayTlsValidationContextTrustTypeDef",
     {
         "acm": VirtualGatewayTlsValidationContextAcmTrustTypeDef,
         "file": VirtualGatewayTlsValidationContextFileTrustTypeDef,
         "sds": VirtualGatewayTlsValidationContextSdsTrustTypeDef,
     },
@@ -1883,14 +2164,23 @@
     {
         "virtualNode": VirtualNodeServiceProviderTypeDef,
         "virtualRouter": VirtualRouterServiceProviderTypeDef,
     },
     total=False,
 )
 
+ServiceDiscoveryOutputTypeDef = TypedDict(
+    "ServiceDiscoveryOutputTypeDef",
+    {
+        "awsCloudMap": AwsCloudMapServiceDiscoveryOutputTypeDef,
+        "dns": DnsServiceDiscoveryTypeDef,
+    },
+    total=False,
+)
+
 ServiceDiscoveryTypeDef = TypedDict(
     "ServiceDiscoveryTypeDef",
     {
         "awsCloudMap": AwsCloudMapServiceDiscoveryTypeDef,
         "dns": DnsServiceDiscoveryTypeDef,
     },
     total=False,
@@ -1917,19 +2207,21 @@
     "_OptionalGrpcGatewayRouteActionTypeDef",
     {
         "rewrite": GrpcGatewayRouteRewriteTypeDef,
     },
     total=False,
 )
 
+
 class GrpcGatewayRouteActionTypeDef(
     _RequiredGrpcGatewayRouteActionTypeDef, _OptionalGrpcGatewayRouteActionTypeDef
 ):
     pass
 
+
 _RequiredGrpcGatewayRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcGatewayRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcGatewayRouteMetadataTypeDef = TypedDict(
@@ -1937,19 +2229,21 @@
     {
         "invert": bool,
         "match": GrpcMetadataMatchMethodTypeDef,
     },
     total=False,
 )
 
+
 class GrpcGatewayRouteMetadataTypeDef(
     _RequiredGrpcGatewayRouteMetadataTypeDef, _OptionalGrpcGatewayRouteMetadataTypeDef
 ):
     pass
 
+
 _RequiredGrpcRouteMetadataTypeDef = TypedDict(
     "_RequiredGrpcRouteMetadataTypeDef",
     {
         "name": str,
     },
 )
 _OptionalGrpcRouteMetadataTypeDef = TypedDict(
@@ -1957,19 +2251,21 @@
     {
         "invert": bool,
         "match": GrpcRouteMetadataMatchMethodTypeDef,
     },
     total=False,
 )
 
+
 class GrpcRouteMetadataTypeDef(
     _RequiredGrpcRouteMetadataTypeDef, _OptionalGrpcRouteMetadataTypeDef
 ):
     pass
 
+
 _RequiredHttpGatewayRouteHeaderTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteHeaderTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpGatewayRouteHeaderTypeDef = TypedDict(
@@ -1977,19 +2273,21 @@
     {
         "invert": bool,
         "match": HeaderMatchMethodTypeDef,
     },
     total=False,
 )
 
+
 class HttpGatewayRouteHeaderTypeDef(
     _RequiredHttpGatewayRouteHeaderTypeDef, _OptionalHttpGatewayRouteHeaderTypeDef
 ):
     pass
 
+
 _RequiredHttpRouteHeaderTypeDef = TypedDict(
     "_RequiredHttpRouteHeaderTypeDef",
     {
         "name": str,
     },
 )
 _OptionalHttpRouteHeaderTypeDef = TypedDict(
@@ -1997,17 +2295,39 @@
     {
         "invert": bool,
         "match": HeaderMatchMethodTypeDef,
     },
     total=False,
 )
 
+
 class HttpRouteHeaderTypeDef(_RequiredHttpRouteHeaderTypeDef, _OptionalHttpRouteHeaderTypeDef):
     pass
 
+
+_RequiredTcpRouteOutputTypeDef = TypedDict(
+    "_RequiredTcpRouteOutputTypeDef",
+    {
+        "action": TcpRouteActionOutputTypeDef,
+    },
+)
+_OptionalTcpRouteOutputTypeDef = TypedDict(
+    "_OptionalTcpRouteOutputTypeDef",
+    {
+        "match": TcpRouteMatchTypeDef,
+        "timeout": TcpTimeoutTypeDef,
+    },
+    total=False,
+)
+
+
+class TcpRouteOutputTypeDef(_RequiredTcpRouteOutputTypeDef, _OptionalTcpRouteOutputTypeDef):
+    pass
+
+
 _RequiredTcpRouteTypeDef = TypedDict(
     "_RequiredTcpRouteTypeDef",
     {
         "action": TcpRouteActionTypeDef,
     },
 )
 _OptionalTcpRouteTypeDef = TypedDict(
@@ -2015,72 +2335,131 @@
     {
         "match": TcpRouteMatchTypeDef,
         "timeout": TcpTimeoutTypeDef,
     },
     total=False,
 )
 
+
 class TcpRouteTypeDef(_RequiredTcpRouteTypeDef, _OptionalTcpRouteTypeDef):
     pass
 
+
 _RequiredHttpGatewayRouteActionTypeDef = TypedDict(
     "_RequiredHttpGatewayRouteActionTypeDef",
     {
         "target": GatewayRouteTargetTypeDef,
     },
 )
 _OptionalHttpGatewayRouteActionTypeDef = TypedDict(
     "_OptionalHttpGatewayRouteActionTypeDef",
     {
         "rewrite": HttpGatewayRouteRewriteTypeDef,
     },
     total=False,
 )
 
+
 class HttpGatewayRouteActionTypeDef(
     _RequiredHttpGatewayRouteActionTypeDef, _OptionalHttpGatewayRouteActionTypeDef
 ):
     pass
 
+
+_RequiredFileAccessLogOutputTypeDef = TypedDict(
+    "_RequiredFileAccessLogOutputTypeDef",
+    {
+        "path": str,
+    },
+)
+_OptionalFileAccessLogOutputTypeDef = TypedDict(
+    "_OptionalFileAccessLogOutputTypeDef",
+    {
+        "format": LoggingFormatOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class FileAccessLogOutputTypeDef(
+    _RequiredFileAccessLogOutputTypeDef, _OptionalFileAccessLogOutputTypeDef
+):
+    pass
+
+
+_RequiredVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayFileAccessLogOutputTypeDef",
+    {
+        "path": str,
+    },
+)
+_OptionalVirtualGatewayFileAccessLogOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayFileAccessLogOutputTypeDef",
+    {
+        "format": LoggingFormatOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualGatewayFileAccessLogOutputTypeDef(
+    _RequiredVirtualGatewayFileAccessLogOutputTypeDef,
+    _OptionalVirtualGatewayFileAccessLogOutputTypeDef,
+):
+    pass
+
+
 _RequiredFileAccessLogTypeDef = TypedDict(
     "_RequiredFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
 _OptionalFileAccessLogTypeDef = TypedDict(
     "_OptionalFileAccessLogTypeDef",
     {
         "format": LoggingFormatTypeDef,
     },
     total=False,
 )
 
+
 class FileAccessLogTypeDef(_RequiredFileAccessLogTypeDef, _OptionalFileAccessLogTypeDef):
     pass
 
+
 _RequiredVirtualGatewayFileAccessLogTypeDef = TypedDict(
     "_RequiredVirtualGatewayFileAccessLogTypeDef",
     {
         "path": str,
     },
 )
 _OptionalVirtualGatewayFileAccessLogTypeDef = TypedDict(
     "_OptionalVirtualGatewayFileAccessLogTypeDef",
     {
         "format": LoggingFormatTypeDef,
     },
     total=False,
 )
 
+
 class VirtualGatewayFileAccessLogTypeDef(
     _RequiredVirtualGatewayFileAccessLogTypeDef, _OptionalVirtualGatewayFileAccessLogTypeDef
 ):
     pass
 
+
+VirtualRouterSpecOutputTypeDef = TypedDict(
+    "VirtualRouterSpecOutputTypeDef",
+    {
+        "listeners": List[VirtualRouterListenerTypeDef],
+    },
+    total=False,
+)
+
 VirtualRouterSpecTypeDef = TypedDict(
     "VirtualRouterSpecTypeDef",
     {
         "listeners": Sequence[VirtualRouterListenerTypeDef],
     },
     total=False,
 )
@@ -2097,19 +2476,21 @@
         "clientToken": str,
         "spec": MeshSpecTypeDef,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateMeshInputRequestTypeDef(
     _RequiredCreateMeshInputRequestTypeDef, _OptionalCreateMeshInputRequestTypeDef
 ):
     pass
 
+
 MeshDataTypeDef = TypedDict(
     "MeshDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
         "spec": MeshSpecTypeDef,
         "status": MeshStatusTypeDef,
@@ -2127,155 +2508,318 @@
     {
         "clientToken": str,
         "spec": MeshSpecTypeDef,
     },
     total=False,
 )
 
+
 class UpdateMeshInputRequestTypeDef(
     _RequiredUpdateMeshInputRequestTypeDef, _OptionalUpdateMeshInputRequestTypeDef
 ):
     pass
 
+
+_RequiredListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredListenerTlsValidationContextOutputTypeDef",
+    {
+        "trust": ListenerTlsValidationContextTrustTypeDef,
+    },
+)
+_OptionalListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalListenerTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ListenerTlsValidationContextOutputTypeDef(
+    _RequiredListenerTlsValidationContextOutputTypeDef,
+    _OptionalListenerTlsValidationContextOutputTypeDef,
+):
+    pass
+
+
 _RequiredListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredListenerTlsValidationContextTypeDef",
     {
         "trust": ListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalListenerTlsValidationContextTypeDef = TypedDict(
     "_OptionalListenerTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
+
 class ListenerTlsValidationContextTypeDef(
     _RequiredListenerTlsValidationContextTypeDef, _OptionalListenerTlsValidationContextTypeDef
 ):
     pass
 
+
+_RequiredTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredTlsValidationContextOutputTypeDef",
+    {
+        "trust": TlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class TlsValidationContextOutputTypeDef(
+    _RequiredTlsValidationContextOutputTypeDef, _OptionalTlsValidationContextOutputTypeDef
+):
+    pass
+
+
 _RequiredTlsValidationContextTypeDef = TypedDict(
     "_RequiredTlsValidationContextTypeDef",
     {
         "trust": TlsValidationContextTrustTypeDef,
     },
 )
 _OptionalTlsValidationContextTypeDef = TypedDict(
     "_OptionalTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
+
 class TlsValidationContextTypeDef(
     _RequiredTlsValidationContextTypeDef, _OptionalTlsValidationContextTypeDef
 ):
     pass
 
+
+_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef",
+    {
+        "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    },
+)
+_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualGatewayListenerTlsValidationContextOutputTypeDef(
+    _RequiredVirtualGatewayListenerTlsValidationContextOutputTypeDef,
+    _OptionalVirtualGatewayListenerTlsValidationContextOutputTypeDef,
+):
+    pass
+
+
 _RequiredVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayListenerTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTlsValidationContextTypeDef = TypedDict(
     "_OptionalVirtualGatewayListenerTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
+
 class VirtualGatewayListenerTlsValidationContextTypeDef(
     _RequiredVirtualGatewayListenerTlsValidationContextTypeDef,
     _OptionalVirtualGatewayListenerTlsValidationContextTypeDef,
 ):
     pass
 
+
+_RequiredVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayTlsValidationContextOutputTypeDef",
+    {
+        "trust": VirtualGatewayTlsValidationContextTrustOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayTlsValidationContextOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayTlsValidationContextOutputTypeDef",
+    {
+        "subjectAlternativeNames": SubjectAlternativeNamesOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualGatewayTlsValidationContextOutputTypeDef(
+    _RequiredVirtualGatewayTlsValidationContextOutputTypeDef,
+    _OptionalVirtualGatewayTlsValidationContextOutputTypeDef,
+):
+    pass
+
+
 _RequiredVirtualGatewayTlsValidationContextTypeDef = TypedDict(
     "_RequiredVirtualGatewayTlsValidationContextTypeDef",
     {
         "trust": VirtualGatewayTlsValidationContextTrustTypeDef,
     },
 )
 _OptionalVirtualGatewayTlsValidationContextTypeDef = TypedDict(
     "_OptionalVirtualGatewayTlsValidationContextTypeDef",
     {
         "subjectAlternativeNames": SubjectAlternativeNamesTypeDef,
     },
     total=False,
 )
 
+
 class VirtualGatewayTlsValidationContextTypeDef(
     _RequiredVirtualGatewayTlsValidationContextTypeDef,
     _OptionalVirtualGatewayTlsValidationContextTypeDef,
 ):
     pass
 
+
 VirtualServiceSpecTypeDef = TypedDict(
     "VirtualServiceSpecTypeDef",
     {
         "provider": VirtualServiceProviderTypeDef,
     },
     total=False,
 )
 
+GrpcGatewayRouteMatchOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteMatchOutputTypeDef",
+    {
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "metadata": List[GrpcGatewayRouteMetadataTypeDef],
+        "port": int,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 GrpcGatewayRouteMatchTypeDef = TypedDict(
     "GrpcGatewayRouteMatchTypeDef",
     {
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "metadata": Sequence[GrpcGatewayRouteMetadataTypeDef],
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
+GrpcRouteMatchOutputTypeDef = TypedDict(
+    "GrpcRouteMatchOutputTypeDef",
+    {
+        "metadata": List[GrpcRouteMetadataTypeDef],
+        "methodName": str,
+        "port": int,
+        "serviceName": str,
+    },
+    total=False,
+)
+
 GrpcRouteMatchTypeDef = TypedDict(
     "GrpcRouteMatchTypeDef",
     {
         "metadata": Sequence[GrpcRouteMetadataTypeDef],
         "methodName": str,
         "port": int,
         "serviceName": str,
     },
     total=False,
 )
 
+HttpGatewayRouteMatchOutputTypeDef = TypedDict(
+    "HttpGatewayRouteMatchOutputTypeDef",
+    {
+        "headers": List[HttpGatewayRouteHeaderTypeDef],
+        "hostname": GatewayRouteHostnameMatchTypeDef,
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
+        "port": int,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterTypeDef],
+    },
+    total=False,
+)
+
 HttpGatewayRouteMatchTypeDef = TypedDict(
     "HttpGatewayRouteMatchTypeDef",
     {
         "headers": Sequence[HttpGatewayRouteHeaderTypeDef],
         "hostname": GatewayRouteHostnameMatchTypeDef,
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
     },
     total=False,
 )
 
+HttpRouteMatchOutputTypeDef = TypedDict(
+    "HttpRouteMatchOutputTypeDef",
+    {
+        "headers": List[HttpRouteHeaderTypeDef],
+        "method": HttpMethodType,
+        "path": HttpPathMatchTypeDef,
+        "port": int,
+        "prefix": str,
+        "queryParameters": List[HttpQueryParameterTypeDef],
+        "scheme": HttpSchemeType,
+    },
+    total=False,
+)
+
 HttpRouteMatchTypeDef = TypedDict(
     "HttpRouteMatchTypeDef",
     {
         "headers": Sequence[HttpRouteHeaderTypeDef],
         "method": HttpMethodType,
         "path": HttpPathMatchTypeDef,
         "port": int,
         "prefix": str,
         "queryParameters": Sequence[HttpQueryParameterTypeDef],
         "scheme": HttpSchemeType,
     },
     total=False,
 )
 
+AccessLogOutputTypeDef = TypedDict(
+    "AccessLogOutputTypeDef",
+    {
+        "file": FileAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
+VirtualGatewayAccessLogOutputTypeDef = TypedDict(
+    "VirtualGatewayAccessLogOutputTypeDef",
+    {
+        "file": VirtualGatewayFileAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
 AccessLogTypeDef = TypedDict(
     "AccessLogTypeDef",
     {
         "file": FileAccessLogTypeDef,
     },
     total=False,
 )
@@ -2284,14 +2828,25 @@
     "VirtualGatewayAccessLogTypeDef",
     {
         "file": VirtualGatewayFileAccessLogTypeDef,
     },
     total=False,
 )
 
+VirtualRouterDataTypeDef = TypedDict(
+    "VirtualRouterDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualRouterSpecOutputTypeDef,
+        "status": VirtualRouterStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2302,19 +2857,21 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateVirtualRouterInputRequestTypeDef(
     _RequiredCreateVirtualRouterInputRequestTypeDef, _OptionalCreateVirtualRouterInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateVirtualRouterInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualRouterInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualRouterSpecTypeDef,
         "virtualRouterName": str,
     },
@@ -2324,62 +2881,76 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class UpdateVirtualRouterInputRequestTypeDef(
     _RequiredUpdateVirtualRouterInputRequestTypeDef, _OptionalUpdateVirtualRouterInputRequestTypeDef
 ):
     pass
 
-VirtualRouterDataTypeDef = TypedDict(
-    "VirtualRouterDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualRouterSpecTypeDef,
-        "status": VirtualRouterStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
 
+VirtualRouterSpecUnionTypeDef = Union[VirtualRouterSpecTypeDef, VirtualRouterSpecOutputTypeDef]
 CreateMeshOutputTypeDef = TypedDict(
     "CreateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteMeshOutputTypeDef = TypedDict(
     "DeleteMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMeshOutputTypeDef = TypedDict(
     "DescribeMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMeshOutputTypeDef = TypedDict(
     "UpdateMeshOutputTypeDef",
     {
         "mesh": MeshDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListenerTlsOutputTypeDef = TypedDict(
+    "_RequiredListenerTlsOutputTypeDef",
+    {
+        "certificate": ListenerTlsCertificateTypeDef,
+        "mode": ListenerTlsModeType,
+    },
+)
+_OptionalListenerTlsOutputTypeDef = TypedDict(
+    "_OptionalListenerTlsOutputTypeDef",
+    {
+        "validation": ListenerTlsValidationContextOutputTypeDef,
     },
+    total=False,
 )
 
+
+class ListenerTlsOutputTypeDef(
+    _RequiredListenerTlsOutputTypeDef, _OptionalListenerTlsOutputTypeDef
+):
+    pass
+
+
 _RequiredListenerTlsTypeDef = TypedDict(
     "_RequiredListenerTlsTypeDef",
     {
         "certificate": ListenerTlsCertificateTypeDef,
         "mode": ListenerTlsModeType,
     },
 )
@@ -2387,17 +2958,42 @@
     "_OptionalListenerTlsTypeDef",
     {
         "validation": ListenerTlsValidationContextTypeDef,
     },
     total=False,
 )
 
+
 class ListenerTlsTypeDef(_RequiredListenerTlsTypeDef, _OptionalListenerTlsTypeDef):
     pass
 
+
+_RequiredClientPolicyTlsOutputTypeDef = TypedDict(
+    "_RequiredClientPolicyTlsOutputTypeDef",
+    {
+        "validation": TlsValidationContextOutputTypeDef,
+    },
+)
+_OptionalClientPolicyTlsOutputTypeDef = TypedDict(
+    "_OptionalClientPolicyTlsOutputTypeDef",
+    {
+        "certificate": ClientTlsCertificateTypeDef,
+        "enforce": bool,
+        "ports": List[int],
+    },
+    total=False,
+)
+
+
+class ClientPolicyTlsOutputTypeDef(
+    _RequiredClientPolicyTlsOutputTypeDef, _OptionalClientPolicyTlsOutputTypeDef
+):
+    pass
+
+
 _RequiredClientPolicyTlsTypeDef = TypedDict(
     "_RequiredClientPolicyTlsTypeDef",
     {
         "validation": TlsValidationContextTypeDef,
     },
 )
 _OptionalClientPolicyTlsTypeDef = TypedDict(
@@ -2406,17 +3002,41 @@
         "certificate": ClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": Sequence[int],
     },
     total=False,
 )
 
+
 class ClientPolicyTlsTypeDef(_RequiredClientPolicyTlsTypeDef, _OptionalClientPolicyTlsTypeDef):
     pass
 
+
+_RequiredVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerTlsOutputTypeDef",
+    {
+        "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
+        "mode": VirtualGatewayListenerTlsModeType,
+    },
+)
+_OptionalVirtualGatewayListenerTlsOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerTlsOutputTypeDef",
+    {
+        "validation": VirtualGatewayListenerTlsValidationContextOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualGatewayListenerTlsOutputTypeDef(
+    _RequiredVirtualGatewayListenerTlsOutputTypeDef, _OptionalVirtualGatewayListenerTlsOutputTypeDef
+):
+    pass
+
+
 _RequiredVirtualGatewayListenerTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTlsTypeDef",
     {
         "certificate": VirtualGatewayListenerTlsCertificateTypeDef,
         "mode": VirtualGatewayListenerTlsModeType,
     },
 )
@@ -2424,19 +3044,45 @@
     "_OptionalVirtualGatewayListenerTlsTypeDef",
     {
         "validation": VirtualGatewayListenerTlsValidationContextTypeDef,
     },
     total=False,
 )
 
+
 class VirtualGatewayListenerTlsTypeDef(
     _RequiredVirtualGatewayListenerTlsTypeDef, _OptionalVirtualGatewayListenerTlsTypeDef
 ):
     pass
 
+
+_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayClientPolicyTlsOutputTypeDef",
+    {
+        "validation": VirtualGatewayTlsValidationContextOutputTypeDef,
+    },
+)
+_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayClientPolicyTlsOutputTypeDef",
+    {
+        "certificate": VirtualGatewayClientTlsCertificateTypeDef,
+        "enforce": bool,
+        "ports": List[int],
+    },
+    total=False,
+)
+
+
+class VirtualGatewayClientPolicyTlsOutputTypeDef(
+    _RequiredVirtualGatewayClientPolicyTlsOutputTypeDef,
+    _OptionalVirtualGatewayClientPolicyTlsOutputTypeDef,
+):
+    pass
+
+
 _RequiredVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
     "_RequiredVirtualGatewayClientPolicyTlsTypeDef",
     {
         "validation": VirtualGatewayTlsValidationContextTypeDef,
     },
 )
 _OptionalVirtualGatewayClientPolicyTlsTypeDef = TypedDict(
@@ -2445,19 +3091,21 @@
         "certificate": VirtualGatewayClientTlsCertificateTypeDef,
         "enforce": bool,
         "ports": Sequence[int],
     },
     total=False,
 )
 
+
 class VirtualGatewayClientPolicyTlsTypeDef(
     _RequiredVirtualGatewayClientPolicyTlsTypeDef, _OptionalVirtualGatewayClientPolicyTlsTypeDef
 ):
     pass
 
+
 _RequiredCreateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -2468,20 +3116,22 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateVirtualServiceInputRequestTypeDef(
     _RequiredCreateVirtualServiceInputRequestTypeDef,
     _OptionalCreateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateVirtualServiceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualServiceInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualServiceSpecTypeDef,
         "virtualServiceName": str,
     },
@@ -2491,39 +3141,70 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class UpdateVirtualServiceInputRequestTypeDef(
     _RequiredUpdateVirtualServiceInputRequestTypeDef,
     _OptionalUpdateVirtualServiceInputRequestTypeDef,
 ):
     pass
 
+
 VirtualServiceDataTypeDef = TypedDict(
     "VirtualServiceDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
         "spec": VirtualServiceSpecTypeDef,
         "status": VirtualServiceStatusTypeDef,
         "virtualServiceName": str,
     },
 )
 
+GrpcGatewayRouteOutputTypeDef = TypedDict(
+    "GrpcGatewayRouteOutputTypeDef",
+    {
+        "action": GrpcGatewayRouteActionTypeDef,
+        "match": GrpcGatewayRouteMatchOutputTypeDef,
+    },
+)
+
 GrpcGatewayRouteTypeDef = TypedDict(
     "GrpcGatewayRouteTypeDef",
     {
         "action": GrpcGatewayRouteActionTypeDef,
         "match": GrpcGatewayRouteMatchTypeDef,
     },
 )
 
+_RequiredGrpcRouteOutputTypeDef = TypedDict(
+    "_RequiredGrpcRouteOutputTypeDef",
+    {
+        "action": GrpcRouteActionOutputTypeDef,
+        "match": GrpcRouteMatchOutputTypeDef,
+    },
+)
+_OptionalGrpcRouteOutputTypeDef = TypedDict(
+    "_OptionalGrpcRouteOutputTypeDef",
+    {
+        "retryPolicy": GrpcRetryPolicyOutputTypeDef,
+        "timeout": GrpcTimeoutTypeDef,
+    },
+    total=False,
+)
+
+
+class GrpcRouteOutputTypeDef(_RequiredGrpcRouteOutputTypeDef, _OptionalGrpcRouteOutputTypeDef):
+    pass
+
+
 _RequiredGrpcRouteTypeDef = TypedDict(
     "_RequiredGrpcRouteTypeDef",
     {
         "action": GrpcRouteActionTypeDef,
         "match": GrpcRouteMatchTypeDef,
     },
 )
@@ -2532,25 +3213,56 @@
     {
         "retryPolicy": GrpcRetryPolicyTypeDef,
         "timeout": GrpcTimeoutTypeDef,
     },
     total=False,
 )
 
+
 class GrpcRouteTypeDef(_RequiredGrpcRouteTypeDef, _OptionalGrpcRouteTypeDef):
     pass
 
+
+HttpGatewayRouteOutputTypeDef = TypedDict(
+    "HttpGatewayRouteOutputTypeDef",
+    {
+        "action": HttpGatewayRouteActionTypeDef,
+        "match": HttpGatewayRouteMatchOutputTypeDef,
+    },
+)
+
 HttpGatewayRouteTypeDef = TypedDict(
     "HttpGatewayRouteTypeDef",
     {
         "action": HttpGatewayRouteActionTypeDef,
         "match": HttpGatewayRouteMatchTypeDef,
     },
 )
 
+_RequiredHttpRouteOutputTypeDef = TypedDict(
+    "_RequiredHttpRouteOutputTypeDef",
+    {
+        "action": HttpRouteActionOutputTypeDef,
+        "match": HttpRouteMatchOutputTypeDef,
+    },
+)
+_OptionalHttpRouteOutputTypeDef = TypedDict(
+    "_OptionalHttpRouteOutputTypeDef",
+    {
+        "retryPolicy": HttpRetryPolicyOutputTypeDef,
+        "timeout": HttpTimeoutTypeDef,
+    },
+    total=False,
+)
+
+
+class HttpRouteOutputTypeDef(_RequiredHttpRouteOutputTypeDef, _OptionalHttpRouteOutputTypeDef):
+    pass
+
+
 _RequiredHttpRouteTypeDef = TypedDict(
     "_RequiredHttpRouteTypeDef",
     {
         "action": HttpRouteActionTypeDef,
         "match": HttpRouteMatchTypeDef,
     },
 )
@@ -2559,17 +3271,35 @@
     {
         "retryPolicy": HttpRetryPolicyTypeDef,
         "timeout": HttpTimeoutTypeDef,
     },
     total=False,
 )
 
+
 class HttpRouteTypeDef(_RequiredHttpRouteTypeDef, _OptionalHttpRouteTypeDef):
     pass
 
+
+LoggingOutputTypeDef = TypedDict(
+    "LoggingOutputTypeDef",
+    {
+        "accessLog": AccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
+VirtualGatewayLoggingOutputTypeDef = TypedDict(
+    "VirtualGatewayLoggingOutputTypeDef",
+    {
+        "accessLog": VirtualGatewayAccessLogOutputTypeDef,
+    },
+    total=False,
+)
+
 LoggingTypeDef = TypedDict(
     "LoggingTypeDef",
     {
         "accessLog": AccessLogTypeDef,
     },
     total=False,
 )
@@ -2582,42 +3312,65 @@
     total=False,
 )
 
 CreateVirtualRouterOutputTypeDef = TypedDict(
     "CreateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualRouterOutputTypeDef = TypedDict(
     "DeleteVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualRouterOutputTypeDef = TypedDict(
     "DescribeVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualRouterOutputTypeDef = TypedDict(
     "UpdateVirtualRouterOutputTypeDef",
     {
         "virtualRouter": VirtualRouterDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListenerOutputTypeDef = TypedDict(
+    "_RequiredListenerOutputTypeDef",
+    {
+        "portMapping": PortMappingTypeDef,
+    },
+)
+_OptionalListenerOutputTypeDef = TypedDict(
+    "_OptionalListenerOutputTypeDef",
+    {
+        "connectionPool": VirtualNodeConnectionPoolTypeDef,
+        "healthCheck": HealthCheckPolicyTypeDef,
+        "outlierDetection": OutlierDetectionTypeDef,
+        "timeout": ListenerTimeoutTypeDef,
+        "tls": ListenerTlsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ListenerOutputTypeDef(_RequiredListenerOutputTypeDef, _OptionalListenerOutputTypeDef):
+    pass
+
+
 _RequiredListenerTypeDef = TypedDict(
     "_RequiredListenerTypeDef",
     {
         "portMapping": PortMappingTypeDef,
     },
 )
 _OptionalListenerTypeDef = TypedDict(
@@ -2628,25 +3381,58 @@
         "outlierDetection": OutlierDetectionTypeDef,
         "timeout": ListenerTimeoutTypeDef,
         "tls": ListenerTlsTypeDef,
     },
     total=False,
 )
 
+
 class ListenerTypeDef(_RequiredListenerTypeDef, _OptionalListenerTypeDef):
     pass
 
+
+ClientPolicyOutputTypeDef = TypedDict(
+    "ClientPolicyOutputTypeDef",
+    {
+        "tls": ClientPolicyTlsOutputTypeDef,
+    },
+    total=False,
+)
+
 ClientPolicyTypeDef = TypedDict(
     "ClientPolicyTypeDef",
     {
         "tls": ClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
+_RequiredVirtualGatewayListenerOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewayListenerOutputTypeDef",
+    {
+        "portMapping": VirtualGatewayPortMappingTypeDef,
+    },
+)
+_OptionalVirtualGatewayListenerOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewayListenerOutputTypeDef",
+    {
+        "connectionPool": VirtualGatewayConnectionPoolTypeDef,
+        "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
+        "tls": VirtualGatewayListenerTlsOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualGatewayListenerOutputTypeDef(
+    _RequiredVirtualGatewayListenerOutputTypeDef, _OptionalVirtualGatewayListenerOutputTypeDef
+):
+    pass
+
+
 _RequiredVirtualGatewayListenerTypeDef = TypedDict(
     "_RequiredVirtualGatewayListenerTypeDef",
     {
         "portMapping": VirtualGatewayPortMappingTypeDef,
     },
 )
 _OptionalVirtualGatewayListenerTypeDef = TypedDict(
@@ -2655,82 +3441,144 @@
         "connectionPool": VirtualGatewayConnectionPoolTypeDef,
         "healthCheck": VirtualGatewayHealthCheckPolicyTypeDef,
         "tls": VirtualGatewayListenerTlsTypeDef,
     },
     total=False,
 )
 
+
 class VirtualGatewayListenerTypeDef(
     _RequiredVirtualGatewayListenerTypeDef, _OptionalVirtualGatewayListenerTypeDef
 ):
     pass
 
+
+VirtualGatewayClientPolicyOutputTypeDef = TypedDict(
+    "VirtualGatewayClientPolicyOutputTypeDef",
+    {
+        "tls": VirtualGatewayClientPolicyTlsOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayClientPolicyTypeDef = TypedDict(
     "VirtualGatewayClientPolicyTypeDef",
     {
         "tls": VirtualGatewayClientPolicyTlsTypeDef,
     },
     total=False,
 )
 
 CreateVirtualServiceOutputTypeDef = TypedDict(
     "CreateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualServiceOutputTypeDef = TypedDict(
     "DeleteVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualServiceOutputTypeDef = TypedDict(
     "DescribeVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualServiceOutputTypeDef = TypedDict(
     "UpdateVirtualServiceOutputTypeDef",
     {
         "virtualService": VirtualServiceDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GatewayRouteSpecOutputTypeDef = TypedDict(
+    "GatewayRouteSpecOutputTypeDef",
+    {
+        "grpcRoute": GrpcGatewayRouteOutputTypeDef,
+        "http2Route": HttpGatewayRouteOutputTypeDef,
+        "httpRoute": HttpGatewayRouteOutputTypeDef,
+        "priority": int,
+    },
+    total=False,
+)
+
 GatewayRouteSpecTypeDef = TypedDict(
     "GatewayRouteSpecTypeDef",
     {
         "grpcRoute": GrpcGatewayRouteTypeDef,
         "http2Route": HttpGatewayRouteTypeDef,
         "httpRoute": HttpGatewayRouteTypeDef,
         "priority": int,
     },
     total=False,
 )
 
+RouteSpecOutputTypeDef = TypedDict(
+    "RouteSpecOutputTypeDef",
+    {
+        "grpcRoute": GrpcRouteOutputTypeDef,
+        "http2Route": HttpRouteOutputTypeDef,
+        "httpRoute": HttpRouteOutputTypeDef,
+        "priority": int,
+        "tcpRoute": TcpRouteOutputTypeDef,
+    },
+    total=False,
+)
+
 RouteSpecTypeDef = TypedDict(
     "RouteSpecTypeDef",
     {
         "grpcRoute": GrpcRouteTypeDef,
         "http2Route": HttpRouteTypeDef,
         "httpRoute": HttpRouteTypeDef,
         "priority": int,
         "tcpRoute": TcpRouteTypeDef,
     },
     total=False,
 )
 
+BackendDefaultsOutputTypeDef = TypedDict(
+    "BackendDefaultsOutputTypeDef",
+    {
+        "clientPolicy": ClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+_RequiredVirtualServiceBackendOutputTypeDef = TypedDict(
+    "_RequiredVirtualServiceBackendOutputTypeDef",
+    {
+        "virtualServiceName": str,
+    },
+)
+_OptionalVirtualServiceBackendOutputTypeDef = TypedDict(
+    "_OptionalVirtualServiceBackendOutputTypeDef",
+    {
+        "clientPolicy": ClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualServiceBackendOutputTypeDef(
+    _RequiredVirtualServiceBackendOutputTypeDef, _OptionalVirtualServiceBackendOutputTypeDef
+):
+    pass
+
+
 BackendDefaultsTypeDef = TypedDict(
     "BackendDefaultsTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
@@ -2745,27 +3593,49 @@
     "_OptionalVirtualServiceBackendTypeDef",
     {
         "clientPolicy": ClientPolicyTypeDef,
     },
     total=False,
 )
 
+
 class VirtualServiceBackendTypeDef(
     _RequiredVirtualServiceBackendTypeDef, _OptionalVirtualServiceBackendTypeDef
 ):
     pass
 
+
+VirtualGatewayBackendDefaultsOutputTypeDef = TypedDict(
+    "VirtualGatewayBackendDefaultsOutputTypeDef",
+    {
+        "clientPolicy": VirtualGatewayClientPolicyOutputTypeDef,
+    },
+    total=False,
+)
+
 VirtualGatewayBackendDefaultsTypeDef = TypedDict(
     "VirtualGatewayBackendDefaultsTypeDef",
     {
         "clientPolicy": VirtualGatewayClientPolicyTypeDef,
     },
     total=False,
 )
 
+GatewayRouteDataTypeDef = TypedDict(
+    "GatewayRouteDataTypeDef",
+    {
+        "gatewayRouteName": str,
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": GatewayRouteSpecOutputTypeDef,
+        "status": GatewayRouteStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredCreateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -2777,31 +3647,22 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateGatewayRouteInputRequestTypeDef(
     _RequiredCreateGatewayRouteInputRequestTypeDef, _OptionalCreateGatewayRouteInputRequestTypeDef
 ):
     pass
 
-GatewayRouteDataTypeDef = TypedDict(
-    "GatewayRouteDataTypeDef",
-    {
-        "gatewayRouteName": str,
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": GatewayRouteSpecTypeDef,
-        "status": GatewayRouteStatusTypeDef,
-        "virtualGatewayName": str,
-    },
-)
 
+GatewayRouteSpecUnionTypeDef = Union[GatewayRouteSpecTypeDef, GatewayRouteSpecOutputTypeDef]
 _RequiredUpdateGatewayRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateGatewayRouteInputRequestTypeDef",
     {
         "gatewayRouteName": str,
         "meshName": str,
         "spec": GatewayRouteSpecTypeDef,
         "virtualGatewayName": str,
@@ -2812,19 +3673,33 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class UpdateGatewayRouteInputRequestTypeDef(
     _RequiredUpdateGatewayRouteInputRequestTypeDef, _OptionalUpdateGatewayRouteInputRequestTypeDef
 ):
     pass
 
+
+RouteDataTypeDef = TypedDict(
+    "RouteDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "routeName": str,
+        "spec": RouteSpecOutputTypeDef,
+        "status": RouteStatusTypeDef,
+        "virtualRouterName": str,
+    },
+)
+
 _RequiredCreateRouteInputRequestTypeDef = TypedDict(
     "_RequiredCreateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -2836,31 +3711,22 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateRouteInputRequestTypeDef(
     _RequiredCreateRouteInputRequestTypeDef, _OptionalCreateRouteInputRequestTypeDef
 ):
     pass
 
-RouteDataTypeDef = TypedDict(
-    "RouteDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "routeName": str,
-        "spec": RouteSpecTypeDef,
-        "status": RouteStatusTypeDef,
-        "virtualRouterName": str,
-    },
-)
 
+RouteSpecUnionTypeDef = Union[RouteSpecTypeDef, RouteSpecOutputTypeDef]
 _RequiredUpdateRouteInputRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteInputRequestTypeDef",
     {
         "meshName": str,
         "routeName": str,
         "spec": RouteSpecTypeDef,
         "virtualRouterName": str,
@@ -2871,27 +3737,59 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class UpdateRouteInputRequestTypeDef(
     _RequiredUpdateRouteInputRequestTypeDef, _OptionalUpdateRouteInputRequestTypeDef
 ):
     pass
 
+
+BackendOutputTypeDef = TypedDict(
+    "BackendOutputTypeDef",
+    {
+        "virtualService": VirtualServiceBackendOutputTypeDef,
+    },
+    total=False,
+)
+
 BackendTypeDef = TypedDict(
     "BackendTypeDef",
     {
         "virtualService": VirtualServiceBackendTypeDef,
     },
     total=False,
 )
 
+_RequiredVirtualGatewaySpecOutputTypeDef = TypedDict(
+    "_RequiredVirtualGatewaySpecOutputTypeDef",
+    {
+        "listeners": List[VirtualGatewayListenerOutputTypeDef],
+    },
+)
+_OptionalVirtualGatewaySpecOutputTypeDef = TypedDict(
+    "_OptionalVirtualGatewaySpecOutputTypeDef",
+    {
+        "backendDefaults": VirtualGatewayBackendDefaultsOutputTypeDef,
+        "logging": VirtualGatewayLoggingOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class VirtualGatewaySpecOutputTypeDef(
+    _RequiredVirtualGatewaySpecOutputTypeDef, _OptionalVirtualGatewaySpecOutputTypeDef
+):
+    pass
+
+
 _RequiredVirtualGatewaySpecTypeDef = TypedDict(
     "_RequiredVirtualGatewaySpecTypeDef",
     {
         "listeners": Sequence[VirtualGatewayListenerTypeDef],
     },
 )
 _OptionalVirtualGatewaySpecTypeDef = TypedDict(
@@ -2899,95 +3797,120 @@
     {
         "backendDefaults": VirtualGatewayBackendDefaultsTypeDef,
         "logging": VirtualGatewayLoggingTypeDef,
     },
     total=False,
 )
 
+
 class VirtualGatewaySpecTypeDef(
     _RequiredVirtualGatewaySpecTypeDef, _OptionalVirtualGatewaySpecTypeDef
 ):
     pass
 
+
 CreateGatewayRouteOutputTypeDef = TypedDict(
     "CreateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteGatewayRouteOutputTypeDef = TypedDict(
     "DeleteGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeGatewayRouteOutputTypeDef = TypedDict(
     "DescribeGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGatewayRouteOutputTypeDef = TypedDict(
     "UpdateGatewayRouteOutputTypeDef",
     {
         "gatewayRoute": GatewayRouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteOutputTypeDef = TypedDict(
     "CreateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteRouteOutputTypeDef = TypedDict(
     "DeleteRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRouteOutputTypeDef = TypedDict(
     "DescribeRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteOutputTypeDef = TypedDict(
     "UpdateRouteOutputTypeDef",
     {
         "route": RouteDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VirtualNodeSpecOutputTypeDef = TypedDict(
+    "VirtualNodeSpecOutputTypeDef",
+    {
+        "backendDefaults": BackendDefaultsOutputTypeDef,
+        "backends": List[BackendOutputTypeDef],
+        "listeners": List[ListenerOutputTypeDef],
+        "logging": LoggingOutputTypeDef,
+        "serviceDiscovery": ServiceDiscoveryOutputTypeDef,
     },
+    total=False,
 )
 
 VirtualNodeSpecTypeDef = TypedDict(
     "VirtualNodeSpecTypeDef",
     {
         "backendDefaults": BackendDefaultsTypeDef,
         "backends": Sequence[BackendTypeDef],
         "listeners": Sequence[ListenerTypeDef],
         "logging": LoggingTypeDef,
         "serviceDiscovery": ServiceDiscoveryTypeDef,
     },
     total=False,
 )
 
+VirtualGatewayDataTypeDef = TypedDict(
+    "VirtualGatewayDataTypeDef",
+    {
+        "meshName": str,
+        "metadata": ResourceMetadataTypeDef,
+        "spec": VirtualGatewaySpecOutputTypeDef,
+        "status": VirtualGatewayStatusTypeDef,
+        "virtualGatewayName": str,
+    },
+)
+
 _RequiredCreateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -2998,20 +3921,22 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateVirtualGatewayInputRequestTypeDef(
     _RequiredCreateVirtualGatewayInputRequestTypeDef,
     _OptionalCreateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
+
 _RequiredUpdateVirtualGatewayInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualGatewayInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualGatewaySpecTypeDef,
         "virtualGatewayName": str,
     },
@@ -3021,28 +3946,31 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class UpdateVirtualGatewayInputRequestTypeDef(
     _RequiredUpdateVirtualGatewayInputRequestTypeDef,
     _OptionalUpdateVirtualGatewayInputRequestTypeDef,
 ):
     pass
 
-VirtualGatewayDataTypeDef = TypedDict(
-    "VirtualGatewayDataTypeDef",
+
+VirtualGatewaySpecUnionTypeDef = Union[VirtualGatewaySpecTypeDef, VirtualGatewaySpecOutputTypeDef]
+VirtualNodeDataTypeDef = TypedDict(
+    "VirtualNodeDataTypeDef",
     {
         "meshName": str,
         "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualGatewaySpecTypeDef,
-        "status": VirtualGatewayStatusTypeDef,
-        "virtualGatewayName": str,
+        "spec": VirtualNodeSpecOutputTypeDef,
+        "status": VirtualNodeStatusTypeDef,
+        "virtualNodeName": str,
     },
 )
 
 _RequiredCreateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredCreateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
@@ -3056,19 +3984,21 @@
         "clientToken": str,
         "meshOwner": str,
         "tags": Sequence[TagRefTypeDef],
     },
     total=False,
 )
 
+
 class CreateVirtualNodeInputRequestTypeDef(
     _RequiredCreateVirtualNodeInputRequestTypeDef, _OptionalCreateVirtualNodeInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateVirtualNodeInputRequestTypeDef = TypedDict(
     "_RequiredUpdateVirtualNodeInputRequestTypeDef",
     {
         "meshName": str,
         "spec": VirtualNodeSpecTypeDef,
         "virtualNodeName": str,
     },
@@ -3078,86 +4008,78 @@
     {
         "clientToken": str,
         "meshOwner": str,
     },
     total=False,
 )
 
+
 class UpdateVirtualNodeInputRequestTypeDef(
     _RequiredUpdateVirtualNodeInputRequestTypeDef, _OptionalUpdateVirtualNodeInputRequestTypeDef
 ):
     pass
 
-VirtualNodeDataTypeDef = TypedDict(
-    "VirtualNodeDataTypeDef",
-    {
-        "meshName": str,
-        "metadata": ResourceMetadataTypeDef,
-        "spec": VirtualNodeSpecTypeDef,
-        "status": VirtualNodeStatusTypeDef,
-        "virtualNodeName": str,
-    },
-)
 
+VirtualNodeSpecUnionTypeDef = Union[VirtualNodeSpecTypeDef, VirtualNodeSpecOutputTypeDef]
 CreateVirtualGatewayOutputTypeDef = TypedDict(
     "CreateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualGatewayOutputTypeDef = TypedDict(
     "DeleteVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualGatewayOutputTypeDef = TypedDict(
     "DescribeVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualGatewayOutputTypeDef = TypedDict(
     "UpdateVirtualGatewayOutputTypeDef",
     {
         "virtualGateway": VirtualGatewayDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateVirtualNodeOutputTypeDef = TypedDict(
     "CreateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteVirtualNodeOutputTypeDef = TypedDict(
     "DeleteVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVirtualNodeOutputTypeDef = TypedDict(
     "DescribeVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateVirtualNodeOutputTypeDef = TypedDict(
     "UpdateVirtualNodeOutputTypeDef",
     {
         "virtualNode": VirtualNodeDataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/PKG-INFO` & `types-aiobotocore-appmesh-2.5.2.post1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-appmesh
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppMesh 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appmesh type-annotations boto3-stubs mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appmesh"></a>
 
 # types-aiobotocore-appmesh
 
 [![PyPI - types-aiobotocore-appmesh](https://img.shields.io/pypi/v/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appmesh.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appmesh)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appmesh?color=blue)](https://pypistats.org/packages/types-aiobotocore-appmesh)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appmesh)](https://pepy.tech/project/types-aiobotocore-appmesh)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppMesh 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appmesh.html#AppMesh)
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
 [types-aiobotocore-appmesh docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appmesh/).
 
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
@@ -359,27 +326,28 @@
 )
 
 
 def check_value(value: DefaultGatewayRouteRewriteType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appmesh.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appmesh.type_defs import (
     AwsCloudMapInstanceAttributeTypeDef,
     ListenerTlsFileCertificateTypeDef,
     ListenerTlsSdsCertificateTypeDef,
     TagRefTypeDef,
+    ResponseMetadataTypeDef,
     DeleteGatewayRouteInputRequestTypeDef,
     DeleteMeshInputRequestTypeDef,
     DeleteRouteInputRequestTypeDef,
     DeleteVirtualGatewayInputRequestTypeDef,
     DeleteVirtualNodeInputRequestTypeDef,
     DeleteVirtualRouterInputRequestTypeDef,
     DeleteVirtualServiceInputRequestTypeDef,
@@ -403,209 +371,263 @@
     WeightedTargetTypeDef,
     HealthCheckPolicyTypeDef,
     HttpPathMatchTypeDef,
     HttpGatewayRoutePathRewriteTypeDef,
     HttpGatewayRoutePrefixRewriteTypeDef,
     QueryParameterMatchTypeDef,
     JsonFormatRefTypeDef,
-    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListGatewayRoutesInputRequestTypeDef,
-    ListMeshesInputListMeshesPaginateTypeDef,
     ListMeshesInputRequestTypeDef,
     MeshRefTypeDef,
-    ListRoutesInputListRoutesPaginateTypeDef,
     ListRoutesInputRequestTypeDef,
     RouteRefTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
     ListVirtualGatewaysInputRequestTypeDef,
     VirtualGatewayRefTypeDef,
-    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
     ListVirtualNodesInputRequestTypeDef,
     VirtualNodeRefTypeDef,
-    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
     ListVirtualRoutersInputRequestTypeDef,
     VirtualRouterRefTypeDef,
-    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListVirtualServicesInputRequestTypeDef,
     VirtualServiceRefTypeDef,
+    PortMappingTypeDef,
     ListenerTlsAcmCertificateTypeDef,
     TlsValidationContextFileTrustTypeDef,
     TlsValidationContextSdsTrustTypeDef,
-    PortMappingTypeDef,
     MeshStatusTypeDef,
     MeshServiceDiscoveryTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RouteStatusTypeDef,
+    SubjectAlternativeNameMatchersOutputTypeDef,
     SubjectAlternativeNameMatchersTypeDef,
     TcpRouteMatchTypeDef,
+    TlsValidationContextAcmTrustOutputTypeDef,
     TlsValidationContextAcmTrustTypeDef,
     UntagResourceInputRequestTypeDef,
     VirtualGatewayListenerTlsFileCertificateTypeDef,
     VirtualGatewayListenerTlsSdsCertificateTypeDef,
     VirtualGatewayGrpcConnectionPoolTypeDef,
     VirtualGatewayHttp2ConnectionPoolTypeDef,
     VirtualGatewayHttpConnectionPoolTypeDef,
     VirtualGatewayStatusTypeDef,
     VirtualGatewayHealthCheckPolicyTypeDef,
+    VirtualGatewayPortMappingTypeDef,
     VirtualGatewayListenerTlsAcmCertificateTypeDef,
     VirtualGatewayTlsValidationContextFileTrustTypeDef,
     VirtualGatewayTlsValidationContextSdsTrustTypeDef,
-    VirtualGatewayPortMappingTypeDef,
+    VirtualGatewayTlsValidationContextAcmTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextAcmTrustTypeDef,
     VirtualNodeGrpcConnectionPoolTypeDef,
     VirtualNodeHttp2ConnectionPoolTypeDef,
     VirtualNodeHttpConnectionPoolTypeDef,
     VirtualNodeTcpConnectionPoolTypeDef,
     VirtualNodeStatusTypeDef,
     VirtualNodeServiceProviderTypeDef,
     VirtualRouterStatusTypeDef,
     VirtualRouterServiceProviderTypeDef,
     VirtualServiceStatusTypeDef,
+    AwsCloudMapServiceDiscoveryOutputTypeDef,
     AwsCloudMapServiceDiscoveryTypeDef,
     ClientTlsCertificateTypeDef,
-    ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    GrpcRetryPolicyOutputTypeDef,
     GrpcRetryPolicyTypeDef,
     GrpcTimeoutTypeDef,
+    HttpRetryPolicyOutputTypeDef,
     HttpRetryPolicyTypeDef,
     HttpTimeoutTypeDef,
     OutlierDetectionTypeDef,
     TcpTimeoutTypeDef,
     GrpcGatewayRouteRewriteTypeDef,
     ListGatewayRoutesOutputTypeDef,
     GatewayRouteTargetTypeDef,
     GrpcMetadataMatchMethodTypeDef,
     GrpcRouteMetadataMatchMethodTypeDef,
     HeaderMatchMethodTypeDef,
+    GrpcRouteActionOutputTypeDef,
     GrpcRouteActionTypeDef,
+    HttpRouteActionOutputTypeDef,
     HttpRouteActionTypeDef,
+    TcpRouteActionOutputTypeDef,
     TcpRouteActionTypeDef,
     HttpGatewayRouteRewriteTypeDef,
     HttpQueryParameterTypeDef,
+    LoggingFormatOutputTypeDef,
     LoggingFormatTypeDef,
+    ListGatewayRoutesInputListGatewayRoutesPaginateTypeDef,
+    ListMeshesInputListMeshesPaginateTypeDef,
+    ListRoutesInputListRoutesPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    ListVirtualGatewaysInputListVirtualGatewaysPaginateTypeDef,
+    ListVirtualNodesInputListVirtualNodesPaginateTypeDef,
+    ListVirtualRoutersInputListVirtualRoutersPaginateTypeDef,
+    ListVirtualServicesInputListVirtualServicesPaginateTypeDef,
     ListMeshesOutputTypeDef,
     ListRoutesOutputTypeDef,
     ListVirtualGatewaysOutputTypeDef,
     ListVirtualNodesOutputTypeDef,
     ListVirtualRoutersOutputTypeDef,
     ListVirtualServicesOutputTypeDef,
+    VirtualRouterListenerTypeDef,
     ListenerTlsCertificateTypeDef,
     ListenerTlsValidationContextTrustTypeDef,
-    VirtualRouterListenerTypeDef,
     MeshSpecTypeDef,
+    SubjectAlternativeNamesOutputTypeDef,
     SubjectAlternativeNamesTypeDef,
+    TlsValidationContextTrustOutputTypeDef,
     TlsValidationContextTrustTypeDef,
     VirtualGatewayClientTlsCertificateTypeDef,
     VirtualGatewayConnectionPoolTypeDef,
     VirtualGatewayListenerTlsCertificateTypeDef,
     VirtualGatewayListenerTlsValidationContextTrustTypeDef,
+    VirtualGatewayTlsValidationContextTrustOutputTypeDef,
     VirtualGatewayTlsValidationContextTrustTypeDef,
     VirtualNodeConnectionPoolTypeDef,
     VirtualServiceProviderTypeDef,
+    ServiceDiscoveryOutputTypeDef,
     ServiceDiscoveryTypeDef,
     ListenerTimeoutTypeDef,
     GrpcGatewayRouteActionTypeDef,
     GrpcGatewayRouteMetadataTypeDef,
     GrpcRouteMetadataTypeDef,
     HttpGatewayRouteHeaderTypeDef,
     HttpRouteHeaderTypeDef,
+    TcpRouteOutputTypeDef,
     TcpRouteTypeDef,
     HttpGatewayRouteActionTypeDef,
+    FileAccessLogOutputTypeDef,
+    VirtualGatewayFileAccessLogOutputTypeDef,
     FileAccessLogTypeDef,
     VirtualGatewayFileAccessLogTypeDef,
+    VirtualRouterSpecOutputTypeDef,
     VirtualRouterSpecTypeDef,
     CreateMeshInputRequestTypeDef,
     MeshDataTypeDef,
     UpdateMeshInputRequestTypeDef,
+    ListenerTlsValidationContextOutputTypeDef,
     ListenerTlsValidationContextTypeDef,
+    TlsValidationContextOutputTypeDef,
     TlsValidationContextTypeDef,
+    VirtualGatewayListenerTlsValidationContextOutputTypeDef,
     VirtualGatewayListenerTlsValidationContextTypeDef,
+    VirtualGatewayTlsValidationContextOutputTypeDef,
     VirtualGatewayTlsValidationContextTypeDef,
     VirtualServiceSpecTypeDef,
+    GrpcGatewayRouteMatchOutputTypeDef,
     GrpcGatewayRouteMatchTypeDef,
+    GrpcRouteMatchOutputTypeDef,
     GrpcRouteMatchTypeDef,
+    HttpGatewayRouteMatchOutputTypeDef,
     HttpGatewayRouteMatchTypeDef,
+    HttpRouteMatchOutputTypeDef,
     HttpRouteMatchTypeDef,
+    AccessLogOutputTypeDef,
+    VirtualGatewayAccessLogOutputTypeDef,
     AccessLogTypeDef,
     VirtualGatewayAccessLogTypeDef,
+    VirtualRouterDataTypeDef,
     CreateVirtualRouterInputRequestTypeDef,
     UpdateVirtualRouterInputRequestTypeDef,
-    VirtualRouterDataTypeDef,
+    VirtualRouterSpecUnionTypeDef,
     CreateMeshOutputTypeDef,
     DeleteMeshOutputTypeDef,
     DescribeMeshOutputTypeDef,
     UpdateMeshOutputTypeDef,
+    ListenerTlsOutputTypeDef,
     ListenerTlsTypeDef,
+    ClientPolicyTlsOutputTypeDef,
     ClientPolicyTlsTypeDef,
+    VirtualGatewayListenerTlsOutputTypeDef,
     VirtualGatewayListenerTlsTypeDef,
+    VirtualGatewayClientPolicyTlsOutputTypeDef,
     VirtualGatewayClientPolicyTlsTypeDef,
     CreateVirtualServiceInputRequestTypeDef,
     UpdateVirtualServiceInputRequestTypeDef,
     VirtualServiceDataTypeDef,
+    GrpcGatewayRouteOutputTypeDef,
     GrpcGatewayRouteTypeDef,
+    GrpcRouteOutputTypeDef,
     GrpcRouteTypeDef,
+    HttpGatewayRouteOutputTypeDef,
     HttpGatewayRouteTypeDef,
+    HttpRouteOutputTypeDef,
     HttpRouteTypeDef,
+    LoggingOutputTypeDef,
+    VirtualGatewayLoggingOutputTypeDef,
     LoggingTypeDef,
     VirtualGatewayLoggingTypeDef,
     CreateVirtualRouterOutputTypeDef,
     DeleteVirtualRouterOutputTypeDef,
     DescribeVirtualRouterOutputTypeDef,
     UpdateVirtualRouterOutputTypeDef,
+    ListenerOutputTypeDef,
     ListenerTypeDef,
+    ClientPolicyOutputTypeDef,
     ClientPolicyTypeDef,
+    VirtualGatewayListenerOutputTypeDef,
     VirtualGatewayListenerTypeDef,
+    VirtualGatewayClientPolicyOutputTypeDef,
     VirtualGatewayClientPolicyTypeDef,
     CreateVirtualServiceOutputTypeDef,
     DeleteVirtualServiceOutputTypeDef,
     DescribeVirtualServiceOutputTypeDef,
     UpdateVirtualServiceOutputTypeDef,
+    GatewayRouteSpecOutputTypeDef,
     GatewayRouteSpecTypeDef,
+    RouteSpecOutputTypeDef,
     RouteSpecTypeDef,
+    BackendDefaultsOutputTypeDef,
+    VirtualServiceBackendOutputTypeDef,
     BackendDefaultsTypeDef,
     VirtualServiceBackendTypeDef,
+    VirtualGatewayBackendDefaultsOutputTypeDef,
     VirtualGatewayBackendDefaultsTypeDef,
-    CreateGatewayRouteInputRequestTypeDef,
     GatewayRouteDataTypeDef,
+    CreateGatewayRouteInputRequestTypeDef,
+    GatewayRouteSpecUnionTypeDef,
     UpdateGatewayRouteInputRequestTypeDef,
-    CreateRouteInputRequestTypeDef,
     RouteDataTypeDef,
+    CreateRouteInputRequestTypeDef,
+    RouteSpecUnionTypeDef,
     UpdateRouteInputRequestTypeDef,
+    BackendOutputTypeDef,
     BackendTypeDef,
+    VirtualGatewaySpecOutputTypeDef,
     VirtualGatewaySpecTypeDef,
     CreateGatewayRouteOutputTypeDef,
     DeleteGatewayRouteOutputTypeDef,
     DescribeGatewayRouteOutputTypeDef,
     UpdateGatewayRouteOutputTypeDef,
     CreateRouteOutputTypeDef,
     DeleteRouteOutputTypeDef,
     DescribeRouteOutputTypeDef,
     UpdateRouteOutputTypeDef,
+    VirtualNodeSpecOutputTypeDef,
     VirtualNodeSpecTypeDef,
+    VirtualGatewayDataTypeDef,
     CreateVirtualGatewayInputRequestTypeDef,
     UpdateVirtualGatewayInputRequestTypeDef,
-    VirtualGatewayDataTypeDef,
+    VirtualGatewaySpecUnionTypeDef,
+    VirtualNodeDataTypeDef,
     CreateVirtualNodeInputRequestTypeDef,
     UpdateVirtualNodeInputRequestTypeDef,
-    VirtualNodeDataTypeDef,
+    VirtualNodeSpecUnionTypeDef,
     CreateVirtualGatewayOutputTypeDef,
     DeleteVirtualGatewayOutputTypeDef,
     DescribeVirtualGatewayOutputTypeDef,
     UpdateVirtualGatewayOutputTypeDef,
     CreateVirtualNodeOutputTypeDef,
     DeleteVirtualNodeOutputTypeDef,
     DescribeVirtualNodeOutputTypeDef,
     UpdateVirtualNodeOutputTypeDef,
 )
 
 
-def get_structure() -> AwsCloudMapInstanceAttributeTypeDef:
+def get_value() -> AwsCloudMapInstanceAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appmesh-2.5.2/types_aiobotocore_appmesh.egg-info/SOURCES.txt` & `types-aiobotocore-appmesh-2.5.2.post1/types_aiobotocore_appmesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*


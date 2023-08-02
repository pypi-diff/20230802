# Comparing `tmp/types-aiobotocore-apigatewayv2-2.5.2.tar.gz` & `tmp/types-aiobotocore-apigatewayv2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigatewayv2-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigatewayv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-apigatewayv2-2.5.2.tar` & `types-aiobotocore-apigatewayv2-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.241650 types-aiobotocore-apigatewayv2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-07-08 01:43:12.241650 types-aiobotocore-apigatewayv2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19271 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.241650 types-aiobotocore-apigatewayv2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.225650 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54790 2023-07-08 01:25:37.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-07-08 01:25:38.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-07-08 01:25:37.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11903 2023-07-08 01:25:37.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11891 2023-07-08 01:25:37.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    75292 2023-07-08 01:25:39.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    75181 2023-07-08 01:25:38.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:36.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.241650 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20856 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19473 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.541660 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54835 2023-08-02 14:33:03.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54744 2023-08-02 14:33:03.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10680 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10678 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11871 2023-08-02 14:33:03.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    76777 2023-08-02 14:33:06.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76667 2023-08-02 14:33:04.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.545660 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21011 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/LICENSE` & `types-aiobotocore-apigatewayv2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/PKG-INFO` & `types-aiobotocore-apigatewayv2-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewayv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore apigatewayv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore apigatewayv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-apigatewayv2"></a>
 
 # types-aiobotocore-apigatewayv2
 
 [![PyPI - types-aiobotocore-apigatewayv2](https://img.shields.io/pypi/v/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigatewayv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigatewayv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApiGatewayV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [types-aiobotocore-apigatewayv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/).
 
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
@@ -354,44 +353,42 @@
 )
 
 
 def check_value(value: AuthorizationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_apigatewayv2.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_apigatewayv2.type_defs import (
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
+    CorsOutputTypeDef,
+    JWTConfigurationOutputTypeDef,
     CorsTypeDef,
-    JWTConfigurationTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
+    JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
-    DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -401,97 +398,92 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
+    CorsUnionTypeDef,
     CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
+    JWTConfigurationUnionTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    CreateDomainNameRequestRequestTypeDef,
-    UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
@@ -513,28 +505,42 @@
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    DomainNameConfigurationTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
+    DomainNameConfigurationUnionTypeDef,
+    CreateDomainNameRequestRequestTypeDef,
+    UpdateDomainNameRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_value() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/README.md` & `types-aiobotocore-apigatewayv2-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-apigatewayv2"></a>
 
 # types-aiobotocore-apigatewayv2
 
 [![PyPI - types-aiobotocore-apigatewayv2](https://img.shields.io/pypi/v/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigatewayv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigatewayv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApiGatewayV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [types-aiobotocore-apigatewayv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/).
 
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
@@ -321,44 +321,42 @@
 )
 
 
 def check_value(value: AuthorizationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_apigatewayv2.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_apigatewayv2.type_defs import (
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
+    CorsOutputTypeDef,
+    JWTConfigurationOutputTypeDef,
     CorsTypeDef,
-    JWTConfigurationTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
+    JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
-    DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -368,97 +366,92 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
+    CorsUnionTypeDef,
     CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
+    JWTConfigurationUnionTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    CreateDomainNameRequestRequestTypeDef,
-    UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
@@ -480,28 +473,42 @@
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    DomainNameConfigurationTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
+    DomainNameConfigurationUnionTypeDef,
+    CreateDomainNameRequestRequestTypeDef,
+    UpdateDomainNameRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_value() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/setup.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigatewayv2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_apigatewayv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with"
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
-    keywords="aiobotocore apigatewayv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore apigatewayv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_apigatewayv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/"
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/__init__.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/__init__.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/__main__.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ApiGatewayV2 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ApiGatewayV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2\nOther"
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

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/client.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,28 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
-    CorsTypeDef,
+    CorsUnionTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
-    DomainNameConfigurationTypeDef,
+    DomainNameConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizerResponseTypeDef,
@@ -83,15 +83,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
-    JWTConfigurationTypeDef,
+    JWTConfigurationUnionTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
@@ -168,15 +168,15 @@
 
     async def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -209,15 +209,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_authorizer)
         """
@@ -232,15 +232,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_deployment)
         """
 
     async def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -856,15 +856,15 @@
         """
 
     async def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -903,15 +903,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...,
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_authorizer)
@@ -927,15 +927,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_deployment)
         """
 
     async def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_domain_name)
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/client.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -40,28 +40,28 @@
     GetModelsPaginator,
     GetRouteResponsesPaginator,
     GetRoutesPaginator,
     GetStagesPaginator,
 )
 from .type_defs import (
     AccessLogSettingsTypeDef,
-    CorsTypeDef,
+    CorsUnionTypeDef,
     CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
     CreateAuthorizerResponseTypeDef,
     CreateDeploymentResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateIntegrationResponseResponseTypeDef,
     CreateIntegrationResultTypeDef,
     CreateModelResponseTypeDef,
     CreateRouteResponseResponseTypeDef,
     CreateRouteResultTypeDef,
     CreateStageResponseTypeDef,
     CreateVpcLinkResponseTypeDef,
-    DomainNameConfigurationTypeDef,
+    DomainNameConfigurationUnionTypeDef,
     EmptyResponseMetadataTypeDef,
     ExportApiResponseTypeDef,
     GetApiMappingResponseTypeDef,
     GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizerResponseTypeDef,
@@ -83,15 +83,15 @@
     GetRoutesResponseTypeDef,
     GetStageResponseTypeDef,
     GetStagesResponseTypeDef,
     GetTagsResponseTypeDef,
     GetVpcLinkResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     ImportApiResponseTypeDef,
-    JWTConfigurationTypeDef,
+    JWTConfigurationUnionTypeDef,
     MutualTlsAuthenticationInputTypeDef,
     ParameterConstraintsTypeDef,
     ReimportApiResponseTypeDef,
     RouteSettingsTypeDef,
     TlsConfigInputTypeDef,
     UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
@@ -161,15 +161,15 @@
         """
     async def create_api(
         self,
         *,
         Name: str,
         ProtocolType: ProtocolTypeType,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
         Tags: Mapping[str, str] = ...,
@@ -200,15 +200,15 @@
         Name: str,
         AuthorizerCredentialsArn: str = ...,
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...
     ) -> CreateAuthorizerResponseTypeDef:
         """
         Creates an Authorizer for an API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_authorizer)
         """
@@ -221,15 +221,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#create_deployment)
         """
     async def create_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...,
         Tags: Mapping[str, str] = ...
     ) -> CreateDomainNameResponseTypeDef:
         """
         Creates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.create_domain_name)
@@ -788,15 +788,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#untag_resource)
         """
     async def update_api(
         self,
         *,
         ApiId: str,
         ApiKeySelectionExpression: str = ...,
-        CorsConfiguration: CorsTypeDef = ...,
+        CorsConfiguration: CorsUnionTypeDef = ...,
         CredentialsArn: str = ...,
         Description: str = ...,
         DisableSchemaValidation: bool = ...,
         DisableExecuteApiEndpoint: bool = ...,
         Name: str = ...,
         RouteKey: str = ...,
         RouteSelectionExpression: str = ...,
@@ -833,15 +833,15 @@
         AuthorizerPayloadFormatVersion: str = ...,
         AuthorizerResultTtlInSeconds: int = ...,
         AuthorizerType: AuthorizerTypeType = ...,
         AuthorizerUri: str = ...,
         EnableSimpleResponses: bool = ...,
         IdentitySource: Sequence[str] = ...,
         IdentityValidationExpression: str = ...,
-        JwtConfiguration: JWTConfigurationTypeDef = ...,
+        JwtConfiguration: JWTConfigurationUnionTypeDef = ...,
         Name: str = ...
     ) -> UpdateAuthorizerResponseTypeDef:
         """
         Updates an Authorizer.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_authorizer)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_authorizer)
@@ -855,15 +855,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_deployment)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_deployment)
         """
     async def update_domain_name(
         self,
         *,
         DomainName: str,
-        DomainNameConfigurations: Sequence[DomainNameConfigurationTypeDef] = ...,
+        DomainNameConfigurations: Sequence[DomainNameConfigurationUnionTypeDef] = ...,
         MutualTlsAuthentication: MutualTlsAuthenticationInputTypeDef = ...
     ) -> UpdateDomainNameResponseTypeDef:
         """
         Updates a domain name.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Client.update_domain_name)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/client/#update_domain_name)
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/literals.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/literals.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/paginator.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,148 +84,148 @@
 class GetApisPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getapispaginator)
         """
 
 
 class GetAuthorizersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getauthorizerspaginator)
         """
 
 
 class GetDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdeploymentspaginator)
         """
 
 
 class GetDomainNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDomainNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdomainnamespaginator)
         """
 
 
 class GetIntegrationResponsesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, IntegrationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, IntegrationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntegrationResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationresponsespaginator)
         """
 
 
 class GetIntegrationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationspaginator)
         """
 
 
 class GetModelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getmodelspaginator)
         """
 
 
 class GetRouteResponsesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getrouteresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, RouteId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, RouteId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRouteResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getrouteresponsespaginator)
         """
 
 
 class GetRoutesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getroutespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getroutespaginator)
         """
 
 
 class GetStagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getstagespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetStagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getstagespaginator)
         """
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/paginator.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -81,139 +81,139 @@
 class GetApisPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getapispaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetApis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getapispaginator)
         """
 
 class GetAuthorizersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getauthorizerspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetAuthorizersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetAuthorizers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getauthorizerspaginator)
         """
 
 class GetDeploymentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdeploymentspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDeploymentsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDeployments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdeploymentspaginator)
         """
 
 class GetDomainNamesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdomainnamespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetDomainNamesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetDomainNames.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getdomainnamespaginator)
         """
 
 class GetIntegrationResponsesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, IntegrationId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, IntegrationId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntegrationResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrationResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationresponsespaginator)
         """
 
 class GetIntegrationsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetIntegrationsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetIntegrations.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getintegrationspaginator)
         """
 
 class GetModelsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getmodelspaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetModelsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetModels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getmodelspaginator)
         """
 
 class GetRouteResponsesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getrouteresponsespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, RouteId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, RouteId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRouteResponsesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRouteResponses.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getrouteresponsespaginator)
         """
 
 class GetRoutesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getroutespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetRoutesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetRoutes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getroutespaginator)
         """
 
 class GetStagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getstagespaginator)
     """
 
     def paginate(
-        self, *, ApiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ApiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetStagesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2.Paginator.GetStages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/paginators/#getstagespaginator)
         """
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/type_defs.py` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_apigatewayv2.type_defs import AccessLogSettingsTypeDef
 
-    data: AccessLogSettingsTypeDef = {...}
+    data: AccessLogSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,37 +39,34 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
+    "CorsOutputTypeDef",
+    "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
-    "JWTConfigurationTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
-    "CreateApiMappingResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
-    "CreateIntegrationResponseResponseTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
-    "CreateModelResponseTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
     "CreateVpcLinkRequestRequestTypeDef",
-    "CreateVpcLinkResponseTypeDef",
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     "DeleteApiMappingRequestRequestTypeDef",
     "DeleteApiRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteCorsConfigurationRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeleteDomainNameRequestRequestTypeDef",
@@ -79,97 +76,92 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "ExportApiRequestRequestTypeDef",
-    "ExportApiResponseTypeDef",
     "GetApiMappingRequestRequestTypeDef",
-    "GetApiMappingResponseTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
-    "GetApisRequestGetApisPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
-    "GetIntegrationResponseResponseTypeDef",
-    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationResponsesRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetIntegrationsRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
-    "GetModelResponseTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
-    "GetModelTemplateResponseTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetRouteResponseRequestRequestTypeDef",
-    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
     "GetRouteResponsesRequestRequestTypeDef",
-    "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetRoutesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
-    "GetTagsResponseTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
-    "GetVpcLinkResponseTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "VpcLinkTypeDef",
     "ImportApiRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ReimportApiRequestRequestTypeDef",
     "ResetAuthorizersCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
-    "UpdateApiMappingResponseTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
-    "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
-    "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelResponseTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
-    "UpdateVpcLinkResponseTypeDef",
-    "GetApiMappingsResponseTypeDef",
     "ApiTypeDef",
+    "AuthorizerTypeDef",
+    "CorsUnionTypeDef",
     "CreateApiRequestRequestTypeDef",
+    "UpdateApiRequestRequestTypeDef",
+    "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateIntegrationResponseResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "CreateVpcLinkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportApiResponseTypeDef",
+    "GetApiMappingResponseTypeDef",
+    "GetApiMappingsResponseTypeDef",
     "GetApiResponseTypeDef",
+    "GetAuthorizerResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "GetIntegrationResponseResponseTypeDef",
+    "GetModelResponseTypeDef",
+    "GetModelTemplateResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "GetVpcLinkResponseTypeDef",
     "ImportApiResponseTypeDef",
     "ReimportApiResponseTypeDef",
-    "UpdateApiRequestRequestTypeDef",
+    "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
-    "AuthorizerTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateDeploymentResponseTypeDef",
+    "UpdateIntegrationResponseResponseTypeDef",
+    "UpdateModelResponseTypeDef",
+    "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "GetAuthorizerResponseTypeDef",
+    "JWTConfigurationUnionTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
-    "CreateDomainNameRequestRequestTypeDef",
-    "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
@@ -191,24 +183,38 @@
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "DomainNameConfigurationTypeDef",
+    "GetApisRequestGetApisPaginateTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
+    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    "GetRoutesRequestGetRoutesPaginateTypeDef",
+    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
+    "DomainNameConfigurationUnionTypeDef",
+    "CreateDomainNameRequestRequestTypeDef",
+    "UpdateDomainNameRequestRequestTypeDef",
 )
 
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
@@ -228,41 +234,52 @@
     {
         "ApiMappingId": str,
         "ApiMappingKey": str,
     },
     total=False,
 )
 
-
 class ApiMappingTypeDef(_RequiredApiMappingTypeDef, _OptionalApiMappingTypeDef):
     pass
 
+CorsOutputTypeDef = TypedDict(
+    "CorsOutputTypeDef",
+    {
+        "AllowCredentials": bool,
+        "AllowHeaders": List[str],
+        "AllowMethods": List[str],
+        "AllowOrigins": List[str],
+        "ExposeHeaders": List[str],
+        "MaxAge": int,
+    },
+    total=False,
+)
+
+JWTConfigurationOutputTypeDef = TypedDict(
+    "JWTConfigurationOutputTypeDef",
+    {
+        "Audience": List[str],
+        "Issuer": str,
+    },
+    total=False,
+)
 
 CorsTypeDef = TypedDict(
     "CorsTypeDef",
     {
         "AllowCredentials": bool,
         "AllowHeaders": Sequence[str],
         "AllowMethods": Sequence[str],
         "AllowOrigins": Sequence[str],
         "ExposeHeaders": Sequence[str],
         "MaxAge": int,
     },
     total=False,
 )
 
-JWTConfigurationTypeDef = TypedDict(
-    "JWTConfigurationTypeDef",
-    {
-        "Audience": Sequence[str],
-        "Issuer": str,
-    },
-    total=False,
-)
-
 _RequiredCreateApiMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiMappingRequestRequestTypeDef",
     {
         "ApiId": str,
         "DomainName": str,
         "Stage": str,
     },
@@ -271,30 +288,37 @@
     "_OptionalCreateApiMappingRequestRequestTypeDef",
     {
         "ApiMappingKey": str,
     },
     total=False,
 )
 
-
 class CreateApiMappingRequestRequestTypeDef(
     _RequiredCreateApiMappingRequestRequestTypeDef, _OptionalCreateApiMappingRequestRequestTypeDef
 ):
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
 
-CreateApiMappingResponseTypeDef = TypedDict(
-    "CreateApiMappingResponseTypeDef",
+JWTConfigurationTypeDef = TypedDict(
+    "JWTConfigurationTypeDef",
     {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Audience": Sequence[str],
+        "Issuer": str,
     },
+    total=False,
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
     },
@@ -304,60 +328,45 @@
     {
         "Description": str,
         "StageName": str,
     },
     total=False,
 )
 
-
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
+MutualTlsAuthenticationInputTypeDef = TypedDict(
+    "MutualTlsAuthenticationInputTypeDef",
     {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TruststoreUri": str,
+        "TruststoreVersion": str,
     },
+    total=False,
 )
 
-DomainNameConfigurationTypeDef = TypedDict(
-    "DomainNameConfigurationTypeDef",
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": Union[datetime, str],
+        "CertificateUploadDate": datetime,
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
-MutualTlsAuthenticationInputTypeDef = TypedDict(
-    "MutualTlsAuthenticationInputTypeDef",
-    {
-        "TruststoreUri": str,
-        "TruststoreVersion": str,
-    },
-    total=False,
-)
-
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -387,35 +396,20 @@
         "ResponseParameters": Mapping[str, str],
         "ResponseTemplates": Mapping[str, str],
         "TemplateSelectionExpression": str,
     },
     total=False,
 )
 
-
 class CreateIntegrationResponseRequestRequestTypeDef(
     _RequiredCreateIntegrationResponseRequestRequestTypeDef,
     _OptionalCreateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-
-CreateIntegrationResponseResponseTypeDef = TypedDict(
-    "CreateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "ServerNameToVerify": str,
     },
     total=False,
 )
@@ -433,33 +427,19 @@
     {
         "ContentType": str,
         "Description": str,
     },
     total=False,
 )
 
-
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "Required": bool,
     },
     total=False,
 )
@@ -488,37 +468,19 @@
     {
         "SecurityGroupIds": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateVpcLinkRequestRequestTypeDef(
     _RequiredCreateVpcLinkRequestRequestTypeDef, _OptionalCreateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-
-CreateVpcLinkResponseTypeDef = TypedDict(
-    "CreateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteAccessLogSettingsRequestRequestTypeDef = TypedDict(
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -652,21 +614,15 @@
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
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
+TimestampTypeDef = Union[datetime, str]
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
         "Specification": Literal["OAS30"],
     },
@@ -677,48 +633,27 @@
         "ExportVersion": str,
         "IncludeExtensions": bool,
         "StageName": str,
     },
     total=False,
 )
 
-
 class ExportApiRequestRequestTypeDef(
     _RequiredExportApiRequestRequestTypeDef, _OptionalExportApiRequestRequestTypeDef
 ):
     pass
 
-
-ExportApiResponseTypeDef = TypedDict(
-    "ExportApiResponseTypeDef",
-    {
-        "body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetApiMappingRequestRequestTypeDef = TypedDict(
     "GetApiMappingRequestRequestTypeDef",
     {
         "ApiMappingId": str,
         "DomainName": str,
     },
 )
 
-GetApiMappingResponseTypeDef = TypedDict(
-    "GetApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetApiMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetApiMappingsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetApiMappingsRequestRequestTypeDef = TypedDict(
@@ -726,32 +661,32 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetApiMappingsRequestRequestTypeDef(
     _RequiredGetApiMappingsRequestRequestTypeDef, _OptionalGetApiMappingsRequestRequestTypeDef
 ):
     pass
 
-
 GetApiRequestRequestTypeDef = TypedDict(
     "GetApiRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 
-GetApisRequestGetApisPaginateTypeDef = TypedDict(
-    "GetApisRequestGetApisPaginateTypeDef",
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
 
 GetApisRequestRequestTypeDef = TypedDict(
     "GetApisRequestRequestTypeDef",
     {
@@ -765,36 +700,14 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
 
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -802,64 +715,27 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetAuthorizersRequestRequestTypeDef(
     _RequiredGetAuthorizersRequestRequestTypeDef, _OptionalGetAuthorizersRequestRequestTypeDef
 ):
     pass
 
-
 GetDeploymentRequestRequestTypeDef = TypedDict(
     "GetDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -867,36 +743,26 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetDeploymentsRequestRequestTypeDef(
     _RequiredGetDeploymentsRequestRequestTypeDef, _OptionalGetDeploymentsRequestRequestTypeDef
 ):
     pass
 
-
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -915,50 +781,14 @@
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
 )
 
-GetIntegrationResponseResponseTypeDef = TypedDict(
-    "GetIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "IntegrationId": str,
-    },
-)
-_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
-    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntegrationResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -967,22 +797,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetIntegrationResponsesRequestRequestTypeDef(
     _RequiredGetIntegrationResponsesRequestRequestTypeDef,
     _OptionalGetIntegrationResponsesRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredIntegrationResponseTypeDef = TypedDict(
     "_RequiredIntegrationResponseTypeDef",
     {
         "IntegrationResponseKey": str,
     },
 )
 _OptionalIntegrationResponseTypeDef = TypedDict(
@@ -993,43 +821,19 @@
         "ResponseParameters": Dict[str, str],
         "ResponseTemplates": Dict[str, str],
         "TemplateSelectionExpression": str,
     },
     total=False,
 )
 
-
 class IntegrationResponseTypeDef(
     _RequiredIntegrationResponseTypeDef, _OptionalIntegrationResponseTypeDef
 ):
     pass
 
-
-_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
-    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetIntegrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetIntegrationsRequestRequestTypeDef = TypedDict(
@@ -1037,79 +841,35 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetIntegrationsRequestRequestTypeDef(
     _RequiredGetIntegrationsRequestRequestTypeDef, _OptionalGetIntegrationsRequestRequestTypeDef
 ):
     pass
 
-
 GetModelRequestRequestTypeDef = TypedDict(
     "GetModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelResponseTypeDef = TypedDict(
-    "GetModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelTemplateRequestRequestTypeDef = TypedDict(
     "GetModelTemplateRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelTemplateResponseTypeDef = TypedDict(
-    "GetModelTemplateResponseTypeDef",
-    {
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1117,21 +877,19 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetModelsRequestRequestTypeDef(
     _RequiredGetModelsRequestRequestTypeDef, _OptionalGetModelsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredModelTypeDef = TypedDict(
     "_RequiredModelTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalModelTypeDef = TypedDict(
@@ -1141,19 +899,17 @@
         "Description": str,
         "ModelId": str,
         "Schema": str,
     },
     total=False,
 )
 
-
 class ModelTypeDef(_RequiredModelTypeDef, _OptionalModelTypeDef):
     pass
 
-
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1163,37 +919,14 @@
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
 )
 
-_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
-    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRouteResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRouteResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1202,43 +935,19 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetRouteResponsesRequestRequestTypeDef(
     _RequiredGetRouteResponsesRequestRequestTypeDef, _OptionalGetRouteResponsesRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetRoutesRequestGetRoutesPaginateTypeDef(
-    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
-    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRoutesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetRoutesRequestRequestTypeDef = TypedDict(
@@ -1246,51 +955,27 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetRoutesRequestRequestTypeDef(
     _RequiredGetRoutesRequestRequestTypeDef, _OptionalGetRoutesRequestRequestTypeDef
 ):
     pass
 
-
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetStagesRequestGetStagesPaginateTypeDef(
-    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
-    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetStagesRequestRequestTypeDef = TypedDict(
     "_RequiredGetStagesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetStagesRequestRequestTypeDef = TypedDict(
@@ -1298,59 +983,33 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetStagesRequestRequestTypeDef(
     _RequiredGetStagesRequestRequestTypeDef, _OptionalGetStagesRequestRequestTypeDef
 ):
     pass
 
-
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 
-GetVpcLinkResponseTypeDef = TypedDict(
-    "GetVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1373,19 +1032,17 @@
         "VpcLinkStatus": VpcLinkStatusType,
         "VpcLinkStatusMessage": str,
         "VpcLinkVersion": Literal["V2"],
     },
     total=False,
 )
 
-
 class VpcLinkTypeDef(_RequiredVpcLinkTypeDef, _OptionalVpcLinkTypeDef):
     pass
 
-
 _RequiredImportApiRequestRequestTypeDef = TypedDict(
     "_RequiredImportApiRequestRequestTypeDef",
     {
         "Body": str,
     },
 )
 _OptionalImportApiRequestRequestTypeDef = TypedDict(
@@ -1393,31 +1050,19 @@
     {
         "Basepath": str,
         "FailOnWarnings": bool,
     },
     total=False,
 )
 
-
 class ImportApiRequestRequestTypeDef(
     _RequiredImportApiRequestRequestTypeDef, _OptionalImportApiRequestRequestTypeDef
 ):
     pass
 
-
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
 _RequiredReimportApiRequestRequestTypeDef = TypedDict(
     "_RequiredReimportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "Body": str,
     },
 )
@@ -1426,61 +1071,46 @@
     {
         "Basepath": str,
         "FailOnWarnings": bool,
     },
     total=False,
 )
 
-
 class ReimportApiRequestRequestTypeDef(
     _RequiredReimportApiRequestRequestTypeDef, _OptionalReimportApiRequestRequestTypeDef
 ):
     pass
 
-
 ResetAuthorizersCacheRequestRequestTypeDef = TypedDict(
     "ResetAuthorizersCacheRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
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
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
-
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1498,32 +1128,19 @@
     {
         "ApiMappingKey": str,
         "Stage": str,
     },
     total=False,
 )
 
-
 class UpdateApiMappingRequestRequestTypeDef(
     _RequiredUpdateApiMappingRequestRequestTypeDef, _OptionalUpdateApiMappingRequestRequestTypeDef
 ):
     pass
 
-
-UpdateApiMappingResponseTypeDef = TypedDict(
-    "UpdateApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
@@ -1531,34 +1148,19 @@
     "_OptionalUpdateDeploymentRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
-
 class UpdateDeploymentRequestRequestTypeDef(
     _RequiredUpdateDeploymentRequestRequestTypeDef, _OptionalUpdateDeploymentRequestRequestTypeDef
 ):
     pass
 
-
-UpdateDeploymentResponseTypeDef = TypedDict(
-    "UpdateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
@@ -1571,35 +1173,20 @@
         "ResponseParameters": Mapping[str, str],
         "ResponseTemplates": Mapping[str, str],
         "TemplateSelectionExpression": str,
     },
     total=False,
 )
 
-
 class UpdateIntegrationResponseRequestRequestTypeDef(
     _RequiredUpdateIntegrationResponseRequestRequestTypeDef,
     _OptionalUpdateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-
-UpdateIntegrationResponseResponseTypeDef = TypedDict(
-    "UpdateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
@@ -1610,79 +1197,38 @@
         "Description": str,
         "Name": str,
         "Schema": str,
     },
     total=False,
 )
 
-
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-
-UpdateModelResponseTypeDef = TypedDict(
-    "UpdateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 _OptionalUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateVpcLinkRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-
-UpdateVpcLinkResponseTypeDef = TypedDict(
-    "UpdateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetApiMappingsResponseTypeDef = TypedDict(
-    "GetApiMappingsResponseTypeDef",
-    {
-        "Items": List[ApiMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredApiTypeDef = TypedDict(
     "_RequiredApiTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
     },
@@ -1690,32 +1236,57 @@
 _OptionalApiTypeDef = TypedDict(
     "_OptionalApiTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
     },
     total=False,
 )
 
-
 class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
     pass
 
+_RequiredAuthorizerTypeDef = TypedDict(
+    "_RequiredAuthorizerTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAuthorizerTypeDef = TypedDict(
+    "_OptionalAuthorizerTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
+    pass
 
+CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
     },
 )
@@ -1733,194 +1304,451 @@
         "Tags": Mapping[str, str],
         "Target": str,
         "Version": str,
     },
     total=False,
 )
 
-
 class CreateApiRequestRequestTypeDef(
     _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
 ):
     pass
 
+_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApiRequestRequestTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApiRequestRequestTypeDef",
+    {
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsTypeDef,
+        "CredentialsArn": str,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "Name": str,
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Target": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+class UpdateApiRequestRequestTypeDef(
+    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
+):
+    pass
+
+CreateApiMappingResponseTypeDef = TypedDict(
+    "CreateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationResponseResponseTypeDef = TypedDict(
+    "CreateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVpcLinkResponseTypeDef = TypedDict(
+    "CreateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
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
+ExportApiResponseTypeDef = TypedDict(
+    "ExportApiResponseTypeDef",
+    {
+        "body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingResponseTypeDef = TypedDict(
+    "GetApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingsResponseTypeDef = TypedDict(
+    "GetApiMappingsResponseTypeDef",
+    {
+        "Items": List[ApiMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizerResponseTypeDef = TypedDict(
+    "GetAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseResponseTypeDef = TypedDict(
+    "GetIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelResponseTypeDef = TypedDict(
+    "GetModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelTemplateResponseTypeDef = TypedDict(
+    "GetModelTemplateResponseTypeDef",
+    {
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVpcLinkResponseTypeDef = TypedDict(
+    "GetVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApiRequestRequestTypeDef",
+UpdateApiMappingResponseTypeDef = TypedDict(
+    "UpdateApiMappingResponseTypeDef",
     {
         "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApiRequestRequestTypeDef",
-    {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
-        "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
-        "Name": str,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Target": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-
-class UpdateApiRequestRequestTypeDef(
-    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
-):
-    pass
-
 
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
     {
         "AuthorizerCredentialsArn": str,
         "AuthorizerId": str,
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateDeploymentResponseTypeDef = TypedDict(
+    "UpdateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
+UpdateIntegrationResponseResponseTypeDef = TypedDict(
+    "UpdateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelResponseTypeDef = TypedDict(
+    "UpdateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+UpdateVpcLinkResponseTypeDef = TypedDict(
+    "UpdateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerType": AuthorizerTypeType,
         "IdentitySource": Sequence[str],
@@ -1937,57 +1765,20 @@
         "EnableSimpleResponses": bool,
         "IdentityValidationExpression": str,
         "JwtConfiguration": JWTConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class CreateAuthorizerRequestRequestTypeDef(
     _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAuthorizerResponseTypeDef = TypedDict(
-    "GetAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+JWTConfigurationUnionTypeDef = Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef]
 _RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
@@ -2004,139 +1795,72 @@
         "IdentityValidationExpression": str,
         "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
     },
     total=False,
 )
 
-
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-
-class CreateDomainNameRequestRequestTypeDef(
-    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
-):
-    pass
-
-
-_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-    },
-    total=False,
-)
-
-
-class UpdateDomainNameRequestRequestTypeDef(
-    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
-):
-    pass
-
-
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDomainNameTypeDef = TypedDict(
     "_RequiredDomainNameTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDomainNameTypeDef = TypedDict(
     "_OptionalDomainNameTypeDef",
     {
         "ApiMappingSelectionExpression": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
     pass
 
-
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2162,21 +1886,19 @@
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigInputTypeDef,
     },
     total=False,
 )
 
-
 class CreateIntegrationRequestRequestTypeDef(
     _RequiredCreateIntegrationRequestRequestTypeDef, _OptionalCreateIntegrationRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -2200,21 +1922,19 @@
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigInputTypeDef,
     },
     total=False,
 )
 
-
 class UpdateIntegrationRequestRequestTypeDef(
     _RequiredUpdateIntegrationRequestRequestTypeDef, _OptionalUpdateIntegrationRequestRequestTypeDef
 ):
     pass
 
-
 CreateIntegrationResultTypeDef = TypedDict(
     "CreateIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ConnectionId": str,
         "ConnectionType": ConnectionTypeType,
         "ContentHandlingStrategy": ContentHandlingStrategyType,
@@ -2230,15 +1950,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationResultTypeDef = TypedDict(
     "GetIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2257,15 +1977,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2311,15 +2031,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2339,21 +2059,19 @@
         "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
-
 class CreateRouteRequestRequestTypeDef(
     _RequiredCreateRouteRequestRequestTypeDef, _OptionalCreateRouteRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredCreateRouteResponseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseKey": str,
     },
@@ -2364,31 +2082,29 @@
         "ModelSelectionExpression": str,
         "ResponseModels": Mapping[str, str],
         "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
     },
     total=False,
 )
 
-
 class CreateRouteResponseRequestRequestTypeDef(
     _RequiredCreateRouteResponseRequestRequestTypeDef,
     _OptionalCreateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
-
 CreateRouteResponseResponseTypeDef = TypedDict(
     "CreateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteResultTypeDef = TypedDict(
     "CreateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2400,27 +2116,27 @@
         "OperationName": str,
         "RequestModels": Dict[str, str],
         "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseResponseTypeDef = TypedDict(
     "GetRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResultTypeDef = TypedDict(
     "GetRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2432,15 +2148,15 @@
         "OperationName": str,
         "RequestModels": Dict[str, str],
         "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRouteResponseTypeDef = TypedDict(
     "_RequiredRouteResponseTypeDef",
     {
         "RouteResponseKey": str,
@@ -2453,19 +2169,17 @@
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
     },
     total=False,
 )
 
-
 class RouteResponseTypeDef(_RequiredRouteResponseTypeDef, _OptionalRouteResponseTypeDef):
     pass
 
-
 _RequiredRouteTypeDef = TypedDict(
     "_RequiredRouteTypeDef",
     {
         "RouteKey": str,
     },
 )
 _OptionalRouteTypeDef = TypedDict(
@@ -2483,19 +2197,17 @@
         "RouteId": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
-
 class RouteTypeDef(_RequiredRouteTypeDef, _OptionalRouteTypeDef):
     pass
 
-
 _RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -2513,21 +2225,19 @@
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
-
 class UpdateRouteRequestRequestTypeDef(
     _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
@@ -2539,31 +2249,29 @@
         "ResponseModels": Mapping[str, str],
         "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
         "RouteResponseKey": str,
     },
     total=False,
 )
 
-
 class UpdateRouteResponseRequestRequestTypeDef(
     _RequiredUpdateRouteResponseRequestRequestTypeDef,
     _OptionalUpdateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
-
 UpdateRouteResponseResponseTypeDef = TypedDict(
     "UpdateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteResultTypeDef = TypedDict(
     "UpdateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2575,15 +2283,15 @@
         "OperationName": str,
         "RequestModels": Dict[str, str],
         "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2602,21 +2310,19 @@
         "RouteSettings": Mapping[str, RouteSettingsTypeDef],
         "StageVariables": Mapping[str, str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
-
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
         "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
@@ -2626,15 +2332,15 @@
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
         "AccessLogSettings": AccessLogSettingsTypeDef,
@@ -2647,15 +2353,15 @@
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStageTypeDef = TypedDict(
     "_RequiredStageTypeDef",
     {
         "StageName": str,
@@ -2677,19 +2383,17 @@
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-
 class StageTypeDef(_RequiredStageTypeDef, _OptionalStageTypeDef):
     pass
 
-
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -2704,21 +2408,19 @@
         "Description": str,
         "RouteSettings": Mapping[str, RouteSettingsTypeDef],
         "StageVariables": Mapping[str, str],
     },
     total=False,
 )
 
-
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
-
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
         "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
@@ -2728,109 +2430,348 @@
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentsResponseTypeDef = TypedDict(
     "GetDeploymentsResponseTypeDef",
     {
         "Items": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DomainNameConfigurationTypeDef = TypedDict(
+    "DomainNameConfigurationTypeDef",
+    {
+        "ApiGatewayDomainName": str,
+        "CertificateArn": str,
+        "CertificateName": str,
+        "CertificateUploadDate": TimestampTypeDef,
+        "DomainNameStatus": DomainNameStatusType,
+        "DomainNameStatusMessage": str,
+        "EndpointType": EndpointTypeType,
+        "HostedZoneId": str,
+        "SecurityPolicy": SecurityPolicyType,
+        "OwnershipVerificationCertificateArn": str,
+    },
+    total=False,
+)
+
+GetApisRequestGetApisPaginateTypeDef = TypedDict(
+    "GetApisRequestGetApisPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
+    pass
+
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+):
+    pass
+
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "IntegrationId": str,
+    },
+)
+_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
+    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
+    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
+    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetRoutesRequestGetRoutesPaginateTypeDef(
+    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
+    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
+):
+    pass
+
+_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetStagesRequestGetStagesPaginateTypeDef(
+    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
+    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
+):
+    pass
+
 GetIntegrationResponsesResponseTypeDef = TypedDict(
     "GetIntegrationResponsesResponseTypeDef",
     {
         "Items": List[IntegrationResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResponseTypeDef = TypedDict(
     "GetModelsResponseTypeDef",
     {
         "Items": List[ModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcLinksResponseTypeDef = TypedDict(
     "GetVpcLinksResponseTypeDef",
     {
         "Items": List[VpcLinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApisResponseTypeDef = TypedDict(
     "GetApisResponseTypeDef",
     {
         "Items": List[ApiTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizersResponseTypeDef = TypedDict(
     "GetAuthorizersResponseTypeDef",
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNamesResponseTypeDef = TypedDict(
     "GetDomainNamesResponseTypeDef",
     {
         "Items": List[DomainNameTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponsesResponseTypeDef = TypedDict(
     "GetRouteResponsesResponseTypeDef",
     {
         "Items": List[RouteResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoutesResponseTypeDef = TypedDict(
     "GetRoutesResponseTypeDef",
     {
         "Items": List[RouteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStagesResponseTypeDef = TypedDict(
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DomainNameConfigurationUnionTypeDef = Union[
+    DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef
+]
+_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateDomainNameRequestRequestTypeDef(
+    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
+):
+    pass
+
+_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
     },
+    total=False,
 )
+
+class UpdateDomainNameRequestRequestTypeDef(
+    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2/type_defs.pyi` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_apigatewayv2.type_defs import AccessLogSettingsTypeDef
 
-    data: AccessLogSettingsTypeDef = {...}
+    data: AccessLogSettingsTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,36 +39,35 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AccessLogSettingsTypeDef",
     "ApiMappingTypeDef",
+    "CorsOutputTypeDef",
+    "JWTConfigurationOutputTypeDef",
     "CorsTypeDef",
-    "JWTConfigurationTypeDef",
     "CreateApiMappingRequestRequestTypeDef",
-    "CreateApiMappingResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "JWTConfigurationTypeDef",
     "CreateDeploymentRequestRequestTypeDef",
-    "CreateDeploymentResponseTypeDef",
-    "DomainNameConfigurationTypeDef",
     "MutualTlsAuthenticationInputTypeDef",
+    "DomainNameConfigurationOutputTypeDef",
     "MutualTlsAuthenticationTypeDef",
     "TlsConfigInputTypeDef",
     "CreateIntegrationResponseRequestRequestTypeDef",
-    "CreateIntegrationResponseResponseTypeDef",
     "TlsConfigTypeDef",
     "CreateModelRequestRequestTypeDef",
-    "CreateModelResponseTypeDef",
     "ParameterConstraintsTypeDef",
     "RouteSettingsTypeDef",
     "CreateVpcLinkRequestRequestTypeDef",
-    "CreateVpcLinkResponseTypeDef",
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     "DeleteApiMappingRequestRequestTypeDef",
     "DeleteApiRequestRequestTypeDef",
     "DeleteAuthorizerRequestRequestTypeDef",
     "DeleteCorsConfigurationRequestRequestTypeDef",
     "DeleteDeploymentRequestRequestTypeDef",
     "DeleteDomainNameRequestRequestTypeDef",
@@ -78,97 +77,92 @@
     "DeleteRouteRequestParameterRequestRequestTypeDef",
     "DeleteRouteRequestRequestTypeDef",
     "DeleteRouteResponseRequestRequestTypeDef",
     "DeleteRouteSettingsRequestRequestTypeDef",
     "DeleteStageRequestRequestTypeDef",
     "DeleteVpcLinkRequestRequestTypeDef",
     "DeploymentTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "TimestampTypeDef",
     "ExportApiRequestRequestTypeDef",
-    "ExportApiResponseTypeDef",
     "GetApiMappingRequestRequestTypeDef",
-    "GetApiMappingResponseTypeDef",
     "GetApiMappingsRequestRequestTypeDef",
     "GetApiRequestRequestTypeDef",
-    "GetApisRequestGetApisPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetApisRequestRequestTypeDef",
     "GetAuthorizerRequestRequestTypeDef",
-    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
     "GetAuthorizersRequestRequestTypeDef",
     "GetDeploymentRequestRequestTypeDef",
-    "GetDeploymentResponseTypeDef",
-    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
     "GetDeploymentsRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
     "GetDomainNamesRequestRequestTypeDef",
     "GetIntegrationRequestRequestTypeDef",
     "GetIntegrationResponseRequestRequestTypeDef",
-    "GetIntegrationResponseResponseTypeDef",
-    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
     "GetIntegrationResponsesRequestRequestTypeDef",
     "IntegrationResponseTypeDef",
-    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
     "GetIntegrationsRequestRequestTypeDef",
     "GetModelRequestRequestTypeDef",
-    "GetModelResponseTypeDef",
     "GetModelTemplateRequestRequestTypeDef",
-    "GetModelTemplateResponseTypeDef",
-    "GetModelsRequestGetModelsPaginateTypeDef",
     "GetModelsRequestRequestTypeDef",
     "ModelTypeDef",
     "GetRouteRequestRequestTypeDef",
     "GetRouteResponseRequestRequestTypeDef",
-    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
     "GetRouteResponsesRequestRequestTypeDef",
-    "GetRoutesRequestGetRoutesPaginateTypeDef",
     "GetRoutesRequestRequestTypeDef",
     "GetStageRequestRequestTypeDef",
-    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetStagesRequestRequestTypeDef",
     "GetTagsRequestRequestTypeDef",
-    "GetTagsResponseTypeDef",
     "GetVpcLinkRequestRequestTypeDef",
-    "GetVpcLinkResponseTypeDef",
     "GetVpcLinksRequestRequestTypeDef",
     "VpcLinkTypeDef",
     "ImportApiRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "ReimportApiRequestRequestTypeDef",
     "ResetAuthorizersCacheRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiMappingRequestRequestTypeDef",
-    "UpdateApiMappingResponseTypeDef",
     "UpdateDeploymentRequestRequestTypeDef",
-    "UpdateDeploymentResponseTypeDef",
     "UpdateIntegrationResponseRequestRequestTypeDef",
-    "UpdateIntegrationResponseResponseTypeDef",
     "UpdateModelRequestRequestTypeDef",
-    "UpdateModelResponseTypeDef",
     "UpdateVpcLinkRequestRequestTypeDef",
-    "UpdateVpcLinkResponseTypeDef",
-    "GetApiMappingsResponseTypeDef",
     "ApiTypeDef",
+    "AuthorizerTypeDef",
+    "CorsUnionTypeDef",
     "CreateApiRequestRequestTypeDef",
+    "UpdateApiRequestRequestTypeDef",
+    "CreateApiMappingResponseTypeDef",
     "CreateApiResponseTypeDef",
+    "CreateAuthorizerResponseTypeDef",
+    "CreateDeploymentResponseTypeDef",
+    "CreateIntegrationResponseResponseTypeDef",
+    "CreateModelResponseTypeDef",
+    "CreateVpcLinkResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportApiResponseTypeDef",
+    "GetApiMappingResponseTypeDef",
+    "GetApiMappingsResponseTypeDef",
     "GetApiResponseTypeDef",
+    "GetAuthorizerResponseTypeDef",
+    "GetDeploymentResponseTypeDef",
+    "GetIntegrationResponseResponseTypeDef",
+    "GetModelResponseTypeDef",
+    "GetModelTemplateResponseTypeDef",
+    "GetTagsResponseTypeDef",
+    "GetVpcLinkResponseTypeDef",
     "ImportApiResponseTypeDef",
     "ReimportApiResponseTypeDef",
-    "UpdateApiRequestRequestTypeDef",
+    "UpdateApiMappingResponseTypeDef",
     "UpdateApiResponseTypeDef",
-    "AuthorizerTypeDef",
+    "UpdateAuthorizerResponseTypeDef",
+    "UpdateDeploymentResponseTypeDef",
+    "UpdateIntegrationResponseResponseTypeDef",
+    "UpdateModelResponseTypeDef",
+    "UpdateVpcLinkResponseTypeDef",
     "CreateAuthorizerRequestRequestTypeDef",
-    "CreateAuthorizerResponseTypeDef",
-    "GetAuthorizerResponseTypeDef",
+    "JWTConfigurationUnionTypeDef",
     "UpdateAuthorizerRequestRequestTypeDef",
-    "UpdateAuthorizerResponseTypeDef",
-    "CreateDomainNameRequestRequestTypeDef",
-    "UpdateDomainNameRequestRequestTypeDef",
     "CreateDomainNameResponseTypeDef",
     "DomainNameTypeDef",
     "GetDomainNameResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateIntegrationRequestRequestTypeDef",
     "UpdateIntegrationRequestRequestTypeDef",
     "CreateIntegrationResultTypeDef",
@@ -190,24 +184,38 @@
     "CreateStageRequestRequestTypeDef",
     "CreateStageResponseTypeDef",
     "GetStageResponseTypeDef",
     "StageTypeDef",
     "UpdateStageRequestRequestTypeDef",
     "UpdateStageResponseTypeDef",
     "GetDeploymentsResponseTypeDef",
+    "DomainNameConfigurationTypeDef",
+    "GetApisRequestGetApisPaginateTypeDef",
+    "GetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    "GetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    "GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    "GetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    "GetModelsRequestGetModelsPaginateTypeDef",
+    "GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    "GetRoutesRequestGetRoutesPaginateTypeDef",
+    "GetStagesRequestGetStagesPaginateTypeDef",
     "GetIntegrationResponsesResponseTypeDef",
     "GetModelsResponseTypeDef",
     "GetVpcLinksResponseTypeDef",
     "GetApisResponseTypeDef",
     "GetAuthorizersResponseTypeDef",
     "GetDomainNamesResponseTypeDef",
     "GetIntegrationsResponseTypeDef",
     "GetRouteResponsesResponseTypeDef",
     "GetRoutesResponseTypeDef",
     "GetStagesResponseTypeDef",
+    "DomainNameConfigurationUnionTypeDef",
+    "CreateDomainNameRequestRequestTypeDef",
+    "UpdateDomainNameRequestRequestTypeDef",
 )
 
 AccessLogSettingsTypeDef = TypedDict(
     "AccessLogSettingsTypeDef",
     {
         "DestinationArn": str,
         "Format": str,
@@ -227,39 +235,54 @@
     {
         "ApiMappingId": str,
         "ApiMappingKey": str,
     },
     total=False,
 )
 
+
 class ApiMappingTypeDef(_RequiredApiMappingTypeDef, _OptionalApiMappingTypeDef):
     pass
 
-CorsTypeDef = TypedDict(
-    "CorsTypeDef",
+
+CorsOutputTypeDef = TypedDict(
+    "CorsOutputTypeDef",
     {
         "AllowCredentials": bool,
-        "AllowHeaders": Sequence[str],
-        "AllowMethods": Sequence[str],
-        "AllowOrigins": Sequence[str],
-        "ExposeHeaders": Sequence[str],
+        "AllowHeaders": List[str],
+        "AllowMethods": List[str],
+        "AllowOrigins": List[str],
+        "ExposeHeaders": List[str],
         "MaxAge": int,
     },
     total=False,
 )
 
-JWTConfigurationTypeDef = TypedDict(
-    "JWTConfigurationTypeDef",
+JWTConfigurationOutputTypeDef = TypedDict(
+    "JWTConfigurationOutputTypeDef",
     {
-        "Audience": Sequence[str],
+        "Audience": List[str],
         "Issuer": str,
     },
     total=False,
 )
 
+CorsTypeDef = TypedDict(
+    "CorsTypeDef",
+    {
+        "AllowCredentials": bool,
+        "AllowHeaders": Sequence[str],
+        "AllowMethods": Sequence[str],
+        "AllowOrigins": Sequence[str],
+        "ExposeHeaders": Sequence[str],
+        "MaxAge": int,
+    },
+    total=False,
+)
+
 _RequiredCreateApiMappingRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiMappingRequestRequestTypeDef",
     {
         "ApiId": str,
         "DomainName": str,
         "Stage": str,
     },
@@ -268,28 +291,39 @@
     "_OptionalCreateApiMappingRequestRequestTypeDef",
     {
         "ApiMappingKey": str,
     },
     total=False,
 )
 
+
 class CreateApiMappingRequestRequestTypeDef(
     _RequiredCreateApiMappingRequestRequestTypeDef, _OptionalCreateApiMappingRequestRequestTypeDef
 ):
     pass
 
-CreateApiMappingResponseTypeDef = TypedDict(
-    "CreateApiMappingResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+JWTConfigurationTypeDef = TypedDict(
+    "JWTConfigurationTypeDef",
+    {
+        "Audience": Sequence[str],
+        "Issuer": str,
     },
+    total=False,
 )
 
 _RequiredCreateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
     },
@@ -299,58 +333,47 @@
     {
         "Description": str,
         "StageName": str,
     },
     total=False,
 )
 
+
 class CreateDeploymentRequestRequestTypeDef(
     _RequiredCreateDeploymentRequestRequestTypeDef, _OptionalCreateDeploymentRequestRequestTypeDef
 ):
     pass
 
-CreateDeploymentResponseTypeDef = TypedDict(
-    "CreateDeploymentResponseTypeDef",
+
+MutualTlsAuthenticationInputTypeDef = TypedDict(
+    "MutualTlsAuthenticationInputTypeDef",
     {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TruststoreUri": str,
+        "TruststoreVersion": str,
     },
+    total=False,
 )
 
-DomainNameConfigurationTypeDef = TypedDict(
-    "DomainNameConfigurationTypeDef",
+DomainNameConfigurationOutputTypeDef = TypedDict(
+    "DomainNameConfigurationOutputTypeDef",
     {
         "ApiGatewayDomainName": str,
         "CertificateArn": str,
         "CertificateName": str,
-        "CertificateUploadDate": Union[datetime, str],
+        "CertificateUploadDate": datetime,
         "DomainNameStatus": DomainNameStatusType,
         "DomainNameStatusMessage": str,
         "EndpointType": EndpointTypeType,
         "HostedZoneId": str,
         "SecurityPolicy": SecurityPolicyType,
         "OwnershipVerificationCertificateArn": str,
     },
     total=False,
 )
 
-MutualTlsAuthenticationInputTypeDef = TypedDict(
-    "MutualTlsAuthenticationInputTypeDef",
-    {
-        "TruststoreUri": str,
-        "TruststoreVersion": str,
-    },
-    total=False,
-)
-
 MutualTlsAuthenticationTypeDef = TypedDict(
     "MutualTlsAuthenticationTypeDef",
     {
         "TruststoreUri": str,
         "TruststoreVersion": str,
         "TruststoreWarnings": List[str],
     },
@@ -380,32 +403,21 @@
         "ResponseParameters": Mapping[str, str],
         "ResponseTemplates": Mapping[str, str],
         "TemplateSelectionExpression": str,
     },
     total=False,
 )
 
+
 class CreateIntegrationResponseRequestRequestTypeDef(
     _RequiredCreateIntegrationResponseRequestRequestTypeDef,
     _OptionalCreateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-CreateIntegrationResponseResponseTypeDef = TypedDict(
-    "CreateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TlsConfigTypeDef = TypedDict(
     "TlsConfigTypeDef",
     {
         "ServerNameToVerify": str,
     },
     total=False,
@@ -424,30 +436,20 @@
     {
         "ContentType": str,
         "Description": str,
     },
     total=False,
 )
 
+
 class CreateModelRequestRequestTypeDef(
     _RequiredCreateModelRequestRequestTypeDef, _OptionalCreateModelRequestRequestTypeDef
 ):
     pass
 
-CreateModelResponseTypeDef = TypedDict(
-    "CreateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "Required": bool,
     },
     total=False,
@@ -477,34 +479,20 @@
     {
         "SecurityGroupIds": Sequence[str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateVpcLinkRequestRequestTypeDef(
     _RequiredCreateVpcLinkRequestRequestTypeDef, _OptionalCreateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-CreateVpcLinkResponseTypeDef = TypedDict(
-    "CreateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteAccessLogSettingsRequestRequestTypeDef = TypedDict(
     "DeleteAccessLogSettingsRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
@@ -639,21 +627,15 @@
         "DeploymentStatus": DeploymentStatusType,
         "DeploymentStatusMessage": str,
         "Description": str,
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
+TimestampTypeDef = Union[datetime, str]
 _RequiredExportApiRequestRequestTypeDef = TypedDict(
     "_RequiredExportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "OutputType": JSONYAMLType,
         "Specification": Literal["OAS30"],
     },
@@ -664,46 +646,29 @@
         "ExportVersion": str,
         "IncludeExtensions": bool,
         "StageName": str,
     },
     total=False,
 )
 
+
 class ExportApiRequestRequestTypeDef(
     _RequiredExportApiRequestRequestTypeDef, _OptionalExportApiRequestRequestTypeDef
 ):
     pass
 
-ExportApiResponseTypeDef = TypedDict(
-    "ExportApiResponseTypeDef",
-    {
-        "body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 GetApiMappingRequestRequestTypeDef = TypedDict(
     "GetApiMappingRequestRequestTypeDef",
     {
         "ApiMappingId": str,
         "DomainName": str,
     },
 )
 
-GetApiMappingResponseTypeDef = TypedDict(
-    "GetApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetApiMappingsRequestRequestTypeDef = TypedDict(
     "_RequiredGetApiMappingsRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalGetApiMappingsRequestRequestTypeDef = TypedDict(
@@ -711,30 +676,34 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetApiMappingsRequestRequestTypeDef(
     _RequiredGetApiMappingsRequestRequestTypeDef, _OptionalGetApiMappingsRequestRequestTypeDef
 ):
     pass
 
+
 GetApiRequestRequestTypeDef = TypedDict(
     "GetApiRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 
-GetApisRequestGetApisPaginateTypeDef = TypedDict(
-    "GetApisRequestGetApisPaginateTypeDef",
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
 
 GetApisRequestRequestTypeDef = TypedDict(
     "GetApisRequestRequestTypeDef",
     {
@@ -748,34 +717,14 @@
     "GetAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
 
-_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
-    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
-    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
-):
-    pass
-
 _RequiredGetAuthorizersRequestRequestTypeDef = TypedDict(
     "_RequiredGetAuthorizersRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetAuthorizersRequestRequestTypeDef = TypedDict(
@@ -783,60 +732,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetAuthorizersRequestRequestTypeDef(
     _RequiredGetAuthorizersRequestRequestTypeDef, _OptionalGetAuthorizersRequestRequestTypeDef
 ):
     pass
 
+
 GetDeploymentRequestRequestTypeDef = TypedDict(
     "GetDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
 )
 
-GetDeploymentResponseTypeDef = TypedDict(
-    "GetDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
-    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
-    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetDeploymentsRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeploymentsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetDeploymentsRequestRequestTypeDef = TypedDict(
@@ -844,34 +762,28 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetDeploymentsRequestRequestTypeDef(
     _RequiredGetDeploymentsRequestRequestTypeDef, _OptionalGetDeploymentsRequestRequestTypeDef
 ):
     pass
 
+
 GetDomainNameRequestRequestTypeDef = TypedDict(
     "GetDomainNameRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
-    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetDomainNamesRequestRequestTypeDef = TypedDict(
     "GetDomainNamesRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -890,48 +802,14 @@
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
     },
 )
 
-GetIntegrationResponseResponseTypeDef = TypedDict(
-    "GetIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "IntegrationId": str,
-    },
-)
-_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
-    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetIntegrationResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -940,20 +818,22 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetIntegrationResponsesRequestRequestTypeDef(
     _RequiredGetIntegrationResponsesRequestRequestTypeDef,
     _OptionalGetIntegrationResponsesRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredIntegrationResponseTypeDef = TypedDict(
     "_RequiredIntegrationResponseTypeDef",
     {
         "IntegrationResponseKey": str,
     },
 )
 _OptionalIntegrationResponseTypeDef = TypedDict(
@@ -964,38 +844,20 @@
         "ResponseParameters": Dict[str, str],
         "ResponseTemplates": Dict[str, str],
         "TemplateSelectionExpression": str,
     },
     total=False,
 )
 
+
 class IntegrationResponseTypeDef(
     _RequiredIntegrationResponseTypeDef, _OptionalIntegrationResponseTypeDef
 ):
     pass
 
-_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
-    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
-    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
-):
-    pass
 
 _RequiredGetIntegrationsRequestRequestTypeDef = TypedDict(
     "_RequiredGetIntegrationsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
@@ -1004,75 +866,37 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetIntegrationsRequestRequestTypeDef(
     _RequiredGetIntegrationsRequestRequestTypeDef, _OptionalGetIntegrationsRequestRequestTypeDef
 ):
     pass
 
+
 GetModelRequestRequestTypeDef = TypedDict(
     "GetModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelResponseTypeDef = TypedDict(
-    "GetModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetModelTemplateRequestRequestTypeDef = TypedDict(
     "GetModelTemplateRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
 )
 
-GetModelTemplateResponseTypeDef = TypedDict(
-    "GetModelTemplateResponseTypeDef",
-    {
-        "Value": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
-    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetModelsRequestGetModelsPaginateTypeDef(
-    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
-    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetModelsRequestRequestTypeDef = TypedDict(
     "_RequiredGetModelsRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetModelsRequestRequestTypeDef = TypedDict(
@@ -1080,19 +904,21 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetModelsRequestRequestTypeDef(
     _RequiredGetModelsRequestRequestTypeDef, _OptionalGetModelsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredModelTypeDef = TypedDict(
     "_RequiredModelTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalModelTypeDef = TypedDict(
@@ -1102,17 +928,19 @@
         "Description": str,
         "ModelId": str,
         "Schema": str,
     },
     total=False,
 )
 
+
 class ModelTypeDef(_RequiredModelTypeDef, _OptionalModelTypeDef):
     pass
 
+
 GetRouteRequestRequestTypeDef = TypedDict(
     "GetRouteRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1122,35 +950,14 @@
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
 )
 
-_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "ApiId": str,
-        "RouteId": str,
-    },
-)
-_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
-    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
-    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetRouteResponsesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRouteResponsesRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -1159,38 +966,20 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetRouteResponsesRequestRequestTypeDef(
     _RequiredGetRouteResponsesRequestRequestTypeDef, _OptionalGetRouteResponsesRequestRequestTypeDef
 ):
     pass
 
-_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
-    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetRoutesRequestGetRoutesPaginateTypeDef(
-    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
-    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
-):
-    pass
 
 _RequiredGetRoutesRequestRequestTypeDef = TypedDict(
     "_RequiredGetRoutesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
@@ -1199,47 +988,29 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetRoutesRequestRequestTypeDef(
     _RequiredGetRoutesRequestRequestTypeDef, _OptionalGetRoutesRequestRequestTypeDef
 ):
     pass
 
+
 GetStageRequestRequestTypeDef = TypedDict(
     "GetStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
 
-_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "ApiId": str,
-    },
-)
-_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
-    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetStagesRequestGetStagesPaginateTypeDef(
-    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
-    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetStagesRequestRequestTypeDef = TypedDict(
     "_RequiredGetStagesRequestRequestTypeDef",
     {
         "ApiId": str,
     },
 )
 _OptionalGetStagesRequestRequestTypeDef = TypedDict(
@@ -1247,57 +1018,35 @@
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetStagesRequestRequestTypeDef(
     _RequiredGetStagesRequestRequestTypeDef, _OptionalGetStagesRequestRequestTypeDef
 ):
     pass
 
+
 GetTagsRequestRequestTypeDef = TypedDict(
     "GetTagsRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetTagsResponseTypeDef = TypedDict(
-    "GetTagsResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinkRequestRequestTypeDef = TypedDict(
     "GetVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
 
-GetVpcLinkResponseTypeDef = TypedDict(
-    "GetVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetVpcLinksRequestRequestTypeDef = TypedDict(
     "GetVpcLinksRequestRequestTypeDef",
     {
         "MaxResults": str,
         "NextToken": str,
     },
     total=False,
@@ -1320,17 +1069,19 @@
         "VpcLinkStatus": VpcLinkStatusType,
         "VpcLinkStatusMessage": str,
         "VpcLinkVersion": Literal["V2"],
     },
     total=False,
 )
 
+
 class VpcLinkTypeDef(_RequiredVpcLinkTypeDef, _OptionalVpcLinkTypeDef):
     pass
 
+
 _RequiredImportApiRequestRequestTypeDef = TypedDict(
     "_RequiredImportApiRequestRequestTypeDef",
     {
         "Body": str,
     },
 )
 _OptionalImportApiRequestRequestTypeDef = TypedDict(
@@ -1338,28 +1089,20 @@
     {
         "Basepath": str,
         "FailOnWarnings": bool,
     },
     total=False,
 )
 
+
 class ImportApiRequestRequestTypeDef(
     _RequiredImportApiRequestRequestTypeDef, _OptionalImportApiRequestRequestTypeDef
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
 
 _RequiredReimportApiRequestRequestTypeDef = TypedDict(
     "_RequiredReimportApiRequestRequestTypeDef",
     {
         "ApiId": str,
         "Body": str,
     },
@@ -1369,57 +1112,50 @@
     {
         "Basepath": str,
         "FailOnWarnings": bool,
     },
     total=False,
 )
 
+
 class ReimportApiRequestRequestTypeDef(
     _RequiredReimportApiRequestRequestTypeDef, _OptionalReimportApiRequestRequestTypeDef
 ):
     pass
 
+
 ResetAuthorizersCacheRequestRequestTypeDef = TypedDict(
     "ResetAuthorizersCacheRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
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
 _RequiredTagResourceRequestRequestTypeDef = TypedDict(
     "_RequiredTagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalTagResourceRequestRequestTypeDef = TypedDict(
     "_OptionalTagResourceRequestRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TagResourceRequestRequestTypeDef(
     _RequiredTagResourceRequestRequestTypeDef, _OptionalTagResourceRequestRequestTypeDef
 ):
     pass
 
+
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1437,29 +1173,20 @@
     {
         "ApiMappingKey": str,
         "Stage": str,
     },
     total=False,
 )
 
+
 class UpdateApiMappingRequestRequestTypeDef(
     _RequiredUpdateApiMappingRequestRequestTypeDef, _OptionalUpdateApiMappingRequestRequestTypeDef
 ):
     pass
 
-UpdateApiMappingResponseTypeDef = TypedDict(
-    "UpdateApiMappingResponseTypeDef",
-    {
-        "ApiId": str,
-        "ApiMappingId": str,
-        "ApiMappingKey": str,
-        "Stage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateDeploymentRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateDeploymentRequestRequestTypeDef",
     {
         "ApiId": str,
         "DeploymentId": str,
     },
@@ -1468,31 +1195,20 @@
     "_OptionalUpdateDeploymentRequestRequestTypeDef",
     {
         "Description": str,
     },
     total=False,
 )
 
+
 class UpdateDeploymentRequestRequestTypeDef(
     _RequiredUpdateDeploymentRequestRequestTypeDef, _OptionalUpdateDeploymentRequestRequestTypeDef
 ):
     pass
 
-UpdateDeploymentResponseTypeDef = TypedDict(
-    "UpdateDeploymentResponseTypeDef",
-    {
-        "AutoDeployed": bool,
-        "CreatedDate": datetime,
-        "DeploymentId": str,
-        "DeploymentStatus": DeploymentStatusType,
-        "DeploymentStatusMessage": str,
-        "Description": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateIntegrationResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
         "IntegrationResponseId": str,
@@ -1506,32 +1222,21 @@
         "ResponseParameters": Mapping[str, str],
         "ResponseTemplates": Mapping[str, str],
         "TemplateSelectionExpression": str,
     },
     total=False,
 )
 
+
 class UpdateIntegrationResponseRequestRequestTypeDef(
     _RequiredUpdateIntegrationResponseRequestRequestTypeDef,
     _OptionalUpdateIntegrationResponseRequestRequestTypeDef,
 ):
     pass
 
-UpdateIntegrationResponseResponseTypeDef = TypedDict(
-    "UpdateIntegrationResponseResponseTypeDef",
-    {
-        "ContentHandlingStrategy": ContentHandlingStrategyType,
-        "IntegrationResponseId": str,
-        "IntegrationResponseKey": str,
-        "ResponseParameters": Dict[str, str],
-        "ResponseTemplates": Dict[str, str],
-        "TemplateSelectionExpression": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateModelRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateModelRequestRequestTypeDef",
     {
         "ApiId": str,
         "ModelId": str,
     },
@@ -1543,30 +1248,20 @@
         "Description": str,
         "Name": str,
         "Schema": str,
     },
     total=False,
 )
 
+
 class UpdateModelRequestRequestTypeDef(
     _RequiredUpdateModelRequestRequestTypeDef, _OptionalUpdateModelRequestRequestTypeDef
 ):
     pass
 
-UpdateModelResponseTypeDef = TypedDict(
-    "UpdateModelResponseTypeDef",
-    {
-        "ContentType": str,
-        "Description": str,
-        "ModelId": str,
-        "Name": str,
-        "Schema": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredUpdateVpcLinkRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateVpcLinkRequestRequestTypeDef",
     {
         "VpcLinkId": str,
     },
 )
@@ -1574,43 +1269,20 @@
     "_OptionalUpdateVpcLinkRequestRequestTypeDef",
     {
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateVpcLinkRequestRequestTypeDef(
     _RequiredUpdateVpcLinkRequestRequestTypeDef, _OptionalUpdateVpcLinkRequestRequestTypeDef
 ):
     pass
 
-UpdateVpcLinkResponseTypeDef = TypedDict(
-    "UpdateVpcLinkResponseTypeDef",
-    {
-        "CreatedDate": datetime,
-        "Name": str,
-        "SecurityGroupIds": List[str],
-        "SubnetIds": List[str],
-        "Tags": Dict[str, str],
-        "VpcLinkId": str,
-        "VpcLinkStatus": VpcLinkStatusType,
-        "VpcLinkStatusMessage": str,
-        "VpcLinkVersion": Literal["V2"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetApiMappingsResponseTypeDef = TypedDict(
-    "GetApiMappingsResponseTypeDef",
-    {
-        "Items": List[ApiMappingTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredApiTypeDef = TypedDict(
     "_RequiredApiTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
@@ -1619,30 +1291,61 @@
 _OptionalApiTypeDef = TypedDict(
     "_OptionalApiTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
     },
     total=False,
 )
 
+
 class ApiTypeDef(_RequiredApiTypeDef, _OptionalApiTypeDef):
     pass
 
+
+_RequiredAuthorizerTypeDef = TypedDict(
+    "_RequiredAuthorizerTypeDef",
+    {
+        "Name": str,
+    },
+)
+_OptionalAuthorizerTypeDef = TypedDict(
+    "_OptionalAuthorizerTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
+    pass
+
+
+CorsUnionTypeDef = Union[CorsTypeDef, CorsOutputTypeDef]
 _RequiredCreateApiRequestRequestTypeDef = TypedDict(
     "_RequiredCreateApiRequestRequestTypeDef",
     {
         "Name": str,
         "ProtocolType": ProtocolTypeType,
     },
 )
@@ -1660,188 +1363,455 @@
         "Tags": Mapping[str, str],
         "Target": str,
         "Version": str,
     },
     total=False,
 )
 
+
 class CreateApiRequestRequestTypeDef(
     _RequiredCreateApiRequestRequestTypeDef, _OptionalCreateApiRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateApiRequestRequestTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateApiRequestRequestTypeDef",
+    {
+        "ApiKeySelectionExpression": str,
+        "CorsConfiguration": CorsTypeDef,
+        "CredentialsArn": str,
+        "Description": str,
+        "DisableSchemaValidation": bool,
+        "DisableExecuteApiEndpoint": bool,
+        "Name": str,
+        "RouteKey": str,
+        "RouteSelectionExpression": str,
+        "Target": str,
+        "Version": str,
+    },
+    total=False,
+)
+
+
+class UpdateApiRequestRequestTypeDef(
+    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
+):
+    pass
+
+
+CreateApiMappingResponseTypeDef = TypedDict(
+    "CreateApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateApiResponseTypeDef = TypedDict(
     "CreateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateAuthorizerResponseTypeDef = TypedDict(
+    "CreateAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDeploymentResponseTypeDef = TypedDict(
+    "CreateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIntegrationResponseResponseTypeDef = TypedDict(
+    "CreateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateModelResponseTypeDef = TypedDict(
+    "CreateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateVpcLinkResponseTypeDef = TypedDict(
+    "CreateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
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
+ExportApiResponseTypeDef = TypedDict(
+    "ExportApiResponseTypeDef",
+    {
+        "body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingResponseTypeDef = TypedDict(
+    "GetApiMappingResponseTypeDef",
+    {
+        "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiMappingsResponseTypeDef = TypedDict(
+    "GetApiMappingsResponseTypeDef",
+    {
+        "Items": List[ApiMappingTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiResponseTypeDef = TypedDict(
     "GetApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAuthorizerResponseTypeDef = TypedDict(
+    "GetAuthorizerResponseTypeDef",
+    {
+        "AuthorizerCredentialsArn": str,
+        "AuthorizerId": str,
+        "AuthorizerPayloadFormatVersion": str,
+        "AuthorizerResultTtlInSeconds": int,
+        "AuthorizerType": AuthorizerTypeType,
+        "AuthorizerUri": str,
+        "EnableSimpleResponses": bool,
+        "IdentitySource": List[str],
+        "IdentityValidationExpression": str,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDeploymentResponseTypeDef = TypedDict(
+    "GetDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIntegrationResponseResponseTypeDef = TypedDict(
+    "GetIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelResponseTypeDef = TypedDict(
+    "GetModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetModelTemplateResponseTypeDef = TypedDict(
+    "GetModelTemplateResponseTypeDef",
+    {
+        "Value": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagsResponseTypeDef = TypedDict(
+    "GetTagsResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetVpcLinkResponseTypeDef = TypedDict(
+    "GetVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ImportApiResponseTypeDef = TypedDict(
     "ImportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReimportApiResponseTypeDef = TypedDict(
     "ReimportApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateApiRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateApiRequestRequestTypeDef",
+UpdateApiMappingResponseTypeDef = TypedDict(
+    "UpdateApiMappingResponseTypeDef",
     {
         "ApiId": str,
+        "ApiMappingId": str,
+        "ApiMappingKey": str,
+        "Stage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateApiRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateApiRequestRequestTypeDef",
-    {
-        "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
-        "CredentialsArn": str,
-        "Description": str,
-        "DisableSchemaValidation": bool,
-        "DisableExecuteApiEndpoint": bool,
-        "Name": str,
-        "RouteKey": str,
-        "RouteSelectionExpression": str,
-        "Target": str,
-        "Version": str,
-    },
-    total=False,
-)
-
-class UpdateApiRequestRequestTypeDef(
-    _RequiredUpdateApiRequestRequestTypeDef, _OptionalUpdateApiRequestRequestTypeDef
-):
-    pass
 
 UpdateApiResponseTypeDef = TypedDict(
     "UpdateApiResponseTypeDef",
     {
         "ApiEndpoint": str,
         "ApiGatewayManaged": bool,
         "ApiId": str,
         "ApiKeySelectionExpression": str,
-        "CorsConfiguration": CorsTypeDef,
+        "CorsConfiguration": CorsOutputTypeDef,
         "CreatedDate": datetime,
         "Description": str,
         "DisableSchemaValidation": bool,
         "DisableExecuteApiEndpoint": bool,
         "ImportInfo": List[str],
         "Name": str,
         "ProtocolType": ProtocolTypeType,
         "RouteSelectionExpression": str,
         "Tags": Dict[str, str],
         "Version": str,
         "Warnings": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredAuthorizerTypeDef = TypedDict(
-    "_RequiredAuthorizerTypeDef",
-    {
-        "Name": str,
-    },
-)
-_OptionalAuthorizerTypeDef = TypedDict(
-    "_OptionalAuthorizerTypeDef",
+UpdateAuthorizerResponseTypeDef = TypedDict(
+    "UpdateAuthorizerResponseTypeDef",
     {
         "AuthorizerCredentialsArn": str,
         "AuthorizerId": str,
         "AuthorizerPayloadFormatVersion": str,
         "AuthorizerResultTtlInSeconds": int,
         "AuthorizerType": AuthorizerTypeType,
         "AuthorizerUri": str,
         "EnableSimpleResponses": bool,
         "IdentitySource": List[str],
         "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
+        "JwtConfiguration": JWTConfigurationOutputTypeDef,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class AuthorizerTypeDef(_RequiredAuthorizerTypeDef, _OptionalAuthorizerTypeDef):
-    pass
+UpdateDeploymentResponseTypeDef = TypedDict(
+    "UpdateDeploymentResponseTypeDef",
+    {
+        "AutoDeployed": bool,
+        "CreatedDate": datetime,
+        "DeploymentId": str,
+        "DeploymentStatus": DeploymentStatusType,
+        "DeploymentStatusMessage": str,
+        "Description": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateIntegrationResponseResponseTypeDef = TypedDict(
+    "UpdateIntegrationResponseResponseTypeDef",
+    {
+        "ContentHandlingStrategy": ContentHandlingStrategyType,
+        "IntegrationResponseId": str,
+        "IntegrationResponseKey": str,
+        "ResponseParameters": Dict[str, str],
+        "ResponseTemplates": Dict[str, str],
+        "TemplateSelectionExpression": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateModelResponseTypeDef = TypedDict(
+    "UpdateModelResponseTypeDef",
+    {
+        "ContentType": str,
+        "Description": str,
+        "ModelId": str,
+        "Name": str,
+        "Schema": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateVpcLinkResponseTypeDef = TypedDict(
+    "UpdateVpcLinkResponseTypeDef",
+    {
+        "CreatedDate": datetime,
+        "Name": str,
+        "SecurityGroupIds": List[str],
+        "SubnetIds": List[str],
+        "Tags": Dict[str, str],
+        "VpcLinkId": str,
+        "VpcLinkStatus": VpcLinkStatusType,
+        "VpcLinkStatusMessage": str,
+        "VpcLinkVersion": Literal["V2"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerType": AuthorizerTypeType,
         "IdentitySource": Sequence[str],
@@ -1858,55 +1828,22 @@
         "EnableSimpleResponses": bool,
         "IdentityValidationExpression": str,
         "JwtConfiguration": JWTConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class CreateAuthorizerRequestRequestTypeDef(
     _RequiredCreateAuthorizerRequestRequestTypeDef, _OptionalCreateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-CreateAuthorizerResponseTypeDef = TypedDict(
-    "CreateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetAuthorizerResponseTypeDef = TypedDict(
-    "GetAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
+JWTConfigurationUnionTypeDef = Union[JWTConfigurationTypeDef, JWTConfigurationOutputTypeDef]
 _RequiredUpdateAuthorizerRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateAuthorizerRequestRequestTypeDef",
     {
         "ApiId": str,
         "AuthorizerId": str,
     },
 )
@@ -1923,131 +1860,76 @@
         "IdentityValidationExpression": str,
         "JwtConfiguration": JWTConfigurationTypeDef,
         "Name": str,
     },
     total=False,
 )
 
+
 class UpdateAuthorizerRequestRequestTypeDef(
     _RequiredUpdateAuthorizerRequestRequestTypeDef, _OptionalUpdateAuthorizerRequestRequestTypeDef
 ):
     pass
 
-UpdateAuthorizerResponseTypeDef = TypedDict(
-    "UpdateAuthorizerResponseTypeDef",
-    {
-        "AuthorizerCredentialsArn": str,
-        "AuthorizerId": str,
-        "AuthorizerPayloadFormatVersion": str,
-        "AuthorizerResultTtlInSeconds": int,
-        "AuthorizerType": AuthorizerTypeType,
-        "AuthorizerUri": str,
-        "EnableSimpleResponses": bool,
-        "IdentitySource": List[str],
-        "IdentityValidationExpression": str,
-        "JwtConfiguration": JWTConfigurationTypeDef,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-        "Tags": Mapping[str, str],
-    },
-    total=False,
-)
-
-class CreateDomainNameRequestRequestTypeDef(
-    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
-):
-    pass
-
-_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainName": str,
-    },
-)
-_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateDomainNameRequestRequestTypeDef",
-    {
-        "DomainNameConfigurations": Sequence[DomainNameConfigurationTypeDef],
-        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
-    },
-    total=False,
-)
-
-class UpdateDomainNameRequestRequestTypeDef(
-    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
-):
-    pass
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDomainNameTypeDef = TypedDict(
     "_RequiredDomainNameTypeDef",
     {
         "DomainName": str,
     },
 )
 _OptionalDomainNameTypeDef = TypedDict(
     "_OptionalDomainNameTypeDef",
     {
         "ApiMappingSelectionExpression": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class DomainNameTypeDef(_RequiredDomainNameTypeDef, _OptionalDomainNameTypeDef):
     pass
 
+
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "ApiMappingSelectionExpression": str,
         "DomainName": str,
-        "DomainNameConfigurations": List[DomainNameConfigurationTypeDef],
+        "DomainNameConfigurations": List[DomainNameConfigurationOutputTypeDef],
         "MutualTlsAuthentication": MutualTlsAuthenticationTypeDef,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredCreateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2073,19 +1955,21 @@
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigInputTypeDef,
     },
     total=False,
 )
 
+
 class CreateIntegrationRequestRequestTypeDef(
     _RequiredCreateIntegrationRequestRequestTypeDef, _OptionalCreateIntegrationRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateIntegrationRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateIntegrationRequestRequestTypeDef",
     {
         "ApiId": str,
         "IntegrationId": str,
     },
 )
@@ -2109,19 +1993,21 @@
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigInputTypeDef,
     },
     total=False,
 )
 
+
 class UpdateIntegrationRequestRequestTypeDef(
     _RequiredUpdateIntegrationRequestRequestTypeDef, _OptionalUpdateIntegrationRequestRequestTypeDef
 ):
     pass
 
+
 CreateIntegrationResultTypeDef = TypedDict(
     "CreateIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
         "ConnectionId": str,
         "ConnectionType": ConnectionTypeType,
         "ContentHandlingStrategy": ContentHandlingStrategyType,
@@ -2137,15 +2023,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationResultTypeDef = TypedDict(
     "GetIntegrationResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2164,15 +2050,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 IntegrationTypeDef = TypedDict(
     "IntegrationTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2218,15 +2104,15 @@
         "PayloadFormatVersion": str,
         "RequestParameters": Dict[str, str],
         "RequestTemplates": Dict[str, str],
         "ResponseParameters": Dict[str, Dict[str, str]],
         "TemplateSelectionExpression": str,
         "TimeoutInMillis": int,
         "TlsConfig": TlsConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2246,19 +2132,21 @@
         "RequestParameters": Mapping[str, ParameterConstraintsTypeDef],
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
+
 class CreateRouteRequestRequestTypeDef(
     _RequiredCreateRouteRequestRequestTypeDef, _OptionalCreateRouteRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredCreateRouteResponseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRouteResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseKey": str,
     },
@@ -2269,29 +2157,31 @@
         "ModelSelectionExpression": str,
         "ResponseModels": Mapping[str, str],
         "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
     },
     total=False,
 )
 
+
 class CreateRouteResponseRequestRequestTypeDef(
     _RequiredCreateRouteResponseRequestRequestTypeDef,
     _OptionalCreateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
+
 CreateRouteResponseResponseTypeDef = TypedDict(
     "CreateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRouteResultTypeDef = TypedDict(
     "CreateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2303,27 +2193,27 @@
         "OperationName": str,
         "RequestModels": Dict[str, str],
         "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponseResponseTypeDef = TypedDict(
     "GetRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResultTypeDef = TypedDict(
     "GetRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2335,15 +2225,15 @@
         "OperationName": str,
         "RequestModels": Dict[str, str],
         "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRouteResponseTypeDef = TypedDict(
     "_RequiredRouteResponseTypeDef",
     {
         "RouteResponseKey": str,
@@ -2356,17 +2246,19 @@
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
     },
     total=False,
 )
 
+
 class RouteResponseTypeDef(_RequiredRouteResponseTypeDef, _OptionalRouteResponseTypeDef):
     pass
 
+
 _RequiredRouteTypeDef = TypedDict(
     "_RequiredRouteTypeDef",
     {
         "RouteKey": str,
     },
 )
 _OptionalRouteTypeDef = TypedDict(
@@ -2384,17 +2276,19 @@
         "RouteId": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
+
 class RouteTypeDef(_RequiredRouteTypeDef, _OptionalRouteTypeDef):
     pass
 
+
 _RequiredUpdateRouteRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
     },
 )
@@ -2412,19 +2306,21 @@
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
     },
     total=False,
 )
 
+
 class UpdateRouteRequestRequestTypeDef(
     _RequiredUpdateRouteRequestRequestTypeDef, _OptionalUpdateRouteRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateRouteResponseRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRouteResponseRequestRequestTypeDef",
     {
         "ApiId": str,
         "RouteId": str,
         "RouteResponseId": str,
     },
@@ -2436,29 +2332,31 @@
         "ResponseModels": Mapping[str, str],
         "ResponseParameters": Mapping[str, ParameterConstraintsTypeDef],
         "RouteResponseKey": str,
     },
     total=False,
 )
 
+
 class UpdateRouteResponseRequestRequestTypeDef(
     _RequiredUpdateRouteResponseRequestRequestTypeDef,
     _OptionalUpdateRouteResponseRequestRequestTypeDef,
 ):
     pass
 
+
 UpdateRouteResponseResponseTypeDef = TypedDict(
     "UpdateRouteResponseResponseTypeDef",
     {
         "ModelSelectionExpression": str,
         "ResponseModels": Dict[str, str],
         "ResponseParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteResponseId": str,
         "RouteResponseKey": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateRouteResultTypeDef = TypedDict(
     "UpdateRouteResultTypeDef",
     {
         "ApiGatewayManaged": bool,
@@ -2470,15 +2368,15 @@
         "OperationName": str,
         "RequestModels": Dict[str, str],
         "RequestParameters": Dict[str, ParameterConstraintsTypeDef],
         "RouteId": str,
         "RouteKey": str,
         "RouteResponseSelectionExpression": str,
         "Target": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateStageRequestRequestTypeDef = TypedDict(
     "_RequiredCreateStageRequestRequestTypeDef",
     {
         "ApiId": str,
@@ -2497,19 +2395,21 @@
         "RouteSettings": Mapping[str, RouteSettingsTypeDef],
         "StageVariables": Mapping[str, str],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateStageRequestRequestTypeDef(
     _RequiredCreateStageRequestRequestTypeDef, _OptionalCreateStageRequestRequestTypeDef
 ):
     pass
 
+
 CreateStageResponseTypeDef = TypedDict(
     "CreateStageResponseTypeDef",
     {
         "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
@@ -2519,15 +2419,15 @@
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStageResponseTypeDef = TypedDict(
     "GetStageResponseTypeDef",
     {
         "AccessLogSettings": AccessLogSettingsTypeDef,
@@ -2540,15 +2440,15 @@
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStageTypeDef = TypedDict(
     "_RequiredStageTypeDef",
     {
         "StageName": str,
@@ -2570,17 +2470,19 @@
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
+
 class StageTypeDef(_RequiredStageTypeDef, _OptionalStageTypeDef):
     pass
 
+
 _RequiredUpdateStageRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateStageRequestRequestTypeDef",
     {
         "ApiId": str,
         "StageName": str,
     },
 )
@@ -2595,19 +2497,21 @@
         "Description": str,
         "RouteSettings": Mapping[str, RouteSettingsTypeDef],
         "StageVariables": Mapping[str, str],
     },
     total=False,
 )
 
+
 class UpdateStageRequestRequestTypeDef(
     _RequiredUpdateStageRequestRequestTypeDef, _OptionalUpdateStageRequestRequestTypeDef
 ):
     pass
 
+
 UpdateStageResponseTypeDef = TypedDict(
     "UpdateStageResponseTypeDef",
     {
         "AccessLogSettings": AccessLogSettingsTypeDef,
         "ApiGatewayManaged": bool,
         "AutoDeploy": bool,
         "ClientCertificateId": str,
@@ -2617,109 +2521,367 @@
         "Description": str,
         "LastDeploymentStatusMessage": str,
         "LastUpdatedDate": datetime,
         "RouteSettings": Dict[str, RouteSettingsTypeDef],
         "StageName": str,
         "StageVariables": Dict[str, str],
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeploymentsResponseTypeDef = TypedDict(
     "GetDeploymentsResponseTypeDef",
     {
         "Items": List[DeploymentTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DomainNameConfigurationTypeDef = TypedDict(
+    "DomainNameConfigurationTypeDef",
+    {
+        "ApiGatewayDomainName": str,
+        "CertificateArn": str,
+        "CertificateName": str,
+        "CertificateUploadDate": TimestampTypeDef,
+        "DomainNameStatus": DomainNameStatusType,
+        "DomainNameStatusMessage": str,
+        "EndpointType": EndpointTypeType,
+        "HostedZoneId": str,
+        "SecurityPolicy": SecurityPolicyType,
+        "OwnershipVerificationCertificateArn": str,
+    },
+    total=False,
+)
+
+GetApisRequestGetApisPaginateTypeDef = TypedDict(
+    "GetApisRequestGetApisPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef = TypedDict(
+    "_OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetAuthorizersRequestGetAuthorizersPaginateTypeDef(
+    _RequiredGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    _OptionalGetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef = TypedDict(
+    "_OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetDeploymentsRequestGetDeploymentsPaginateTypeDef(
+    _RequiredGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    _OptionalGetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+):
+    pass
+
+
+GetDomainNamesRequestGetDomainNamesPaginateTypeDef = TypedDict(
+    "GetDomainNamesRequestGetDomainNamesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "IntegrationId": str,
+    },
+)
+_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef(
+    _RequiredGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    _OptionalGetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef = TypedDict(
+    "_OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetIntegrationsRequestGetIntegrationsPaginateTypeDef(
+    _RequiredGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    _OptionalGetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_RequiredGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetModelsRequestGetModelsPaginateTypeDef = TypedDict(
+    "_OptionalGetModelsRequestGetModelsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetModelsRequestGetModelsPaginateTypeDef(
+    _RequiredGetModelsRequestGetModelsPaginateTypeDef,
+    _OptionalGetModelsRequestGetModelsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "ApiId": str,
+        "RouteId": str,
+    },
+)
+_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef = TypedDict(
+    "_OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef(
+    _RequiredGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    _OptionalGetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_RequiredGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetRoutesRequestGetRoutesPaginateTypeDef = TypedDict(
+    "_OptionalGetRoutesRequestGetRoutesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetRoutesRequestGetRoutesPaginateTypeDef(
+    _RequiredGetRoutesRequestGetRoutesPaginateTypeDef,
+    _OptionalGetRoutesRequestGetRoutesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_RequiredGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "ApiId": str,
+    },
+)
+_OptionalGetStagesRequestGetStagesPaginateTypeDef = TypedDict(
+    "_OptionalGetStagesRequestGetStagesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class GetStagesRequestGetStagesPaginateTypeDef(
+    _RequiredGetStagesRequestGetStagesPaginateTypeDef,
+    _OptionalGetStagesRequestGetStagesPaginateTypeDef,
+):
+    pass
+
+
 GetIntegrationResponsesResponseTypeDef = TypedDict(
     "GetIntegrationResponsesResponseTypeDef",
     {
         "Items": List[IntegrationResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetModelsResponseTypeDef = TypedDict(
     "GetModelsResponseTypeDef",
     {
         "Items": List[ModelTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetVpcLinksResponseTypeDef = TypedDict(
     "GetVpcLinksResponseTypeDef",
     {
         "Items": List[VpcLinkTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApisResponseTypeDef = TypedDict(
     "GetApisResponseTypeDef",
     {
         "Items": List[ApiTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetAuthorizersResponseTypeDef = TypedDict(
     "GetAuthorizersResponseTypeDef",
     {
         "Items": List[AuthorizerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNamesResponseTypeDef = TypedDict(
     "GetDomainNamesResponseTypeDef",
     {
         "Items": List[DomainNameTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIntegrationsResponseTypeDef = TypedDict(
     "GetIntegrationsResponseTypeDef",
     {
         "Items": List[IntegrationTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRouteResponsesResponseTypeDef = TypedDict(
     "GetRouteResponsesResponseTypeDef",
     {
         "Items": List[RouteResponseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoutesResponseTypeDef = TypedDict(
     "GetRoutesResponseTypeDef",
     {
         "Items": List[RouteTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetStagesResponseTypeDef = TypedDict(
     "GetStagesResponseTypeDef",
     {
         "Items": List[StageTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+DomainNameConfigurationUnionTypeDef = Union[
+    DomainNameConfigurationTypeDef, DomainNameConfigurationOutputTypeDef
+]
+_RequiredCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalCreateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+        "Tags": Mapping[str, str],
+    },
+    total=False,
+)
+
+
+class CreateDomainNameRequestRequestTypeDef(
+    _RequiredCreateDomainNameRequestRequestTypeDef, _OptionalCreateDomainNameRequestRequestTypeDef
+):
+    pass
+
+
+_RequiredUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainName": str,
+    },
+)
+_OptionalUpdateDomainNameRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateDomainNameRequestRequestTypeDef",
+    {
+        "DomainNameConfigurations": Sequence[DomainNameConfigurationUnionTypeDef],
+        "MutualTlsAuthentication": MutualTlsAuthenticationInputTypeDef,
+    },
+    total=False,
+)
+
+
+class UpdateDomainNameRequestRequestTypeDef(
+    _RequiredUpdateDomainNameRequestRequestTypeDef, _OptionalUpdateDomainNameRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewayv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApiGatewayV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore apigatewayv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore apigatewayv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-apigatewayv2"></a>
 
 # types-aiobotocore-apigatewayv2
 
 [![PyPI - types-aiobotocore-apigatewayv2](https://img.shields.io/pypi/v/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewayv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewayv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigatewayv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigatewayv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewayv2)](https://pepy.tech/project/types-aiobotocore-apigatewayv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApiGatewayV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewayv2.html#ApiGatewayV2)
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
 [types-aiobotocore-apigatewayv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewayv2/).
 
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
@@ -354,44 +353,42 @@
 )
 
 
 def check_value(value: AuthorizationTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_apigatewayv2.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_apigatewayv2.type_defs import (
     AccessLogSettingsTypeDef,
     ApiMappingTypeDef,
+    CorsOutputTypeDef,
+    JWTConfigurationOutputTypeDef,
     CorsTypeDef,
-    JWTConfigurationTypeDef,
     CreateApiMappingRequestRequestTypeDef,
-    CreateApiMappingResponseTypeDef,
+    ResponseMetadataTypeDef,
+    JWTConfigurationTypeDef,
     CreateDeploymentRequestRequestTypeDef,
-    CreateDeploymentResponseTypeDef,
-    DomainNameConfigurationTypeDef,
     MutualTlsAuthenticationInputTypeDef,
+    DomainNameConfigurationOutputTypeDef,
     MutualTlsAuthenticationTypeDef,
     TlsConfigInputTypeDef,
     CreateIntegrationResponseRequestRequestTypeDef,
-    CreateIntegrationResponseResponseTypeDef,
     TlsConfigTypeDef,
     CreateModelRequestRequestTypeDef,
-    CreateModelResponseTypeDef,
     ParameterConstraintsTypeDef,
     RouteSettingsTypeDef,
     CreateVpcLinkRequestRequestTypeDef,
-    CreateVpcLinkResponseTypeDef,
     DeleteAccessLogSettingsRequestRequestTypeDef,
     DeleteApiMappingRequestRequestTypeDef,
     DeleteApiRequestRequestTypeDef,
     DeleteAuthorizerRequestRequestTypeDef,
     DeleteCorsConfigurationRequestRequestTypeDef,
     DeleteDeploymentRequestRequestTypeDef,
     DeleteDomainNameRequestRequestTypeDef,
@@ -401,97 +398,92 @@
     DeleteRouteRequestParameterRequestRequestTypeDef,
     DeleteRouteRequestRequestTypeDef,
     DeleteRouteResponseRequestRequestTypeDef,
     DeleteRouteSettingsRequestRequestTypeDef,
     DeleteStageRequestRequestTypeDef,
     DeleteVpcLinkRequestRequestTypeDef,
     DeploymentTypeDef,
-    EmptyResponseMetadataTypeDef,
+    TimestampTypeDef,
     ExportApiRequestRequestTypeDef,
-    ExportApiResponseTypeDef,
     GetApiMappingRequestRequestTypeDef,
-    GetApiMappingResponseTypeDef,
     GetApiMappingsRequestRequestTypeDef,
     GetApiRequestRequestTypeDef,
-    GetApisRequestGetApisPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetApisRequestRequestTypeDef,
     GetAuthorizerRequestRequestTypeDef,
-    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
     GetAuthorizersRequestRequestTypeDef,
     GetDeploymentRequestRequestTypeDef,
-    GetDeploymentResponseTypeDef,
-    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
     GetDeploymentsRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
-    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
     GetDomainNamesRequestRequestTypeDef,
     GetIntegrationRequestRequestTypeDef,
     GetIntegrationResponseRequestRequestTypeDef,
-    GetIntegrationResponseResponseTypeDef,
-    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
     GetIntegrationResponsesRequestRequestTypeDef,
     IntegrationResponseTypeDef,
-    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
     GetIntegrationsRequestRequestTypeDef,
     GetModelRequestRequestTypeDef,
-    GetModelResponseTypeDef,
     GetModelTemplateRequestRequestTypeDef,
-    GetModelTemplateResponseTypeDef,
-    GetModelsRequestGetModelsPaginateTypeDef,
     GetModelsRequestRequestTypeDef,
     ModelTypeDef,
     GetRouteRequestRequestTypeDef,
     GetRouteResponseRequestRequestTypeDef,
-    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
     GetRouteResponsesRequestRequestTypeDef,
-    GetRoutesRequestGetRoutesPaginateTypeDef,
     GetRoutesRequestRequestTypeDef,
     GetStageRequestRequestTypeDef,
-    GetStagesRequestGetStagesPaginateTypeDef,
     GetStagesRequestRequestTypeDef,
     GetTagsRequestRequestTypeDef,
-    GetTagsResponseTypeDef,
     GetVpcLinkRequestRequestTypeDef,
-    GetVpcLinkResponseTypeDef,
     GetVpcLinksRequestRequestTypeDef,
     VpcLinkTypeDef,
     ImportApiRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     ReimportApiRequestRequestTypeDef,
     ResetAuthorizersCacheRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiMappingRequestRequestTypeDef,
-    UpdateApiMappingResponseTypeDef,
     UpdateDeploymentRequestRequestTypeDef,
-    UpdateDeploymentResponseTypeDef,
     UpdateIntegrationResponseRequestRequestTypeDef,
-    UpdateIntegrationResponseResponseTypeDef,
     UpdateModelRequestRequestTypeDef,
-    UpdateModelResponseTypeDef,
     UpdateVpcLinkRequestRequestTypeDef,
-    UpdateVpcLinkResponseTypeDef,
-    GetApiMappingsResponseTypeDef,
     ApiTypeDef,
+    AuthorizerTypeDef,
+    CorsUnionTypeDef,
     CreateApiRequestRequestTypeDef,
+    UpdateApiRequestRequestTypeDef,
+    CreateApiMappingResponseTypeDef,
     CreateApiResponseTypeDef,
+    CreateAuthorizerResponseTypeDef,
+    CreateDeploymentResponseTypeDef,
+    CreateIntegrationResponseResponseTypeDef,
+    CreateModelResponseTypeDef,
+    CreateVpcLinkResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportApiResponseTypeDef,
+    GetApiMappingResponseTypeDef,
+    GetApiMappingsResponseTypeDef,
     GetApiResponseTypeDef,
+    GetAuthorizerResponseTypeDef,
+    GetDeploymentResponseTypeDef,
+    GetIntegrationResponseResponseTypeDef,
+    GetModelResponseTypeDef,
+    GetModelTemplateResponseTypeDef,
+    GetTagsResponseTypeDef,
+    GetVpcLinkResponseTypeDef,
     ImportApiResponseTypeDef,
     ReimportApiResponseTypeDef,
-    UpdateApiRequestRequestTypeDef,
+    UpdateApiMappingResponseTypeDef,
     UpdateApiResponseTypeDef,
-    AuthorizerTypeDef,
+    UpdateAuthorizerResponseTypeDef,
+    UpdateDeploymentResponseTypeDef,
+    UpdateIntegrationResponseResponseTypeDef,
+    UpdateModelResponseTypeDef,
+    UpdateVpcLinkResponseTypeDef,
     CreateAuthorizerRequestRequestTypeDef,
-    CreateAuthorizerResponseTypeDef,
-    GetAuthorizerResponseTypeDef,
+    JWTConfigurationUnionTypeDef,
     UpdateAuthorizerRequestRequestTypeDef,
-    UpdateAuthorizerResponseTypeDef,
-    CreateDomainNameRequestRequestTypeDef,
-    UpdateDomainNameRequestRequestTypeDef,
     CreateDomainNameResponseTypeDef,
     DomainNameTypeDef,
     GetDomainNameResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateIntegrationRequestRequestTypeDef,
     UpdateIntegrationRequestRequestTypeDef,
     CreateIntegrationResultTypeDef,
@@ -513,28 +505,42 @@
     CreateStageRequestRequestTypeDef,
     CreateStageResponseTypeDef,
     GetStageResponseTypeDef,
     StageTypeDef,
     UpdateStageRequestRequestTypeDef,
     UpdateStageResponseTypeDef,
     GetDeploymentsResponseTypeDef,
+    DomainNameConfigurationTypeDef,
+    GetApisRequestGetApisPaginateTypeDef,
+    GetAuthorizersRequestGetAuthorizersPaginateTypeDef,
+    GetDeploymentsRequestGetDeploymentsPaginateTypeDef,
+    GetDomainNamesRequestGetDomainNamesPaginateTypeDef,
+    GetIntegrationResponsesRequestGetIntegrationResponsesPaginateTypeDef,
+    GetIntegrationsRequestGetIntegrationsPaginateTypeDef,
+    GetModelsRequestGetModelsPaginateTypeDef,
+    GetRouteResponsesRequestGetRouteResponsesPaginateTypeDef,
+    GetRoutesRequestGetRoutesPaginateTypeDef,
+    GetStagesRequestGetStagesPaginateTypeDef,
     GetIntegrationResponsesResponseTypeDef,
     GetModelsResponseTypeDef,
     GetVpcLinksResponseTypeDef,
     GetApisResponseTypeDef,
     GetAuthorizersResponseTypeDef,
     GetDomainNamesResponseTypeDef,
     GetIntegrationsResponseTypeDef,
     GetRouteResponsesResponseTypeDef,
     GetRoutesResponseTypeDef,
     GetStagesResponseTypeDef,
+    DomainNameConfigurationUnionTypeDef,
+    CreateDomainNameRequestRequestTypeDef,
+    UpdateDomainNameRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AccessLogSettingsTypeDef:
+def get_value() -> AccessLogSettingsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-apigatewayv2-2.5.2/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt` & `types-aiobotocore-apigatewayv2-2.5.2.post1/types_aiobotocore_apigatewayv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


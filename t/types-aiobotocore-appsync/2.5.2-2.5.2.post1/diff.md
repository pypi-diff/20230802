# Comparing `tmp/types-aiobotocore-appsync-2.5.2.tar.gz` & `tmp/types-aiobotocore-appsync-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-appsync-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-appsync-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
```

## Comparing `types-aiobotocore-appsync-2.5.2.tar` & `types-aiobotocore-appsync-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.681696 types-aiobotocore-appsync-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-07-08 01:43:14.681696 types-aiobotocore-appsync-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18788 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.681696 types-aiobotocore-appsync-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.673696 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45985 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    45909 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-07-08 01:26:01.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-07-08 01:26:01.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8729 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8720 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    57225 2023-07-08 01:26:02.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    57142 2023-07-08 01:26:01.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:00.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.681696 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    20353 2023-07-08 01:43:14.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:14.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:14.000000 types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18916 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45944 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45868 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11472 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11470 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    58030 2023-08-02 14:33:29.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57945 2023-08-02 14:33:28.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:27.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.925654 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    20434 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:52.000000 types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-appsync-2.5.2/LICENSE` & `types-aiobotocore-appsync-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2/PKG-INFO` & `types-aiobotocore-appsync-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appsync
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppSync 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppSync 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appsync type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appsync type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appsync"></a>
 
 # types-aiobotocore-appsync
 
 [![PyPI - types-aiobotocore-appsync](https://img.shields.io/pypi/v/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appsync?color=blue)](https://pypistats.org/packages/types-aiobotocore-appsync)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appsync)](https://pepy.tech/project/types-aiobotocore-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [types-aiobotocore-appsync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/).
 
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
@@ -352,33 +351,36 @@
 )
 
 
 def check_value(value: ApiCacheStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appsync.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appsync.type_defs import (
     CognitoUserPoolConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
@@ -397,96 +399,98 @@
     DeleteFunctionRequestRequestTypeDef,
     DeleteGraphqlApiRequestRequestTypeDef,
     DeleteResolverRequestRequestTypeDef,
     DeleteTypeRequestRequestTypeDef,
     DeltaSyncConfigTypeDef,
     DisassociateApiRequestRequestTypeDef,
     DisassociateMergedGraphqlApiRequestRequestTypeDef,
-    DisassociateMergedGraphqlApiResponseTypeDef,
     DisassociateSourceGraphqlApiRequestRequestTypeDef,
-    DisassociateSourceGraphqlApiResponseTypeDef,
     ErrorDetailTypeDef,
     EvaluateMappingTemplateRequestRequestTypeDef,
     FlushApiCacheRequestRequestTypeDef,
     GetApiAssociationRequestRequestTypeDef,
     GetApiCacheRequestRequestTypeDef,
     GetDataSourceRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetGraphqlApiRequestRequestTypeDef,
     GetIntrospectionSchemaRequestRequestTypeDef,
-    GetIntrospectionSchemaResponseTypeDef,
     GetResolverRequestRequestTypeDef,
     GetSchemaCreationStatusRequestRequestTypeDef,
-    GetSchemaCreationStatusResponseTypeDef,
     GetSourceApiAssociationRequestRequestTypeDef,
     GetTypeRequestRequestTypeDef,
     LambdaConflictHandlerConfigTypeDef,
-    ListApiKeysRequestListApiKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApiKeysRequestRequestTypeDef,
-    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListDomainNamesRequestRequestTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListGraphqlApisRequestRequestTypeDef,
-    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversByFunctionRequestRequestTypeDef,
-    ListResolversRequestListResolversPaginateTypeDef,
     ListResolversRequestRequestTypeDef,
     ListSourceApiAssociationsRequestRequestTypeDef,
     SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationRequestRequestTypeDef,
-    ListTypesRequestListTypesPaginateTypeDef,
     ListTypesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PipelineConfigOutputTypeDef,
     RdsHttpEndpointConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartSchemaCreationRequestRequestTypeDef,
-    StartSchemaCreationResponseTypeDef,
     StartSchemaMergeRequestRequestTypeDef,
-    StartSchemaMergeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
     AdditionalAuthenticationProviderTypeDef,
+    EvaluateCodeRequestRequestTypeDef,
     AssociateApiResponseTypeDef,
-    GetApiAssociationResponseTypeDef,
     CreateApiCacheResponseTypeDef,
-    GetApiCacheResponseTypeDef,
-    UpdateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
+    GetApiAssociationResponseTypeDef,
+    GetApiCacheResponseTypeDef,
+    GetIntrospectionSchemaResponseTypeDef,
+    GetSchemaCreationStatusResponseTypeDef,
     ListApiKeysResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeResponseTypeDef,
+    UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
-    EvaluateCodeRequestRequestTypeDef,
     AssociateMergedGraphqlApiRequestRequestTypeDef,
     AssociateSourceGraphqlApiRequestRequestTypeDef,
     SourceApiAssociationTypeDef,
     UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
+    StartSchemaCreationRequestRequestTypeDef,
+    CachingConfigUnionTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     UpdateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     SyncConfigTypeDef,
+    ListApiKeysRequestListApiKeysPaginateTypeDef,
+    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
+    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
+    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    ListResolversRequestListResolversPaginateTypeDef,
+    ListTypesRequestListTypesPaginateTypeDef,
     ListSourceApiAssociationsResponseTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     GetSourceApiAssociationResponseTypeDef,
@@ -519,15 +523,15 @@
     CreateDataSourceResponseTypeDef,
     GetDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
 )
 
 
-def get_structure() -> CognitoUserPoolConfigTypeDef:
+def get_value() -> CognitoUserPoolConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appsync-2.5.2/README.md` & `types-aiobotocore-appsync-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-appsync"></a>
 
 # types-aiobotocore-appsync
 
 [![PyPI - types-aiobotocore-appsync](https://img.shields.io/pypi/v/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appsync?color=blue)](https://pypistats.org/packages/types-aiobotocore-appsync)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appsync)](https://pepy.tech/project/types-aiobotocore-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [types-aiobotocore-appsync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/).
 
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
@@ -319,33 +319,36 @@
 )
 
 
 def check_value(value: ApiCacheStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appsync.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appsync.type_defs import (
     CognitoUserPoolConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
@@ -364,96 +367,98 @@
     DeleteFunctionRequestRequestTypeDef,
     DeleteGraphqlApiRequestRequestTypeDef,
     DeleteResolverRequestRequestTypeDef,
     DeleteTypeRequestRequestTypeDef,
     DeltaSyncConfigTypeDef,
     DisassociateApiRequestRequestTypeDef,
     DisassociateMergedGraphqlApiRequestRequestTypeDef,
-    DisassociateMergedGraphqlApiResponseTypeDef,
     DisassociateSourceGraphqlApiRequestRequestTypeDef,
-    DisassociateSourceGraphqlApiResponseTypeDef,
     ErrorDetailTypeDef,
     EvaluateMappingTemplateRequestRequestTypeDef,
     FlushApiCacheRequestRequestTypeDef,
     GetApiAssociationRequestRequestTypeDef,
     GetApiCacheRequestRequestTypeDef,
     GetDataSourceRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetGraphqlApiRequestRequestTypeDef,
     GetIntrospectionSchemaRequestRequestTypeDef,
-    GetIntrospectionSchemaResponseTypeDef,
     GetResolverRequestRequestTypeDef,
     GetSchemaCreationStatusRequestRequestTypeDef,
-    GetSchemaCreationStatusResponseTypeDef,
     GetSourceApiAssociationRequestRequestTypeDef,
     GetTypeRequestRequestTypeDef,
     LambdaConflictHandlerConfigTypeDef,
-    ListApiKeysRequestListApiKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApiKeysRequestRequestTypeDef,
-    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListDomainNamesRequestRequestTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListGraphqlApisRequestRequestTypeDef,
-    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversByFunctionRequestRequestTypeDef,
-    ListResolversRequestListResolversPaginateTypeDef,
     ListResolversRequestRequestTypeDef,
     ListSourceApiAssociationsRequestRequestTypeDef,
     SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationRequestRequestTypeDef,
-    ListTypesRequestListTypesPaginateTypeDef,
     ListTypesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PipelineConfigOutputTypeDef,
     RdsHttpEndpointConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartSchemaCreationRequestRequestTypeDef,
-    StartSchemaCreationResponseTypeDef,
     StartSchemaMergeRequestRequestTypeDef,
-    StartSchemaMergeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
     AdditionalAuthenticationProviderTypeDef,
+    EvaluateCodeRequestRequestTypeDef,
     AssociateApiResponseTypeDef,
-    GetApiAssociationResponseTypeDef,
     CreateApiCacheResponseTypeDef,
-    GetApiCacheResponseTypeDef,
-    UpdateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
+    GetApiAssociationResponseTypeDef,
+    GetApiCacheResponseTypeDef,
+    GetIntrospectionSchemaResponseTypeDef,
+    GetSchemaCreationStatusResponseTypeDef,
     ListApiKeysResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeResponseTypeDef,
+    UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
-    EvaluateCodeRequestRequestTypeDef,
     AssociateMergedGraphqlApiRequestRequestTypeDef,
     AssociateSourceGraphqlApiRequestRequestTypeDef,
     SourceApiAssociationTypeDef,
     UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
+    StartSchemaCreationRequestRequestTypeDef,
+    CachingConfigUnionTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     UpdateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     SyncConfigTypeDef,
+    ListApiKeysRequestListApiKeysPaginateTypeDef,
+    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
+    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
+    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    ListResolversRequestListResolversPaginateTypeDef,
+    ListTypesRequestListTypesPaginateTypeDef,
     ListSourceApiAssociationsResponseTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     GetSourceApiAssociationResponseTypeDef,
@@ -486,15 +491,15 @@
     CreateDataSourceResponseTypeDef,
     GetDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
 )
 
 
-def get_structure() -> CognitoUserPoolConfigTypeDef:
+def get_value() -> CognitoUserPoolConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appsync-2.5.2/setup.py` & `types-aiobotocore-appsync-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-appsync",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_appsync"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AppSync 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore appsync type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore appsync type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_appsync": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/"
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/__init__.py` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/__init__.pyi` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/__main__.py` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AppSync 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AppSync 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync\nOther"
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

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/client.py` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("appsync") as client:
         client: AppSyncClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ApiCacheTypeType,
     ApiCachingBehaviorType,
     AuthenticationTypeType,
     DataSourceTypeType,
@@ -44,15 +43,16 @@
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
-    CachingConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigUnionTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -88,15 +88,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
@@ -327,17 +327,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -712,15 +712,15 @@
         Lists `Type` objects by the source API association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_types_by_association)
         """
 
     async def start_schema_creation(
-        self, *, apiId: str, definition: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, apiId: str, definition: BlobTypeDef
     ) -> StartSchemaCreationResponseTypeDef:
         """
         Adds a new schema to your GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#start_schema_creation)
         """
@@ -860,17 +860,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/client.pyi` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,18 +11,17 @@
 
     session = get_session()
     async with session.create_client("appsync") as client:
         client: AppSyncClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import (
     ApiCacheTypeType,
     ApiCachingBehaviorType,
     AuthenticationTypeType,
     DataSourceTypeType,
@@ -44,15 +43,16 @@
 )
 from .type_defs import (
     AdditionalAuthenticationProviderTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiResponseTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
-    CachingConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigUnionTypeDef,
     CreateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateDomainNameResponseTypeDef,
     CreateFunctionResponseTypeDef,
     CreateGraphqlApiResponseTypeDef,
     CreateResolverResponseTypeDef,
@@ -88,15 +88,15 @@
     ListSourceApiAssociationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     LogConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     OpenSearchServiceDataSourceConfigTypeDef,
-    PipelineConfigTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     SourceApiAssociationConfigTypeDef,
     StartSchemaCreationResponseTypeDef,
     StartSchemaMergeResponseTypeDef,
     SyncConfigTypeDef,
     UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
@@ -311,17 +311,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> CreateResolverResponseTypeDef:
         """
         Creates a `Resolver` object.
 
@@ -657,15 +657,15 @@
         """
         Lists `Type` objects by the source API association ID.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.list_types_by_association)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#list_types_by_association)
         """
     async def start_schema_creation(
-        self, *, apiId: str, definition: Union[str, bytes, IO[Any], StreamingBody]
+        self, *, apiId: str, definition: BlobTypeDef
     ) -> StartSchemaCreationResponseTypeDef:
         """
         Adds a new schema to your GraphQL API.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Client.start_schema_creation)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/client/#start_schema_creation)
         """
@@ -795,17 +795,17 @@
         apiId: str,
         typeName: str,
         fieldName: str,
         dataSourceName: str = ...,
         requestMappingTemplate: str = ...,
         responseMappingTemplate: str = ...,
         kind: ResolverKindType = ...,
-        pipelineConfig: PipelineConfigTypeDef = ...,
+        pipelineConfig: PipelineConfigUnionTypeDef = ...,
         syncConfig: SyncConfigTypeDef = ...,
-        cachingConfig: CachingConfigTypeDef = ...,
+        cachingConfig: CachingConfigUnionTypeDef = ...,
         maxBatchSize: int = ...,
         runtime: AppSyncRuntimeTypeDef = ...,
         code: str = ...
     ) -> UpdateResolverResponseTypeDef:
         """
         Updates a `Resolver` object.
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/literals.py` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/literals.pyi` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/paginator.py` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,45 +73,45 @@
 class ListApiKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listapikeyspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApiKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listapikeyspaginator)
         """
 
 
 class ListDataSourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listdatasourcespaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listdatasourcespaginator)
         """
 
 
 class ListFunctionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listfunctionspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listfunctionspaginator)
         """
 
 
@@ -122,45 +122,45 @@
     """
 
     def paginate(
         self,
         *,
         apiType: GraphQLApiTypeType = ...,
         owner: OwnershipType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGraphqlApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listgraphqlapispaginator)
         """
 
 
 class ListResolversPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolverspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, typeName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, typeName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResolversResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolverspaginator)
         """
 
 
 class ListResolversByFunctionPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolversbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, apiId: str, functionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, functionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResolversByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolversbyfunctionpaginator)
         """
 
 
@@ -171,13 +171,13 @@
     """
 
     def paginate(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/paginator.pyi` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -70,43 +70,43 @@
 class ListApiKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listapikeyspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListApiKeysResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListApiKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listapikeyspaginator)
         """
 
 class ListDataSourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listdatasourcespaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListDataSources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listdatasourcespaginator)
         """
 
 class ListFunctionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listfunctionspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFunctionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListFunctions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listfunctionspaginator)
         """
 
 class ListGraphqlApisPaginator(AioPaginator):
@@ -116,43 +116,43 @@
     """
 
     def paginate(
         self,
         *,
         apiType: GraphQLApiTypeType = ...,
         owner: OwnershipType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListGraphqlApisResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListGraphqlApis.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listgraphqlapispaginator)
         """
 
 class ListResolversPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolverspaginator)
     """
 
     def paginate(
-        self, *, apiId: str, typeName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, typeName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResolversResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolvers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolverspaginator)
         """
 
 class ListResolversByFunctionPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolversbyfunctionpaginator)
     """
 
     def paginate(
-        self, *, apiId: str, functionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, apiId: str, functionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResolversByFunctionResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListResolversByFunction.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listresolversbyfunctionpaginator)
         """
 
 class ListTypesPaginator(AioPaginator):
@@ -162,13 +162,13 @@
     """
 
     def paginate(
         self,
         *,
         apiId: str,
         format: TypeDefinitionFormatType,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTypesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync.Paginator.ListTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/paginators/#listtypespaginator)
         """
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/type_defs.py` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appsync.type_defs import CognitoUserPoolConfigTypeDef
 
-    data: CognitoUserPoolConfigTypeDef = {...}
+    data: CognitoUserPoolConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -54,16 +54,19 @@
     "LambdaAuthorizerConfigTypeDef",
     "OpenIDConnectConfigTypeDef",
     "ApiAssociationTypeDef",
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
+    "BlobTypeDef",
+    "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
@@ -82,96 +85,98 @@
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteGraphqlApiRequestRequestTypeDef",
     "DeleteResolverRequestRequestTypeDef",
     "DeleteTypeRequestRequestTypeDef",
     "DeltaSyncConfigTypeDef",
     "DisassociateApiRequestRequestTypeDef",
     "DisassociateMergedGraphqlApiRequestRequestTypeDef",
-    "DisassociateMergedGraphqlApiResponseTypeDef",
     "DisassociateSourceGraphqlApiRequestRequestTypeDef",
-    "DisassociateSourceGraphqlApiResponseTypeDef",
     "ErrorDetailTypeDef",
     "EvaluateMappingTemplateRequestRequestTypeDef",
     "FlushApiCacheRequestRequestTypeDef",
     "GetApiAssociationRequestRequestTypeDef",
     "GetApiCacheRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetGraphqlApiRequestRequestTypeDef",
     "GetIntrospectionSchemaRequestRequestTypeDef",
-    "GetIntrospectionSchemaResponseTypeDef",
     "GetResolverRequestRequestTypeDef",
     "GetSchemaCreationStatusRequestRequestTypeDef",
-    "GetSchemaCreationStatusResponseTypeDef",
     "GetSourceApiAssociationRequestRequestTypeDef",
     "GetTypeRequestRequestTypeDef",
     "LambdaConflictHandlerConfigTypeDef",
-    "ListApiKeysRequestListApiKeysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApiKeysRequestRequestTypeDef",
-    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListGraphqlApisRequestRequestTypeDef",
-    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversByFunctionRequestRequestTypeDef",
-    "ListResolversRequestListResolversPaginateTypeDef",
     "ListResolversRequestRequestTypeDef",
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
-    "ListTypesRequestListTypesPaginateTypeDef",
     "ListTypesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "PipelineConfigOutputTypeDef",
     "RdsHttpEndpointConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartSchemaCreationRequestRequestTypeDef",
-    "StartSchemaCreationResponseTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
-    "StartSchemaMergeResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "UpdateTypeRequestRequestTypeDef",
     "AdditionalAuthenticationProviderTypeDef",
+    "EvaluateCodeRequestRequestTypeDef",
     "AssociateApiResponseTypeDef",
-    "GetApiAssociationResponseTypeDef",
     "CreateApiCacheResponseTypeDef",
-    "GetApiCacheResponseTypeDef",
-    "UpdateApiCacheResponseTypeDef",
     "CreateApiKeyResponseTypeDef",
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    "DisassociateSourceGraphqlApiResponseTypeDef",
+    "GetApiAssociationResponseTypeDef",
+    "GetApiCacheResponseTypeDef",
+    "GetIntrospectionSchemaResponseTypeDef",
+    "GetSchemaCreationStatusResponseTypeDef",
     "ListApiKeysResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartSchemaCreationResponseTypeDef",
+    "StartSchemaMergeResponseTypeDef",
+    "UpdateApiCacheResponseTypeDef",
     "UpdateApiKeyResponseTypeDef",
-    "EvaluateCodeRequestRequestTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
+    "StartSchemaCreationRequestRequestTypeDef",
+    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
     "ListTypesByAssociationResponseTypeDef",
     "ListTypesResponseTypeDef",
     "UpdateTypeResponseTypeDef",
     "DynamodbDataSourceConfigTypeDef",
     "EvaluateMappingTemplateResponseTypeDef",
     "SyncConfigTypeDef",
+    "ListApiKeysRequestListApiKeysPaginateTypeDef",
+    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
+    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    "ListResolversRequestListResolversPaginateTypeDef",
+    "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
+    "PipelineConfigUnionTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
     "GetSourceApiAssociationResponseTypeDef",
@@ -321,14 +326,25 @@
     "AssociateApiRequestRequestTypeDef",
     {
         "domainName": str,
         "apiId": str,
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
 SourceApiAssociationConfigTypeDef = TypedDict(
     "SourceApiAssociationConfigTypeDef",
     {
         "mergeType": MergeTypeType,
     },
     total=False,
 )
@@ -338,14 +354,36 @@
     {
         "signingRegion": str,
         "signingServiceName": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredCachingConfigOutputTypeDef = TypedDict(
+    "_RequiredCachingConfigOutputTypeDef",
+    {
+        "ttl": int,
+    },
+)
+_OptionalCachingConfigOutputTypeDef = TypedDict(
+    "_OptionalCachingConfigOutputTypeDef",
+    {
+        "cachingKeys": List[str],
+    },
+    total=False,
+)
+
+
+class CachingConfigOutputTypeDef(
+    _RequiredCachingConfigOutputTypeDef, _OptionalCachingConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredCachingConfigTypeDef = TypedDict(
     "_RequiredCachingConfigTypeDef",
     {
         "ttl": int,
     },
 )
 _OptionalCachingConfigTypeDef = TypedDict(
@@ -635,38 +673,22 @@
     "DisassociateMergedGraphqlApiRequestRequestTypeDef",
     {
         "sourceApiIdentifier": str,
         "associationId": str,
     },
 )
 
-DisassociateMergedGraphqlApiResponseTypeDef = TypedDict(
-    "DisassociateMergedGraphqlApiResponseTypeDef",
-    {
-        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
     "DisassociateSourceGraphqlApiRequestRequestTypeDef",
     {
         "mergedApiIdentifier": str,
         "associationId": str,
     },
 )
 
-DisassociateSourceGraphqlApiResponseTypeDef = TypedDict(
-    "DisassociateSourceGraphqlApiResponseTypeDef",
-    {
-        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "message": str,
     },
     total=False,
 )
@@ -749,22 +771,14 @@
 class GetIntrospectionSchemaRequestRequestTypeDef(
     _RequiredGetIntrospectionSchemaRequestRequestTypeDef,
     _OptionalGetIntrospectionSchemaRequestRequestTypeDef,
 ):
     pass
 
 
-GetIntrospectionSchemaResponseTypeDef = TypedDict(
-    "GetIntrospectionSchemaResponseTypeDef",
-    {
-        "schema": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverRequestRequestTypeDef = TypedDict(
     "GetResolverRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
         "fieldName": str,
     },
@@ -773,23 +787,14 @@
 GetSchemaCreationStatusRequestRequestTypeDef = TypedDict(
     "GetSchemaCreationStatusRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 
-GetSchemaCreationStatusResponseTypeDef = TypedDict(
-    "GetSchemaCreationStatusResponseTypeDef",
-    {
-        "status": SchemaStatusType,
-        "details": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceApiAssociationRequestRequestTypeDef = TypedDict(
     "GetSourceApiAssociationRequestRequestTypeDef",
     {
         "mergedApiIdentifier": str,
         "associationId": str,
     },
 )
@@ -807,36 +812,24 @@
     "LambdaConflictHandlerConfigTypeDef",
     {
         "lambdaConflictHandlerArn": str,
     },
     total=False,
 )
 
-_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
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
-class ListApiKeysRequestListApiKeysPaginateTypeDef(
-    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
-    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListApiKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListApiKeysRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListApiKeysRequestRequestTypeDef = TypedDict(
@@ -851,36 +844,14 @@
 
 class ListApiKeysRequestRequestTypeDef(
     _RequiredListApiKeysRequestRequestTypeDef, _OptionalListApiKeysRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
-    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListDataSourcesRequestRequestTypeDef = TypedDict(
@@ -904,36 +875,14 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListFunctionsRequestListFunctionsPaginateTypeDef(
-    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
-    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListFunctionsRequestRequestTypeDef = TypedDict(
@@ -948,58 +897,25 @@
 
 class ListFunctionsRequestRequestTypeDef(
     _RequiredListFunctionsRequestRequestTypeDef, _OptionalListFunctionsRequestRequestTypeDef
 ):
     pass
 
 
-ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
-    {
-        "apiType": GraphQLApiTypeType,
-        "owner": OwnershipType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGraphqlApisRequestRequestTypeDef = TypedDict(
     "ListGraphqlApisRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "apiType": GraphQLApiTypeType,
         "owner": OwnershipType,
     },
     total=False,
 )
 
-_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "apiId": str,
-        "functionId": str,
-    },
-)
-_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
-    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResolversByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversByFunctionRequestRequestTypeDef",
     {
         "apiId": str,
         "functionId": str,
     },
 )
@@ -1016,37 +932,14 @@
 class ListResolversByFunctionRequestRequestTypeDef(
     _RequiredListResolversByFunctionRequestRequestTypeDef,
     _OptionalListResolversByFunctionRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_RequiredListResolversRequestListResolversPaginateTypeDef",
-    {
-        "apiId": str,
-        "typeName": str,
-    },
-)
-_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_OptionalListResolversRequestListResolversPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResolversRequestListResolversPaginateTypeDef(
-    _RequiredListResolversRequestListResolversPaginateTypeDef,
-    _OptionalListResolversRequestListResolversPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResolversRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
     },
 )
@@ -1106,22 +999,14 @@
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
 _RequiredListTypesByAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredListTypesByAssociationRequestRequestTypeDef",
     {
         "mergedApiIdentifier": str,
         "associationId": str,
         "format": TypeDefinitionFormatType,
     },
@@ -1139,37 +1024,14 @@
 class ListTypesByAssociationRequestRequestTypeDef(
     _RequiredListTypesByAssociationRequestRequestTypeDef,
     _OptionalListTypesByAssociationRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_RequiredListTypesRequestListTypesPaginateTypeDef",
-    {
-        "apiId": str,
-        "format": TypeDefinitionFormatType,
-    },
-)
-_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_OptionalListTypesRequestListTypesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTypesRequestListTypesPaginateTypeDef(
-    _RequiredListTypesRequestListTypesPaginateTypeDef,
-    _OptionalListTypesRequestListTypesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypesRequestRequestTypeDef",
     {
         "apiId": str,
         "format": TypeDefinitionFormatType,
     },
 )
@@ -1185,20 +1047,18 @@
 
 class ListTypesRequestRequestTypeDef(
     _RequiredListTypesRequestRequestTypeDef, _OptionalListTypesRequestRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PipelineConfigOutputTypeDef = TypedDict(
+    "PipelineConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "functions": List[str],
     },
     total=False,
 )
 
 RdsHttpEndpointConfigTypeDef = TypedDict(
     "RdsHttpEndpointConfigTypeDef",
     {
@@ -1207,57 +1067,22 @@
         "databaseName": str,
         "schema": str,
         "awsSecretStoreArn": str,
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
-StartSchemaCreationRequestRequestTypeDef = TypedDict(
-    "StartSchemaCreationRequestRequestTypeDef",
-    {
-        "apiId": str,
-        "definition": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
-StartSchemaCreationResponseTypeDef = TypedDict(
-    "StartSchemaCreationResponseTypeDef",
-    {
-        "status": SchemaStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartSchemaMergeRequestRequestTypeDef = TypedDict(
     "StartSchemaMergeRequestRequestTypeDef",
     {
         "associationId": str,
         "mergedApiIdentifier": str,
     },
 )
 
-StartSchemaMergeResponseTypeDef = TypedDict(
-    "StartSchemaMergeResponseTypeDef",
-    {
-        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1354,101 +1179,158 @@
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "userPoolConfig": CognitoUserPoolConfigTypeDef,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
     },
     total=False,
 )
 
-AssociateApiResponseTypeDef = TypedDict(
-    "AssociateApiResponseTypeDef",
+_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_RequiredEvaluateCodeRequestRequestTypeDef",
     {
-        "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "runtime": AppSyncRuntimeTypeDef,
+        "code": str,
+        "context": str,
     },
 )
+_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_OptionalEvaluateCodeRequestRequestTypeDef",
+    {
+        "function": str,
+    },
+    total=False,
+)
 
-GetApiAssociationResponseTypeDef = TypedDict(
-    "GetApiAssociationResponseTypeDef",
+
+class EvaluateCodeRequestRequestTypeDef(
+    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
+):
+    pass
+
+
+AssociateApiResponseTypeDef = TypedDict(
+    "AssociateApiResponseTypeDef",
     {
         "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApiCacheResponseTypeDef = TypedDict(
     "CreateApiCacheResponseTypeDef",
     {
         "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApiKeyResponseTypeDef = TypedDict(
+    "CreateApiKeyResponseTypeDef",
+    {
+        "apiKey": ApiKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateMergedGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateSourceGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateSourceGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiAssociationResponseTypeDef = TypedDict(
+    "GetApiAssociationResponseTypeDef",
+    {
+        "apiAssociation": ApiAssociationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiCacheResponseTypeDef = TypedDict(
     "GetApiCacheResponseTypeDef",
     {
         "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApiCacheResponseTypeDef = TypedDict(
-    "UpdateApiCacheResponseTypeDef",
+GetIntrospectionSchemaResponseTypeDef = TypedDict(
+    "GetIntrospectionSchemaResponseTypeDef",
     {
-        "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "schema": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApiKeyResponseTypeDef = TypedDict(
-    "CreateApiKeyResponseTypeDef",
+GetSchemaCreationStatusResponseTypeDef = TypedDict(
+    "GetSchemaCreationStatusResponseTypeDef",
     {
-        "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": SchemaStatusType,
+        "details": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApiKeysResponseTypeDef = TypedDict(
     "ListApiKeysResponseTypeDef",
     {
         "apiKeys": List[ApiKeyTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApiKeyResponseTypeDef = TypedDict(
-    "UpdateApiKeyResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_RequiredEvaluateCodeRequestRequestTypeDef",
+StartSchemaCreationResponseTypeDef = TypedDict(
+    "StartSchemaCreationResponseTypeDef",
     {
-        "runtime": AppSyncRuntimeTypeDef,
-        "code": str,
-        "context": str,
+        "status": SchemaStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_OptionalEvaluateCodeRequestRequestTypeDef",
+
+StartSchemaMergeResponseTypeDef = TypedDict(
+    "StartSchemaMergeResponseTypeDef",
     {
-        "function": str,
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+UpdateApiCacheResponseTypeDef = TypedDict(
+    "UpdateApiCacheResponseTypeDef",
+    {
+        "apiCache": ApiCacheTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class EvaluateCodeRequestRequestTypeDef(
-    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
-):
-    pass
-
+UpdateApiKeyResponseTypeDef = TypedDict(
+    "UpdateApiKeyResponseTypeDef",
+    {
+        "apiKey": ApiKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredAssociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateMergedGraphqlApiRequestRequestTypeDef",
     {
         "sourceApiIdentifier": str,
         "mergedApiIdentifier": str,
     },
@@ -1553,96 +1435,105 @@
 
 class AuthorizationConfigTypeDef(
     _RequiredAuthorizationConfigTypeDef, _OptionalAuthorizationConfigTypeDef
 ):
     pass
 
 
+StartSchemaCreationRequestRequestTypeDef = TypedDict(
+    "StartSchemaCreationRequestRequestTypeDef",
+    {
+        "apiId": str,
+        "definition": BlobTypeDef,
+    },
+)
+
+CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": str,
         "value": str,
         "location": CodeErrorLocationTypeDef,
     },
     total=False,
 )
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "domainNameConfigs": List[DomainNameConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTypeResponseTypeDef = TypedDict(
     "CreateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTypeResponseTypeDef = TypedDict(
     "GetTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesByAssociationResponseTypeDef = TypedDict(
     "ListTypesByAssociationResponseTypeDef",
     {
         "types": List[TypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesResponseTypeDef = TypedDict(
     "ListTypesResponseTypeDef",
     {
         "types": List[TypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTypeResponseTypeDef = TypedDict(
     "UpdateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDynamodbDataSourceConfigTypeDef = TypedDict(
     "_RequiredDynamodbDataSourceConfigTypeDef",
     {
         "tableName": str,
@@ -1668,37 +1559,183 @@
 
 EvaluateMappingTemplateResponseTypeDef = TypedDict(
     "EvaluateMappingTemplateResponseTypeDef",
     {
         "evaluationResult": str,
         "error": ErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SyncConfigTypeDef = TypedDict(
     "SyncConfigTypeDef",
     {
         "conflictHandler": ConflictHandlerTypeType,
         "conflictDetection": ConflictDetectionTypeType,
         "lambdaConflictHandlerConfig": LambdaConflictHandlerConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListApiKeysRequestListApiKeysPaginateTypeDef(
+    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
+    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
+    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListFunctionsRequestListFunctionsPaginateTypeDef(
+    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
+    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
+):
+    pass
+
+
+ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
+    {
+        "apiType": GraphQLApiTypeType,
+        "owner": OwnershipType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "apiId": str,
+        "functionId": str,
+    },
+)
+_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
+    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_RequiredListResolversRequestListResolversPaginateTypeDef",
+    {
+        "apiId": str,
+        "typeName": str,
+    },
+)
+_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_OptionalListResolversRequestListResolversPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResolversRequestListResolversPaginateTypeDef(
+    _RequiredListResolversRequestListResolversPaginateTypeDef,
+    _OptionalListResolversRequestListResolversPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_RequiredListTypesRequestListTypesPaginateTypeDef",
+    {
+        "apiId": str,
+        "format": TypeDefinitionFormatType,
+    },
+)
+_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_OptionalListTypesRequestListTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTypesRequestListTypesPaginateTypeDef(
+    _RequiredListTypesRequestListTypesPaginateTypeDef,
+    _OptionalListTypesRequestListTypesPaginateTypeDef,
+):
+    pass
+
+
 ListSourceApiAssociationsResponseTypeDef = TypedDict(
     "ListSourceApiAssociationsResponseTypeDef",
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef]
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
@@ -1792,39 +1829,39 @@
     pass
 
 
 AssociateMergedGraphqlApiResponseTypeDef = TypedDict(
     "AssociateMergedGraphqlApiResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateSourceGraphqlApiResponseTypeDef = TypedDict(
     "AssociateSourceGraphqlApiResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSourceApiAssociationResponseTypeDef = TypedDict(
     "GetSourceApiAssociationResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSourceApiAssociationResponseTypeDef = TypedDict(
     "UpdateSourceApiAssociationResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HttpDataSourceConfigTypeDef = TypedDict(
     "HttpDataSourceConfigTypeDef",
     {
         "endpoint": str,
@@ -1929,17 +1966,17 @@
         "typeName": str,
         "fieldName": str,
         "dataSourceName": str,
         "resolverArn": str,
         "requestMappingTemplate": str,
         "responseMappingTemplate": str,
         "kind": ResolverKindType,
-        "pipelineConfig": PipelineConfigTypeDef,
+        "pipelineConfig": PipelineConfigOutputTypeDef,
         "syncConfig": SyncConfigTypeDef,
-        "cachingConfig": CachingConfigTypeDef,
+        "cachingConfig": CachingConfigOutputTypeDef,
         "maxBatchSize": int,
         "runtime": AppSyncRuntimeTypeDef,
         "code": str,
     },
     total=False,
 )
 
@@ -2006,40 +2043,40 @@
     pass
 
 
 CreateGraphqlApiResponseTypeDef = TypedDict(
     "CreateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGraphqlApiResponseTypeDef = TypedDict(
     "GetGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGraphqlApisResponseTypeDef = TypedDict(
     "ListGraphqlApisResponseTypeDef",
     {
         "graphqlApis": List[GraphqlApiTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGraphqlApiResponseTypeDef = TypedDict(
     "UpdateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "apiId": str,
@@ -2122,118 +2159,118 @@
 
 EvaluateCodeResponseTypeDef = TypedDict(
     "EvaluateCodeResponseTypeDef",
     {
         "evaluationResult": str,
         "error": EvaluateCodeErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFunctionResponseTypeDef = TypedDict(
     "CreateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "functions": List[FunctionConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFunctionResponseTypeDef = TypedDict(
     "UpdateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResolverResponseTypeDef = TypedDict(
     "CreateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverResponseTypeDef = TypedDict(
     "GetResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolversByFunctionResponseTypeDef = TypedDict(
     "ListResolversByFunctionResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolversResponseTypeDef = TypedDict(
     "ListResolversResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverResponseTypeDef = TypedDict(
     "UpdateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDataSourceResponseTypeDef = TypedDict(
     "CreateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataSourceResponseTypeDef = TypedDict(
     "GetDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "dataSources": List[DataSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataSourceResponseTypeDef = TypedDict(
     "UpdateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync/type_defs.pyi` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_appsync.type_defs import CognitoUserPoolConfigTypeDef
 
-    data: CognitoUserPoolConfigTypeDef = {...}
+    data: CognitoUserPoolConfigTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -53,16 +53,19 @@
     "LambdaAuthorizerConfigTypeDef",
     "OpenIDConnectConfigTypeDef",
     "ApiAssociationTypeDef",
     "ApiCacheTypeDef",
     "ApiKeyTypeDef",
     "AppSyncRuntimeTypeDef",
     "AssociateApiRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "SourceApiAssociationConfigTypeDef",
     "AwsIamConfigTypeDef",
+    "BlobTypeDef",
+    "CachingConfigOutputTypeDef",
     "CachingConfigTypeDef",
     "CodeErrorLocationTypeDef",
     "CreateApiCacheRequestRequestTypeDef",
     "CreateApiKeyRequestRequestTypeDef",
     "ElasticsearchDataSourceConfigTypeDef",
     "EventBridgeDataSourceConfigTypeDef",
     "LambdaDataSourceConfigTypeDef",
@@ -81,96 +84,98 @@
     "DeleteFunctionRequestRequestTypeDef",
     "DeleteGraphqlApiRequestRequestTypeDef",
     "DeleteResolverRequestRequestTypeDef",
     "DeleteTypeRequestRequestTypeDef",
     "DeltaSyncConfigTypeDef",
     "DisassociateApiRequestRequestTypeDef",
     "DisassociateMergedGraphqlApiRequestRequestTypeDef",
-    "DisassociateMergedGraphqlApiResponseTypeDef",
     "DisassociateSourceGraphqlApiRequestRequestTypeDef",
-    "DisassociateSourceGraphqlApiResponseTypeDef",
     "ErrorDetailTypeDef",
     "EvaluateMappingTemplateRequestRequestTypeDef",
     "FlushApiCacheRequestRequestTypeDef",
     "GetApiAssociationRequestRequestTypeDef",
     "GetApiCacheRequestRequestTypeDef",
     "GetDataSourceRequestRequestTypeDef",
     "GetDomainNameRequestRequestTypeDef",
     "GetFunctionRequestRequestTypeDef",
     "GetGraphqlApiRequestRequestTypeDef",
     "GetIntrospectionSchemaRequestRequestTypeDef",
-    "GetIntrospectionSchemaResponseTypeDef",
     "GetResolverRequestRequestTypeDef",
     "GetSchemaCreationStatusRequestRequestTypeDef",
-    "GetSchemaCreationStatusResponseTypeDef",
     "GetSourceApiAssociationRequestRequestTypeDef",
     "GetTypeRequestRequestTypeDef",
     "LambdaConflictHandlerConfigTypeDef",
-    "ListApiKeysRequestListApiKeysPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListApiKeysRequestRequestTypeDef",
-    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
     "ListDataSourcesRequestRequestTypeDef",
     "ListDomainNamesRequestRequestTypeDef",
-    "ListFunctionsRequestListFunctionsPaginateTypeDef",
     "ListFunctionsRequestRequestTypeDef",
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
     "ListGraphqlApisRequestRequestTypeDef",
-    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
     "ListResolversByFunctionRequestRequestTypeDef",
-    "ListResolversRequestListResolversPaginateTypeDef",
     "ListResolversRequestRequestTypeDef",
     "ListSourceApiAssociationsRequestRequestTypeDef",
     "SourceApiAssociationSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTypesByAssociationRequestRequestTypeDef",
-    "ListTypesRequestListTypesPaginateTypeDef",
     "ListTypesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "PipelineConfigOutputTypeDef",
     "RdsHttpEndpointConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartSchemaCreationRequestRequestTypeDef",
-    "StartSchemaCreationResponseTypeDef",
     "StartSchemaMergeRequestRequestTypeDef",
-    "StartSchemaMergeResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateApiCacheRequestRequestTypeDef",
     "UpdateApiKeyRequestRequestTypeDef",
     "UpdateDomainNameRequestRequestTypeDef",
     "UpdateTypeRequestRequestTypeDef",
     "AdditionalAuthenticationProviderTypeDef",
+    "EvaluateCodeRequestRequestTypeDef",
     "AssociateApiResponseTypeDef",
-    "GetApiAssociationResponseTypeDef",
     "CreateApiCacheResponseTypeDef",
-    "GetApiCacheResponseTypeDef",
-    "UpdateApiCacheResponseTypeDef",
     "CreateApiKeyResponseTypeDef",
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    "DisassociateSourceGraphqlApiResponseTypeDef",
+    "GetApiAssociationResponseTypeDef",
+    "GetApiCacheResponseTypeDef",
+    "GetIntrospectionSchemaResponseTypeDef",
+    "GetSchemaCreationStatusResponseTypeDef",
     "ListApiKeysResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "StartSchemaCreationResponseTypeDef",
+    "StartSchemaMergeResponseTypeDef",
+    "UpdateApiCacheResponseTypeDef",
     "UpdateApiKeyResponseTypeDef",
-    "EvaluateCodeRequestRequestTypeDef",
     "AssociateMergedGraphqlApiRequestRequestTypeDef",
     "AssociateSourceGraphqlApiRequestRequestTypeDef",
     "SourceApiAssociationTypeDef",
     "UpdateSourceApiAssociationRequestRequestTypeDef",
     "AuthorizationConfigTypeDef",
+    "StartSchemaCreationRequestRequestTypeDef",
+    "CachingConfigUnionTypeDef",
     "CodeErrorTypeDef",
     "CreateDomainNameResponseTypeDef",
     "GetDomainNameResponseTypeDef",
     "ListDomainNamesResponseTypeDef",
     "UpdateDomainNameResponseTypeDef",
     "CreateTypeResponseTypeDef",
     "GetTypeResponseTypeDef",
     "ListTypesByAssociationResponseTypeDef",
     "ListTypesResponseTypeDef",
     "UpdateTypeResponseTypeDef",
     "DynamodbDataSourceConfigTypeDef",
     "EvaluateMappingTemplateResponseTypeDef",
     "SyncConfigTypeDef",
+    "ListApiKeysRequestListApiKeysPaginateTypeDef",
+    "ListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    "ListFunctionsRequestListFunctionsPaginateTypeDef",
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
+    "ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    "ListResolversRequestListResolversPaginateTypeDef",
+    "ListTypesRequestListTypesPaginateTypeDef",
     "ListSourceApiAssociationsResponseTypeDef",
+    "PipelineConfigUnionTypeDef",
     "RelationalDatabaseDataSourceConfigTypeDef",
     "CreateGraphqlApiRequestRequestTypeDef",
     "GraphqlApiTypeDef",
     "UpdateGraphqlApiRequestRequestTypeDef",
     "AssociateMergedGraphqlApiResponseTypeDef",
     "AssociateSourceGraphqlApiResponseTypeDef",
     "GetSourceApiAssociationResponseTypeDef",
@@ -314,14 +319,25 @@
     "AssociateApiRequestRequestTypeDef",
     {
         "domainName": str,
         "apiId": str,
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
 SourceApiAssociationConfigTypeDef = TypedDict(
     "SourceApiAssociationConfigTypeDef",
     {
         "mergeType": MergeTypeType,
     },
     total=False,
 )
@@ -331,14 +347,34 @@
     {
         "signingRegion": str,
         "signingServiceName": str,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
+_RequiredCachingConfigOutputTypeDef = TypedDict(
+    "_RequiredCachingConfigOutputTypeDef",
+    {
+        "ttl": int,
+    },
+)
+_OptionalCachingConfigOutputTypeDef = TypedDict(
+    "_OptionalCachingConfigOutputTypeDef",
+    {
+        "cachingKeys": List[str],
+    },
+    total=False,
+)
+
+class CachingConfigOutputTypeDef(
+    _RequiredCachingConfigOutputTypeDef, _OptionalCachingConfigOutputTypeDef
+):
+    pass
+
 _RequiredCachingConfigTypeDef = TypedDict(
     "_RequiredCachingConfigTypeDef",
     {
         "ttl": int,
     },
 )
 _OptionalCachingConfigTypeDef = TypedDict(
@@ -616,38 +652,22 @@
     "DisassociateMergedGraphqlApiRequestRequestTypeDef",
     {
         "sourceApiIdentifier": str,
         "associationId": str,
     },
 )
 
-DisassociateMergedGraphqlApiResponseTypeDef = TypedDict(
-    "DisassociateMergedGraphqlApiResponseTypeDef",
-    {
-        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DisassociateSourceGraphqlApiRequestRequestTypeDef = TypedDict(
     "DisassociateSourceGraphqlApiRequestRequestTypeDef",
     {
         "mergedApiIdentifier": str,
         "associationId": str,
     },
 )
 
-DisassociateSourceGraphqlApiResponseTypeDef = TypedDict(
-    "DisassociateSourceGraphqlApiResponseTypeDef",
-    {
-        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "message": str,
     },
     total=False,
 )
@@ -728,22 +748,14 @@
 
 class GetIntrospectionSchemaRequestRequestTypeDef(
     _RequiredGetIntrospectionSchemaRequestRequestTypeDef,
     _OptionalGetIntrospectionSchemaRequestRequestTypeDef,
 ):
     pass
 
-GetIntrospectionSchemaResponseTypeDef = TypedDict(
-    "GetIntrospectionSchemaResponseTypeDef",
-    {
-        "schema": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResolverRequestRequestTypeDef = TypedDict(
     "GetResolverRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
         "fieldName": str,
     },
@@ -752,23 +764,14 @@
 GetSchemaCreationStatusRequestRequestTypeDef = TypedDict(
     "GetSchemaCreationStatusRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 
-GetSchemaCreationStatusResponseTypeDef = TypedDict(
-    "GetSchemaCreationStatusResponseTypeDef",
-    {
-        "status": SchemaStatusType,
-        "details": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSourceApiAssociationRequestRequestTypeDef = TypedDict(
     "GetSourceApiAssociationRequestRequestTypeDef",
     {
         "mergedApiIdentifier": str,
         "associationId": str,
     },
 )
@@ -786,34 +789,24 @@
     "LambdaConflictHandlerConfigTypeDef",
     {
         "lambdaConflictHandlerArn": str,
     },
     total=False,
 )
 
-_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
-    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
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
 
-class ListApiKeysRequestListApiKeysPaginateTypeDef(
-    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
-    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
-):
-    pass
-
 _RequiredListApiKeysRequestRequestTypeDef = TypedDict(
     "_RequiredListApiKeysRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListApiKeysRequestRequestTypeDef = TypedDict(
@@ -826,34 +819,14 @@
 )
 
 class ListApiKeysRequestRequestTypeDef(
     _RequiredListApiKeysRequestRequestTypeDef, _OptionalListApiKeysRequestRequestTypeDef
 ):
     pass
 
-_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
-    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
-    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
-    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDataSourcesRequestRequestTypeDef = TypedDict(
     "_RequiredListDataSourcesRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListDataSourcesRequestRequestTypeDef = TypedDict(
@@ -875,34 +848,14 @@
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "apiId": str,
-    },
-)
-_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
-    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListFunctionsRequestListFunctionsPaginateTypeDef(
-    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
-    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListFunctionsRequestRequestTypeDef = TypedDict(
     "_RequiredListFunctionsRequestRequestTypeDef",
     {
         "apiId": str,
     },
 )
 _OptionalListFunctionsRequestRequestTypeDef = TypedDict(
@@ -915,56 +868,25 @@
 )
 
 class ListFunctionsRequestRequestTypeDef(
     _RequiredListFunctionsRequestRequestTypeDef, _OptionalListFunctionsRequestRequestTypeDef
 ):
     pass
 
-ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
-    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
-    {
-        "apiType": GraphQLApiTypeType,
-        "owner": OwnershipType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListGraphqlApisRequestRequestTypeDef = TypedDict(
     "ListGraphqlApisRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
         "apiType": GraphQLApiTypeType,
         "owner": OwnershipType,
     },
     total=False,
 )
 
-_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "apiId": str,
-        "functionId": str,
-    },
-)
-_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
-    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
-    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
-):
-    pass
-
 _RequiredListResolversByFunctionRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversByFunctionRequestRequestTypeDef",
     {
         "apiId": str,
         "functionId": str,
     },
 )
@@ -979,35 +901,14 @@
 
 class ListResolversByFunctionRequestRequestTypeDef(
     _RequiredListResolversByFunctionRequestRequestTypeDef,
     _OptionalListResolversByFunctionRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_RequiredListResolversRequestListResolversPaginateTypeDef",
-    {
-        "apiId": str,
-        "typeName": str,
-    },
-)
-_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
-    "_OptionalListResolversRequestListResolversPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResolversRequestListResolversPaginateTypeDef(
-    _RequiredListResolversRequestListResolversPaginateTypeDef,
-    _OptionalListResolversRequestListResolversPaginateTypeDef,
-):
-    pass
-
 _RequiredListResolversRequestRequestTypeDef = TypedDict(
     "_RequiredListResolversRequestRequestTypeDef",
     {
         "apiId": str,
         "typeName": str,
     },
 )
@@ -1063,22 +964,14 @@
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
 _RequiredListTypesByAssociationRequestRequestTypeDef = TypedDict(
     "_RequiredListTypesByAssociationRequestRequestTypeDef",
     {
         "mergedApiIdentifier": str,
         "associationId": str,
         "format": TypeDefinitionFormatType,
     },
@@ -1094,35 +987,14 @@
 
 class ListTypesByAssociationRequestRequestTypeDef(
     _RequiredListTypesByAssociationRequestRequestTypeDef,
     _OptionalListTypesByAssociationRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_RequiredListTypesRequestListTypesPaginateTypeDef",
-    {
-        "apiId": str,
-        "format": TypeDefinitionFormatType,
-    },
-)
-_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
-    "_OptionalListTypesRequestListTypesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTypesRequestListTypesPaginateTypeDef(
-    _RequiredListTypesRequestListTypesPaginateTypeDef,
-    _OptionalListTypesRequestListTypesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTypesRequestRequestTypeDef = TypedDict(
     "_RequiredListTypesRequestRequestTypeDef",
     {
         "apiId": str,
         "format": TypeDefinitionFormatType,
     },
 )
@@ -1136,20 +1008,18 @@
 )
 
 class ListTypesRequestRequestTypeDef(
     _RequiredListTypesRequestRequestTypeDef, _OptionalListTypesRequestRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PipelineConfigOutputTypeDef = TypedDict(
+    "PipelineConfigOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "functions": List[str],
     },
     total=False,
 )
 
 RdsHttpEndpointConfigTypeDef = TypedDict(
     "RdsHttpEndpointConfigTypeDef",
     {
@@ -1158,57 +1028,22 @@
         "databaseName": str,
         "schema": str,
         "awsSecretStoreArn": str,
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
-StartSchemaCreationRequestRequestTypeDef = TypedDict(
-    "StartSchemaCreationRequestRequestTypeDef",
-    {
-        "apiId": str,
-        "definition": Union[str, bytes, IO[Any], StreamingBody],
-    },
-)
-
-StartSchemaCreationResponseTypeDef = TypedDict(
-    "StartSchemaCreationResponseTypeDef",
-    {
-        "status": SchemaStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartSchemaMergeRequestRequestTypeDef = TypedDict(
     "StartSchemaMergeRequestRequestTypeDef",
     {
         "associationId": str,
         "mergedApiIdentifier": str,
     },
 )
 
-StartSchemaMergeResponseTypeDef = TypedDict(
-    "StartSchemaMergeResponseTypeDef",
-    {
-        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
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
@@ -1299,99 +1134,156 @@
         "openIDConnectConfig": OpenIDConnectConfigTypeDef,
         "userPoolConfig": CognitoUserPoolConfigTypeDef,
         "lambdaAuthorizerConfig": LambdaAuthorizerConfigTypeDef,
     },
     total=False,
 )
 
-AssociateApiResponseTypeDef = TypedDict(
-    "AssociateApiResponseTypeDef",
+_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_RequiredEvaluateCodeRequestRequestTypeDef",
     {
-        "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "runtime": AppSyncRuntimeTypeDef,
+        "code": str,
+        "context": str,
+    },
+)
+_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
+    "_OptionalEvaluateCodeRequestRequestTypeDef",
+    {
+        "function": str,
     },
+    total=False,
 )
 
-GetApiAssociationResponseTypeDef = TypedDict(
-    "GetApiAssociationResponseTypeDef",
+class EvaluateCodeRequestRequestTypeDef(
+    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
+):
+    pass
+
+AssociateApiResponseTypeDef = TypedDict(
+    "AssociateApiResponseTypeDef",
     {
         "apiAssociation": ApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateApiCacheResponseTypeDef = TypedDict(
     "CreateApiCacheResponseTypeDef",
     {
         "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateApiKeyResponseTypeDef = TypedDict(
+    "CreateApiKeyResponseTypeDef",
+    {
+        "apiKey": ApiKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateMergedGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateMergedGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateSourceGraphqlApiResponseTypeDef = TypedDict(
+    "DisassociateSourceGraphqlApiResponseTypeDef",
+    {
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetApiAssociationResponseTypeDef = TypedDict(
+    "GetApiAssociationResponseTypeDef",
+    {
+        "apiAssociation": ApiAssociationTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetApiCacheResponseTypeDef = TypedDict(
     "GetApiCacheResponseTypeDef",
     {
         "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApiCacheResponseTypeDef = TypedDict(
-    "UpdateApiCacheResponseTypeDef",
+GetIntrospectionSchemaResponseTypeDef = TypedDict(
+    "GetIntrospectionSchemaResponseTypeDef",
     {
-        "apiCache": ApiCacheTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "schema": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CreateApiKeyResponseTypeDef = TypedDict(
-    "CreateApiKeyResponseTypeDef",
+GetSchemaCreationStatusResponseTypeDef = TypedDict(
+    "GetSchemaCreationStatusResponseTypeDef",
     {
-        "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "status": SchemaStatusType,
+        "details": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApiKeysResponseTypeDef = TypedDict(
     "ListApiKeysResponseTypeDef",
     {
         "apiKeys": List[ApiKeyTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateApiKeyResponseTypeDef = TypedDict(
-    "UpdateApiKeyResponseTypeDef",
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
     {
-        "apiKey": ApiKeyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_RequiredEvaluateCodeRequestRequestTypeDef",
+StartSchemaCreationResponseTypeDef = TypedDict(
+    "StartSchemaCreationResponseTypeDef",
     {
-        "runtime": AppSyncRuntimeTypeDef,
-        "code": str,
-        "context": str,
+        "status": SchemaStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalEvaluateCodeRequestRequestTypeDef = TypedDict(
-    "_OptionalEvaluateCodeRequestRequestTypeDef",
+
+StartSchemaMergeResponseTypeDef = TypedDict(
+    "StartSchemaMergeResponseTypeDef",
     {
-        "function": str,
+        "sourceApiAssociationStatus": SourceApiAssociationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class EvaluateCodeRequestRequestTypeDef(
-    _RequiredEvaluateCodeRequestRequestTypeDef, _OptionalEvaluateCodeRequestRequestTypeDef
-):
-    pass
+UpdateApiCacheResponseTypeDef = TypedDict(
+    "UpdateApiCacheResponseTypeDef",
+    {
+        "apiCache": ApiCacheTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateApiKeyResponseTypeDef = TypedDict(
+    "UpdateApiKeyResponseTypeDef",
+    {
+        "apiKey": ApiKeyTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredAssociateMergedGraphqlApiRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateMergedGraphqlApiRequestRequestTypeDef",
     {
         "sourceApiIdentifier": str,
         "mergedApiIdentifier": str,
     },
@@ -1488,96 +1380,105 @@
 )
 
 class AuthorizationConfigTypeDef(
     _RequiredAuthorizationConfigTypeDef, _OptionalAuthorizationConfigTypeDef
 ):
     pass
 
+StartSchemaCreationRequestRequestTypeDef = TypedDict(
+    "StartSchemaCreationRequestRequestTypeDef",
+    {
+        "apiId": str,
+        "definition": BlobTypeDef,
+    },
+)
+
+CachingConfigUnionTypeDef = Union[CachingConfigTypeDef, CachingConfigOutputTypeDef]
 CodeErrorTypeDef = TypedDict(
     "CodeErrorTypeDef",
     {
         "errorType": str,
         "value": str,
         "location": CodeErrorLocationTypeDef,
     },
     total=False,
 )
 
 CreateDomainNameResponseTypeDef = TypedDict(
     "CreateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDomainNameResponseTypeDef = TypedDict(
     "GetDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDomainNamesResponseTypeDef = TypedDict(
     "ListDomainNamesResponseTypeDef",
     {
         "domainNameConfigs": List[DomainNameConfigTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDomainNameResponseTypeDef = TypedDict(
     "UpdateDomainNameResponseTypeDef",
     {
         "domainNameConfig": DomainNameConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateTypeResponseTypeDef = TypedDict(
     "CreateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetTypeResponseTypeDef = TypedDict(
     "GetTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesByAssociationResponseTypeDef = TypedDict(
     "ListTypesByAssociationResponseTypeDef",
     {
         "types": List[TypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTypesResponseTypeDef = TypedDict(
     "ListTypesResponseTypeDef",
     {
         "types": List[TypeTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTypeResponseTypeDef = TypedDict(
     "UpdateTypeResponseTypeDef",
     {
         "type": TypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDynamodbDataSourceConfigTypeDef = TypedDict(
     "_RequiredDynamodbDataSourceConfigTypeDef",
     {
         "tableName": str,
@@ -1601,37 +1502,171 @@
 
 EvaluateMappingTemplateResponseTypeDef = TypedDict(
     "EvaluateMappingTemplateResponseTypeDef",
     {
         "evaluationResult": str,
         "error": ErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SyncConfigTypeDef = TypedDict(
     "SyncConfigTypeDef",
     {
         "conflictHandler": ConflictHandlerTypeType,
         "conflictDetection": ConflictDetectionTypeType,
         "lambdaConflictHandlerConfig": LambdaConflictHandlerConfigTypeDef,
     },
     total=False,
 )
 
+_RequiredListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_RequiredListApiKeysRequestListApiKeysPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListApiKeysRequestListApiKeysPaginateTypeDef = TypedDict(
+    "_OptionalListApiKeysRequestListApiKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListApiKeysRequestListApiKeysPaginateTypeDef(
+    _RequiredListApiKeysRequestListApiKeysPaginateTypeDef,
+    _OptionalListApiKeysRequestListApiKeysPaginateTypeDef,
+):
+    pass
+
+_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef = TypedDict(
+    "_OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDataSourcesRequestListDataSourcesPaginateTypeDef(
+    _RequiredListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    _OptionalListDataSourcesRequestListDataSourcesPaginateTypeDef,
+):
+    pass
+
+_RequiredListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_RequiredListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "apiId": str,
+    },
+)
+_OptionalListFunctionsRequestListFunctionsPaginateTypeDef = TypedDict(
+    "_OptionalListFunctionsRequestListFunctionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListFunctionsRequestListFunctionsPaginateTypeDef(
+    _RequiredListFunctionsRequestListFunctionsPaginateTypeDef,
+    _OptionalListFunctionsRequestListFunctionsPaginateTypeDef,
+):
+    pass
+
+ListGraphqlApisRequestListGraphqlApisPaginateTypeDef = TypedDict(
+    "ListGraphqlApisRequestListGraphqlApisPaginateTypeDef",
+    {
+        "apiType": GraphQLApiTypeType,
+        "owner": OwnershipType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "apiId": str,
+        "functionId": str,
+    },
+)
+_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef = TypedDict(
+    "_OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef(
+    _RequiredListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    _OptionalListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+):
+    pass
+
+_RequiredListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_RequiredListResolversRequestListResolversPaginateTypeDef",
+    {
+        "apiId": str,
+        "typeName": str,
+    },
+)
+_OptionalListResolversRequestListResolversPaginateTypeDef = TypedDict(
+    "_OptionalListResolversRequestListResolversPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResolversRequestListResolversPaginateTypeDef(
+    _RequiredListResolversRequestListResolversPaginateTypeDef,
+    _OptionalListResolversRequestListResolversPaginateTypeDef,
+):
+    pass
+
+_RequiredListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_RequiredListTypesRequestListTypesPaginateTypeDef",
+    {
+        "apiId": str,
+        "format": TypeDefinitionFormatType,
+    },
+)
+_OptionalListTypesRequestListTypesPaginateTypeDef = TypedDict(
+    "_OptionalListTypesRequestListTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTypesRequestListTypesPaginateTypeDef(
+    _RequiredListTypesRequestListTypesPaginateTypeDef,
+    _OptionalListTypesRequestListTypesPaginateTypeDef,
+):
+    pass
+
 ListSourceApiAssociationsResponseTypeDef = TypedDict(
     "ListSourceApiAssociationsResponseTypeDef",
     {
         "sourceApiAssociationSummaries": List[SourceApiAssociationSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+PipelineConfigUnionTypeDef = Union[PipelineConfigTypeDef, PipelineConfigOutputTypeDef]
 RelationalDatabaseDataSourceConfigTypeDef = TypedDict(
     "RelationalDatabaseDataSourceConfigTypeDef",
     {
         "relationalDatabaseSourceType": Literal["RDS_HTTP_ENDPOINT"],
         "rdsHttpEndpointConfig": RdsHttpEndpointConfigTypeDef,
     },
     total=False,
@@ -1721,39 +1756,39 @@
 ):
     pass
 
 AssociateMergedGraphqlApiResponseTypeDef = TypedDict(
     "AssociateMergedGraphqlApiResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AssociateSourceGraphqlApiResponseTypeDef = TypedDict(
     "AssociateSourceGraphqlApiResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSourceApiAssociationResponseTypeDef = TypedDict(
     "GetSourceApiAssociationResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateSourceApiAssociationResponseTypeDef = TypedDict(
     "UpdateSourceApiAssociationResponseTypeDef",
     {
         "sourceApiAssociation": SourceApiAssociationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 HttpDataSourceConfigTypeDef = TypedDict(
     "HttpDataSourceConfigTypeDef",
     {
         "endpoint": str,
@@ -1854,17 +1889,17 @@
         "typeName": str,
         "fieldName": str,
         "dataSourceName": str,
         "resolverArn": str,
         "requestMappingTemplate": str,
         "responseMappingTemplate": str,
         "kind": ResolverKindType,
-        "pipelineConfig": PipelineConfigTypeDef,
+        "pipelineConfig": PipelineConfigOutputTypeDef,
         "syncConfig": SyncConfigTypeDef,
-        "cachingConfig": CachingConfigTypeDef,
+        "cachingConfig": CachingConfigOutputTypeDef,
         "maxBatchSize": int,
         "runtime": AppSyncRuntimeTypeDef,
         "code": str,
     },
     total=False,
 )
 
@@ -1927,40 +1962,40 @@
 ):
     pass
 
 CreateGraphqlApiResponseTypeDef = TypedDict(
     "CreateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGraphqlApiResponseTypeDef = TypedDict(
     "GetGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGraphqlApisResponseTypeDef = TypedDict(
     "ListGraphqlApisResponseTypeDef",
     {
         "graphqlApis": List[GraphqlApiTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGraphqlApiResponseTypeDef = TypedDict(
     "UpdateGraphqlApiResponseTypeDef",
     {
         "graphqlApi": GraphqlApiTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDataSourceRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDataSourceRequestRequestTypeDef",
     {
         "apiId": str,
@@ -2039,118 +2074,118 @@
 
 EvaluateCodeResponseTypeDef = TypedDict(
     "EvaluateCodeResponseTypeDef",
     {
         "evaluationResult": str,
         "error": EvaluateCodeErrorDetailTypeDef,
         "logs": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateFunctionResponseTypeDef = TypedDict(
     "CreateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetFunctionResponseTypeDef = TypedDict(
     "GetFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListFunctionsResponseTypeDef = TypedDict(
     "ListFunctionsResponseTypeDef",
     {
         "functions": List[FunctionConfigurationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateFunctionResponseTypeDef = TypedDict(
     "UpdateFunctionResponseTypeDef",
     {
         "functionConfiguration": FunctionConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResolverResponseTypeDef = TypedDict(
     "CreateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResolverResponseTypeDef = TypedDict(
     "GetResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolversByFunctionResponseTypeDef = TypedDict(
     "ListResolversByFunctionResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResolversResponseTypeDef = TypedDict(
     "ListResolversResponseTypeDef",
     {
         "resolvers": List[ResolverTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResolverResponseTypeDef = TypedDict(
     "UpdateResolverResponseTypeDef",
     {
         "resolver": ResolverTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateDataSourceResponseTypeDef = TypedDict(
     "CreateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataSourceResponseTypeDef = TypedDict(
     "GetDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "dataSources": List[DataSourceTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDataSourceResponseTypeDef = TypedDict(
     "UpdateDataSourceResponseTypeDef",
     {
         "dataSource": DataSourceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/PKG-INFO` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-appsync
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AppSync 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AppSync 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore appsync type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore appsync type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-appsync"></a>
 
 # types-aiobotocore-appsync
 
 [![PyPI - types-aiobotocore-appsync](https://img.shields.io/pypi/v/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-appsync.svg?color=blue)](https://pypi.org/project/types-aiobotocore-appsync)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-appsync?color=blue)](https://pypistats.org/packages/types-aiobotocore-appsync)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-appsync)](https://pepy.tech/project/types-aiobotocore-appsync)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AppSync 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/appsync.html#AppSync)
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
 [types-aiobotocore-appsync docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_appsync/).
 
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
@@ -352,33 +351,36 @@
 )
 
 
 def check_value(value: ApiCacheStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_appsync.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_appsync.type_defs import (
     CognitoUserPoolConfigTypeDef,
     LambdaAuthorizerConfigTypeDef,
     OpenIDConnectConfigTypeDef,
     ApiAssociationTypeDef,
     ApiCacheTypeDef,
     ApiKeyTypeDef,
     AppSyncRuntimeTypeDef,
     AssociateApiRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     SourceApiAssociationConfigTypeDef,
     AwsIamConfigTypeDef,
+    BlobTypeDef,
+    CachingConfigOutputTypeDef,
     CachingConfigTypeDef,
     CodeErrorLocationTypeDef,
     CreateApiCacheRequestRequestTypeDef,
     CreateApiKeyRequestRequestTypeDef,
     ElasticsearchDataSourceConfigTypeDef,
     EventBridgeDataSourceConfigTypeDef,
     LambdaDataSourceConfigTypeDef,
@@ -397,96 +399,98 @@
     DeleteFunctionRequestRequestTypeDef,
     DeleteGraphqlApiRequestRequestTypeDef,
     DeleteResolverRequestRequestTypeDef,
     DeleteTypeRequestRequestTypeDef,
     DeltaSyncConfigTypeDef,
     DisassociateApiRequestRequestTypeDef,
     DisassociateMergedGraphqlApiRequestRequestTypeDef,
-    DisassociateMergedGraphqlApiResponseTypeDef,
     DisassociateSourceGraphqlApiRequestRequestTypeDef,
-    DisassociateSourceGraphqlApiResponseTypeDef,
     ErrorDetailTypeDef,
     EvaluateMappingTemplateRequestRequestTypeDef,
     FlushApiCacheRequestRequestTypeDef,
     GetApiAssociationRequestRequestTypeDef,
     GetApiCacheRequestRequestTypeDef,
     GetDataSourceRequestRequestTypeDef,
     GetDomainNameRequestRequestTypeDef,
     GetFunctionRequestRequestTypeDef,
     GetGraphqlApiRequestRequestTypeDef,
     GetIntrospectionSchemaRequestRequestTypeDef,
-    GetIntrospectionSchemaResponseTypeDef,
     GetResolverRequestRequestTypeDef,
     GetSchemaCreationStatusRequestRequestTypeDef,
-    GetSchemaCreationStatusResponseTypeDef,
     GetSourceApiAssociationRequestRequestTypeDef,
     GetTypeRequestRequestTypeDef,
     LambdaConflictHandlerConfigTypeDef,
-    ListApiKeysRequestListApiKeysPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListApiKeysRequestRequestTypeDef,
-    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
     ListDataSourcesRequestRequestTypeDef,
     ListDomainNamesRequestRequestTypeDef,
-    ListFunctionsRequestListFunctionsPaginateTypeDef,
     ListFunctionsRequestRequestTypeDef,
-    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
     ListGraphqlApisRequestRequestTypeDef,
-    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
     ListResolversByFunctionRequestRequestTypeDef,
-    ListResolversRequestListResolversPaginateTypeDef,
     ListResolversRequestRequestTypeDef,
     ListSourceApiAssociationsRequestRequestTypeDef,
     SourceApiAssociationSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTypesByAssociationRequestRequestTypeDef,
-    ListTypesRequestListTypesPaginateTypeDef,
     ListTypesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PipelineConfigOutputTypeDef,
     RdsHttpEndpointConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartSchemaCreationRequestRequestTypeDef,
-    StartSchemaCreationResponseTypeDef,
     StartSchemaMergeRequestRequestTypeDef,
-    StartSchemaMergeResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateApiCacheRequestRequestTypeDef,
     UpdateApiKeyRequestRequestTypeDef,
     UpdateDomainNameRequestRequestTypeDef,
     UpdateTypeRequestRequestTypeDef,
     AdditionalAuthenticationProviderTypeDef,
+    EvaluateCodeRequestRequestTypeDef,
     AssociateApiResponseTypeDef,
-    GetApiAssociationResponseTypeDef,
     CreateApiCacheResponseTypeDef,
-    GetApiCacheResponseTypeDef,
-    UpdateApiCacheResponseTypeDef,
     CreateApiKeyResponseTypeDef,
+    DisassociateMergedGraphqlApiResponseTypeDef,
+    DisassociateSourceGraphqlApiResponseTypeDef,
+    GetApiAssociationResponseTypeDef,
+    GetApiCacheResponseTypeDef,
+    GetIntrospectionSchemaResponseTypeDef,
+    GetSchemaCreationStatusResponseTypeDef,
     ListApiKeysResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    StartSchemaCreationResponseTypeDef,
+    StartSchemaMergeResponseTypeDef,
+    UpdateApiCacheResponseTypeDef,
     UpdateApiKeyResponseTypeDef,
-    EvaluateCodeRequestRequestTypeDef,
     AssociateMergedGraphqlApiRequestRequestTypeDef,
     AssociateSourceGraphqlApiRequestRequestTypeDef,
     SourceApiAssociationTypeDef,
     UpdateSourceApiAssociationRequestRequestTypeDef,
     AuthorizationConfigTypeDef,
+    StartSchemaCreationRequestRequestTypeDef,
+    CachingConfigUnionTypeDef,
     CodeErrorTypeDef,
     CreateDomainNameResponseTypeDef,
     GetDomainNameResponseTypeDef,
     ListDomainNamesResponseTypeDef,
     UpdateDomainNameResponseTypeDef,
     CreateTypeResponseTypeDef,
     GetTypeResponseTypeDef,
     ListTypesByAssociationResponseTypeDef,
     ListTypesResponseTypeDef,
     UpdateTypeResponseTypeDef,
     DynamodbDataSourceConfigTypeDef,
     EvaluateMappingTemplateResponseTypeDef,
     SyncConfigTypeDef,
+    ListApiKeysRequestListApiKeysPaginateTypeDef,
+    ListDataSourcesRequestListDataSourcesPaginateTypeDef,
+    ListFunctionsRequestListFunctionsPaginateTypeDef,
+    ListGraphqlApisRequestListGraphqlApisPaginateTypeDef,
+    ListResolversByFunctionRequestListResolversByFunctionPaginateTypeDef,
+    ListResolversRequestListResolversPaginateTypeDef,
+    ListTypesRequestListTypesPaginateTypeDef,
     ListSourceApiAssociationsResponseTypeDef,
+    PipelineConfigUnionTypeDef,
     RelationalDatabaseDataSourceConfigTypeDef,
     CreateGraphqlApiRequestRequestTypeDef,
     GraphqlApiTypeDef,
     UpdateGraphqlApiRequestRequestTypeDef,
     AssociateMergedGraphqlApiResponseTypeDef,
     AssociateSourceGraphqlApiResponseTypeDef,
     GetSourceApiAssociationResponseTypeDef,
@@ -519,15 +523,15 @@
     CreateDataSourceResponseTypeDef,
     GetDataSourceResponseTypeDef,
     ListDataSourcesResponseTypeDef,
     UpdateDataSourceResponseTypeDef,
 )
 
 
-def get_structure() -> CognitoUserPoolConfigTypeDef:
+def get_value() -> CognitoUserPoolConfigTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-appsync-2.5.2/types_aiobotocore_appsync.egg-info/SOURCES.txt` & `types-aiobotocore-appsync-2.5.2.post1/types_aiobotocore_appsync.egg-info/SOURCES.txt`

 * *Files identical despite different names*


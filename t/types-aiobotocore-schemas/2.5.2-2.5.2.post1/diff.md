# Comparing `tmp/types-aiobotocore-schemas-2.5.2.tar.gz` & `tmp/types-aiobotocore-schemas-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-schemas-2.5.2.tar", last modified: Sat Jul  8 01:44:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-schemas-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:58 2023, max compression
```

## Comparing `types-aiobotocore-schemas-2.5.2.tar` & `types-aiobotocore-schemas-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.250866 types-aiobotocore-schemas-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-08 01:44:17.250866 types-aiobotocore-schemas-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:17.250866 types-aiobotocore-schemas-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.230866 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25217 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-07-08 01:40:29.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    26157 2023-07-08 01:40:29.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-08 01:40:28.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.250866 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17115 2023-07-08 01:44:17.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-08 01:44:17.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:17.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:44:17.000000 types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.769464 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25217 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8950 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6559 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26134 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26095 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:03.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-08-02 14:49:04.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:58.773464 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17051 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:52:58.000000 types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-schemas-2.5.2/LICENSE` & `types-aiobotocore-schemas-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/PKG-INFO` & `types-aiobotocore-schemas-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-schemas
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore schemas type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore schemas type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-schemas"></a>
 
 # types-aiobotocore-schemas
 
 [![PyPI - types-aiobotocore-schemas](https://img.shields.io/pypi/v/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-schemas?color=blue)](https://pypistats.org/packages/types-aiobotocore-schemas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Schemas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
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
@@ -348,98 +347,98 @@
 )
 
 
 def check_value(value: CodeBindingExistsWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_schemas.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRegistryRequestRequestTypeDef,
-    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
-    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
-    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
-    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
-    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
-    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
-    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
-    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
-    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateDiscovererResponseTypeDef,
     UpdateRegistryRequestRequestTypeDef,
-    UpdateRegistryResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    CreateDiscovererResponseTypeDef,
+    CreateRegistryResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DescribeCodeBindingResponseTypeDef,
+    DescribeDiscovererResponseTypeDef,
+    DescribeRegistryResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSchemaResponseTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutCodeBindingResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartDiscovererResponseTypeDef,
+    StopDiscovererResponseTypeDef,
+    UpdateDiscovererResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
 
 
-def get_structure() -> CreateDiscovererRequestRequestTypeDef:
+def get_value() -> CreateDiscovererRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-schemas-2.5.2/README.md` & `types-aiobotocore-schemas-2.5.2.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-schemas"></a>
 
 # types-aiobotocore-schemas
 
 [![PyPI - types-aiobotocore-schemas](https://img.shields.io/pypi/v/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-schemas?color=blue)](https://pypistats.org/packages/types-aiobotocore-schemas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Schemas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
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
@@ -315,98 +315,98 @@
 )
 
 
 def check_value(value: CodeBindingExistsWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_schemas.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRegistryRequestRequestTypeDef,
-    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
-    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
-    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
-    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
-    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
-    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
-    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
-    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
-    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateDiscovererResponseTypeDef,
     UpdateRegistryRequestRequestTypeDef,
-    UpdateRegistryResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    CreateDiscovererResponseTypeDef,
+    CreateRegistryResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DescribeCodeBindingResponseTypeDef,
+    DescribeDiscovererResponseTypeDef,
+    DescribeRegistryResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSchemaResponseTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutCodeBindingResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartDiscovererResponseTypeDef,
+    StopDiscovererResponseTypeDef,
+    UpdateDiscovererResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
 
 
-def get_structure() -> CreateDiscovererRequestRequestTypeDef:
+def get_value() -> CreateDiscovererRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-schemas-2.5.2/setup.py` & `types-aiobotocore-schemas-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-schemas",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_schemas"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore schemas type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore schemas type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_schemas": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/"
```

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/__init__.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/__init__.pyi` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/__main__.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Schemas 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Schemas 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas\nOther"
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

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/client.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/client.pyi` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/literals.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/literals.pyi` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/paginator.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -46,107 +46,96 @@
     "ListDiscoverersPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
     "SearchSchemasPaginator",
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
 class ListDiscoverersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listdiscovererspaginator)
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listdiscovererspaginator)
         """
 
-
 class ListRegistriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listregistriespaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listregistriespaginator)
         """
 
-
 class ListSchemaVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        RegistryName: str,
-        SchemaName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RegistryName: str, SchemaName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaversionspaginator)
         """
 
-
 class ListSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaspaginator)
         """
 
-
 class SearchSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#searchschemaspaginator)
     """
 
     def paginate(
-        self, *, Keywords: str, RegistryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Keywords: str, RegistryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#searchschemaspaginator)
         """
```

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/paginator.pyi` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,100 +46,103 @@
     "ListDiscoverersPaginator",
     "ListRegistriesPaginator",
     "ListSchemaVersionsPaginator",
     "ListSchemasPaginator",
     "SearchSchemasPaginator",
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
 class ListDiscoverersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listdiscovererspaginator)
     """
 
     def paginate(
         self,
         *,
         DiscovererIdPrefix: str = ...,
         SourceArnPrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDiscoverersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListDiscoverers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listdiscovererspaginator)
         """
 
+
 class ListRegistriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listregistriespaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryNamePrefix: str = ...,
         Scope: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRegistriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListRegistries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listregistriespaginator)
         """
 
+
 class ListSchemaVersionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaversionspaginator)
     """
 
     def paginate(
-        self,
-        *,
-        RegistryName: str,
-        SchemaName: str,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, RegistryName: str, SchemaName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemaVersionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemaVersions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaversionspaginator)
         """
 
+
 class ListSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaspaginator)
     """
 
     def paginate(
         self,
         *,
         RegistryName: str,
         SchemaNamePrefix: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#listschemaspaginator)
         """
 
+
 class SearchSchemasPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#searchschemaspaginator)
     """
 
     def paginate(
-        self, *, Keywords: str, RegistryName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Keywords: str, RegistryName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas.Paginator.SearchSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/paginators/#searchschemaspaginator)
         """
```

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/type_defs.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_schemas.type_defs import CreateDiscovererRequestRequestTypeDef
 
-    data: CreateDiscovererRequestRequestTypeDef = {...}
+    data: CreateDiscovererRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from aiobotocore.response import StreamingBody
@@ -23,79 +23,79 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateDiscovererRequestRequestTypeDef",
-    "CreateDiscovererResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRegistryRequestRequestTypeDef",
-    "CreateRegistryResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSchemaVersionRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeBindingRequestRequestTypeDef",
-    "DescribeCodeBindingResponseTypeDef",
     "DescribeDiscovererRequestRequestTypeDef",
-    "DescribeDiscovererResponseTypeDef",
     "DescribeRegistryRequestRequestTypeDef",
-    "DescribeRegistryResponseTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
-    "DescribeSchemaResponseTypeDef",
     "DiscovererSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSchemaRequestRequestTypeDef",
-    "ExportSchemaResponseTypeDef",
     "GetCodeBindingSourceRequestRequestTypeDef",
-    "GetCodeBindingSourceResponseTypeDef",
     "GetDiscoveredSchemaRequestRequestTypeDef",
-    "GetDiscoveredSchemaResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDiscoverersRequestRequestTypeDef",
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
     "ListRegistriesRequestRequestTypeDef",
     "RegistrySummaryTypeDef",
-    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsRequestRequestTypeDef",
     "SchemaVersionSummaryTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutCodeBindingRequestRequestTypeDef",
-    "PutCodeBindingResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchSchemaVersionSummaryTypeDef",
     "SearchSchemasRequestRequestTypeDef",
-    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "StartDiscovererRequestRequestTypeDef",
-    "StartDiscovererResponseTypeDef",
     "StopDiscovererRequestRequestTypeDef",
-    "StopDiscovererResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDiscovererRequestRequestTypeDef",
-    "UpdateDiscovererResponseTypeDef",
     "UpdateRegistryRequestRequestTypeDef",
-    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
+    "CreateDiscovererResponseTypeDef",
+    "CreateRegistryResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DescribeCodeBindingResponseTypeDef",
+    "DescribeDiscovererResponseTypeDef",
+    "DescribeRegistryResponseTypeDef",
+    "DescribeSchemaResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSchemaResponseTypeDef",
+    "GetCodeBindingSourceResponseTypeDef",
+    "GetDiscoveredSchemaResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutCodeBindingResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartDiscovererResponseTypeDef",
+    "StopDiscovererResponseTypeDef",
+    "UpdateDiscovererResponseTypeDef",
+    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     "ListDiscoverersResponseTypeDef",
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "SearchSchemaSummaryTypeDef",
     "SearchSchemasResponseTypeDef",
 )
 
@@ -118,25 +118,22 @@
 
 class CreateDiscovererRequestRequestTypeDef(
     _RequiredCreateDiscovererRequestRequestTypeDef, _OptionalCreateDiscovererRequestRequestTypeDef
 ):
     pass
 
 
-CreateDiscovererResponseTypeDef = TypedDict(
-    "CreateDiscovererResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
@@ -154,25 +151,14 @@
 
 class CreateRegistryRequestRequestTypeDef(
     _RequiredCreateRegistryRequestRequestTypeDef, _OptionalCreateRegistryRequestRequestTypeDef
 ):
     pass
 
 
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "Content": str,
         "RegistryName": str,
         "SchemaName": str,
         "Type": TypeType,
@@ -190,29 +176,14 @@
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDiscovererRequestRequestTypeDef = TypedDict(
     "DeleteDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
@@ -277,64 +248,28 @@
 class DescribeCodeBindingRequestRequestTypeDef(
     _RequiredDescribeCodeBindingRequestRequestTypeDef,
     _OptionalDescribeCodeBindingRequestRequestTypeDef,
 ):
     pass
 
 
-DescribeCodeBindingResponseTypeDef = TypedDict(
-    "DescribeCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDiscovererRequestRequestTypeDef = TypedDict(
     "DescribeDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-DescribeDiscovererResponseTypeDef = TypedDict(
-    "DescribeDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRegistryRequestRequestTypeDef = TypedDict(
     "DescribeRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 
-DescribeRegistryResponseTypeDef = TypedDict(
-    "DescribeRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -349,50 +284,27 @@
 
 class DescribeSchemaRequestRequestTypeDef(
     _RequiredDescribeSchemaRequestRequestTypeDef, _OptionalDescribeSchemaRequestRequestTypeDef
 ):
     pass
 
 
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscovererSummaryTypeDef = TypedDict(
     "DiscovererSummaryTypeDef",
     {
         "DiscovererArn": str,
         "DiscovererId": str,
         "SourceArn": str,
         "State": DiscovererStateType,
         "CrossAccount": bool,
         "Tags": Dict[str, str],
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
 _RequiredExportSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredExportSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "Type": str,
     },
@@ -408,26 +320,14 @@
 
 class ExportSchemaRequestRequestTypeDef(
     _RequiredExportSchemaRequestRequestTypeDef, _OptionalExportSchemaRequestRequestTypeDef
 ):
     pass
 
 
-ExportSchemaResponseTypeDef = TypedDict(
-    "ExportSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCodeBindingSourceRequestRequestTypeDef = TypedDict(
     "_RequiredGetCodeBindingSourceRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -444,61 +344,36 @@
 class GetCodeBindingSourceRequestRequestTypeDef(
     _RequiredGetCodeBindingSourceRequestRequestTypeDef,
     _OptionalGetCodeBindingSourceRequestRequestTypeDef,
 ):
     pass
 
 
-GetCodeBindingSourceResponseTypeDef = TypedDict(
-    "GetCodeBindingSourceResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredSchemaRequestRequestTypeDef = TypedDict(
     "GetDiscoveredSchemaRequestRequestTypeDef",
     {
         "Events": Sequence[str],
         "Type": TypeType,
     },
 )
 
-GetDiscoveredSchemaResponseTypeDef = TypedDict(
-    "GetDiscoveredSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
     total=False,
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DiscovererIdPrefix": str,
-        "SourceArnPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDiscoverersRequestRequestTypeDef = TypedDict(
     "ListDiscoverersRequestRequestTypeDef",
     {
@@ -506,24 +381,14 @@
         "Limit": int,
         "NextToken": str,
         "SourceArnPrefix": str,
     },
     total=False,
 )
 
-ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    {
-        "RegistryNamePrefix": str,
-        "Scope": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegistriesRequestRequestTypeDef = TypedDict(
     "ListRegistriesRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
         "RegistryNamePrefix": str,
         "Scope": str,
@@ -537,37 +402,14 @@
         "RegistryArn": str,
         "RegistryName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "RegistryName": str,
-        "SchemaName": str,
-    },
-)
-_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemaVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -595,37 +437,14 @@
         "SchemaName": str,
         "SchemaVersion": str,
         "Type": TypeType,
     },
     total=False,
 )
 
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "RegistryName": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "SchemaNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -660,32 +479,14 @@
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
 _RequiredPutCodeBindingRequestRequestTypeDef = TypedDict(
     "_RequiredPutCodeBindingRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -701,25 +502,14 @@
 
 class PutCodeBindingRequestRequestTypeDef(
     _RequiredPutCodeBindingRequestRequestTypeDef, _OptionalPutCodeBindingRequestRequestTypeDef
 ):
     pass
 
 
-PutCodeBindingResponseTypeDef = TypedDict(
-    "PutCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -734,34 +524,14 @@
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 SearchSchemaVersionSummaryTypeDef = TypedDict(
     "SearchSchemaVersionSummaryTypeDef",
     {
         "CreatedDate": datetime,
         "SchemaVersion": str,
         "Type": TypeType,
     },
@@ -787,69 +557,28 @@
 
 class SearchSchemasRequestRequestTypeDef(
     _RequiredSearchSchemasRequestRequestTypeDef, _OptionalSearchSchemasRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "Keywords": str,
-        "RegistryName": str,
-    },
-)
-_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchSchemasRequestSearchSchemasPaginateTypeDef(
-    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
-    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
-):
-    pass
-
-
 StartDiscovererRequestRequestTypeDef = TypedDict(
     "StartDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StartDiscovererResponseTypeDef = TypedDict(
-    "StartDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDiscovererRequestRequestTypeDef = TypedDict(
     "StopDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StopDiscovererResponseTypeDef = TypedDict(
-    "StopDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -880,28 +609,14 @@
 
 class UpdateDiscovererRequestRequestTypeDef(
     _RequiredUpdateDiscovererRequestRequestTypeDef, _OptionalUpdateDiscovererRequestRequestTypeDef
 ):
     pass
 
 
-UpdateDiscovererResponseTypeDef = TypedDict(
-    "UpdateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalUpdateRegistryRequestRequestTypeDef = TypedDict(
@@ -915,25 +630,14 @@
 
 class UpdateRegistryRequestRequestTypeDef(
     _RequiredUpdateRegistryRequestRequestTypeDef, _OptionalUpdateRegistryRequestRequestTypeDef
 ):
     pass
 
 
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -951,26 +655,233 @@
 
 class UpdateSchemaRequestRequestTypeDef(
     _RequiredUpdateSchemaRequestRequestTypeDef, _OptionalUpdateSchemaRequestRequestTypeDef
 ):
     pass
 
 
+CreateDiscovererResponseTypeDef = TypedDict(
+    "CreateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCodeBindingResponseTypeDef = TypedDict(
+    "DescribeCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDiscovererResponseTypeDef = TypedDict(
+    "DescribeDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRegistryResponseTypeDef = TypedDict(
+    "DescribeRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
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
+ExportSchemaResponseTypeDef = TypedDict(
+    "ExportSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Type": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCodeBindingSourceResponseTypeDef = TypedDict(
+    "GetCodeBindingSourceResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDiscoveredSchemaResponseTypeDef = TypedDict(
+    "GetDiscoveredSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
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
+PutCodeBindingResponseTypeDef = TypedDict(
+    "PutCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDiscovererResponseTypeDef = TypedDict(
+    "StartDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDiscovererResponseTypeDef = TypedDict(
+    "StopDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDiscovererResponseTypeDef = TypedDict(
+    "UpdateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSchemaResponseTypeDef = TypedDict(
     "UpdateSchemaResponseTypeDef",
     {
         "Description": str,
         "LastModified": datetime,
         "SchemaArn": str,
         "SchemaName": str,
         "SchemaVersion": str,
         "Tags": Dict[str, str],
         "Type": str,
         "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     {
         "Language": str,
@@ -996,42 +907,131 @@
 
 
 ListDiscoverersResponseTypeDef = TypedDict(
     "ListDiscoverersResponseTypeDef",
     {
         "Discoverers": List[DiscovererSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    {
+        "DiscovererIdPrefix": str,
+        "SourceArnPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    {
+        "RegistryNamePrefix": str,
+        "Scope": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "RegistryName": str,
+        "SchemaName": str,
+    },
+)
+_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "RegistryName": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "SchemaNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+
+_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "Keywords": str,
+        "RegistryName": str,
+    },
+)
+_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchSchemasRequestSearchSchemasPaginateTypeDef(
+    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
+    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
+):
+    pass
+
+
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "NextToken": str,
         "Registries": List[RegistrySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "NextToken": str,
         "SchemaVersions": List[SchemaVersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSchemaSummaryTypeDef = TypedDict(
     "SearchSchemaSummaryTypeDef",
     {
         "RegistryName": str,
@@ -1043,10 +1043,10 @@
 )
 
 SearchSchemasResponseTypeDef = TypedDict(
     "SearchSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SearchSchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/type_defs.pyi` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_schemas.type_defs import CreateDiscovererRequestRequestTypeDef
 
-    data: CreateDiscovererRequestRequestTypeDef = {...}
+    data: CreateDiscovererRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from aiobotocore.response import StreamingBody
@@ -22,79 +22,79 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateDiscovererRequestRequestTypeDef",
-    "CreateDiscovererResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateRegistryRequestRequestTypeDef",
-    "CreateRegistryResponseTypeDef",
     "CreateSchemaRequestRequestTypeDef",
-    "CreateSchemaResponseTypeDef",
     "DeleteDiscovererRequestRequestTypeDef",
     "DeleteRegistryRequestRequestTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DeleteSchemaRequestRequestTypeDef",
     "DeleteSchemaVersionRequestRequestTypeDef",
     "WaiterConfigTypeDef",
     "DescribeCodeBindingRequestRequestTypeDef",
-    "DescribeCodeBindingResponseTypeDef",
     "DescribeDiscovererRequestRequestTypeDef",
-    "DescribeDiscovererResponseTypeDef",
     "DescribeRegistryRequestRequestTypeDef",
-    "DescribeRegistryResponseTypeDef",
     "DescribeSchemaRequestRequestTypeDef",
-    "DescribeSchemaResponseTypeDef",
     "DiscovererSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ExportSchemaRequestRequestTypeDef",
-    "ExportSchemaResponseTypeDef",
     "GetCodeBindingSourceRequestRequestTypeDef",
-    "GetCodeBindingSourceResponseTypeDef",
     "GetDiscoveredSchemaRequestRequestTypeDef",
-    "GetDiscoveredSchemaResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListDiscoverersRequestRequestTypeDef",
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
     "ListRegistriesRequestRequestTypeDef",
     "RegistrySummaryTypeDef",
-    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
     "ListSchemaVersionsRequestRequestTypeDef",
     "SchemaVersionSummaryTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
     "SchemaSummaryTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "PutCodeBindingRequestRequestTypeDef",
-    "PutCodeBindingResponseTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchSchemaVersionSummaryTypeDef",
     "SearchSchemasRequestRequestTypeDef",
-    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "StartDiscovererRequestRequestTypeDef",
-    "StartDiscovererResponseTypeDef",
     "StopDiscovererRequestRequestTypeDef",
-    "StopDiscovererResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDiscovererRequestRequestTypeDef",
-    "UpdateDiscovererResponseTypeDef",
     "UpdateRegistryRequestRequestTypeDef",
-    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaRequestRequestTypeDef",
+    "CreateDiscovererResponseTypeDef",
+    "CreateRegistryResponseTypeDef",
+    "CreateSchemaResponseTypeDef",
+    "DescribeCodeBindingResponseTypeDef",
+    "DescribeDiscovererResponseTypeDef",
+    "DescribeRegistryResponseTypeDef",
+    "DescribeSchemaResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "ExportSchemaResponseTypeDef",
+    "GetCodeBindingSourceResponseTypeDef",
+    "GetDiscoveredSchemaResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "PutCodeBindingResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "StartDiscovererResponseTypeDef",
+    "StopDiscovererResponseTypeDef",
+    "UpdateDiscovererResponseTypeDef",
+    "UpdateRegistryResponseTypeDef",
     "UpdateSchemaResponseTypeDef",
     "DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     "ListDiscoverersResponseTypeDef",
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    "ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "SearchSchemasRequestSearchSchemasPaginateTypeDef",
     "ListRegistriesResponseTypeDef",
     "ListSchemaVersionsResponseTypeDef",
     "ListSchemasResponseTypeDef",
     "SearchSchemaSummaryTypeDef",
     "SearchSchemasResponseTypeDef",
 )
 
@@ -115,25 +115,22 @@
 )
 
 class CreateDiscovererRequestRequestTypeDef(
     _RequiredCreateDiscovererRequestRequestTypeDef, _OptionalCreateDiscovererRequestRequestTypeDef
 ):
     pass
 
-CreateDiscovererResponseTypeDef = TypedDict(
-    "CreateDiscovererResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredCreateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
@@ -149,25 +146,14 @@
 )
 
 class CreateRegistryRequestRequestTypeDef(
     _RequiredCreateRegistryRequestRequestTypeDef, _OptionalCreateRegistryRequestRequestTypeDef
 ):
     pass
 
-CreateRegistryResponseTypeDef = TypedDict(
-    "CreateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSchemaRequestRequestTypeDef",
     {
         "Content": str,
         "RegistryName": str,
         "SchemaName": str,
         "Type": TypeType,
@@ -183,29 +169,14 @@
 )
 
 class CreateSchemaRequestRequestTypeDef(
     _RequiredCreateSchemaRequestRequestTypeDef, _OptionalCreateSchemaRequestRequestTypeDef
 ):
     pass
 
-CreateSchemaResponseTypeDef = TypedDict(
-    "CreateSchemaResponseTypeDef",
-    {
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDiscovererRequestRequestTypeDef = TypedDict(
     "DeleteDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
@@ -268,64 +239,28 @@
 
 class DescribeCodeBindingRequestRequestTypeDef(
     _RequiredDescribeCodeBindingRequestRequestTypeDef,
     _OptionalDescribeCodeBindingRequestRequestTypeDef,
 ):
     pass
 
-DescribeCodeBindingResponseTypeDef = TypedDict(
-    "DescribeCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeDiscovererRequestRequestTypeDef = TypedDict(
     "DescribeDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-DescribeDiscovererResponseTypeDef = TypedDict(
-    "DescribeDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeRegistryRequestRequestTypeDef = TypedDict(
     "DescribeRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 
-DescribeRegistryResponseTypeDef = TypedDict(
-    "DescribeRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDescribeSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -338,50 +273,27 @@
 )
 
 class DescribeSchemaRequestRequestTypeDef(
     _RequiredDescribeSchemaRequestRequestTypeDef, _OptionalDescribeSchemaRequestRequestTypeDef
 ):
     pass
 
-DescribeSchemaResponseTypeDef = TypedDict(
-    "DescribeSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "Description": str,
-        "LastModified": datetime,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Tags": Dict[str, str],
-        "Type": str,
-        "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DiscovererSummaryTypeDef = TypedDict(
     "DiscovererSummaryTypeDef",
     {
         "DiscovererArn": str,
         "DiscovererId": str,
         "SourceArn": str,
         "State": DiscovererStateType,
         "CrossAccount": bool,
         "Tags": Dict[str, str],
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
 _RequiredExportSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredExportSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
         "Type": str,
     },
@@ -395,26 +307,14 @@
 )
 
 class ExportSchemaRequestRequestTypeDef(
     _RequiredExportSchemaRequestRequestTypeDef, _OptionalExportSchemaRequestRequestTypeDef
 ):
     pass
 
-ExportSchemaResponseTypeDef = TypedDict(
-    "ExportSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "SchemaArn": str,
-        "SchemaName": str,
-        "SchemaVersion": str,
-        "Type": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetCodeBindingSourceRequestRequestTypeDef = TypedDict(
     "_RequiredGetCodeBindingSourceRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -429,61 +329,36 @@
 
 class GetCodeBindingSourceRequestRequestTypeDef(
     _RequiredGetCodeBindingSourceRequestRequestTypeDef,
     _OptionalGetCodeBindingSourceRequestRequestTypeDef,
 ):
     pass
 
-GetCodeBindingSourceResponseTypeDef = TypedDict(
-    "GetCodeBindingSourceResponseTypeDef",
-    {
-        "Body": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetDiscoveredSchemaRequestRequestTypeDef = TypedDict(
     "GetDiscoveredSchemaRequestRequestTypeDef",
     {
         "Events": Sequence[str],
         "Type": TypeType,
     },
 )
 
-GetDiscoveredSchemaResponseTypeDef = TypedDict(
-    "GetDiscoveredSchemaResponseTypeDef",
-    {
-        "Content": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
     total=False,
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
-    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DiscovererIdPrefix": str,
-        "SourceArnPrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListDiscoverersRequestRequestTypeDef = TypedDict(
     "ListDiscoverersRequestRequestTypeDef",
     {
@@ -491,24 +366,14 @@
         "Limit": int,
         "NextToken": str,
         "SourceArnPrefix": str,
     },
     total=False,
 )
 
-ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
-    "ListRegistriesRequestListRegistriesPaginateTypeDef",
-    {
-        "RegistryNamePrefix": str,
-        "Scope": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListRegistriesRequestRequestTypeDef = TypedDict(
     "ListRegistriesRequestRequestTypeDef",
     {
         "Limit": int,
         "NextToken": str,
         "RegistryNamePrefix": str,
         "Scope": str,
@@ -522,35 +387,14 @@
         "RegistryArn": str,
         "RegistryName": str,
         "Tags": Dict[str, str],
     },
     total=False,
 )
 
-_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "RegistryName": str,
-        "SchemaName": str,
-    },
-)
-_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
-    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
-    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemaVersionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemaVersionsRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -576,35 +420,14 @@
         "SchemaName": str,
         "SchemaVersion": str,
         "Type": TypeType,
     },
     total=False,
 )
 
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "RegistryName": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "SchemaNamePrefix": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -637,32 +460,14 @@
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
 _RequiredPutCodeBindingRequestRequestTypeDef = TypedDict(
     "_RequiredPutCodeBindingRequestRequestTypeDef",
     {
         "Language": str,
         "RegistryName": str,
         "SchemaName": str,
     },
@@ -676,25 +481,14 @@
 )
 
 class PutCodeBindingRequestRequestTypeDef(
     _RequiredPutCodeBindingRequestRequestTypeDef, _OptionalPutCodeBindingRequestRequestTypeDef
 ):
     pass
 
-PutCodeBindingResponseTypeDef = TypedDict(
-    "PutCodeBindingResponseTypeDef",
-    {
-        "CreationDate": datetime,
-        "LastModified": datetime,
-        "SchemaVersion": str,
-        "Status": CodeGenerationStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutResourcePolicyRequestRequestTypeDef = TypedDict(
     "_RequiredPutResourcePolicyRequestRequestTypeDef",
     {
         "Policy": str,
     },
 )
 _OptionalPutResourcePolicyRequestRequestTypeDef = TypedDict(
@@ -707,34 +501,14 @@
 )
 
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "Policy": str,
-        "RevisionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
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
 SearchSchemaVersionSummaryTypeDef = TypedDict(
     "SearchSchemaVersionSummaryTypeDef",
     {
         "CreatedDate": datetime,
         "SchemaVersion": str,
         "Type": TypeType,
     },
@@ -758,67 +532,28 @@
 )
 
 class SearchSchemasRequestRequestTypeDef(
     _RequiredSearchSchemasRequestRequestTypeDef, _OptionalSearchSchemasRequestRequestTypeDef
 ):
     pass
 
-_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "Keywords": str,
-        "RegistryName": str,
-    },
-)
-_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
-    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchSchemasRequestSearchSchemasPaginateTypeDef(
-    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
-    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
-):
-    pass
-
 StartDiscovererRequestRequestTypeDef = TypedDict(
     "StartDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StartDiscovererResponseTypeDef = TypedDict(
-    "StartDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopDiscovererRequestRequestTypeDef = TypedDict(
     "StopDiscovererRequestRequestTypeDef",
     {
         "DiscovererId": str,
     },
 )
 
-StopDiscovererResponseTypeDef = TypedDict(
-    "StopDiscovererResponseTypeDef",
-    {
-        "DiscovererId": str,
-        "State": DiscovererStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -847,28 +582,14 @@
 )
 
 class UpdateDiscovererRequestRequestTypeDef(
     _RequiredUpdateDiscovererRequestRequestTypeDef, _OptionalUpdateDiscovererRequestRequestTypeDef
 ):
     pass
 
-UpdateDiscovererResponseTypeDef = TypedDict(
-    "UpdateDiscovererResponseTypeDef",
-    {
-        "Description": str,
-        "DiscovererArn": str,
-        "DiscovererId": str,
-        "SourceArn": str,
-        "State": DiscovererStateType,
-        "CrossAccount": bool,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateRegistryRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRegistryRequestRequestTypeDef",
     {
         "RegistryName": str,
     },
 )
 _OptionalUpdateRegistryRequestRequestTypeDef = TypedDict(
@@ -880,25 +601,14 @@
 )
 
 class UpdateRegistryRequestRequestTypeDef(
     _RequiredUpdateRegistryRequestRequestTypeDef, _OptionalUpdateRegistryRequestRequestTypeDef
 ):
     pass
 
-UpdateRegistryResponseTypeDef = TypedDict(
-    "UpdateRegistryResponseTypeDef",
-    {
-        "Description": str,
-        "RegistryArn": str,
-        "RegistryName": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredUpdateSchemaRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSchemaRequestRequestTypeDef",
     {
         "RegistryName": str,
         "SchemaName": str,
     },
 )
@@ -914,26 +624,233 @@
 )
 
 class UpdateSchemaRequestRequestTypeDef(
     _RequiredUpdateSchemaRequestRequestTypeDef, _OptionalUpdateSchemaRequestRequestTypeDef
 ):
     pass
 
+CreateDiscovererResponseTypeDef = TypedDict(
+    "CreateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRegistryResponseTypeDef = TypedDict(
+    "CreateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateSchemaResponseTypeDef = TypedDict(
+    "CreateSchemaResponseTypeDef",
+    {
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeCodeBindingResponseTypeDef = TypedDict(
+    "DescribeCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeDiscovererResponseTypeDef = TypedDict(
+    "DescribeDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeRegistryResponseTypeDef = TypedDict(
+    "DescribeRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeSchemaResponseTypeDef = TypedDict(
+    "DescribeSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "Description": str,
+        "LastModified": datetime,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Tags": Dict[str, str],
+        "Type": str,
+        "VersionCreatedDate": datetime,
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
+ExportSchemaResponseTypeDef = TypedDict(
+    "ExportSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "SchemaArn": str,
+        "SchemaName": str,
+        "SchemaVersion": str,
+        "Type": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCodeBindingSourceResponseTypeDef = TypedDict(
+    "GetCodeBindingSourceResponseTypeDef",
+    {
+        "Body": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDiscoveredSchemaResponseTypeDef = TypedDict(
+    "GetDiscoveredSchemaResponseTypeDef",
+    {
+        "Content": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
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
+PutCodeBindingResponseTypeDef = TypedDict(
+    "PutCodeBindingResponseTypeDef",
+    {
+        "CreationDate": datetime,
+        "LastModified": datetime,
+        "SchemaVersion": str,
+        "Status": CodeGenerationStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "RevisionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartDiscovererResponseTypeDef = TypedDict(
+    "StartDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopDiscovererResponseTypeDef = TypedDict(
+    "StopDiscovererResponseTypeDef",
+    {
+        "DiscovererId": str,
+        "State": DiscovererStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateDiscovererResponseTypeDef = TypedDict(
+    "UpdateDiscovererResponseTypeDef",
+    {
+        "Description": str,
+        "DiscovererArn": str,
+        "DiscovererId": str,
+        "SourceArn": str,
+        "State": DiscovererStateType,
+        "CrossAccount": bool,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateRegistryResponseTypeDef = TypedDict(
+    "UpdateRegistryResponseTypeDef",
+    {
+        "Description": str,
+        "RegistryArn": str,
+        "RegistryName": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateSchemaResponseTypeDef = TypedDict(
     "UpdateSchemaResponseTypeDef",
     {
         "Description": str,
         "LastModified": datetime,
         "SchemaArn": str,
         "SchemaName": str,
         "SchemaVersion": str,
         "Tags": Dict[str, str],
         "Type": str,
         "VersionCreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef = TypedDict(
     "_RequiredDescribeCodeBindingRequestCodeBindingExistsWaitTypeDef",
     {
         "Language": str,
@@ -957,42 +874,125 @@
     pass
 
 ListDiscoverersResponseTypeDef = TypedDict(
     "ListDiscoverersResponseTypeDef",
     {
         "Discoverers": List[DiscovererSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDiscoverersRequestListDiscoverersPaginateTypeDef = TypedDict(
+    "ListDiscoverersRequestListDiscoverersPaginateTypeDef",
+    {
+        "DiscovererIdPrefix": str,
+        "SourceArnPrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListRegistriesRequestListRegistriesPaginateTypeDef = TypedDict(
+    "ListRegistriesRequestListRegistriesPaginateTypeDef",
+    {
+        "RegistryNamePrefix": str,
+        "Scope": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "RegistryName": str,
+        "SchemaName": str,
+    },
+)
+_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef = TypedDict(
+    "_OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef(
+    _RequiredListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    _OptionalListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+):
+    pass
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "RegistryName": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "SchemaNamePrefix": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "Keywords": str,
+        "RegistryName": str,
     },
 )
+_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef = TypedDict(
+    "_OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchSchemasRequestSearchSchemasPaginateTypeDef(
+    _RequiredSearchSchemasRequestSearchSchemasPaginateTypeDef,
+    _OptionalSearchSchemasRequestSearchSchemasPaginateTypeDef,
+):
+    pass
 
 ListRegistriesResponseTypeDef = TypedDict(
     "ListRegistriesResponseTypeDef",
     {
         "NextToken": str,
         "Registries": List[RegistrySummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemaVersionsResponseTypeDef = TypedDict(
     "ListSchemaVersionsResponseTypeDef",
     {
         "NextToken": str,
         "SchemaVersions": List[SchemaVersionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSchemasResponseTypeDef = TypedDict(
     "ListSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchSchemaSummaryTypeDef = TypedDict(
     "SearchSchemaSummaryTypeDef",
     {
         "RegistryName": str,
@@ -1004,10 +1004,10 @@
 )
 
 SearchSchemasResponseTypeDef = TypedDict(
     "SearchSchemasResponseTypeDef",
     {
         "NextToken": str,
         "Schemas": List[SearchSchemaSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/waiter.py` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas/waiter.pyi` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/PKG-INFO` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-schemas
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Schemas 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore schemas type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore schemas type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-schemas"></a>
 
 # types-aiobotocore-schemas
 
 [![PyPI - types-aiobotocore-schemas](https://img.shields.io/pypi/v/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-schemas.svg?color=blue)](https://pypi.org/project/types-aiobotocore-schemas)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-schemas?color=blue)](https://pypistats.org/packages/types-aiobotocore-schemas)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-schemas)](https://pepy.tech/project/types-aiobotocore-schemas)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Schemas 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/schemas.html#Schemas)
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
 [types-aiobotocore-schemas docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_schemas/).
 
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
@@ -348,98 +347,98 @@
 )
 
 
 def check_value(value: CodeBindingExistsWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_schemas.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_schemas.type_defs import (
     CreateDiscovererRequestRequestTypeDef,
-    CreateDiscovererResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateRegistryRequestRequestTypeDef,
-    CreateRegistryResponseTypeDef,
     CreateSchemaRequestRequestTypeDef,
-    CreateSchemaResponseTypeDef,
     DeleteDiscovererRequestRequestTypeDef,
     DeleteRegistryRequestRequestTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DeleteSchemaRequestRequestTypeDef,
     DeleteSchemaVersionRequestRequestTypeDef,
     WaiterConfigTypeDef,
     DescribeCodeBindingRequestRequestTypeDef,
-    DescribeCodeBindingResponseTypeDef,
     DescribeDiscovererRequestRequestTypeDef,
-    DescribeDiscovererResponseTypeDef,
     DescribeRegistryRequestRequestTypeDef,
-    DescribeRegistryResponseTypeDef,
     DescribeSchemaRequestRequestTypeDef,
-    DescribeSchemaResponseTypeDef,
     DiscovererSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     ExportSchemaRequestRequestTypeDef,
-    ExportSchemaResponseTypeDef,
     GetCodeBindingSourceRequestRequestTypeDef,
-    GetCodeBindingSourceResponseTypeDef,
     GetDiscoveredSchemaRequestRequestTypeDef,
-    GetDiscoveredSchemaResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
-    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListDiscoverersRequestRequestTypeDef,
-    ListRegistriesRequestListRegistriesPaginateTypeDef,
     ListRegistriesRequestRequestTypeDef,
     RegistrySummaryTypeDef,
-    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
     ListSchemaVersionsRequestRequestTypeDef,
     SchemaVersionSummaryTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
     SchemaSummaryTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
-    PaginatorConfigTypeDef,
     PutCodeBindingRequestRequestTypeDef,
-    PutCodeBindingResponseTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    ResponseMetadataTypeDef,
     SearchSchemaVersionSummaryTypeDef,
     SearchSchemasRequestRequestTypeDef,
-    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     StartDiscovererRequestRequestTypeDef,
-    StartDiscovererResponseTypeDef,
     StopDiscovererRequestRequestTypeDef,
-    StopDiscovererResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDiscovererRequestRequestTypeDef,
-    UpdateDiscovererResponseTypeDef,
     UpdateRegistryRequestRequestTypeDef,
-    UpdateRegistryResponseTypeDef,
     UpdateSchemaRequestRequestTypeDef,
+    CreateDiscovererResponseTypeDef,
+    CreateRegistryResponseTypeDef,
+    CreateSchemaResponseTypeDef,
+    DescribeCodeBindingResponseTypeDef,
+    DescribeDiscovererResponseTypeDef,
+    DescribeRegistryResponseTypeDef,
+    DescribeSchemaResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    ExportSchemaResponseTypeDef,
+    GetCodeBindingSourceResponseTypeDef,
+    GetDiscoveredSchemaResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    PutCodeBindingResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    StartDiscovererResponseTypeDef,
+    StopDiscovererResponseTypeDef,
+    UpdateDiscovererResponseTypeDef,
+    UpdateRegistryResponseTypeDef,
     UpdateSchemaResponseTypeDef,
     DescribeCodeBindingRequestCodeBindingExistsWaitTypeDef,
     ListDiscoverersResponseTypeDef,
+    ListDiscoverersRequestListDiscoverersPaginateTypeDef,
+    ListRegistriesRequestListRegistriesPaginateTypeDef,
+    ListSchemaVersionsRequestListSchemaVersionsPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    SearchSchemasRequestSearchSchemasPaginateTypeDef,
     ListRegistriesResponseTypeDef,
     ListSchemaVersionsResponseTypeDef,
     ListSchemasResponseTypeDef,
     SearchSchemaSummaryTypeDef,
     SearchSchemasResponseTypeDef,
 )
 
 
-def get_structure() -> CreateDiscovererRequestRequestTypeDef:
+def get_value() -> CreateDiscovererRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-schemas-2.5.2/types_aiobotocore_schemas.egg-info/SOURCES.txt` & `types-aiobotocore-schemas-2.5.2.post1/types_aiobotocore_schemas.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-connectcases-2.5.2.tar.gz` & `tmp/types-aiobotocore-connectcases-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.tar", last modified: Sat Jul  8 01:43:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectcases-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
```

## Comparing `types-aiobotocore-connectcases-2.5.2.tar` & `types-aiobotocore-connectcases-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.337955 types-aiobotocore-connectcases-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-08 01:43:28.337955 types-aiobotocore-connectcases-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:28.337955 types-aiobotocore-connectcases-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:28:16.000000 types-aiobotocore-connectcases-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.337955 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23885 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    29522 2023-07-08 01:28:18.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29478 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:17.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.337955 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16590 2023-07-08 01:43:28.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:28.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:28.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:28.000000 types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:35:53.000000 types-aiobotocore-connectcases-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23950 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23909 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8583 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    32011 2023-08-02 14:35:55.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31963 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:54.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16868 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:07.000000 types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectcases-2.5.2/LICENSE` & `types-aiobotocore-connectcases-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2/PKG-INFO` & `types-aiobotocore-connectcases-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectcases type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore connectcases type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectcases"></a>
 
 # types-aiobotocore-connectcases
 
 [![PyPI - types-aiobotocore-connectcases](https://img.shields.io/pypi/v/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectcases?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectcases)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectCases 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
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
@@ -319,120 +318,130 @@
 )
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectcases.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     CaseSummaryTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
     GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
+    FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
+    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
+    SectionOutputTypeDef,
     SectionTypeDef,
     CreateCaseRequestRequestTypeDef,
     FieldFilterTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
     UpdateCaseRequestRequestTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
     SearchRelatedItemsResponseTypeDef,
+    LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
     CaseFilterTypeDef,
     SearchCasesResponseTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
+    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
-    CreateLayoutRequestRequestTypeDef,
     GetLayoutResponseTypeDef,
+    CreateLayoutRequestRequestTypeDef,
+    LayoutContentUnionTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
-def get_structure() -> FieldIdentifierTypeDef:
+def get_value() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectcases-2.5.2/README.md` & `types-aiobotocore-connectcases-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-connectcases"></a>
 
 # types-aiobotocore-connectcases
 
 [![PyPI - types-aiobotocore-connectcases](https://img.shields.io/pypi/v/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectcases?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectcases)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectCases 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
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
@@ -286,120 +286,130 @@
 )
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectcases.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     CaseSummaryTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
     GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
+    FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
+    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
+    SectionOutputTypeDef,
     SectionTypeDef,
     CreateCaseRequestRequestTypeDef,
     FieldFilterTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
     UpdateCaseRequestRequestTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
     SearchRelatedItemsResponseTypeDef,
+    LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
     CaseFilterTypeDef,
     SearchCasesResponseTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
+    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
-    CreateLayoutRequestRequestTypeDef,
     GetLayoutResponseTypeDef,
+    CreateLayoutRequestRequestTypeDef,
+    LayoutContentUnionTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
-def get_structure() -> FieldIdentifierTypeDef:
+def get_value() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectcases-2.5.2/setup.py` & `types-aiobotocore-connectcases-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectcases",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_connectcases"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with"
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
-    keywords="aiobotocore connectcases type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore connectcases type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_connectcases": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/"
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/__init__.py` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/__init__.pyi` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/__main__.py` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ConnectCases 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases\nOther"
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

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/client.py` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
     FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentTypeDef,
+    LayoutContentUnionTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -172,15 +172,15 @@
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_field)
         """
 
     async def create_layout(
-        self, *, content: LayoutContentTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_layout)
         """
@@ -365,15 +365,15 @@
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_templates)
         """
 
     async def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#put_case_event_configuration)
@@ -450,15 +450,20 @@
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_field)
         """
 
     async def update_layout(
-        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
+        self,
+        *,
+        domainId: str,
+        layoutId: str,
+        content: LayoutContentUnionTypeDef = ...,
+        name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_layout)
         """
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/client.pyi` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -29,25 +29,25 @@
     CreateCaseResponseTypeDef,
     CreateDomainResponseTypeDef,
     CreateFieldResponseTypeDef,
     CreateLayoutResponseTypeDef,
     CreateRelatedItemResponseTypeDef,
     CreateTemplateResponseTypeDef,
     EmptyResponseMetadataTypeDef,
-    EventBridgeConfigurationTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     FieldIdentifierTypeDef,
     FieldOptionTypeDef,
     FieldValueTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
     GetCaseResponseTypeDef,
     GetDomainResponseTypeDef,
     GetLayoutResponseTypeDef,
     GetTemplateResponseTypeDef,
     LayoutConfigurationTypeDef,
-    LayoutContentTypeDef,
+    LayoutContentUnionTypeDef,
     ListCasesForContactResponseTypeDef,
     ListDomainsResponseTypeDef,
     ListFieldOptionsResponseTypeDef,
     ListFieldsResponseTypeDef,
     ListLayoutsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTemplatesResponseTypeDef,
@@ -160,15 +160,15 @@
         """
         Creates a field in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_field)
         """
     async def create_layout(
-        self, *, content: LayoutContentTypeDef, domainId: str, name: str
+        self, *, content: LayoutContentUnionTypeDef, domainId: str, name: str
     ) -> CreateLayoutResponseTypeDef:
         """
         Creates a layout in the Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.create_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#create_layout)
         """
@@ -336,15 +336,15 @@
         """
         Lists all of the templates in a Cases domain.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.list_templates)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#list_templates)
         """
     async def put_case_event_configuration(
-        self, *, domainId: str, eventBridge: EventBridgeConfigurationTypeDef
+        self, *, domainId: str, eventBridge: EventBridgeConfigurationUnionTypeDef
     ) -> Dict[str, Any]:
         """
         API for adding case event publishing configuration See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/connectcases-2022-10-03/PutCaseEventConfiguration).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.put_case_event_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#put_case_event_configuration)
@@ -414,15 +414,20 @@
         """
         Updates the properties of an existing field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_field)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_field)
         """
     async def update_layout(
-        self, *, domainId: str, layoutId: str, content: LayoutContentTypeDef = ..., name: str = ...
+        self,
+        *,
+        domainId: str,
+        layoutId: str,
+        content: LayoutContentUnionTypeDef = ...,
+        name: str = ...
     ) -> Dict[str, Any]:
         """
         Updates the attributes of an existing layout.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Client.update_layout)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/client/#update_layout)
         """
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/literals.py` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/literals.pyi` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/paginator.py` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchcasespaginator)
         """
 
 
@@ -80,13 +80,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/paginator.pyi` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self,
         *,
         domainId: str,
         fields: Sequence[FieldIdentifierTypeDef] = ...,
         filter: "CaseFilterTypeDef" = ...,
         searchTerm: str = ...,
         sorts: Sequence[SortTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchCasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchCases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchcasespaginator)
         """
 
 class SearchRelatedItemsPaginator(AioPaginator):
@@ -76,13 +76,13 @@
 
     def paginate(
         self,
         *,
         caseId: str,
         domainId: str,
         filters: Sequence[RelatedItemTypeFilterTypeDef] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchRelatedItemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases.Paginator.SearchRelatedItems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/paginators/#searchrelateditemspaginator)
         """
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/type_defs.py` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef
 
-    data: FieldIdentifierTypeDef = {...}
+    data: FieldIdentifierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -34,103 +34,113 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
     "CaseSummaryTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
-    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "CreateDomainResponseTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
+    "CreateTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDomainResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
+    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
+    "SectionOutputTypeDef",
     "SectionTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "UpdateCaseRequestRequestTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
     "SearchRelatedItemsResponseTypeDef",
+    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
+    "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
+    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "CreateLayoutRequestRequestTypeDef",
     "GetLayoutResponseTypeDef",
+    "CreateLayoutRequestRequestTypeDef",
+    "LayoutContentUnionTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
@@ -177,14 +187,25 @@
 )
 
 
 class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
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
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -236,40 +257,21 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -285,41 +287,14 @@
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
 
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -327,23 +302,14 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -352,21 +318,14 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
@@ -408,27 +367,14 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -554,22 +500,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
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
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -605,25 +543,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -671,18 +598,25 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
+    {
+        "fields": List[FieldIdentifierTypeDef],
+    },
+)
+
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": List[FieldIdentifierTypeDef],
+        "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
 _RequiredGetCaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetCaseRequestRequestTypeDef",
     {
         "caseId": str,
@@ -706,15 +640,98 @@
 
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
+        "fieldId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
+    {
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
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
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
     "BatchPutFieldOptionsRequestRequestTypeDef",
     {
         "domainId": str,
@@ -724,32 +741,32 @@
 )
 
 ListFieldOptionsResponseTypeDef = TypedDict(
     "ListFieldOptionsResponseTypeDef",
     {
         "nextToken": str,
         "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
         "comment": CommentContentTypeDef,
@@ -808,15 +825,15 @@
         "layoutConfiguration": LayoutConfigurationTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
@@ -843,18 +860,37 @@
 
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredFieldGroupOutputTypeDef = TypedDict(
+    "_RequiredFieldGroupOutputTypeDef",
+    {
+        "fields": List[FieldItemTypeDef],
+    },
+)
+_OptionalFieldGroupOutputTypeDef = TypedDict(
+    "_OptionalFieldGroupOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
+
+class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
+    pass
+
+
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -871,15 +907,15 @@
 
 
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
@@ -888,24 +924,24 @@
 )
 
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -940,27 +976,36 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
 
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
+    {
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
+    },
+    total=False,
+)
+
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
@@ -1022,15 +1067,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1045,14 +1090,22 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
     },
 )
 
+SectionOutputTypeDef = TypedDict(
+    "SectionOutputTypeDef",
+    {
+        "fieldGroup": FieldGroupOutputTypeDef,
+    },
+    total=False,
+)
+
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
@@ -1096,15 +1149,15 @@
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesResponseItemTypeDef = TypedDict(
     "_RequiredSearchCasesResponseItemTypeDef",
     {
         "caseId": str,
@@ -1132,14 +1185,35 @@
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
     },
 )
 
+_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEventBridgeConfigurationOutputTypeDef",
+    {
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class EventBridgeConfigurationOutputTypeDef(
+    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1158,18 +1232,26 @@
 
 
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LayoutSectionsOutputTypeDef = TypedDict(
+    "LayoutSectionsOutputTypeDef",
+    {
+        "sections": List[SectionOutputTypeDef],
+    },
+    total=False,
+)
+
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
@@ -1185,72 +1267,93 @@
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EventBridgeConfigurationUnionTypeDef = Union[
+    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
+]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
+BasicLayoutOutputTypeDef = TypedDict(
+    "BasicLayoutOutputTypeDef",
+    {
+        "moreInfo": LayoutSectionsOutputTypeDef,
+        "topPanel": LayoutSectionsOutputTypeDef,
+    },
+    total=False,
+)
+
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
     },
     total=False,
 )
 
-LayoutContentTypeDef = TypedDict(
-    "LayoutContentTypeDef",
+LayoutContentOutputTypeDef = TypedDict(
+    "LayoutContentOutputTypeDef",
     {
-        "basic": BasicLayoutTypeDef,
+        "basic": BasicLayoutOutputTypeDef,
     },
     total=False,
 )
 
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
+LayoutContentTypeDef = TypedDict(
+    "LayoutContentTypeDef",
     {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
-        "name": str,
+        "basic": BasicLayoutTypeDef,
     },
+    total=False,
 )
 
 GetLayoutResponseTypeDef = TypedDict(
     "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentTypeDef,
+        "content": LayoutContentOutputTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
+    {
+        "content": LayoutContentTypeDef,
+        "domainId": str,
+        "name": str,
     },
 )
 
+LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases/type_defs.pyi` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases/type_defs.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_connectcases.type_defs import FieldIdentifierTypeDef
 
-    data: FieldIdentifierTypeDef = {...}
+    data: FieldIdentifierTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     DomainStatusType,
     FieldNamespaceType,
     FieldTypeType,
     OrderType,
     RelatedItemTypeType,
@@ -33,103 +33,113 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FieldIdentifierTypeDef",
     "FieldErrorTypeDef",
     "GetFieldResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "FieldOptionTypeDef",
     "FieldOptionErrorTypeDef",
     "CaseSummaryTypeDef",
     "CommentContentTypeDef",
     "ContactContentTypeDef",
     "ContactFilterTypeDef",
     "ContactTypeDef",
-    "CreateCaseResponseTypeDef",
     "CreateDomainRequestRequestTypeDef",
-    "CreateDomainResponseTypeDef",
     "CreateFieldRequestRequestTypeDef",
-    "CreateFieldResponseTypeDef",
-    "CreateLayoutResponseTypeDef",
-    "CreateRelatedItemResponseTypeDef",
     "LayoutConfigurationTypeDef",
     "RequiredFieldTypeDef",
-    "CreateTemplateResponseTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainSummaryTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "RelatedItemEventIncludedDataTypeDef",
     "FieldItemTypeDef",
     "FieldSummaryTypeDef",
     "FieldValueUnionTypeDef",
     "GetCaseEventConfigurationRequestRequestTypeDef",
     "GetDomainRequestRequestTypeDef",
-    "GetDomainResponseTypeDef",
     "GetLayoutRequestRequestTypeDef",
     "GetTemplateRequestRequestTypeDef",
     "LayoutSummaryTypeDef",
     "ListCasesForContactRequestRequestTypeDef",
     "ListDomainsRequestRequestTypeDef",
     "ListFieldOptionsRequestRequestTypeDef",
     "ListFieldsRequestRequestTypeDef",
     "ListLayoutsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListTemplatesRequestRequestTypeDef",
     "TemplateSummaryTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "SortTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFieldRequestRequestTypeDef",
     "BatchGetFieldRequestRequestTypeDef",
+    "CaseEventIncludedDataOutputTypeDef",
     "CaseEventIncludedDataTypeDef",
     "GetCaseRequestRequestTypeDef",
     "BatchGetFieldResponseTypeDef",
+    "CreateCaseResponseTypeDef",
+    "CreateDomainResponseTypeDef",
+    "CreateFieldResponseTypeDef",
+    "CreateLayoutResponseTypeDef",
+    "CreateRelatedItemResponseTypeDef",
+    "CreateTemplateResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDomainResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "BatchPutFieldOptionsRequestRequestTypeDef",
     "ListFieldOptionsResponseTypeDef",
     "BatchPutFieldOptionsResponseTypeDef",
     "ListCasesForContactResponseTypeDef",
     "RelatedItemContentTypeDef",
     "RelatedItemTypeFilterTypeDef",
     "RelatedItemInputContentTypeDef",
     "CreateTemplateRequestRequestTypeDef",
     "GetTemplateResponseTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
     "ListDomainsResponseTypeDef",
+    "FieldGroupOutputTypeDef",
     "FieldGroupTypeDef",
     "ListFieldsResponseTypeDef",
     "FieldValueTypeDef",
     "ListLayoutsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "SearchCasesRequestRequestTypeDef",
     "SearchCasesRequestSearchCasesPaginateTypeDef",
+    "EventIncludedDataOutputTypeDef",
     "EventIncludedDataTypeDef",
     "SearchRelatedItemsResponseItemTypeDef",
     "SearchRelatedItemsRequestRequestTypeDef",
     "SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     "CreateRelatedItemRequestRequestTypeDef",
+    "SectionOutputTypeDef",
     "SectionTypeDef",
     "CreateCaseRequestRequestTypeDef",
     "FieldFilterTypeDef",
     "GetCaseResponseTypeDef",
     "SearchCasesResponseItemTypeDef",
     "UpdateCaseRequestRequestTypeDef",
+    "EventBridgeConfigurationOutputTypeDef",
     "EventBridgeConfigurationTypeDef",
     "SearchRelatedItemsResponseTypeDef",
+    "LayoutSectionsOutputTypeDef",
     "LayoutSectionsTypeDef",
     "CaseFilterTypeDef",
     "SearchCasesResponseTypeDef",
     "GetCaseEventConfigurationResponseTypeDef",
+    "EventBridgeConfigurationUnionTypeDef",
     "PutCaseEventConfigurationRequestRequestTypeDef",
+    "BasicLayoutOutputTypeDef",
     "BasicLayoutTypeDef",
+    "LayoutContentOutputTypeDef",
     "LayoutContentTypeDef",
-    "CreateLayoutRequestRequestTypeDef",
     "GetLayoutResponseTypeDef",
+    "CreateLayoutRequestRequestTypeDef",
+    "LayoutContentUnionTypeDef",
     "UpdateLayoutRequestRequestTypeDef",
 )
 
 FieldIdentifierTypeDef = TypedDict(
     "FieldIdentifierTypeDef",
     {
         "id": str,
@@ -172,14 +182,25 @@
     },
     total=False,
 )
 
 class GetFieldResponseTypeDef(_RequiredGetFieldResponseTypeDef, _OptionalGetFieldResponseTypeDef):
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
 FieldOptionTypeDef = TypedDict(
     "FieldOptionTypeDef",
     {
         "active": bool,
         "name": str,
         "value": str,
     },
@@ -231,40 +252,21 @@
 ContactTypeDef = TypedDict(
     "ContactTypeDef",
     {
         "contactArn": str,
     },
 )
 
-CreateCaseResponseTypeDef = TypedDict(
-    "CreateCaseResponseTypeDef",
-    {
-        "caseArn": str,
-        "caseId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CreateDomainRequestRequestTypeDef = TypedDict(
     "CreateDomainRequestRequestTypeDef",
     {
         "name": str,
     },
 )
 
-CreateDomainResponseTypeDef = TypedDict(
-    "CreateDomainResponseTypeDef",
-    {
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateFieldRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "name": str,
         "type": FieldTypeType,
     },
@@ -278,41 +280,14 @@
 )
 
 class CreateFieldRequestRequestTypeDef(
     _RequiredCreateFieldRequestRequestTypeDef, _OptionalCreateFieldRequestRequestTypeDef
 ):
     pass
 
-CreateFieldResponseTypeDef = TypedDict(
-    "CreateFieldResponseTypeDef",
-    {
-        "fieldArn": str,
-        "fieldId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateLayoutResponseTypeDef = TypedDict(
-    "CreateLayoutResponseTypeDef",
-    {
-        "layoutArn": str,
-        "layoutId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-CreateRelatedItemResponseTypeDef = TypedDict(
-    "CreateRelatedItemResponseTypeDef",
-    {
-        "relatedItemArn": str,
-        "relatedItemId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "defaultLayout": str,
     },
     total=False,
 )
@@ -320,23 +295,14 @@
 RequiredFieldTypeDef = TypedDict(
     "RequiredFieldTypeDef",
     {
         "fieldId": str,
     },
 )
 
-CreateTemplateResponseTypeDef = TypedDict(
-    "CreateTemplateResponseTypeDef",
-    {
-        "templateArn": str,
-        "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteDomainRequestRequestTypeDef = TypedDict(
     "DeleteDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
@@ -345,21 +311,14 @@
     {
         "domainArn": str,
         "domainId": str,
         "name": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RelatedItemEventIncludedDataTypeDef = TypedDict(
     "RelatedItemEventIncludedDataTypeDef",
     {
         "includeContent": bool,
     },
 )
 
@@ -401,27 +360,14 @@
 GetDomainRequestRequestTypeDef = TypedDict(
     "GetDomainRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 
-GetDomainResponseTypeDef = TypedDict(
-    "GetDomainResponseTypeDef",
-    {
-        "createdTime": datetime,
-        "domainArn": str,
-        "domainId": str,
-        "domainStatus": DomainStatusType,
-        "name": str,
-        "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetLayoutRequestRequestTypeDef = TypedDict(
     "GetLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
@@ -539,22 +485,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "arn": str,
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
 _RequiredListTemplatesRequestRequestTypeDef = TypedDict(
     "_RequiredListTemplatesRequestRequestTypeDef",
     {
         "domainId": str,
     },
 )
 _OptionalListTemplatesRequestRequestTypeDef = TypedDict(
@@ -588,25 +526,14 @@
         "MaxItems": int,
         "PageSize": int,
         "StartingToken": str,
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
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "fieldId": str,
         "sortOrder": OrderType,
     },
 )
@@ -652,18 +579,25 @@
     "BatchGetFieldRequestRequestTypeDef",
     {
         "domainId": str,
         "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
+CaseEventIncludedDataOutputTypeDef = TypedDict(
+    "CaseEventIncludedDataOutputTypeDef",
+    {
+        "fields": List[FieldIdentifierTypeDef],
+    },
+)
+
 CaseEventIncludedDataTypeDef = TypedDict(
     "CaseEventIncludedDataTypeDef",
     {
-        "fields": List[FieldIdentifierTypeDef],
+        "fields": Sequence[FieldIdentifierTypeDef],
     },
 )
 
 _RequiredGetCaseRequestRequestTypeDef = TypedDict(
     "_RequiredGetCaseRequestRequestTypeDef",
     {
         "caseId": str,
@@ -685,15 +619,98 @@
     pass
 
 BatchGetFieldResponseTypeDef = TypedDict(
     "BatchGetFieldResponseTypeDef",
     {
         "errors": List[FieldErrorTypeDef],
         "fields": List[GetFieldResponseTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateCaseResponseTypeDef = TypedDict(
+    "CreateCaseResponseTypeDef",
+    {
+        "caseArn": str,
+        "caseId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateDomainResponseTypeDef = TypedDict(
+    "CreateDomainResponseTypeDef",
+    {
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateFieldResponseTypeDef = TypedDict(
+    "CreateFieldResponseTypeDef",
+    {
+        "fieldArn": str,
+        "fieldId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayoutResponseTypeDef = TypedDict(
+    "CreateLayoutResponseTypeDef",
+    {
+        "layoutArn": str,
+        "layoutId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateRelatedItemResponseTypeDef = TypedDict(
+    "CreateRelatedItemResponseTypeDef",
+    {
+        "relatedItemArn": str,
+        "relatedItemId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateTemplateResponseTypeDef = TypedDict(
+    "CreateTemplateResponseTypeDef",
+    {
+        "templateArn": str,
+        "templateId": str,
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
+GetDomainResponseTypeDef = TypedDict(
+    "GetDomainResponseTypeDef",
+    {
+        "createdTime": datetime,
+        "domainArn": str,
+        "domainId": str,
+        "domainStatus": DomainStatusType,
+        "name": str,
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutFieldOptionsRequestRequestTypeDef = TypedDict(
     "BatchPutFieldOptionsRequestRequestTypeDef",
     {
         "domainId": str,
@@ -703,32 +720,32 @@
 )
 
 ListFieldOptionsResponseTypeDef = TypedDict(
     "ListFieldOptionsResponseTypeDef",
     {
         "nextToken": str,
         "options": List[FieldOptionTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutFieldOptionsResponseTypeDef = TypedDict(
     "BatchPutFieldOptionsResponseTypeDef",
     {
         "errors": List[FieldOptionErrorTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCasesForContactResponseTypeDef = TypedDict(
     "ListCasesForContactResponseTypeDef",
     {
         "cases": List[CaseSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RelatedItemContentTypeDef = TypedDict(
     "RelatedItemContentTypeDef",
     {
         "comment": CommentContentTypeDef,
@@ -785,15 +802,15 @@
         "layoutConfiguration": LayoutConfigurationTypeDef,
         "name": str,
         "requiredFields": List[RequiredFieldTypeDef],
         "status": TemplateStatusType,
         "tags": Dict[str, str],
         "templateArn": str,
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateTemplateRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTemplateRequestRequestTypeDef",
     {
         "domainId": str,
@@ -818,18 +835,35 @@
     pass
 
 ListDomainsResponseTypeDef = TypedDict(
     "ListDomainsResponseTypeDef",
     {
         "domains": List[DomainSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredFieldGroupOutputTypeDef = TypedDict(
+    "_RequiredFieldGroupOutputTypeDef",
+    {
+        "fields": List[FieldItemTypeDef],
+    },
+)
+_OptionalFieldGroupOutputTypeDef = TypedDict(
+    "_OptionalFieldGroupOutputTypeDef",
+    {
+        "name": str,
+    },
+    total=False,
+)
+
+class FieldGroupOutputTypeDef(_RequiredFieldGroupOutputTypeDef, _OptionalFieldGroupOutputTypeDef):
+    pass
+
 _RequiredFieldGroupTypeDef = TypedDict(
     "_RequiredFieldGroupTypeDef",
     {
         "fields": Sequence[FieldItemTypeDef],
     },
 )
 _OptionalFieldGroupTypeDef = TypedDict(
@@ -844,15 +878,15 @@
     pass
 
 ListFieldsResponseTypeDef = TypedDict(
     "ListFieldsResponseTypeDef",
     {
         "fields": List[FieldSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 FieldValueTypeDef = TypedDict(
     "FieldValueTypeDef",
     {
         "id": str,
@@ -861,24 +895,24 @@
 )
 
 ListLayoutsResponseTypeDef = TypedDict(
     "ListLayoutsResponseTypeDef",
     {
         "layouts": List[LayoutSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "nextToken": str,
         "templates": List[TemplateSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesRequestRequestTypeDef = TypedDict(
     "_RequiredSearchCasesRequestRequestTypeDef",
     {
         "domainId": str,
@@ -911,25 +945,34 @@
 _OptionalSearchCasesRequestSearchCasesPaginateTypeDef = TypedDict(
     "_OptionalSearchCasesRequestSearchCasesPaginateTypeDef",
     {
         "fields": Sequence[FieldIdentifierTypeDef],
         "filter": "CaseFilterTypeDef",
         "searchTerm": str,
         "sorts": Sequence[SortTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchCasesRequestSearchCasesPaginateTypeDef(
     _RequiredSearchCasesRequestSearchCasesPaginateTypeDef,
     _OptionalSearchCasesRequestSearchCasesPaginateTypeDef,
 ):
     pass
 
+EventIncludedDataOutputTypeDef = TypedDict(
+    "EventIncludedDataOutputTypeDef",
+    {
+        "caseData": CaseEventIncludedDataOutputTypeDef,
+        "relatedItemData": RelatedItemEventIncludedDataTypeDef,
+    },
+    total=False,
+)
+
 EventIncludedDataTypeDef = TypedDict(
     "EventIncludedDataTypeDef",
     {
         "caseData": CaseEventIncludedDataTypeDef,
         "relatedItemData": RelatedItemEventIncludedDataTypeDef,
     },
     total=False,
@@ -987,15 +1030,15 @@
         "domainId": str,
     },
 )
 _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef = TypedDict(
     "_OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef",
     {
         "filters": Sequence[RelatedItemTypeFilterTypeDef],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 class SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef(
     _RequiredSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     _OptionalSearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
@@ -1008,14 +1051,22 @@
         "caseId": str,
         "content": RelatedItemInputContentTypeDef,
         "domainId": str,
         "type": RelatedItemTypeType,
     },
 )
 
+SectionOutputTypeDef = TypedDict(
+    "SectionOutputTypeDef",
+    {
+        "fieldGroup": FieldGroupOutputTypeDef,
+    },
+    total=False,
+)
+
 SectionTypeDef = TypedDict(
     "SectionTypeDef",
     {
         "fieldGroup": FieldGroupTypeDef,
     },
     total=False,
 )
@@ -1057,15 +1108,15 @@
 GetCaseResponseTypeDef = TypedDict(
     "GetCaseResponseTypeDef",
     {
         "fields": List[FieldValueTypeDef],
         "nextToken": str,
         "tags": Dict[str, str],
         "templateId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSearchCasesResponseItemTypeDef = TypedDict(
     "_RequiredSearchCasesResponseItemTypeDef",
     {
         "caseId": str,
@@ -1091,14 +1142,33 @@
     {
         "caseId": str,
         "domainId": str,
         "fields": Sequence[FieldValueTypeDef],
     },
 )
 
+_RequiredEventBridgeConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEventBridgeConfigurationOutputTypeDef",
+    {
+        "enabled": bool,
+    },
+)
+_OptionalEventBridgeConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEventBridgeConfigurationOutputTypeDef",
+    {
+        "includedData": EventIncludedDataOutputTypeDef,
+    },
+    total=False,
+)
+
+class EventBridgeConfigurationOutputTypeDef(
+    _RequiredEventBridgeConfigurationOutputTypeDef, _OptionalEventBridgeConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredEventBridgeConfigurationTypeDef = TypedDict(
     "_RequiredEventBridgeConfigurationTypeDef",
     {
         "enabled": bool,
     },
 )
 _OptionalEventBridgeConfigurationTypeDef = TypedDict(
@@ -1115,18 +1185,26 @@
     pass
 
 SearchRelatedItemsResponseTypeDef = TypedDict(
     "SearchRelatedItemsResponseTypeDef",
     {
         "nextToken": str,
         "relatedItems": List[SearchRelatedItemsResponseItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+LayoutSectionsOutputTypeDef = TypedDict(
+    "LayoutSectionsOutputTypeDef",
+    {
+        "sections": List[SectionOutputTypeDef],
+    },
+    total=False,
+)
+
 LayoutSectionsTypeDef = TypedDict(
     "LayoutSectionsTypeDef",
     {
         "sections": Sequence[SectionTypeDef],
     },
     total=False,
 )
@@ -1142,72 +1220,93 @@
 )
 
 SearchCasesResponseTypeDef = TypedDict(
     "SearchCasesResponseTypeDef",
     {
         "cases": List[SearchCasesResponseItemTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCaseEventConfigurationResponseTypeDef = TypedDict(
     "GetCaseEventConfigurationResponseTypeDef",
     {
-        "eventBridge": EventBridgeConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "eventBridge": EventBridgeConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+EventBridgeConfigurationUnionTypeDef = Union[
+    EventBridgeConfigurationTypeDef, EventBridgeConfigurationOutputTypeDef
+]
 PutCaseEventConfigurationRequestRequestTypeDef = TypedDict(
     "PutCaseEventConfigurationRequestRequestTypeDef",
     {
         "domainId": str,
         "eventBridge": EventBridgeConfigurationTypeDef,
     },
 )
 
+BasicLayoutOutputTypeDef = TypedDict(
+    "BasicLayoutOutputTypeDef",
+    {
+        "moreInfo": LayoutSectionsOutputTypeDef,
+        "topPanel": LayoutSectionsOutputTypeDef,
+    },
+    total=False,
+)
+
 BasicLayoutTypeDef = TypedDict(
     "BasicLayoutTypeDef",
     {
         "moreInfo": LayoutSectionsTypeDef,
         "topPanel": LayoutSectionsTypeDef,
     },
     total=False,
 )
 
-LayoutContentTypeDef = TypedDict(
-    "LayoutContentTypeDef",
+LayoutContentOutputTypeDef = TypedDict(
+    "LayoutContentOutputTypeDef",
     {
-        "basic": BasicLayoutTypeDef,
+        "basic": BasicLayoutOutputTypeDef,
     },
     total=False,
 )
 
-CreateLayoutRequestRequestTypeDef = TypedDict(
-    "CreateLayoutRequestRequestTypeDef",
+LayoutContentTypeDef = TypedDict(
+    "LayoutContentTypeDef",
     {
-        "content": LayoutContentTypeDef,
-        "domainId": str,
-        "name": str,
+        "basic": BasicLayoutTypeDef,
     },
+    total=False,
 )
 
 GetLayoutResponseTypeDef = TypedDict(
     "GetLayoutResponseTypeDef",
     {
-        "content": LayoutContentTypeDef,
+        "content": LayoutContentOutputTypeDef,
         "layoutArn": str,
         "layoutId": str,
         "name": str,
         "tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLayoutRequestRequestTypeDef = TypedDict(
+    "CreateLayoutRequestRequestTypeDef",
+    {
+        "content": LayoutContentTypeDef,
+        "domainId": str,
+        "name": str,
     },
 )
 
+LayoutContentUnionTypeDef = Union[LayoutContentTypeDef, LayoutContentOutputTypeDef]
 _RequiredUpdateLayoutRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateLayoutRequestRequestTypeDef",
     {
         "domainId": str,
         "layoutId": str,
     },
 )
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/PKG-INFO` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectcases
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectCases 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectcases type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore connectcases type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectcases"></a>
 
 # types-aiobotocore-connectcases
 
 [![PyPI - types-aiobotocore-connectcases](https://img.shields.io/pypi/v/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectcases.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectcases)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectcases?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectcases)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectcases)](https://pepy.tech/project/types-aiobotocore-connectcases)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectCases 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectcases.html#ConnectCases)
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
 [types-aiobotocore-connectcases docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectcases/).
 
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
@@ -319,120 +318,130 @@
 )
 
 
 def check_value(value: CommentBodyTextTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectcases.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectcases.type_defs import (
     FieldIdentifierTypeDef,
     FieldErrorTypeDef,
     GetFieldResponseTypeDef,
+    ResponseMetadataTypeDef,
     FieldOptionTypeDef,
     FieldOptionErrorTypeDef,
     CaseSummaryTypeDef,
     CommentContentTypeDef,
     ContactContentTypeDef,
     ContactFilterTypeDef,
     ContactTypeDef,
-    CreateCaseResponseTypeDef,
     CreateDomainRequestRequestTypeDef,
-    CreateDomainResponseTypeDef,
     CreateFieldRequestRequestTypeDef,
-    CreateFieldResponseTypeDef,
-    CreateLayoutResponseTypeDef,
-    CreateRelatedItemResponseTypeDef,
     LayoutConfigurationTypeDef,
     RequiredFieldTypeDef,
-    CreateTemplateResponseTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainSummaryTypeDef,
-    EmptyResponseMetadataTypeDef,
     RelatedItemEventIncludedDataTypeDef,
     FieldItemTypeDef,
     FieldSummaryTypeDef,
     FieldValueUnionTypeDef,
     GetCaseEventConfigurationRequestRequestTypeDef,
     GetDomainRequestRequestTypeDef,
-    GetDomainResponseTypeDef,
     GetLayoutRequestRequestTypeDef,
     GetTemplateRequestRequestTypeDef,
     LayoutSummaryTypeDef,
     ListCasesForContactRequestRequestTypeDef,
     ListDomainsRequestRequestTypeDef,
     ListFieldOptionsRequestRequestTypeDef,
     ListFieldsRequestRequestTypeDef,
     ListLayoutsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListTemplatesRequestRequestTypeDef,
     TemplateSummaryTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     SortTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFieldRequestRequestTypeDef,
     BatchGetFieldRequestRequestTypeDef,
+    CaseEventIncludedDataOutputTypeDef,
     CaseEventIncludedDataTypeDef,
     GetCaseRequestRequestTypeDef,
     BatchGetFieldResponseTypeDef,
+    CreateCaseResponseTypeDef,
+    CreateDomainResponseTypeDef,
+    CreateFieldResponseTypeDef,
+    CreateLayoutResponseTypeDef,
+    CreateRelatedItemResponseTypeDef,
+    CreateTemplateResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDomainResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
     BatchPutFieldOptionsRequestRequestTypeDef,
     ListFieldOptionsResponseTypeDef,
     BatchPutFieldOptionsResponseTypeDef,
     ListCasesForContactResponseTypeDef,
     RelatedItemContentTypeDef,
     RelatedItemTypeFilterTypeDef,
     RelatedItemInputContentTypeDef,
     CreateTemplateRequestRequestTypeDef,
     GetTemplateResponseTypeDef,
     UpdateTemplateRequestRequestTypeDef,
     ListDomainsResponseTypeDef,
+    FieldGroupOutputTypeDef,
     FieldGroupTypeDef,
     ListFieldsResponseTypeDef,
     FieldValueTypeDef,
     ListLayoutsResponseTypeDef,
     ListTemplatesResponseTypeDef,
     SearchCasesRequestRequestTypeDef,
     SearchCasesRequestSearchCasesPaginateTypeDef,
+    EventIncludedDataOutputTypeDef,
     EventIncludedDataTypeDef,
     SearchRelatedItemsResponseItemTypeDef,
     SearchRelatedItemsRequestRequestTypeDef,
     SearchRelatedItemsRequestSearchRelatedItemsPaginateTypeDef,
     CreateRelatedItemRequestRequestTypeDef,
+    SectionOutputTypeDef,
     SectionTypeDef,
     CreateCaseRequestRequestTypeDef,
     FieldFilterTypeDef,
     GetCaseResponseTypeDef,
     SearchCasesResponseItemTypeDef,
     UpdateCaseRequestRequestTypeDef,
+    EventBridgeConfigurationOutputTypeDef,
     EventBridgeConfigurationTypeDef,
     SearchRelatedItemsResponseTypeDef,
+    LayoutSectionsOutputTypeDef,
     LayoutSectionsTypeDef,
     CaseFilterTypeDef,
     SearchCasesResponseTypeDef,
     GetCaseEventConfigurationResponseTypeDef,
+    EventBridgeConfigurationUnionTypeDef,
     PutCaseEventConfigurationRequestRequestTypeDef,
+    BasicLayoutOutputTypeDef,
     BasicLayoutTypeDef,
+    LayoutContentOutputTypeDef,
     LayoutContentTypeDef,
-    CreateLayoutRequestRequestTypeDef,
     GetLayoutResponseTypeDef,
+    CreateLayoutRequestRequestTypeDef,
+    LayoutContentUnionTypeDef,
     UpdateLayoutRequestRequestTypeDef,
 )
 
 
-def get_structure() -> FieldIdentifierTypeDef:
+def get_value() -> FieldIdentifierTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectcases-2.5.2/types_aiobotocore_connectcases.egg-info/SOURCES.txt` & `types-aiobotocore-connectcases-2.5.2.post1/types_aiobotocore_connectcases.egg-info/SOURCES.txt`

 * *Files identical despite different names*


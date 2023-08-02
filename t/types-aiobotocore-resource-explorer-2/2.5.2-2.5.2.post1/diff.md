# Comparing `tmp/types-aiobotocore-resource-explorer-2-2.5.2.tar.gz` & `tmp/types-aiobotocore-resource-explorer-2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resource-explorer-2-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-resource-explorer-2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-resource-explorer-2-2.5.2.tar` & `types-aiobotocore-resource-explorer-2-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.882771 types-aiobotocore-resource-explorer-2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-07-08 01:44:11.882771 types-aiobotocore-resource-explorer-2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13978 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.882771 types-aiobotocore-resource-explorer-2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.878771 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:16.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.882771 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-07-08 01:44:11.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-08 01:44:11.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.000000 types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-02 14:47:53.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18703 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8648 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5657 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13070 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:54.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.893481 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15524 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.000000 types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/LICENSE` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/PKG-INFO` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-explorer-2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resource-explorer-2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resource-explorer-2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resource-explorer-2?color=blue)](https://pypistats.org/packages/types-aiobotocore-resource-explorer-2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-explorer-2)](https://pepy.tech/project/types-aiobotocore-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
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
@@ -320,75 +319,76 @@
 )
 
 
 def check_value(value: IndexStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resource_explorer_2.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
-    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
-    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
     IndexTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
-    ListViewsOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    ResponseMetadataTypeDef,
     SearchInputRequestTypeDef,
-    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
+    AssociateDefaultViewOutputTypeDef,
+    CreateIndexOutputTypeDef,
+    DeleteIndexOutputTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
     ViewTypeDef,
     ListIndexesOutputTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
+    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
     SearchOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
+def get_value() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/README.md` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resource-explorer-2?color=blue)](https://pypistats.org/packages/types-aiobotocore-resource-explorer-2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-explorer-2)](https://pepy.tech/project/types-aiobotocore-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
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
@@ -287,75 +287,76 @@
 )
 
 
 def check_value(value: IndexStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resource_explorer_2.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
-    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
-    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
     IndexTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
-    ListViewsOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    ResponseMetadataTypeDef,
     SearchInputRequestTypeDef,
-    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
+    AssociateDefaultViewOutputTypeDef,
+    CreateIndexOutputTypeDef,
+    DeleteIndexOutputTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
     ViewTypeDef,
     ListIndexesOutputTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
+    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
     SearchOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
+def get_value() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/setup.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resource-explorer-2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_resource_explorer_2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore resource-explorer-2 type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore resource-explorer-2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resource_explorer_2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/__init__.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/__init__.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/__main__.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ResourceExplorer 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ResourceExplorer 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer\nOther"
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

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/client.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/client.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/literals.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/literals.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/paginator.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,45 +65,45 @@
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listindexespaginator)
         """
 
 
 class ListSupportedResourceTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSupportedResourceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
         """
 
 
 class ListViewsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listviewspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListViewsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listviewspaginator)
         """
 
 
@@ -114,13 +114,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/paginator.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -62,43 +62,43 @@
     """
 
     def paginate(
         self,
         *,
         Regions: Sequence[str] = ...,
         Type: IndexTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListIndexesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListIndexes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listindexespaginator)
         """
 
 class ListSupportedResourceTypesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSupportedResourceTypesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListSupportedResourceTypes.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listsupportedresourcetypespaginator)
         """
 
 class ListViewsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listviewspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListViewsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.ListViews.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#listviewspaginator)
         """
 
 class SearchPaginator(AioPaginator):
@@ -108,13 +108,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ViewArn: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SearchOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer.Paginator.Search.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/paginators/#searchpaginator)
         """
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/type_defs.py` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,71 +4,70 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputRequestTypeDef
 
-    data: AssociateDefaultViewInputRequestTypeDef = {...}
+    data: AssociateDefaultViewInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import IndexStateType, IndexTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
-    "AssociateDefaultViewOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
-    "CreateIndexOutputTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
-    "DeleteIndexOutputTypeDef",
     "DeleteViewInputRequestTypeDef",
-    "DeleteViewOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDefaultViewOutputTypeDef",
-    "GetIndexOutputTypeDef",
     "GetViewInputRequestTypeDef",
     "IndexTypeDef",
-    "ListIndexesInputListIndexesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIndexesInputRequestTypeDef",
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListViewsInputListViewsPaginateTypeDef",
     "ListViewsInputRequestTypeDef",
-    "ListViewsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchInputRequestTypeDef",
-    "SearchInputSearchPaginateTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
+    "AssociateDefaultViewOutputTypeDef",
+    "CreateIndexOutputTypeDef",
+    "DeleteIndexOutputTypeDef",
+    "DeleteViewOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDefaultViewOutputTypeDef",
+    "GetIndexOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
     "ViewTypeDef",
     "ListIndexesOutputTypeDef",
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    "ListViewsInputListViewsPaginateTypeDef",
+    "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
     "SearchOutputTypeDef",
@@ -77,19 +76,22 @@
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-AssociateDefaultViewOutputTypeDef = TypedDict(
-    "AssociateDefaultViewOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchGetViewErrorTypeDef = TypedDict(
     "BatchGetViewErrorTypeDef",
     {
         "ErrorMessage": str,
@@ -110,24 +112,14 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateIndexOutputTypeDef = TypedDict(
-    "CreateIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IncludedPropertyTypeDef = TypedDict(
     "IncludedPropertyTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -141,69 +133,21 @@
 DeleteIndexInputRequestTypeDef = TypedDict(
     "DeleteIndexInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteIndexOutputTypeDef = TypedDict(
-    "DeleteIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "LastUpdatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteViewInputRequestTypeDef = TypedDict(
     "DeleteViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-DeleteViewOutputTypeDef = TypedDict(
-    "DeleteViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDefaultViewOutputTypeDef = TypedDict(
-    "GetDefaultViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetIndexOutputTypeDef = TypedDict(
-    "GetIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "ReplicatingFrom": List[str],
-        "ReplicatingTo": List[str],
-        "State": IndexStateType,
-        "Tags": Dict[str, str],
-        "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetViewInputRequestTypeDef = TypedDict(
     "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
@@ -213,20 +157,20 @@
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
-    "ListIndexesInputListIndexesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Regions": Sequence[str],
-        "Type": IndexTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListIndexesInputRequestTypeDef = TypedDict(
     "ListIndexesInputRequestTypeDef",
     {
@@ -234,22 +178,14 @@
         "NextToken": str,
         "Regions": Sequence[str],
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSupportedResourceTypesInputRequestTypeDef = TypedDict(
     "ListSupportedResourceTypesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -267,58 +203,23 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListViewsInputListViewsPaginateTypeDef = TypedDict(
-    "ListViewsInputListViewsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListViewsInputRequestTypeDef = TypedDict(
     "ListViewsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListViewsOutputTypeDef = TypedDict(
-    "ListViewsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Views": List[str],
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
 ResourceCountTypeDef = TypedDict(
     "ResourceCountTypeDef",
     {
         "Complete": bool,
         "TotalResources": int,
     },
     total=False,
@@ -330,25 +231,14 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
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
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalSearchInputRequestTypeDef = TypedDict(
@@ -357,64 +247,38 @@
         "MaxResults": int,
         "NextToken": str,
         "ViewArn": str,
     },
     total=False,
 )
 
-
 class SearchInputRequestTypeDef(
     _RequiredSearchInputRequestTypeDef, _OptionalSearchInputRequestTypeDef
 ):
     pass
 
-
-_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
-    "_RequiredSearchInputSearchPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
-    "_OptionalSearchInputSearchPaginateTypeDef",
-    {
-        "ViewArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SearchInputSearchPaginateTypeDef(
-    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
-):
-    pass
-
-
 _RequiredTagResourceInputRequestTypeDef = TypedDict(
     "_RequiredTagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 _OptionalTagResourceInputRequestTypeDef = TypedDict(
     "_OptionalTagResourceInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class TagResourceInputRequestTypeDef(
     _RequiredTagResourceInputRequestTypeDef, _OptionalTagResourceInputRequestTypeDef
 ):
     pass
 
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -423,22 +287,105 @@
     "UpdateIndexTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": IndexTypeType,
     },
 )
 
+AssociateDefaultViewOutputTypeDef = TypedDict(
+    "AssociateDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexOutputTypeDef = TypedDict(
+    "CreateIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIndexOutputTypeDef = TypedDict(
+    "DeleteIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "LastUpdatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteViewOutputTypeDef = TypedDict(
+    "DeleteViewOutputTypeDef",
+    {
+        "ViewArn": str,
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
+GetDefaultViewOutputTypeDef = TypedDict(
+    "GetDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIndexOutputTypeDef = TypedDict(
+    "GetIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "ReplicatingFrom": List[str],
+        "ReplicatingTo": List[str],
+        "State": IndexStateType,
+        "Tags": Dict[str, str],
+        "Type": IndexTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListViewsOutputTypeDef = TypedDict(
+    "ListViewsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Views": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateIndexTypeOutputTypeDef = TypedDict(
     "UpdateIndexTypeOutputTypeDef",
     {
         "Arn": str,
         "LastUpdatedAt": datetime,
         "State": IndexStateType,
         "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateViewInputRequestTypeDef = TypedDict(
     "_RequiredCreateViewInputRequestTypeDef",
     {
         "ViewName": str,
@@ -451,21 +398,19 @@
         "Filters": SearchFilterTypeDef,
         "IncludedProperties": Sequence[IncludedPropertyTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-
 class CreateViewInputRequestTypeDef(
     _RequiredCreateViewInputRequestTypeDef, _OptionalCreateViewInputRequestTypeDef
 ):
     pass
 
-
 _RequiredUpdateViewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 _OptionalUpdateViewInputRequestTypeDef = TypedDict(
@@ -473,21 +418,19 @@
     {
         "Filters": SearchFilterTypeDef,
         "IncludedProperties": Sequence[IncludedPropertyTypeDef],
     },
     total=False,
 )
 
-
 class UpdateViewInputRequestTypeDef(
     _RequiredUpdateViewInputRequestTypeDef, _OptionalUpdateViewInputRequestTypeDef
 ):
     pass
 
-
 ViewTypeDef = TypedDict(
     "ViewTypeDef",
     {
         "Filters": SearchFilterTypeDef,
         "IncludedProperties": List[IncludedPropertyTypeDef],
         "LastUpdatedAt": datetime,
         "Owner": str,
@@ -498,24 +441,70 @@
 )
 
 ListIndexesOutputTypeDef = TypedDict(
     "ListIndexesOutputTypeDef",
     {
         "Indexes": List[IndexTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    {
+        "Regions": Sequence[str],
+        "Type": IndexTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListViewsInputListViewsPaginateTypeDef = TypedDict(
+    "ListViewsInputListViewsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
+    "_RequiredSearchInputSearchPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
+    "_OptionalSearchInputSearchPaginateTypeDef",
+    {
+        "ViewArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SearchInputSearchPaginateTypeDef(
+    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
+):
+    pass
+
 ListSupportedResourceTypesOutputTypeDef = TypedDict(
     "ListSupportedResourceTypesOutputTypeDef",
     {
         "NextToken": str,
         "ResourceTypes": List[SupportedResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Arn": str,
@@ -530,46 +519,46 @@
 )
 
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateViewOutputTypeDef = TypedDict(
     "CreateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetViewOutputTypeDef = TypedDict(
     "GetViewOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchOutputTypeDef = TypedDict(
     "SearchOutputTypeDef",
     {
         "Count": ResourceCountTypeDef,
         "NextToken": str,
         "Resources": List[ResourceTypeDef],
         "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2/type_defs.pyi` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,70 +4,71 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_resource_explorer_2.type_defs import AssociateDefaultViewInputRequestTypeDef
 
-    data: AssociateDefaultViewInputRequestTypeDef = {...}
+    data: AssociateDefaultViewInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Mapping, Sequence
 
 from .literals import IndexStateType, IndexTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "AssociateDefaultViewInputRequestTypeDef",
-    "AssociateDefaultViewOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchGetViewErrorTypeDef",
     "BatchGetViewInputRequestTypeDef",
     "CreateIndexInputRequestTypeDef",
-    "CreateIndexOutputTypeDef",
     "IncludedPropertyTypeDef",
     "SearchFilterTypeDef",
     "DeleteIndexInputRequestTypeDef",
-    "DeleteIndexOutputTypeDef",
     "DeleteViewInputRequestTypeDef",
-    "DeleteViewOutputTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "GetDefaultViewOutputTypeDef",
-    "GetIndexOutputTypeDef",
     "GetViewInputRequestTypeDef",
     "IndexTypeDef",
-    "ListIndexesInputListIndexesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListIndexesInputRequestTypeDef",
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
     "ListSupportedResourceTypesInputRequestTypeDef",
     "SupportedResourceTypeTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "ListViewsInputListViewsPaginateTypeDef",
     "ListViewsInputRequestTypeDef",
-    "ListViewsOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "ResourceCountTypeDef",
     "ResourcePropertyTypeDef",
-    "ResponseMetadataTypeDef",
     "SearchInputRequestTypeDef",
-    "SearchInputSearchPaginateTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateIndexTypeInputRequestTypeDef",
+    "AssociateDefaultViewOutputTypeDef",
+    "CreateIndexOutputTypeDef",
+    "DeleteIndexOutputTypeDef",
+    "DeleteViewOutputTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetDefaultViewOutputTypeDef",
+    "GetIndexOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListViewsOutputTypeDef",
     "UpdateIndexTypeOutputTypeDef",
     "CreateViewInputRequestTypeDef",
     "UpdateViewInputRequestTypeDef",
     "ViewTypeDef",
     "ListIndexesOutputTypeDef",
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    "ListViewsInputListViewsPaginateTypeDef",
+    "SearchInputSearchPaginateTypeDef",
     "ListSupportedResourceTypesOutputTypeDef",
     "ResourceTypeDef",
     "BatchGetViewOutputTypeDef",
     "CreateViewOutputTypeDef",
     "GetViewOutputTypeDef",
     "UpdateViewOutputTypeDef",
     "SearchOutputTypeDef",
@@ -76,19 +77,22 @@
 AssociateDefaultViewInputRequestTypeDef = TypedDict(
     "AssociateDefaultViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-AssociateDefaultViewOutputTypeDef = TypedDict(
-    "AssociateDefaultViewOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BatchGetViewErrorTypeDef = TypedDict(
     "BatchGetViewErrorTypeDef",
     {
         "ErrorMessage": str,
@@ -109,24 +113,14 @@
     {
         "ClientToken": str,
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
-CreateIndexOutputTypeDef = TypedDict(
-    "CreateIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IncludedPropertyTypeDef = TypedDict(
     "IncludedPropertyTypeDef",
     {
         "Name": str,
     },
 )
 
@@ -140,69 +134,21 @@
 DeleteIndexInputRequestTypeDef = TypedDict(
     "DeleteIndexInputRequestTypeDef",
     {
         "Arn": str,
     },
 )
 
-DeleteIndexOutputTypeDef = TypedDict(
-    "DeleteIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "LastUpdatedAt": datetime,
-        "State": IndexStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteViewInputRequestTypeDef = TypedDict(
     "DeleteViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
-DeleteViewOutputTypeDef = TypedDict(
-    "DeleteViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetDefaultViewOutputTypeDef = TypedDict(
-    "GetDefaultViewOutputTypeDef",
-    {
-        "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetIndexOutputTypeDef = TypedDict(
-    "GetIndexOutputTypeDef",
-    {
-        "Arn": str,
-        "CreatedAt": datetime,
-        "LastUpdatedAt": datetime,
-        "ReplicatingFrom": List[str],
-        "ReplicatingTo": List[str],
-        "State": IndexStateType,
-        "Tags": Dict[str, str],
-        "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetViewInputRequestTypeDef = TypedDict(
     "GetViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 
@@ -212,20 +158,20 @@
         "Arn": str,
         "Region": str,
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
-    "ListIndexesInputListIndexesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Regions": Sequence[str],
-        "Type": IndexTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListIndexesInputRequestTypeDef = TypedDict(
     "ListIndexesInputRequestTypeDef",
     {
@@ -233,22 +179,14 @@
         "NextToken": str,
         "Regions": Sequence[str],
         "Type": IndexTypeType,
     },
     total=False,
 )
 
-ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
-    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSupportedResourceTypesInputRequestTypeDef = TypedDict(
     "ListSupportedResourceTypesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -266,58 +204,23 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListViewsInputListViewsPaginateTypeDef = TypedDict(
-    "ListViewsInputListViewsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListViewsInputRequestTypeDef = TypedDict(
     "ListViewsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListViewsOutputTypeDef = TypedDict(
-    "ListViewsOutputTypeDef",
-    {
-        "NextToken": str,
-        "Views": List[str],
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
 ResourceCountTypeDef = TypedDict(
     "ResourceCountTypeDef",
     {
         "Complete": bool,
         "TotalResources": int,
     },
     total=False,
@@ -329,25 +232,14 @@
         "Data": Dict[str, Any],
         "LastReportedAt": datetime,
         "Name": str,
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
 _RequiredSearchInputRequestTypeDef = TypedDict(
     "_RequiredSearchInputRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalSearchInputRequestTypeDef = TypedDict(
@@ -356,38 +248,20 @@
         "MaxResults": int,
         "NextToken": str,
         "ViewArn": str,
     },
     total=False,
 )
 
+
 class SearchInputRequestTypeDef(
     _RequiredSearchInputRequestTypeDef, _OptionalSearchInputRequestTypeDef
 ):
     pass
 
-_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
-    "_RequiredSearchInputSearchPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
-    "_OptionalSearchInputSearchPaginateTypeDef",
-    {
-        "ViewArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SearchInputSearchPaginateTypeDef(
-    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
-):
-    pass
 
 _RequiredTagResourceInputRequestTypeDef = TypedDict(
     "_RequiredTagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
@@ -395,19 +269,21 @@
     "_OptionalTagResourceInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class TagResourceInputRequestTypeDef(
     _RequiredTagResourceInputRequestTypeDef, _OptionalTagResourceInputRequestTypeDef
 ):
     pass
 
+
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "resourceArn": str,
         "tagKeys": Sequence[str],
     },
 )
@@ -416,22 +292,105 @@
     "UpdateIndexTypeInputRequestTypeDef",
     {
         "Arn": str,
         "Type": IndexTypeType,
     },
 )
 
+AssociateDefaultViewOutputTypeDef = TypedDict(
+    "AssociateDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateIndexOutputTypeDef = TypedDict(
+    "CreateIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteIndexOutputTypeDef = TypedDict(
+    "DeleteIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "LastUpdatedAt": datetime,
+        "State": IndexStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteViewOutputTypeDef = TypedDict(
+    "DeleteViewOutputTypeDef",
+    {
+        "ViewArn": str,
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
+GetDefaultViewOutputTypeDef = TypedDict(
+    "GetDefaultViewOutputTypeDef",
+    {
+        "ViewArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetIndexOutputTypeDef = TypedDict(
+    "GetIndexOutputTypeDef",
+    {
+        "Arn": str,
+        "CreatedAt": datetime,
+        "LastUpdatedAt": datetime,
+        "ReplicatingFrom": List[str],
+        "ReplicatingTo": List[str],
+        "State": IndexStateType,
+        "Tags": Dict[str, str],
+        "Type": IndexTypeType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListViewsOutputTypeDef = TypedDict(
+    "ListViewsOutputTypeDef",
+    {
+        "NextToken": str,
+        "Views": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdateIndexTypeOutputTypeDef = TypedDict(
     "UpdateIndexTypeOutputTypeDef",
     {
         "Arn": str,
         "LastUpdatedAt": datetime,
         "State": IndexStateType,
         "Type": IndexTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateViewInputRequestTypeDef = TypedDict(
     "_RequiredCreateViewInputRequestTypeDef",
     {
         "ViewName": str,
@@ -444,19 +403,21 @@
         "Filters": SearchFilterTypeDef,
         "IncludedProperties": Sequence[IncludedPropertyTypeDef],
         "Tags": Mapping[str, str],
     },
     total=False,
 )
 
+
 class CreateViewInputRequestTypeDef(
     _RequiredCreateViewInputRequestTypeDef, _OptionalCreateViewInputRequestTypeDef
 ):
     pass
 
+
 _RequiredUpdateViewInputRequestTypeDef = TypedDict(
     "_RequiredUpdateViewInputRequestTypeDef",
     {
         "ViewArn": str,
     },
 )
 _OptionalUpdateViewInputRequestTypeDef = TypedDict(
@@ -464,19 +425,21 @@
     {
         "Filters": SearchFilterTypeDef,
         "IncludedProperties": Sequence[IncludedPropertyTypeDef],
     },
     total=False,
 )
 
+
 class UpdateViewInputRequestTypeDef(
     _RequiredUpdateViewInputRequestTypeDef, _OptionalUpdateViewInputRequestTypeDef
 ):
     pass
 
+
 ViewTypeDef = TypedDict(
     "ViewTypeDef",
     {
         "Filters": SearchFilterTypeDef,
         "IncludedProperties": List[IncludedPropertyTypeDef],
         "LastUpdatedAt": datetime,
         "Owner": str,
@@ -487,24 +450,72 @@
 )
 
 ListIndexesOutputTypeDef = TypedDict(
     "ListIndexesOutputTypeDef",
     {
         "Indexes": List[IndexTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListIndexesInputListIndexesPaginateTypeDef = TypedDict(
+    "ListIndexesInputListIndexesPaginateTypeDef",
+    {
+        "Regions": Sequence[str],
+        "Type": IndexTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef = TypedDict(
+    "ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListViewsInputListViewsPaginateTypeDef = TypedDict(
+    "ListViewsInputListViewsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSearchInputSearchPaginateTypeDef = TypedDict(
+    "_RequiredSearchInputSearchPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalSearchInputSearchPaginateTypeDef = TypedDict(
+    "_OptionalSearchInputSearchPaginateTypeDef",
+    {
+        "ViewArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SearchInputSearchPaginateTypeDef(
+    _RequiredSearchInputSearchPaginateTypeDef, _OptionalSearchInputSearchPaginateTypeDef
+):
+    pass
+
+
 ListSupportedResourceTypesOutputTypeDef = TypedDict(
     "ListSupportedResourceTypesOutputTypeDef",
     {
         "NextToken": str,
         "ResourceTypes": List[SupportedResourceTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResourceTypeDef = TypedDict(
     "ResourceTypeDef",
     {
         "Arn": str,
@@ -519,46 +530,46 @@
 )
 
 BatchGetViewOutputTypeDef = TypedDict(
     "BatchGetViewOutputTypeDef",
     {
         "Errors": List[BatchGetViewErrorTypeDef],
         "Views": List[ViewTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateViewOutputTypeDef = TypedDict(
     "CreateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetViewOutputTypeDef = TypedDict(
     "GetViewOutputTypeDef",
     {
         "Tags": Dict[str, str],
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateViewOutputTypeDef = TypedDict(
     "UpdateViewOutputTypeDef",
     {
         "View": ViewTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SearchOutputTypeDef = TypedDict(
     "SearchOutputTypeDef",
     {
         "Count": ResourceCountTypeDef,
         "NextToken": str,
         "Resources": List[ResourceTypeDef],
         "ViewArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resource-explorer-2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResourceExplorer 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resource-explorer-2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resource-explorer-2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resource-explorer-2"></a>
 
 # types-aiobotocore-resource-explorer-2
 
 [![PyPI - types-aiobotocore-resource-explorer-2](https://img.shields.io/pypi/v/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resource-explorer-2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resource-explorer-2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resource-explorer-2?color=blue)](https://pypistats.org/packages/types-aiobotocore-resource-explorer-2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resource-explorer-2)](https://pepy.tech/project/types-aiobotocore-resource-explorer-2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceExplorer 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resource-explorer-2.html#ResourceExplorer)
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
 [types-aiobotocore-resource-explorer-2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resource_explorer_2/).
 
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
@@ -320,75 +319,76 @@
 )
 
 
 def check_value(value: IndexStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resource_explorer_2.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_resource_explorer_2.type_defs import (
     AssociateDefaultViewInputRequestTypeDef,
-    AssociateDefaultViewOutputTypeDef,
+    ResponseMetadataTypeDef,
     BatchGetViewErrorTypeDef,
     BatchGetViewInputRequestTypeDef,
     CreateIndexInputRequestTypeDef,
-    CreateIndexOutputTypeDef,
     IncludedPropertyTypeDef,
     SearchFilterTypeDef,
     DeleteIndexInputRequestTypeDef,
-    DeleteIndexOutputTypeDef,
     DeleteViewInputRequestTypeDef,
-    DeleteViewOutputTypeDef,
-    EmptyResponseMetadataTypeDef,
-    GetDefaultViewOutputTypeDef,
-    GetIndexOutputTypeDef,
     GetViewInputRequestTypeDef,
     IndexTypeDef,
-    ListIndexesInputListIndexesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListIndexesInputRequestTypeDef,
-    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
     ListSupportedResourceTypesInputRequestTypeDef,
     SupportedResourceTypeTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    ListViewsInputListViewsPaginateTypeDef,
     ListViewsInputRequestTypeDef,
-    ListViewsOutputTypeDef,
-    PaginatorConfigTypeDef,
     ResourceCountTypeDef,
     ResourcePropertyTypeDef,
-    ResponseMetadataTypeDef,
     SearchInputRequestTypeDef,
-    SearchInputSearchPaginateTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateIndexTypeInputRequestTypeDef,
+    AssociateDefaultViewOutputTypeDef,
+    CreateIndexOutputTypeDef,
+    DeleteIndexOutputTypeDef,
+    DeleteViewOutputTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetDefaultViewOutputTypeDef,
+    GetIndexOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListViewsOutputTypeDef,
     UpdateIndexTypeOutputTypeDef,
     CreateViewInputRequestTypeDef,
     UpdateViewInputRequestTypeDef,
     ViewTypeDef,
     ListIndexesOutputTypeDef,
+    ListIndexesInputListIndexesPaginateTypeDef,
+    ListSupportedResourceTypesInputListSupportedResourceTypesPaginateTypeDef,
+    ListViewsInputListViewsPaginateTypeDef,
+    SearchInputSearchPaginateTypeDef,
     ListSupportedResourceTypesOutputTypeDef,
     ResourceTypeDef,
     BatchGetViewOutputTypeDef,
     CreateViewOutputTypeDef,
     GetViewOutputTypeDef,
     UpdateViewOutputTypeDef,
     SearchOutputTypeDef,
 )
 
 
-def get_structure() -> AssociateDefaultViewInputRequestTypeDef:
+def get_value() -> AssociateDefaultViewInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resource-explorer-2-2.5.2/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt` & `types-aiobotocore-resource-explorer-2-2.5.2.post1/types_aiobotocore_resource_explorer_2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


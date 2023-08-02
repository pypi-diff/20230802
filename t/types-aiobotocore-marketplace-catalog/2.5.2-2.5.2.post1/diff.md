# Comparing `tmp/types-aiobotocore-marketplace-catalog-2.5.2.tar.gz` & `tmp/types-aiobotocore-marketplace-catalog-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.5.2.tar", last modified: Sat Jul  8 01:43:57 2023, max compression
+gzip compressed data, was "types-aiobotocore-marketplace-catalog-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:38 2023, max compression
```

## Comparing `types-aiobotocore-marketplace-catalog-2.5.2.tar` & `types-aiobotocore-marketplace-catalog-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:57.562506 types-aiobotocore-marketplace-catalog-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-08 01:43:57.562506 types-aiobotocore-marketplace-catalog-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13250 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:57.562506 types-aiobotocore-marketplace-catalog-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:57.554506 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-07-08 01:34:38.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-08 01:34:38.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3652 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-08 01:34:38.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11099 2023-07-08 01:34:38.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:37.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:57.562506 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14862 2023-07-08 01:43:57.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-08 01:43:57.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:57.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:57.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:57.000000 types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.013527 types-aiobotocore-marketplace-catalog-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-08-02 14:52:38.005527 types-aiobotocore-marketplace-catalog-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13233 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:38.013527 types-aiobotocore-marketplace-catalog-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.005527 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13997 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13974 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-08-02 14:42:50.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:49.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:38.005527 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14798 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:37.000000 types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/LICENSE` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore marketplace-catalog type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-marketplace-catalog?color=blue)](https://pypistats.org/packages/types-aiobotocore-marketplace-catalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MarketplaceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
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
@@ -314,44 +313,45 @@
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_marketplace_catalog.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
-    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CancelChangeSetResponseTypeDef,
+    DescribeEntityResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
@@ -359,15 +359,15 @@
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CancelChangeSetRequestRequestTypeDef:
+def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/README.md` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-marketplace-catalog?color=blue)](https://pypistats.org/packages/types-aiobotocore-marketplace-catalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MarketplaceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
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
@@ -281,44 +281,45 @@
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_marketplace_catalog.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
-    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CancelChangeSetResponseTypeDef,
+    DescribeEntityResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
@@ -326,15 +327,15 @@
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CancelChangeSetRequestRequestTypeDef:
+def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/setup.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-marketplace-catalog",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_marketplace_catalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with"
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
-        "aiobotocore marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore marketplace-catalog type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_marketplace_catalog": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/__init__.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/__init__.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/__main__.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.MarketplaceCatalog 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog\nOther"
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

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/client.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/client.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/literals.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/literals.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/paginator.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def paginate(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChangeSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listchangesetspaginator)
         """
 
 
@@ -79,13 +79,13 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         OwnershipType: OwnershipTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listentitiespaginator)
         """
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/paginator.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     def paginate(
         self,
         *,
         Catalog: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListChangeSetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListChangeSets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listchangesetspaginator)
         """
 
 class ListEntitiesPaginator(AioPaginator):
@@ -75,13 +75,13 @@
         self,
         *,
         Catalog: str,
         EntityType: str,
         FilterList: Sequence[FilterTypeDef] = ...,
         Sort: SortTypeDef = ...,
         OwnershipType: OwnershipTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEntitiesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog.Paginator.ListEntities.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/paginators/#listentitiespaginator)
         """
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/type_defs.py` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,50 +4,49 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
-    data: CancelChangeSetRequestRequestTypeDef = {...}
+    data: CancelChangeSetRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
-    "CancelChangeSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
-    "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartChangeSetResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CancelChangeSetResponseTypeDef",
+    "DescribeEntityResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "StartChangeSetResponseTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
@@ -62,20 +61,22 @@
     "CancelChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
 
-CancelChangeSetResponseTypeDef = TypedDict(
-    "CancelChangeSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChangeSetSummaryListItemTypeDef = TypedDict(
     "ChangeSetSummaryListItemTypeDef",
     {
         "ChangeSetId": str,
@@ -100,19 +101,17 @@
     "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
-
 class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
-
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -145,26 +144,14 @@
     "DescribeEntityRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityId": str,
     },
 )
 
-DescribeEntityResponseTypeDef = TypedDict(
-    "DescribeEntityResponseTypeDef",
-    {
-        "EntityType": str,
-        "EntityIdentifier": str,
-        "EntityArn": str,
-        "LastModifiedDate": str,
-        "Details": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EntitySummaryTypeDef = TypedDict(
     "EntitySummaryTypeDef",
     {
         "Name": str,
         "EntityType": str,
         "EntityId": str,
         "EntityArn": str,
@@ -186,20 +173,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -210,66 +199,74 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-StartChangeSetResponseTypeDef = TypedDict(
-    "StartChangeSetResponseTypeDef",
+CancelChangeSetResponseTypeDef = TypedDict(
+    "CancelChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+DescribeEntityResponseTypeDef = TypedDict(
+    "DescribeEntityResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "EntityType": str,
+        "EntityIdentifier": str,
+        "EntityArn": str,
+        "LastModifiedDate": str,
+        "Details": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartChangeSetResponseTypeDef = TypedDict(
+    "StartChangeSetResponseTypeDef",
+    {
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChangeSetsResponseTypeDef = TypedDict(
     "ListChangeSetsResponseTypeDef",
     {
         "ChangeSetSummaryList": List[ChangeSetSummaryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
@@ -294,25 +291,23 @@
     {
         "EntityTags": Sequence[TagTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
-
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -321,42 +316,40 @@
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "EntitySummaryList": List[EntitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
     _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
     _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListChangeSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestRequestTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestRequestTypeDef = TypedDict(
@@ -366,47 +359,43 @@
         "Sort": SortTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListChangeSetsRequestRequestTypeDef(
     _RequiredListChangeSetsRequestRequestTypeDef, _OptionalListChangeSetsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_RequiredListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
 _OptionalListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_OptionalListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "OwnershipType": OwnershipTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-
 class ListEntitiesRequestListEntitiesPaginateTypeDef(
     _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
     _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
 ):
     pass
 
-
 _RequiredListEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
@@ -418,34 +407,32 @@
         "NextToken": str,
         "MaxResults": int,
         "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
-
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
-
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
         "EndTime": str,
         "Status": ChangeStatusType,
         "FailureCode": FailureCodeType,
         "FailureDescription": str,
         "ChangeSet": List[ChangeSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
@@ -458,12 +445,11 @@
         "ChangeSetName": str,
         "ClientRequestToken": str,
         "ChangeSetTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class StartChangeSetRequestRequestTypeDef(
     _RequiredStartChangeSetRequestRequestTypeDef, _OptionalStartChangeSetRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog/type_defs.pyi` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,49 +4,50 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_marketplace_catalog.type_defs import CancelChangeSetRequestRequestTypeDef
 
-    data: CancelChangeSetRequestRequestTypeDef = {...}
+    data: CancelChangeSetRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import ChangeStatusType, FailureCodeType, OwnershipTypeType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CancelChangeSetRequestRequestTypeDef",
-    "CancelChangeSetResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ChangeSetSummaryListItemTypeDef",
     "EntityTypeDef",
     "ErrorDetailTypeDef",
     "TagTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
     "DescribeChangeSetRequestRequestTypeDef",
     "DescribeEntityRequestRequestTypeDef",
-    "DescribeEntityResponseTypeDef",
     "EntitySummaryTypeDef",
     "FilterTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
+    "PaginatorConfigTypeDef",
     "SortTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartChangeSetResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
+    "CancelChangeSetResponseTypeDef",
+    "DescribeEntityResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "StartChangeSetResponseTypeDef",
     "ListChangeSetsResponseTypeDef",
     "ChangeSummaryTypeDef",
     "ChangeTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListEntitiesResponseTypeDef",
     "ListChangeSetsRequestListChangeSetsPaginateTypeDef",
@@ -61,20 +62,22 @@
     "CancelChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
         "ChangeSetId": str,
     },
 )
 
-CancelChangeSetResponseTypeDef = TypedDict(
-    "CancelChangeSetResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChangeSetId": str,
-        "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ChangeSetSummaryListItemTypeDef = TypedDict(
     "ChangeSetSummaryListItemTypeDef",
     {
         "ChangeSetId": str,
@@ -99,17 +102,19 @@
     "_OptionalEntityTypeDef",
     {
         "Identifier": str,
     },
     total=False,
 )
 
+
 class EntityTypeDef(_RequiredEntityTypeDef, _OptionalEntityTypeDef):
     pass
 
+
 ErrorDetailTypeDef = TypedDict(
     "ErrorDetailTypeDef",
     {
         "ErrorCode": str,
         "ErrorMessage": str,
     },
     total=False,
@@ -142,26 +147,14 @@
     "DescribeEntityRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityId": str,
     },
 )
 
-DescribeEntityResponseTypeDef = TypedDict(
-    "DescribeEntityResponseTypeDef",
-    {
-        "EntityType": str,
-        "EntityIdentifier": str,
-        "EntityArn": str,
-        "LastModifiedDate": str,
-        "Details": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EntitySummaryTypeDef = TypedDict(
     "EntitySummaryTypeDef",
     {
         "Name": str,
         "EntityType": str,
         "EntityId": str,
         "EntityArn": str,
@@ -183,20 +176,22 @@
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
 SortTypeDef = TypedDict(
     "SortTypeDef",
     {
         "SortBy": str,
         "SortOrder": SortOrderType,
@@ -207,66 +202,74 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
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
 PutResourcePolicyRequestRequestTypeDef = TypedDict(
     "PutResourcePolicyRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Policy": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-StartChangeSetResponseTypeDef = TypedDict(
-    "StartChangeSetResponseTypeDef",
+CancelChangeSetResponseTypeDef = TypedDict(
+    "CancelChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+DescribeEntityResponseTypeDef = TypedDict(
+    "DescribeEntityResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "EntityType": str,
+        "EntityIdentifier": str,
+        "EntityArn": str,
+        "LastModifiedDate": str,
+        "Details": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartChangeSetResponseTypeDef = TypedDict(
+    "StartChangeSetResponseTypeDef",
+    {
+        "ChangeSetId": str,
+        "ChangeSetArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListChangeSetsResponseTypeDef = TypedDict(
     "ListChangeSetsResponseTypeDef",
     {
         "ChangeSetSummaryList": List[ChangeSetSummaryListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ChangeSummaryTypeDef = TypedDict(
     "ChangeSummaryTypeDef",
     {
         "ChangeType": str,
@@ -291,23 +294,25 @@
     {
         "EntityTags": Sequence[TagTypeDef],
         "ChangeName": str,
     },
     total=False,
 )
 
+
 class ChangeTypeDef(_RequiredChangeTypeDef, _OptionalChangeTypeDef):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "ResourceArn": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
@@ -316,40 +321,42 @@
 )
 
 ListEntitiesResponseTypeDef = TypedDict(
     "ListEntitiesResponseTypeDef",
     {
         "EntitySummaryList": List[EntitySummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef = TypedDict(
     "_OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListChangeSetsRequestListChangeSetsPaginateTypeDef(
     _RequiredListChangeSetsRequestListChangeSetsPaginateTypeDef,
     _OptionalListChangeSetsRequestListChangeSetsPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListChangeSetsRequestRequestTypeDef = TypedDict(
     "_RequiredListChangeSetsRequestRequestTypeDef",
     {
         "Catalog": str,
     },
 )
 _OptionalListChangeSetsRequestRequestTypeDef = TypedDict(
@@ -359,43 +366,47 @@
         "Sort": SortTypeDef,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListChangeSetsRequestRequestTypeDef(
     _RequiredListChangeSetsRequestRequestTypeDef, _OptionalListChangeSetsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_RequiredListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
 _OptionalListEntitiesRequestListEntitiesPaginateTypeDef = TypedDict(
     "_OptionalListEntitiesRequestListEntitiesPaginateTypeDef",
     {
         "FilterList": Sequence[FilterTypeDef],
         "Sort": SortTypeDef,
         "OwnershipType": OwnershipTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
+
 class ListEntitiesRequestListEntitiesPaginateTypeDef(
     _RequiredListEntitiesRequestListEntitiesPaginateTypeDef,
     _OptionalListEntitiesRequestListEntitiesPaginateTypeDef,
 ):
     pass
 
+
 _RequiredListEntitiesRequestRequestTypeDef = TypedDict(
     "_RequiredListEntitiesRequestRequestTypeDef",
     {
         "Catalog": str,
         "EntityType": str,
     },
 )
@@ -407,32 +418,34 @@
         "NextToken": str,
         "MaxResults": int,
         "OwnershipType": OwnershipTypeType,
     },
     total=False,
 )
 
+
 class ListEntitiesRequestRequestTypeDef(
     _RequiredListEntitiesRequestRequestTypeDef, _OptionalListEntitiesRequestRequestTypeDef
 ):
     pass
 
+
 DescribeChangeSetResponseTypeDef = TypedDict(
     "DescribeChangeSetResponseTypeDef",
     {
         "ChangeSetId": str,
         "ChangeSetArn": str,
         "ChangeSetName": str,
         "StartTime": str,
         "EndTime": str,
         "Status": ChangeStatusType,
         "FailureCode": FailureCodeType,
         "FailureDescription": str,
         "ChangeSet": List[ChangeSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartChangeSetRequestRequestTypeDef = TypedDict(
     "_RequiredStartChangeSetRequestRequestTypeDef",
     {
         "Catalog": str,
@@ -445,11 +458,12 @@
         "ChangeSetName": str,
         "ClientRequestToken": str,
         "ChangeSetTags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class StartChangeSetRequestRequestTypeDef(
     _RequiredStartChangeSetRequestRequestTypeDef, _OptionalStartChangeSetRequestRequestTypeDef
 ):
     pass
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-marketplace-catalog
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.MarketplaceCatalog 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore marketplace-catalog type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore marketplace-catalog type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-marketplace-catalog"></a>
 
 # types-aiobotocore-marketplace-catalog
 
 [![PyPI - types-aiobotocore-marketplace-catalog](https://img.shields.io/pypi/v/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-marketplace-catalog.svg?color=blue)](https://pypi.org/project/types-aiobotocore-marketplace-catalog)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-marketplace-catalog?color=blue)](https://pypistats.org/packages/types-aiobotocore-marketplace-catalog)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-marketplace-catalog)](https://pepy.tech/project/types-aiobotocore-marketplace-catalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.MarketplaceCatalog 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/marketplace-catalog.html#MarketplaceCatalog)
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
 [types-aiobotocore-marketplace-catalog docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_marketplace_catalog/).
 
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
@@ -314,44 +313,45 @@
 )
 
 
 def check_value(value: ChangeStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_marketplace_catalog.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_marketplace_catalog.type_defs import (
     CancelChangeSetRequestRequestTypeDef,
-    CancelChangeSetResponseTypeDef,
+    ResponseMetadataTypeDef,
     ChangeSetSummaryListItemTypeDef,
     EntityTypeDef,
     ErrorDetailTypeDef,
     TagTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
     DescribeChangeSetRequestRequestTypeDef,
     DescribeEntityRequestRequestTypeDef,
-    DescribeEntityResponseTypeDef,
     EntitySummaryTypeDef,
     FilterTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
+    PaginatorConfigTypeDef,
     SortTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
-    StartChangeSetResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
+    CancelChangeSetResponseTypeDef,
+    DescribeEntityResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    StartChangeSetResponseTypeDef,
     ListChangeSetsResponseTypeDef,
     ChangeSummaryTypeDef,
     ChangeTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListEntitiesResponseTypeDef,
     ListChangeSetsRequestListChangeSetsPaginateTypeDef,
@@ -359,15 +359,15 @@
     ListEntitiesRequestListEntitiesPaginateTypeDef,
     ListEntitiesRequestRequestTypeDef,
     DescribeChangeSetResponseTypeDef,
     StartChangeSetRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CancelChangeSetRequestRequestTypeDef:
+def get_value() -> CancelChangeSetRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-marketplace-catalog-2.5.2/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt` & `types-aiobotocore-marketplace-catalog-2.5.2.post1/types_aiobotocore_marketplace_catalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-oam-2.5.2.tar.gz` & `tmp/types-aiobotocore-oam-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-oam-2.5.2.tar", last modified: Sat Jul  8 01:44:02 2023, max compression
+gzip compressed data, was "types-aiobotocore-oam-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:43 2023, max compression
```

## Comparing `types-aiobotocore-oam-2.5.2.tar` & `types-aiobotocore-oam-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.886605 types-aiobotocore-oam-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14398 2023-07-08 01:44:02.886605 types-aiobotocore-oam-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12816 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:02.886605 types-aiobotocore-oam-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.886605 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9677 2023-07-08 01:35:54.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:35:53.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:02.886605 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14398 2023-07-08 01:44:02.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:02.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:02.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:02.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:02.000000 types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.709510 types-aiobotocore-oam-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-02 14:52:43.701510 types-aiobotocore-oam-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12799 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:43.709510 types-aiobotocore-oam-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.701510 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14752 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14725 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 2023-08-02 14:44:12.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:11.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:43.701510 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14334 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:43.000000 types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-oam-2.5.2/LICENSE` & `types-aiobotocore-oam-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/PKG-INFO` & `types-aiobotocore-oam-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-oam
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore oam type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore oam type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-oam"></a>
 
 # types-aiobotocore-oam
 
 [![PyPI - types-aiobotocore-oam](https://img.shields.io/pypi/v/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-oam?color=blue)](https://pypistats.org/packages/types-aiobotocore-oam)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-oam)](https://pepy.tech/project/types-aiobotocore-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchObservabilityAccessManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
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
 [types-aiobotocore-oam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/).
 
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
@@ -315,61 +314,61 @@
 )
 
 
 def check_value(value: ListAttachedLinksPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_oam.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_oam.type_defs import (
     CreateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSinkInputRequestTypeDef,
-    CreateSinkOutputTypeDef,
     DeleteLinkInputRequestTypeDef,
     DeleteSinkInputRequestTypeDef,
     GetLinkInputRequestTypeDef,
-    GetLinkOutputTypeDef,
     GetSinkInputRequestTypeDef,
-    GetSinkOutputTypeDef,
     GetSinkPolicyInputRequestTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAttachedLinksInputRequestTypeDef,
     ListAttachedLinksItemTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
     ListLinksInputRequestTypeDef,
     ListLinksItemTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
     ListSinksInputRequestTypeDef,
     ListSinksItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutSinkPolicyInputRequestTypeDef,
-    PutSinkPolicyOutputTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateLinkInputRequestTypeDef,
+    CreateLinkOutputTypeDef,
+    CreateSinkOutputTypeDef,
+    GetLinkOutputTypeDef,
+    GetSinkOutputTypeDef,
+    GetSinkPolicyOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
+    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    ListLinksInputListLinksPaginateTypeDef,
+    ListSinksInputListSinksPaginateTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
 )
 
 
-def get_structure() -> CreateLinkInputRequestTypeDef:
+def get_value() -> CreateLinkInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-oam-2.5.2/README.md` & `types-aiobotocore-oam-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-oam"></a>
 
 # types-aiobotocore-oam
 
 [![PyPI - types-aiobotocore-oam](https://img.shields.io/pypi/v/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-oam?color=blue)](https://pypistats.org/packages/types-aiobotocore-oam)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-oam)](https://pepy.tech/project/types-aiobotocore-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchObservabilityAccessManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
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
 [types-aiobotocore-oam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/).
 
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
@@ -282,61 +282,61 @@
 )
 
 
 def check_value(value: ListAttachedLinksPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_oam.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_oam.type_defs import (
     CreateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSinkInputRequestTypeDef,
-    CreateSinkOutputTypeDef,
     DeleteLinkInputRequestTypeDef,
     DeleteSinkInputRequestTypeDef,
     GetLinkInputRequestTypeDef,
-    GetLinkOutputTypeDef,
     GetSinkInputRequestTypeDef,
-    GetSinkOutputTypeDef,
     GetSinkPolicyInputRequestTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAttachedLinksInputRequestTypeDef,
     ListAttachedLinksItemTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
     ListLinksInputRequestTypeDef,
     ListLinksItemTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
     ListSinksInputRequestTypeDef,
     ListSinksItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutSinkPolicyInputRequestTypeDef,
-    PutSinkPolicyOutputTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateLinkInputRequestTypeDef,
+    CreateLinkOutputTypeDef,
+    CreateSinkOutputTypeDef,
+    GetLinkOutputTypeDef,
+    GetSinkOutputTypeDef,
+    GetSinkPolicyOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
+    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    ListLinksInputListLinksPaginateTypeDef,
+    ListSinksInputListSinksPaginateTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
 )
 
 
-def get_structure() -> CreateLinkInputRequestTypeDef:
+def get_value() -> CreateLinkInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-oam-2.5.2/setup.py` & `types-aiobotocore-oam-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-oam",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_oam"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service"
-        " generated with mypy-boto3-builder 7.14.5"
+        " generated with mypy-boto3-builder 7.17.1"
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
-    keywords="aiobotocore oam type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore oam type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_oam": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/__init__.py` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/__init__.pyi` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/__main__.py` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2\nVersion:     "
-        "    2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        "    2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager\nOther"
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

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/client.py` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/client.pyi` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/literals.py` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/literals.pyi` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/paginator.py` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,43 +52,43 @@
 class ListAttachedLinksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listattachedlinkspaginator)
     """
 
     def paginate(
-        self, *, SinkIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SinkIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listattachedlinkspaginator)
         """
 
 
 class ListLinksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listlinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listlinkspaginator)
         """
 
 
 class ListSinksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listsinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listsinkspaginator)
         """
```

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/paginator.pyi` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,41 +49,41 @@
 class ListAttachedLinksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listattachedlinkspaginator)
     """
 
     def paginate(
-        self, *, SinkIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, SinkIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAttachedLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListAttachedLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listattachedlinkspaginator)
         """
 
 class ListLinksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listlinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListLinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listlinkspaginator)
         """
 
 class ListSinksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listsinkspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSinksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager.Paginator.ListSinks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/paginators/#listsinkspaginator)
         """
```

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/type_defs.py` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_oam.type_defs import CreateLinkInputRequestTypeDef
 
-    data: CreateLinkInputRequestTypeDef = {...}
+    data: CreateLinkInputRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceTypeType
 
@@ -20,44 +20,44 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CreateLinkInputRequestTypeDef",
-    "CreateLinkOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSinkInputRequestTypeDef",
-    "CreateSinkOutputTypeDef",
     "DeleteLinkInputRequestTypeDef",
     "DeleteSinkInputRequestTypeDef",
     "GetLinkInputRequestTypeDef",
-    "GetLinkOutputTypeDef",
     "GetSinkInputRequestTypeDef",
-    "GetSinkOutputTypeDef",
     "GetSinkPolicyInputRequestTypeDef",
-    "GetSinkPolicyOutputTypeDef",
-    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAttachedLinksInputRequestTypeDef",
     "ListAttachedLinksItemTypeDef",
-    "ListLinksInputListLinksPaginateTypeDef",
     "ListLinksInputRequestTypeDef",
     "ListLinksItemTypeDef",
-    "ListSinksInputListSinksPaginateTypeDef",
     "ListSinksInputRequestTypeDef",
     "ListSinksItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutSinkPolicyInputRequestTypeDef",
-    "PutSinkPolicyOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateLinkInputRequestTypeDef",
+    "CreateLinkOutputTypeDef",
+    "CreateSinkOutputTypeDef",
+    "GetLinkOutputTypeDef",
+    "GetSinkOutputTypeDef",
+    "GetSinkPolicyOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PutSinkPolicyOutputTypeDef",
     "UpdateLinkOutputTypeDef",
+    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    "ListLinksInputListLinksPaginateTypeDef",
+    "ListSinksInputListSinksPaginateTypeDef",
     "ListAttachedLinksOutputTypeDef",
     "ListLinksOutputTypeDef",
     "ListSinksOutputTypeDef",
 )
 
 _RequiredCreateLinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateLinkInputRequestTypeDef",
@@ -78,25 +78,22 @@
 
 class CreateLinkInputRequestTypeDef(
     _RequiredCreateLinkInputRequestTypeDef, _OptionalCreateLinkInputRequestTypeDef
 ):
     pass
 
 
-CreateLinkOutputTypeDef = TypedDict(
-    "CreateLinkOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateSinkInputRequestTypeDef",
     {
         "Name": str,
@@ -113,25 +110,14 @@
 
 class CreateSinkInputRequestTypeDef(
     _RequiredCreateSinkInputRequestTypeDef, _OptionalCreateSinkInputRequestTypeDef
 ):
     pass
 
 
-CreateSinkOutputTypeDef = TypedDict(
-    "CreateSinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLinkInputRequestTypeDef = TypedDict(
     "DeleteLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -145,85 +131,38 @@
 GetLinkInputRequestTypeDef = TypedDict(
     "GetLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-GetLinkOutputTypeDef = TypedDict(
-    "GetLinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSinkInputRequestTypeDef = TypedDict(
     "GetSinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-GetSinkOutputTypeDef = TypedDict(
-    "GetSinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSinkPolicyInputRequestTypeDef = TypedDict(
     "GetSinkPolicyInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 
-GetSinkPolicyOutputTypeDef = TypedDict(
-    "GetSinkPolicyOutputTypeDef",
-    {
-        "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    {
-        "SinkIdentifier": str,
-    },
-)
-_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
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
-class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
-    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAttachedLinksInputRequestTypeDef = TypedDict(
     "_RequiredListAttachedLinksInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 _OptionalListAttachedLinksInputRequestTypeDef = TypedDict(
@@ -248,22 +187,14 @@
         "Label": str,
         "LinkArn": str,
         "ResourceTypes": List[str],
     },
     total=False,
 )
 
-ListLinksInputListLinksPaginateTypeDef = TypedDict(
-    "ListLinksInputListLinksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLinksInputRequestTypeDef = TypedDict(
     "ListLinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -277,22 +208,14 @@
         "Label": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
     },
     total=False,
 )
 
-ListSinksInputListSinksPaginateTypeDef = TypedDict(
-    "ListSinksInputListSinksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSinksInputRequestTypeDef = TypedDict(
     "ListSinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -311,118 +234,195 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+PutSinkPolicyInputRequestTypeDef = TypedDict(
+    "PutSinkPolicyInputRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SinkIdentifier": str,
+        "Policy": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
-    total=False,
 )
 
-PutSinkPolicyInputRequestTypeDef = TypedDict(
-    "PutSinkPolicyInputRequestTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "SinkIdentifier": str,
-        "Policy": str,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-PutSinkPolicyOutputTypeDef = TypedDict(
-    "PutSinkPolicyOutputTypeDef",
+UpdateLinkInputRequestTypeDef = TypedDict(
+    "UpdateLinkInputRequestTypeDef",
     {
+        "Identifier": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
+    },
+)
+
+CreateLinkOutputTypeDef = TypedDict(
+    "CreateLinkOutputTypeDef",
+    {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
         "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSinkOutputTypeDef = TypedDict(
+    "CreateSinkOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+GetLinkOutputTypeDef = TypedDict(
+    "GetLinkOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
+GetSinkOutputTypeDef = TypedDict(
+    "GetSinkOutputTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLinkInputRequestTypeDef = TypedDict(
-    "UpdateLinkInputRequestTypeDef",
+GetSinkPolicyOutputTypeDef = TypedDict(
+    "GetSinkPolicyOutputTypeDef",
     {
-        "Identifier": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
+        "SinkArn": str,
+        "SinkId": str,
+        "Policy": str,
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
+PutSinkPolicyOutputTypeDef = TypedDict(
+    "PutSinkPolicyOutputTypeDef",
+    {
+        "SinkArn": str,
+        "SinkId": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLinkOutputTypeDef = TypedDict(
     "UpdateLinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Label": str,
         "LabelTemplate": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "SinkIdentifier": str,
+    },
+)
+_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
+    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+):
+    pass
+
+
+ListLinksInputListLinksPaginateTypeDef = TypedDict(
+    "ListLinksInputListLinksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListSinksInputListSinksPaginateTypeDef = TypedDict(
+    "ListSinksInputListSinksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
 
 ListAttachedLinksOutputTypeDef = TypedDict(
     "ListAttachedLinksOutputTypeDef",
     {
         "Items": List[ListAttachedLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLinksOutputTypeDef = TypedDict(
     "ListLinksOutputTypeDef",
     {
         "Items": List[ListLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSinksOutputTypeDef = TypedDict(
     "ListSinksOutputTypeDef",
     {
         "Items": List[ListSinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam/type_defs.pyi` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,59 +4,59 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_oam.type_defs import CreateLinkInputRequestTypeDef
 
-    data: CreateLinkInputRequestTypeDef = {...}
+    data: CreateLinkInputRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ResourceTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CreateLinkInputRequestTypeDef",
-    "CreateLinkOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateSinkInputRequestTypeDef",
-    "CreateSinkOutputTypeDef",
     "DeleteLinkInputRequestTypeDef",
     "DeleteSinkInputRequestTypeDef",
     "GetLinkInputRequestTypeDef",
-    "GetLinkOutputTypeDef",
     "GetSinkInputRequestTypeDef",
-    "GetSinkOutputTypeDef",
     "GetSinkPolicyInputRequestTypeDef",
-    "GetSinkPolicyOutputTypeDef",
-    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAttachedLinksInputRequestTypeDef",
     "ListAttachedLinksItemTypeDef",
-    "ListLinksInputListLinksPaginateTypeDef",
     "ListLinksInputRequestTypeDef",
     "ListLinksItemTypeDef",
-    "ListSinksInputListSinksPaginateTypeDef",
     "ListSinksInputRequestTypeDef",
     "ListSinksItemTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "PutSinkPolicyInputRequestTypeDef",
-    "PutSinkPolicyOutputTypeDef",
-    "ResponseMetadataTypeDef",
     "TagResourceInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateLinkInputRequestTypeDef",
+    "CreateLinkOutputTypeDef",
+    "CreateSinkOutputTypeDef",
+    "GetLinkOutputTypeDef",
+    "GetSinkOutputTypeDef",
+    "GetSinkPolicyOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "PutSinkPolicyOutputTypeDef",
     "UpdateLinkOutputTypeDef",
+    "ListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    "ListLinksInputListLinksPaginateTypeDef",
+    "ListSinksInputListSinksPaginateTypeDef",
     "ListAttachedLinksOutputTypeDef",
     "ListLinksOutputTypeDef",
     "ListSinksOutputTypeDef",
 )
 
 _RequiredCreateLinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateLinkInputRequestTypeDef",
@@ -75,25 +75,22 @@
 )
 
 class CreateLinkInputRequestTypeDef(
     _RequiredCreateLinkInputRequestTypeDef, _OptionalCreateLinkInputRequestTypeDef
 ):
     pass
 
-CreateLinkOutputTypeDef = TypedDict(
-    "CreateLinkOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateSinkInputRequestTypeDef = TypedDict(
     "_RequiredCreateSinkInputRequestTypeDef",
     {
         "Name": str,
@@ -108,25 +105,14 @@
 )
 
 class CreateSinkInputRequestTypeDef(
     _RequiredCreateSinkInputRequestTypeDef, _OptionalCreateSinkInputRequestTypeDef
 ):
     pass
 
-CreateSinkOutputTypeDef = TypedDict(
-    "CreateSinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLinkInputRequestTypeDef = TypedDict(
     "DeleteLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
@@ -140,83 +126,38 @@
 GetLinkInputRequestTypeDef = TypedDict(
     "GetLinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-GetLinkOutputTypeDef = TypedDict(
-    "GetLinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Label": str,
-        "LabelTemplate": str,
-        "ResourceTypes": List[str],
-        "SinkArn": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSinkInputRequestTypeDef = TypedDict(
     "GetSinkInputRequestTypeDef",
     {
         "Identifier": str,
     },
 )
 
-GetSinkOutputTypeDef = TypedDict(
-    "GetSinkOutputTypeDef",
-    {
-        "Arn": str,
-        "Id": str,
-        "Name": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetSinkPolicyInputRequestTypeDef = TypedDict(
     "GetSinkPolicyInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 
-GetSinkPolicyOutputTypeDef = TypedDict(
-    "GetSinkPolicyOutputTypeDef",
-    {
-        "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
-    {
-        "SinkIdentifier": str,
-    },
-)
-_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
-    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
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
 
-class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
-    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
-):
-    pass
-
 _RequiredListAttachedLinksInputRequestTypeDef = TypedDict(
     "_RequiredListAttachedLinksInputRequestTypeDef",
     {
         "SinkIdentifier": str,
     },
 )
 _OptionalListAttachedLinksInputRequestTypeDef = TypedDict(
@@ -239,22 +180,14 @@
         "Label": str,
         "LinkArn": str,
         "ResourceTypes": List[str],
     },
     total=False,
 )
 
-ListLinksInputListLinksPaginateTypeDef = TypedDict(
-    "ListLinksInputListLinksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLinksInputRequestTypeDef = TypedDict(
     "ListLinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -268,22 +201,14 @@
         "Label": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
     },
     total=False,
 )
 
-ListSinksInputListSinksPaginateTypeDef = TypedDict(
-    "ListSinksInputListSinksPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSinksInputRequestTypeDef = TypedDict(
     "ListSinksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -302,118 +227,193 @@
 ListTagsForResourceInputRequestTypeDef = TypedDict(
     "ListTagsForResourceInputRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
+PutSinkPolicyInputRequestTypeDef = TypedDict(
+    "PutSinkPolicyInputRequestTypeDef",
     {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SinkIdentifier": str,
+        "Policy": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+TagResourceInputRequestTypeDef = TypedDict(
+    "TagResourceInputRequestTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ResourceArn": str,
+        "Tags": Mapping[str, str],
     },
-    total=False,
 )
 
-PutSinkPolicyInputRequestTypeDef = TypedDict(
-    "PutSinkPolicyInputRequestTypeDef",
+UntagResourceInputRequestTypeDef = TypedDict(
+    "UntagResourceInputRequestTypeDef",
     {
-        "SinkIdentifier": str,
-        "Policy": str,
+        "ResourceArn": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-PutSinkPolicyOutputTypeDef = TypedDict(
-    "PutSinkPolicyOutputTypeDef",
+UpdateLinkInputRequestTypeDef = TypedDict(
+    "UpdateLinkInputRequestTypeDef",
+    {
+        "Identifier": str,
+        "ResourceTypes": Sequence[ResourceTypeType],
+    },
+)
+
+CreateLinkOutputTypeDef = TypedDict(
+    "CreateLinkOutputTypeDef",
     {
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
         "SinkArn": str,
-        "SinkId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateSinkOutputTypeDef = TypedDict(
+    "CreateSinkOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceInputRequestTypeDef = TypedDict(
-    "TagResourceInputRequestTypeDef",
+GetLinkOutputTypeDef = TypedDict(
+    "GetLinkOutputTypeDef",
     {
-        "ResourceArn": str,
-        "Tags": Mapping[str, str],
+        "Arn": str,
+        "Id": str,
+        "Label": str,
+        "LabelTemplate": str,
+        "ResourceTypes": List[str],
+        "SinkArn": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UntagResourceInputRequestTypeDef = TypedDict(
-    "UntagResourceInputRequestTypeDef",
+GetSinkOutputTypeDef = TypedDict(
+    "GetSinkOutputTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeys": Sequence[str],
+        "Arn": str,
+        "Id": str,
+        "Name": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-UpdateLinkInputRequestTypeDef = TypedDict(
-    "UpdateLinkInputRequestTypeDef",
+GetSinkPolicyOutputTypeDef = TypedDict(
+    "GetSinkPolicyOutputTypeDef",
     {
-        "Identifier": str,
-        "ResourceTypes": Sequence[ResourceTypeType],
+        "SinkArn": str,
+        "SinkId": str,
+        "Policy": str,
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
+PutSinkPolicyOutputTypeDef = TypedDict(
+    "PutSinkPolicyOutputTypeDef",
+    {
+        "SinkArn": str,
+        "SinkId": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateLinkOutputTypeDef = TypedDict(
     "UpdateLinkOutputTypeDef",
     {
         "Arn": str,
         "Id": str,
         "Label": str,
         "LabelTemplate": str,
         "ResourceTypes": List[str],
         "SinkArn": str,
         "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "SinkIdentifier": str,
+    },
+)
+_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef = TypedDict(
+    "_OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAttachedLinksInputListAttachedLinksPaginateTypeDef(
+    _RequiredListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    _OptionalListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+):
+    pass
+
+ListLinksInputListLinksPaginateTypeDef = TypedDict(
+    "ListLinksInputListLinksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSinksInputListSinksPaginateTypeDef = TypedDict(
+    "ListSinksInputListSinksPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListAttachedLinksOutputTypeDef = TypedDict(
     "ListAttachedLinksOutputTypeDef",
     {
         "Items": List[ListAttachedLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLinksOutputTypeDef = TypedDict(
     "ListLinksOutputTypeDef",
     {
         "Items": List[ListLinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSinksOutputTypeDef = TypedDict(
     "ListSinksOutputTypeDef",
     {
         "Items": List[ListSinksItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/PKG-INFO` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-oam
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudWatchObservabilityAccessManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore oam type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore oam type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-oam"></a>
 
 # types-aiobotocore-oam
 
 [![PyPI - types-aiobotocore-oam](https://img.shields.io/pypi/v/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-oam.svg?color=blue)](https://pypi.org/project/types-aiobotocore-oam)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-oam?color=blue)](https://pypistats.org/packages/types-aiobotocore-oam)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-oam)](https://pepy.tech/project/types-aiobotocore-oam)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudWatchObservabilityAccessManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/oam.html#CloudWatchObservabilityAccessManager)
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
 [types-aiobotocore-oam docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_oam/).
 
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
@@ -315,61 +314,61 @@
 )
 
 
 def check_value(value: ListAttachedLinksPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_oam.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_oam.type_defs import (
     CreateLinkInputRequestTypeDef,
-    CreateLinkOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateSinkInputRequestTypeDef,
-    CreateSinkOutputTypeDef,
     DeleteLinkInputRequestTypeDef,
     DeleteSinkInputRequestTypeDef,
     GetLinkInputRequestTypeDef,
-    GetLinkOutputTypeDef,
     GetSinkInputRequestTypeDef,
-    GetSinkOutputTypeDef,
     GetSinkPolicyInputRequestTypeDef,
-    GetSinkPolicyOutputTypeDef,
-    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAttachedLinksInputRequestTypeDef,
     ListAttachedLinksItemTypeDef,
-    ListLinksInputListLinksPaginateTypeDef,
     ListLinksInputRequestTypeDef,
     ListLinksItemTypeDef,
-    ListSinksInputListSinksPaginateTypeDef,
     ListSinksInputRequestTypeDef,
     ListSinksItemTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
-    PaginatorConfigTypeDef,
     PutSinkPolicyInputRequestTypeDef,
-    PutSinkPolicyOutputTypeDef,
-    ResponseMetadataTypeDef,
     TagResourceInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateLinkInputRequestTypeDef,
+    CreateLinkOutputTypeDef,
+    CreateSinkOutputTypeDef,
+    GetLinkOutputTypeDef,
+    GetSinkOutputTypeDef,
+    GetSinkPolicyOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    PutSinkPolicyOutputTypeDef,
     UpdateLinkOutputTypeDef,
+    ListAttachedLinksInputListAttachedLinksPaginateTypeDef,
+    ListLinksInputListLinksPaginateTypeDef,
+    ListSinksInputListSinksPaginateTypeDef,
     ListAttachedLinksOutputTypeDef,
     ListLinksOutputTypeDef,
     ListSinksOutputTypeDef,
 )
 
 
-def get_structure() -> CreateLinkInputRequestTypeDef:
+def get_value() -> CreateLinkInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-oam-2.5.2/types_aiobotocore_oam.egg-info/SOURCES.txt` & `types-aiobotocore-oam-2.5.2.post1/types_aiobotocore_oam.egg-info/SOURCES.txt`

 * *Files identical despite different names*


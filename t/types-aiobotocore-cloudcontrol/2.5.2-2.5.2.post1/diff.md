# Comparing `tmp/types-aiobotocore-cloudcontrol-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudcontrol-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudcontrol-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudcontrol-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
```

## Comparing `types-aiobotocore-cloudcontrol-2.5.2.tar` & `types-aiobotocore-cloudcontrol-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.213819 types-aiobotocore-cloudcontrol-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-08 01:43:21.205819 types-aiobotocore-cloudcontrol-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13602 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.213819 types-aiobotocore-cloudcontrol-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.205819 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-07-08 01:26:51.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-07-08 01:26:51.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9726 2023-07-08 01:26:51.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-08 01:26:50.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.205819 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15190 2023-07-08 01:43:21.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-08 01:43:21.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:21.000000 types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12087 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9217 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-08-02 14:34:20.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-02 14:34:19.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.917637 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15126 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:51:59.000000 types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/LICENSE` & `types-aiobotocore-cloudcontrol-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudcontrol type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudcontrol type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudcontrol"></a>
 
 # types-aiobotocore-cloudcontrol
 
 [![PyPI - types-aiobotocore-cloudcontrol](https://img.shields.io/pypi/v/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudcontrol?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudcontrol)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudControlApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
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
@@ -342,52 +341,52 @@
 )
 
 
 def check_value(value: HandlerErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudcontrol.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
+    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
-def get_structure() -> CancelResourceRequestInputRequestTypeDef:
+def get_value() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/README.md` & `types-aiobotocore-cloudcontrol-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudcontrol"></a>
 
 # types-aiobotocore-cloudcontrol
 
 [![PyPI - types-aiobotocore-cloudcontrol](https://img.shields.io/pypi/v/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudcontrol?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudcontrol)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudControlApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
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
@@ -309,52 +309,52 @@
 )
 
 
 def check_value(value: HandlerErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudcontrol.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
+    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
-def get_structure() -> CancelResourceRequestInputRequestTypeDef:
+def get_value() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/setup.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudcontrol",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudcontrol"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudcontrol type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudcontrol type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudcontrol": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/"
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/__init__.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/__init__.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/__main__.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudControlApi 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudControlApi 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi\nOther"
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

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/client.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/client.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/literals.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/literals.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/paginator.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 
@@ -74,13 +74,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/paginator.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceRequestStatusFilter: ResourceRequestStatusFilterTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourceRequestsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResourceRequests.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcerequestspaginator)
         """
 
 class ListResourcesPaginator(AioPaginator):
@@ -70,13 +70,13 @@
     def paginate(
         self,
         *,
         TypeName: str,
         TypeVersionId: str = ...,
         RoleArn: str = ...,
         ResourceModel: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi.Paginator.ListResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/paginators/#listresourcespaginator)
         """
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/type_defs.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef
 
-    data: CancelResourceRequestInputRequestTypeDef = {...}
+    data: CancelResourceRequestInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import HandlerErrorCodeType, OperationStatusType, OperationType
@@ -22,35 +22,35 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
     "ResourceDescriptionTypeDef",
     "GetResourceRequestStatusInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceRequestStatusFilterTypeDef",
-    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourcesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateResourceInputRequestTypeDef",
     "CancelResourceRequestOutputTypeDef",
     "CreateResourceOutputTypeDef",
     "DeleteResourceOutputTypeDef",
     "GetResourceRequestStatusOutputTypeDef",
     "ListResourceRequestsOutputTypeDef",
     "UpdateResourceOutputTypeDef",
     "GetResourceOutputTypeDef",
     "ListResourcesOutputTypeDef",
     "GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
+    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     "ListResourceRequestsInputRequestTypeDef",
 )
 
 CancelResourceRequestInputRequestTypeDef = TypedDict(
     "CancelResourceRequestInputRequestTypeDef",
     {
@@ -71,14 +71,25 @@
         "StatusMessage": str,
         "ErrorCode": HandlerErrorCodeType,
         "RetryAfter": datetime,
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
 _RequiredCreateResourceInputRequestTypeDef = TypedDict(
     "_RequiredCreateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "DesiredState": str,
     },
 )
@@ -167,48 +178,33 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-ResourceRequestStatusFilterTypeDef = TypedDict(
-    "ResourceRequestStatusFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Operations": Sequence[OperationType],
-        "OperationStatuses": Sequence[OperationStatusType],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeName": str,
-    },
-)
-_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+ResourceRequestStatusFilterTypeDef = TypedDict(
+    "ResourceRequestStatusFilterTypeDef",
     {
-        "TypeVersionId": str,
-        "RoleArn": str,
-        "ResourceModel": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Operations": Sequence[OperationType],
+        "OperationStatuses": Sequence[OperationStatusType],
     },
     total=False,
 )
 
-
-class ListResourcesInputListResourcesPaginateTypeDef(
-    _RequiredListResourcesInputListResourcesPaginateTypeDef,
-    _OptionalListResourcesInputListResourcesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesInputRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalListResourcesInputRequestTypeDef = TypedDict(
@@ -226,35 +222,14 @@
 
 class ListResourcesInputRequestTypeDef(
     _RequiredListResourcesInputRequestTypeDef, _OptionalListResourcesInputRequestTypeDef
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
 _RequiredUpdateResourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "Identifier": str,
         "PatchDocument": str,
     },
@@ -276,75 +251,75 @@
     pass
 
 
 CancelResourceRequestOutputTypeDef = TypedDict(
     "CancelResourceRequestOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceOutputTypeDef = TypedDict(
     "CreateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResourceOutputTypeDef = TypedDict(
     "DeleteResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceRequestStatusOutputTypeDef = TypedDict(
     "GetResourceRequestStatusOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceRequestsOutputTypeDef = TypedDict(
     "ListResourceRequestsOutputTypeDef",
     {
         "ResourceRequestStatusSummaries": List[ProgressEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceOutputTypeDef = TypedDict(
     "UpdateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceOutputTypeDef = TypedDict(
     "GetResourceOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescription": ResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesOutputTypeDef = TypedDict(
     "ListResourcesOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescriptions": List[ResourceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef = TypedDict(
     "_RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
     {
         "RequestToken": str,
@@ -362,19 +337,44 @@
 class GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef(
     _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
     _OptionalGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
 ):
     pass
 
 
+_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeName": str,
+    },
+)
+_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeVersionId": str,
+        "RoleArn": str,
+        "ResourceModel": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourcesInputListResourcesPaginateTypeDef(
+    _RequiredListResourcesInputListResourcesPaginateTypeDef,
+    _OptionalListResourcesInputListResourcesPaginateTypeDef,
+):
+    pass
+
+
 ListResourceRequestsInputListResourceRequestsPaginateTypeDef = TypedDict(
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     {
         "ResourceRequestStatusFilter": ResourceRequestStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListResourceRequestsInputRequestTypeDef = TypedDict(
     "ListResourceRequestsInputRequestTypeDef",
     {
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/type_defs.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudcontrol.type_defs import CancelResourceRequestInputRequestTypeDef
 
-    data: CancelResourceRequestInputRequestTypeDef = {...}
+    data: CancelResourceRequestInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import HandlerErrorCodeType, OperationStatusType, OperationType
@@ -21,35 +21,35 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelResourceRequestInputRequestTypeDef",
     "ProgressEventTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateResourceInputRequestTypeDef",
     "DeleteResourceInputRequestTypeDef",
     "GetResourceInputRequestTypeDef",
     "ResourceDescriptionTypeDef",
     "GetResourceRequestStatusInputRequestTypeDef",
     "WaiterConfigTypeDef",
+    "PaginatorConfigTypeDef",
     "ResourceRequestStatusFilterTypeDef",
-    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourcesInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateResourceInputRequestTypeDef",
     "CancelResourceRequestOutputTypeDef",
     "CreateResourceOutputTypeDef",
     "DeleteResourceOutputTypeDef",
     "GetResourceRequestStatusOutputTypeDef",
     "ListResourceRequestsOutputTypeDef",
     "UpdateResourceOutputTypeDef",
     "GetResourceOutputTypeDef",
     "ListResourcesOutputTypeDef",
     "GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
+    "ListResourcesInputListResourcesPaginateTypeDef",
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     "ListResourceRequestsInputRequestTypeDef",
 )
 
 CancelResourceRequestInputRequestTypeDef = TypedDict(
     "CancelResourceRequestInputRequestTypeDef",
     {
@@ -70,14 +70,25 @@
         "StatusMessage": str,
         "ErrorCode": HandlerErrorCodeType,
         "RetryAfter": datetime,
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
 _RequiredCreateResourceInputRequestTypeDef = TypedDict(
     "_RequiredCreateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "DesiredState": str,
     },
 )
@@ -160,46 +171,33 @@
     {
         "Delay": int,
         "MaxAttempts": int,
     },
     total=False,
 )
 
-ResourceRequestStatusFilterTypeDef = TypedDict(
-    "ResourceRequestStatusFilterTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Operations": Sequence[OperationType],
-        "OperationStatuses": Sequence[OperationStatusType],
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
-    {
-        "TypeName": str,
-    },
-)
-_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
-    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+ResourceRequestStatusFilterTypeDef = TypedDict(
+    "ResourceRequestStatusFilterTypeDef",
     {
-        "TypeVersionId": str,
-        "RoleArn": str,
-        "ResourceModel": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "Operations": Sequence[OperationType],
+        "OperationStatuses": Sequence[OperationStatusType],
     },
     total=False,
 )
 
-class ListResourcesInputListResourcesPaginateTypeDef(
-    _RequiredListResourcesInputListResourcesPaginateTypeDef,
-    _OptionalListResourcesInputListResourcesPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourcesInputRequestTypeDef = TypedDict(
     "_RequiredListResourcesInputRequestTypeDef",
     {
         "TypeName": str,
     },
 )
 _OptionalListResourcesInputRequestTypeDef = TypedDict(
@@ -215,35 +213,14 @@
 )
 
 class ListResourcesInputRequestTypeDef(
     _RequiredListResourcesInputRequestTypeDef, _OptionalListResourcesInputRequestTypeDef
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
 _RequiredUpdateResourceInputRequestTypeDef = TypedDict(
     "_RequiredUpdateResourceInputRequestTypeDef",
     {
         "TypeName": str,
         "Identifier": str,
         "PatchDocument": str,
     },
@@ -263,75 +240,75 @@
 ):
     pass
 
 CancelResourceRequestOutputTypeDef = TypedDict(
     "CancelResourceRequestOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateResourceOutputTypeDef = TypedDict(
     "CreateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteResourceOutputTypeDef = TypedDict(
     "DeleteResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceRequestStatusOutputTypeDef = TypedDict(
     "GetResourceRequestStatusOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceRequestsOutputTypeDef = TypedDict(
     "ListResourceRequestsOutputTypeDef",
     {
         "ResourceRequestStatusSummaries": List[ProgressEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceOutputTypeDef = TypedDict(
     "UpdateResourceOutputTypeDef",
     {
         "ProgressEvent": ProgressEventTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourceOutputTypeDef = TypedDict(
     "GetResourceOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescription": ResourceDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourcesOutputTypeDef = TypedDict(
     "ListResourcesOutputTypeDef",
     {
         "TypeName": str,
         "ResourceDescriptions": List[ResourceDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef = TypedDict(
     "_RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef",
     {
         "RequestToken": str,
@@ -347,19 +324,42 @@
 
 class GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef(
     _RequiredGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
     _OptionalGetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
 ):
     pass
 
+_RequiredListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_RequiredListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeName": str,
+    },
+)
+_OptionalListResourcesInputListResourcesPaginateTypeDef = TypedDict(
+    "_OptionalListResourcesInputListResourcesPaginateTypeDef",
+    {
+        "TypeVersionId": str,
+        "RoleArn": str,
+        "ResourceModel": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourcesInputListResourcesPaginateTypeDef(
+    _RequiredListResourcesInputListResourcesPaginateTypeDef,
+    _OptionalListResourcesInputListResourcesPaginateTypeDef,
+):
+    pass
+
 ListResourceRequestsInputListResourceRequestsPaginateTypeDef = TypedDict(
     "ListResourceRequestsInputListResourceRequestsPaginateTypeDef",
     {
         "ResourceRequestStatusFilter": ResourceRequestStatusFilterTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListResourceRequestsInputRequestTypeDef = TypedDict(
     "ListResourceRequestsInputRequestTypeDef",
     {
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/waiter.py` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol/waiter.pyi` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudcontrol
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudControlApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudcontrol type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudcontrol type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudcontrol"></a>
 
 # types-aiobotocore-cloudcontrol
 
 [![PyPI - types-aiobotocore-cloudcontrol](https://img.shields.io/pypi/v/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudcontrol.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudcontrol)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudcontrol?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudcontrol)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudcontrol)](https://pepy.tech/project/types-aiobotocore-cloudcontrol)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudControlApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudcontrol.html#CloudControlApi)
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
 [types-aiobotocore-cloudcontrol docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudcontrol/).
 
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
@@ -342,52 +341,52 @@
 )
 
 
 def check_value(value: HandlerErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudcontrol.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudcontrol.type_defs import (
     CancelResourceRequestInputRequestTypeDef,
     ProgressEventTypeDef,
+    ResponseMetadataTypeDef,
     CreateResourceInputRequestTypeDef,
     DeleteResourceInputRequestTypeDef,
     GetResourceInputRequestTypeDef,
     ResourceDescriptionTypeDef,
     GetResourceRequestStatusInputRequestTypeDef,
     WaiterConfigTypeDef,
+    PaginatorConfigTypeDef,
     ResourceRequestStatusFilterTypeDef,
-    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourcesInputRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateResourceInputRequestTypeDef,
     CancelResourceRequestOutputTypeDef,
     CreateResourceOutputTypeDef,
     DeleteResourceOutputTypeDef,
     GetResourceRequestStatusOutputTypeDef,
     ListResourceRequestsOutputTypeDef,
     UpdateResourceOutputTypeDef,
     GetResourceOutputTypeDef,
     ListResourcesOutputTypeDef,
     GetResourceRequestStatusInputResourceRequestSuccessWaitTypeDef,
+    ListResourcesInputListResourcesPaginateTypeDef,
     ListResourceRequestsInputListResourceRequestsPaginateTypeDef,
     ListResourceRequestsInputRequestTypeDef,
 )
 
 
-def get_structure() -> CancelResourceRequestInputRequestTypeDef:
+def get_value() -> CancelResourceRequestInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudcontrol-2.5.2/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt` & `types-aiobotocore-cloudcontrol-2.5.2.post1/types_aiobotocore_cloudcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*


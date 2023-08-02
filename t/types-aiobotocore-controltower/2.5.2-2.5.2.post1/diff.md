# Comparing `tmp/types-aiobotocore-controltower-2.5.2.tar.gz` & `tmp/types-aiobotocore-controltower-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-controltower-2.5.2.tar", last modified: Sat Jul  8 01:43:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-controltower-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
```

## Comparing `types-aiobotocore-controltower-2.5.2.tar` & `types-aiobotocore-controltower-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.473958 types-aiobotocore-controltower-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-07-08 01:43:28.473958 types-aiobotocore-controltower-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:28.473958 types-aiobotocore-controltower-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.473958 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-07-08 01:28:20.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:19.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.473958 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13660 2023-07-08 01:43:28.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:28.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:28.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:28.000000 types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.357613 types-aiobotocore-controltower-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-02 14:52:07.345613 types-aiobotocore-controltower-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.357613 types-aiobotocore-controltower-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:35:55.000000 types-aiobotocore-controltower-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.337613 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7361 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8413 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-08-02 14:35:57.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:56.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.345613 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13596 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:07.000000 types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-controltower-2.5.2/LICENSE` & `types-aiobotocore-controltower-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/PKG-INFO` & `types-aiobotocore-controltower-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-controltower
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore controltower type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore controltower type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-controltower"></a>
 
 # types-aiobotocore-controltower
 
 [![PyPI - types-aiobotocore-controltower](https://img.shields.io/pypi/v/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-controltower?color=blue)](https://pypistats.org/packages/types-aiobotocore-controltower)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-controltower)](https://pepy.tech/project/types-aiobotocore-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ControlTower 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
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
@@ -309,40 +308,40 @@
 )
 
 
 def check_value(value: ControlOperationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_controltower.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_controltower.type_defs import (
     ControlOperationTypeDef,
     DisableControlInputRequestTypeDef,
-    DisableControlOutputTypeDef,
+    ResponseMetadataTypeDef,
     EnableControlInputRequestTypeDef,
-    EnableControlOutputTypeDef,
     EnabledControlSummaryTypeDef,
     GetControlOperationInputRequestTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListEnabledControlsInputRequestTypeDef,
+    DisableControlOutputTypeDef,
+    EnableControlOutputTypeDef,
     GetControlOperationOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
+    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
 )
 
 
-def get_structure() -> ControlOperationTypeDef:
+def get_value() -> ControlOperationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-controltower-2.5.2/README.md` & `types-aiobotocore-controltower-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-controltower"></a>
 
 # types-aiobotocore-controltower
 
 [![PyPI - types-aiobotocore-controltower](https://img.shields.io/pypi/v/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-controltower?color=blue)](https://pypistats.org/packages/types-aiobotocore-controltower)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-controltower)](https://pepy.tech/project/types-aiobotocore-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ControlTower 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
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
@@ -276,40 +276,40 @@
 )
 
 
 def check_value(value: ControlOperationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_controltower.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_controltower.type_defs import (
     ControlOperationTypeDef,
     DisableControlInputRequestTypeDef,
-    DisableControlOutputTypeDef,
+    ResponseMetadataTypeDef,
     EnableControlInputRequestTypeDef,
-    EnableControlOutputTypeDef,
     EnabledControlSummaryTypeDef,
     GetControlOperationInputRequestTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListEnabledControlsInputRequestTypeDef,
+    DisableControlOutputTypeDef,
+    EnableControlOutputTypeDef,
     GetControlOperationOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
+    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
 )
 
 
-def get_structure() -> ControlOperationTypeDef:
+def get_value() -> ControlOperationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-controltower-2.5.2/setup.py` & `types-aiobotocore-controltower-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-controltower",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_controltower"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ControlTower 2.5.2 service generated with"
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
-    keywords="aiobotocore controltower type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore controltower type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_controltower": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/"
```

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/__init__.py` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/__init__.pyi` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/__main__.py` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ControlTower 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ControlTower 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower\nOther"
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

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/client.py` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/client.pyi` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/literals.py` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/literals.pyi` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/paginator.py` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,13 +43,13 @@
 class ListEnabledControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/paginators/#listenabledcontrolspaginator)
     """
 
     def paginate(
-        self, *, targetIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnabledControlsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/paginators/#listenabledcontrolspaginator)
         """
```

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/paginator.pyi` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/paginator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -40,13 +40,13 @@
 class ListEnabledControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/paginators/#listenabledcontrolspaginator)
     """
 
     def paginate(
-        self, *, targetIdentifier: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, targetIdentifier: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnabledControlsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower.Paginator.ListEnabledControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/paginators/#listenabledcontrolspaginator)
         """
```

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/type_defs.py` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_controltower.type_defs import ControlOperationTypeDef
 
-    data: ControlOperationTypeDef = {...}
+    data: ControlOperationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import ControlOperationStatusType, ControlOperationTypeType
@@ -22,25 +22,25 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ControlOperationTypeDef",
     "DisableControlInputRequestTypeDef",
-    "DisableControlOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EnableControlInputRequestTypeDef",
-    "EnableControlOutputTypeDef",
     "EnabledControlSummaryTypeDef",
     "GetControlOperationInputRequestTypeDef",
-    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    "ListEnabledControlsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListEnabledControlsInputRequestTypeDef",
+    "DisableControlOutputTypeDef",
+    "EnableControlOutputTypeDef",
     "GetControlOperationOutputTypeDef",
     "ListEnabledControlsOutputTypeDef",
+    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
 )
 
 ControlOperationTypeDef = TypedDict(
     "ControlOperationTypeDef",
     {
         "endTime": datetime,
         "operationType": ControlOperationTypeType,
@@ -55,38 +55,33 @@
     "DisableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-DisableControlOutputTypeDef = TypedDict(
-    "DisableControlOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EnableControlInputRequestTypeDef = TypedDict(
     "EnableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-EnableControlOutputTypeDef = TypedDict(
-    "EnableControlOutputTypeDef",
-    {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnabledControlSummaryTypeDef = TypedDict(
     "EnabledControlSummaryTypeDef",
     {
         "controlIdentifier": str,
     },
     total=False,
 )
@@ -94,36 +89,24 @@
 GetControlOperationInputRequestTypeDef = TypedDict(
     "GetControlOperationInputRequestTypeDef",
     {
         "operationIdentifier": str,
     },
 )
 
-_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    {
-        "targetIdentifier": str,
-    },
-)
-_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
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
-class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
-    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListEnabledControlsInputRequestTypeDef = TypedDict(
     "_RequiredListEnabledControlsInputRequestTypeDef",
     {
         "targetIdentifier": str,
     },
 )
 _OptionalListEnabledControlsInputRequestTypeDef = TypedDict(
@@ -138,44 +121,60 @@
 
 class ListEnabledControlsInputRequestTypeDef(
     _RequiredListEnabledControlsInputRequestTypeDef, _OptionalListEnabledControlsInputRequestTypeDef
 ):
     pass
 
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DisableControlOutputTypeDef = TypedDict(
+    "DisableControlOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EnableControlOutputTypeDef = TypedDict(
+    "EnableControlOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlOperationOutputTypeDef = TypedDict(
     "GetControlOperationOutputTypeDef",
     {
         "controlOperation": ControlOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnabledControlsOutputTypeDef = TypedDict(
     "ListEnabledControlsOutputTypeDef",
     {
         "enabledControls": List[EnabledControlSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "targetIdentifier": str,
+    },
+)
+_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
+    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower/type_defs.pyi` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_controltower.type_defs import ControlOperationTypeDef
 
-    data: ControlOperationTypeDef = {...}
+    data: ControlOperationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import ControlOperationStatusType, ControlOperationTypeType
@@ -21,25 +21,25 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ControlOperationTypeDef",
     "DisableControlInputRequestTypeDef",
-    "DisableControlOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "EnableControlInputRequestTypeDef",
-    "EnableControlOutputTypeDef",
     "EnabledControlSummaryTypeDef",
     "GetControlOperationInputRequestTypeDef",
-    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    "ListEnabledControlsInputRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "ListEnabledControlsInputRequestTypeDef",
+    "DisableControlOutputTypeDef",
+    "EnableControlOutputTypeDef",
     "GetControlOperationOutputTypeDef",
     "ListEnabledControlsOutputTypeDef",
+    "ListEnabledControlsInputListEnabledControlsPaginateTypeDef",
 )
 
 ControlOperationTypeDef = TypedDict(
     "ControlOperationTypeDef",
     {
         "endTime": datetime,
         "operationType": ControlOperationTypeType,
@@ -54,38 +54,33 @@
     "DisableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-DisableControlOutputTypeDef = TypedDict(
-    "DisableControlOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 EnableControlInputRequestTypeDef = TypedDict(
     "EnableControlInputRequestTypeDef",
     {
         "controlIdentifier": str,
         "targetIdentifier": str,
     },
 )
 
-EnableControlOutputTypeDef = TypedDict(
-    "EnableControlOutputTypeDef",
-    {
-        "operationIdentifier": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 EnabledControlSummaryTypeDef = TypedDict(
     "EnabledControlSummaryTypeDef",
     {
         "controlIdentifier": str,
     },
     total=False,
 )
@@ -93,34 +88,24 @@
 GetControlOperationInputRequestTypeDef = TypedDict(
     "GetControlOperationInputRequestTypeDef",
     {
         "operationIdentifier": str,
     },
 )
 
-_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
-    {
-        "targetIdentifier": str,
-    },
-)
-_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
-    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
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
 
-class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
-    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-):
-    pass
-
 _RequiredListEnabledControlsInputRequestTypeDef = TypedDict(
     "_RequiredListEnabledControlsInputRequestTypeDef",
     {
         "targetIdentifier": str,
     },
 )
 _OptionalListEnabledControlsInputRequestTypeDef = TypedDict(
@@ -133,44 +118,59 @@
 )
 
 class ListEnabledControlsInputRequestTypeDef(
     _RequiredListEnabledControlsInputRequestTypeDef, _OptionalListEnabledControlsInputRequestTypeDef
 ):
     pass
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DisableControlOutputTypeDef = TypedDict(
+    "DisableControlOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EnableControlOutputTypeDef = TypedDict(
+    "EnableControlOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "operationIdentifier": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetControlOperationOutputTypeDef = TypedDict(
     "GetControlOperationOutputTypeDef",
     {
         "controlOperation": ControlOperationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListEnabledControlsOutputTypeDef = TypedDict(
     "ListEnabledControlsOutputTypeDef",
     {
         "enabledControls": List[EnabledControlSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "targetIdentifier": str,
+    },
+)
+_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef = TypedDict(
+    "_OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListEnabledControlsInputListEnabledControlsPaginateTypeDef(
+    _RequiredListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+    _OptionalListEnabledControlsInputListEnabledControlsPaginateTypeDef,
+):
+    pass
```

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/PKG-INFO` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-controltower
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ControlTower 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore controltower type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore controltower type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-controltower"></a>
 
 # types-aiobotocore-controltower
 
 [![PyPI - types-aiobotocore-controltower](https://img.shields.io/pypi/v/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-controltower.svg?color=blue)](https://pypi.org/project/types-aiobotocore-controltower)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-controltower?color=blue)](https://pypistats.org/packages/types-aiobotocore-controltower)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-controltower)](https://pepy.tech/project/types-aiobotocore-controltower)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ControlTower 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/controltower.html#ControlTower)
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
 [types-aiobotocore-controltower docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_controltower/).
 
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
@@ -309,40 +308,40 @@
 )
 
 
 def check_value(value: ControlOperationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_controltower.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_controltower.type_defs import (
     ControlOperationTypeDef,
     DisableControlInputRequestTypeDef,
-    DisableControlOutputTypeDef,
+    ResponseMetadataTypeDef,
     EnableControlInputRequestTypeDef,
-    EnableControlOutputTypeDef,
     EnabledControlSummaryTypeDef,
     GetControlOperationInputRequestTypeDef,
-    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
-    ListEnabledControlsInputRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    ListEnabledControlsInputRequestTypeDef,
+    DisableControlOutputTypeDef,
+    EnableControlOutputTypeDef,
     GetControlOperationOutputTypeDef,
     ListEnabledControlsOutputTypeDef,
+    ListEnabledControlsInputListEnabledControlsPaginateTypeDef,
 )
 
 
-def get_structure() -> ControlOperationTypeDef:
+def get_value() -> ControlOperationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-controltower-2.5.2/types_aiobotocore_controltower.egg-info/SOURCES.txt` & `types-aiobotocore-controltower-2.5.2.post1/types_aiobotocore_controltower.egg-info/SOURCES.txt`

 * *Files identical despite different names*


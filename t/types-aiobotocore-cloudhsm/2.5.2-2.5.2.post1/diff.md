# Comparing `tmp/types-aiobotocore-cloudhsm-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudhsm-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsm-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
```

## Comparing `types-aiobotocore-cloudhsm-2.5.2.tar` & `types-aiobotocore-cloudhsm-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.469824 types-aiobotocore-cloudhsm-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-07-08 01:43:21.469824 types-aiobotocore-cloudhsm-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13304 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.469824 types-aiobotocore-cloudhsm-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.461824 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    12642 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:07.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.469824 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14873 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13287 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.061637 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16664 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16632 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8289 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12603 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:39.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.065636 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14809 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/LICENSE` & `types-aiobotocore-cloudhsm-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/PKG-INFO` & `types-aiobotocore-cloudhsm-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudhsm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudhsm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsm?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudHSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
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
@@ -318,72 +317,72 @@
 )
 
 
 def check_value(value: ClientVersionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudhsm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudhsm.type_defs import (
     TagTypeDef,
-    AddTagsToResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateHapgRequestRequestTypeDef,
-    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
-    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
-    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
-    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
-    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
-    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
-    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
-    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHapgsRequestRequestTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyHapgRequestRequestTypeDef,
-    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
-    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
+    AddTagsToResourceResponseTypeDef,
+    CreateHapgResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    CreateLunaClientResponseTypeDef,
+    DeleteHapgResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    DeleteLunaClientResponseTypeDef,
+    DescribeHapgResponseTypeDef,
+    DescribeHsmResponseTypeDef,
+    DescribeLunaClientResponseTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModifyHapgResponseTypeDef,
+    ModifyHsmResponseTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/README.md` & `types-aiobotocore-cloudhsm-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsm?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudHSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
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
@@ -285,72 +285,72 @@
 )
 
 
 def check_value(value: ClientVersionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudhsm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudhsm.type_defs import (
     TagTypeDef,
-    AddTagsToResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateHapgRequestRequestTypeDef,
-    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
-    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
-    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
-    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
-    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
-    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
-    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
-    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHapgsRequestRequestTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyHapgRequestRequestTypeDef,
-    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
-    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
+    AddTagsToResourceResponseTypeDef,
+    CreateHapgResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    CreateLunaClientResponseTypeDef,
+    DeleteHapgResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    DeleteLunaClientResponseTypeDef,
+    DescribeHapgResponseTypeDef,
+    DescribeHsmResponseTypeDef,
+    DescribeLunaClientResponseTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModifyHapgResponseTypeDef,
+    ModifyHsmResponseTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/setup.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsm",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudhsm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore cloudhsm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudhsm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudhsm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/"
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/__init__.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/__init__.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/__main__.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSM 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudHSM 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM\nOther"
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

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/client.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/client.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/literals.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/literals.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/paginator.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,43 +52,43 @@
 class ListHapgsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhapgspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHapgsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhapgspaginator)
         """
 
 
 class ListHsmsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhsmspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHsmsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhsmspaginator)
         """
 
 
 class ListLunaClientsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listlunaclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLunaClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listlunaclientspaginator)
         """
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/paginator.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -49,41 +49,41 @@
 class ListHapgsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhapgspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHapgsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHapgs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhapgspaginator)
         """
 
 class ListHsmsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhsmspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHsmsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListHsms.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listhsmspaginator)
         """
 
 class ListLunaClientsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listlunaclientspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLunaClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM.Paginator.ListLunaClients.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/paginators/#listlunaclientspaginator)
         """
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/type_defs.py` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudhsm.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import ClientVersionType, CloudHsmObjectStateType, HsmStatusType
 
@@ -21,94 +21,88 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "TagTypeDef",
-    "AddTagsToResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHapgRequestRequestTypeDef",
-    "CreateHapgResponseTypeDef",
     "CreateHsmRequestRequestTypeDef",
-    "CreateHsmResponseTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
-    "CreateLunaClientResponseTypeDef",
     "DeleteHapgRequestRequestTypeDef",
-    "DeleteHapgResponseTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
     "DeleteLunaClientRequestRequestTypeDef",
-    "DeleteLunaClientResponseTypeDef",
     "DescribeHapgRequestRequestTypeDef",
-    "DescribeHapgResponseTypeDef",
     "DescribeHsmRequestRequestTypeDef",
-    "DescribeHsmResponseTypeDef",
     "DescribeLunaClientRequestRequestTypeDef",
-    "DescribeLunaClientResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
-    "GetConfigResponseTypeDef",
-    "ListAvailableZonesResponseTypeDef",
-    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListHapgsRequestRequestTypeDef",
-    "ListHapgsResponseTypeDef",
-    "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
-    "ListHsmsResponseTypeDef",
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
-    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyHapgRequestRequestTypeDef",
-    "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
-    "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
-    "ModifyLunaClientResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
-    "RemoveTagsFromResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
+    "AddTagsToResourceResponseTypeDef",
+    "CreateHapgResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "CreateLunaClientResponseTypeDef",
+    "DeleteHapgResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "DeleteLunaClientResponseTypeDef",
+    "DescribeHapgResponseTypeDef",
+    "DescribeHsmResponseTypeDef",
+    "DescribeLunaClientResponseTypeDef",
+    "GetConfigResponseTypeDef",
+    "ListAvailableZonesResponseTypeDef",
+    "ListHapgsResponseTypeDef",
+    "ListHsmsResponseTypeDef",
+    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ModifyHapgResponseTypeDef",
+    "ModifyHsmResponseTypeDef",
+    "ModifyLunaClientResponseTypeDef",
+    "RemoveTagsFromResourceResponseTypeDef",
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AddTagsToResourceResponseTypeDef = TypedDict(
-    "AddTagsToResourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateHapgRequestRequestTypeDef = TypedDict(
     "CreateHapgRequestRequestTypeDef",
     {
         "Label": str,
     },
 )
 
-CreateHapgResponseTypeDef = TypedDict(
-    "CreateHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "SubnetId": str,
         "SshKey": str,
         "IamRoleArn": str,
         "SubscriptionType": Literal["PRODUCTION"],
@@ -121,286 +115,127 @@
         "ExternalId": str,
         "ClientToken": str,
         "SyslogIp": str,
     },
     total=False,
 )
 
-
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
-
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLunaClientRequestRequestTypeDef",
     {
         "Certificate": str,
     },
 )
 _OptionalCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_OptionalCreateLunaClientRequestRequestTypeDef",
     {
         "Label": str,
     },
     total=False,
 )
 
-
 class CreateLunaClientRequestRequestTypeDef(
     _RequiredCreateLunaClientRequestRequestTypeDef, _OptionalCreateLunaClientRequestRequestTypeDef
 ):
     pass
 
-
-CreateLunaClientResponseTypeDef = TypedDict(
-    "CreateLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHapgRequestRequestTypeDef = TypedDict(
     "DeleteHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DeleteHapgResponseTypeDef = TypedDict(
-    "DeleteHapgResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHsmRequestRequestTypeDef = TypedDict(
     "DeleteHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLunaClientRequestRequestTypeDef = TypedDict(
     "DeleteLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
     },
 )
 
-DeleteLunaClientResponseTypeDef = TypedDict(
-    "DeleteLunaClientResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHapgRequestRequestTypeDef = TypedDict(
     "DescribeHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DescribeHapgResponseTypeDef = TypedDict(
-    "DescribeHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "HapgSerial": str,
-        "HsmsLastActionFailed": List[str],
-        "HsmsPendingDeletion": List[str],
-        "HsmsPendingRegistration": List[str],
-        "Label": str,
-        "LastModifiedTimestamp": str,
-        "PartitionSerialList": List[str],
-        "State": CloudHsmObjectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHsmRequestRequestTypeDef = TypedDict(
     "DescribeHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
         "HsmSerialNumber": str,
     },
     total=False,
 )
 
-DescribeHsmResponseTypeDef = TypedDict(
-    "DescribeHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "Status": HsmStatusType,
-        "StatusDetails": str,
-        "AvailabilityZone": str,
-        "EniId": str,
-        "EniIp": str,
-        "SubscriptionType": Literal["PRODUCTION"],
-        "SubscriptionStartDate": str,
-        "SubscriptionEndDate": str,
-        "VpcId": str,
-        "SubnetId": str,
-        "IamRoleArn": str,
-        "SerialNumber": str,
-        "VendorName": str,
-        "HsmType": str,
-        "SoftwareVersion": str,
-        "SshPublicKey": str,
-        "SshKeyLastUpdated": str,
-        "ServerCertUri": str,
-        "ServerCertLastUpdated": str,
-        "Partitions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeLunaClientRequestRequestTypeDef = TypedDict(
     "DescribeLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "CertificateFingerprint": str,
     },
     total=False,
 )
 
-DescribeLunaClientResponseTypeDef = TypedDict(
-    "DescribeLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "Certificate": str,
-        "CertificateFingerprint": str,
-        "LastModifiedTimestamp": str,
-        "Label": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "ClientArn": str,
         "ClientVersion": ClientVersionType,
         "HapgList": Sequence[str],
     },
 )
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "ConfigType": str,
-        "ConfigFile": str,
-        "ConfigCred": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAvailableZonesResponseTypeDef = TypedDict(
-    "ListAvailableZonesResponseTypeDef",
-    {
-        "AZList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
-    "ListHapgsRequestListHapgsPaginateTypeDef",
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
 
 ListHapgsRequestRequestTypeDef = TypedDict(
     "ListHapgsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHapgsResponseTypeDef = TypedDict(
-    "ListHapgsResponseTypeDef",
-    {
-        "HapgList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
-    "ListHsmsRequestListHsmsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHsmsRequestRequestTypeDef = TypedDict(
     "ListHsmsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHsmsResponseTypeDef = TypedDict(
-    "ListHsmsResponseTypeDef",
-    {
-        "HsmList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLunaClientsRequestRequestTypeDef = TypedDict(
     "ListLunaClientsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListLunaClientsResponseTypeDef = TypedDict(
-    "ListLunaClientsResponseTypeDef",
-    {
-        "ClientList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -415,29 +250,19 @@
     {
         "Label": str,
         "PartitionSerialList": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyHapgRequestRequestTypeDef(
     _RequiredModifyHapgRequestRequestTypeDef, _OptionalModifyHapgRequestRequestTypeDef
 ):
     pass
 
-
-ModifyHapgResponseTypeDef = TypedDict(
-    "ModifyHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredModifyHsmRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 _OptionalModifyHsmRequestRequestTypeDef = TypedDict(
@@ -448,90 +273,256 @@
         "IamRoleArn": str,
         "ExternalId": str,
         "SyslogIp": str,
     },
     total=False,
 )
 
-
 class ModifyHsmRequestRequestTypeDef(
     _RequiredModifyHsmRequestRequestTypeDef, _OptionalModifyHsmRequestRequestTypeDef
 ):
     pass
 
+ModifyLunaClientRequestRequestTypeDef = TypedDict(
+    "ModifyLunaClientRequestRequestTypeDef",
+    {
+        "ClientArn": str,
+        "Certificate": str,
+    },
+)
+
+RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeyList": Sequence[str],
+    },
+)
 
-ModifyHsmResponseTypeDef = TypedDict(
-    "ModifyHsmResponseTypeDef",
+AddTagsToResourceRequestRequestTypeDef = TypedDict(
+    "AddTagsToResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
+    },
+)
+
+AddTagsToResourceResponseTypeDef = TypedDict(
+    "AddTagsToResourceResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHapgResponseTypeDef = TypedDict(
+    "CreateHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
     {
         "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLunaClientRequestRequestTypeDef = TypedDict(
-    "ModifyLunaClientRequestRequestTypeDef",
+CreateLunaClientResponseTypeDef = TypedDict(
+    "CreateLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "Certificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ModifyLunaClientResponseTypeDef = TypedDict(
-    "ModifyLunaClientResponseTypeDef",
+DeleteHapgResponseTypeDef = TypedDict(
+    "DeleteHapgResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DeleteLunaClientResponseTypeDef = TypedDict(
+    "DeleteLunaClientResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHapgResponseTypeDef = TypedDict(
+    "DescribeHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "HapgSerial": str,
+        "HsmsLastActionFailed": List[str],
+        "HsmsPendingDeletion": List[str],
+        "HsmsPendingRegistration": List[str],
+        "Label": str,
+        "LastModifiedTimestamp": str,
+        "PartitionSerialList": List[str],
+        "State": CloudHsmObjectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeHsmResponseTypeDef = TypedDict(
+    "DescribeHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "Status": HsmStatusType,
+        "StatusDetails": str,
+        "AvailabilityZone": str,
+        "EniId": str,
+        "EniIp": str,
+        "SubscriptionType": Literal["PRODUCTION"],
+        "SubscriptionStartDate": str,
+        "SubscriptionEndDate": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "IamRoleArn": str,
+        "SerialNumber": str,
+        "VendorName": str,
+        "HsmType": str,
+        "SoftwareVersion": str,
+        "SshPublicKey": str,
+        "SshKeyLastUpdated": str,
+        "ServerCertUri": str,
+        "ServerCertLastUpdated": str,
+        "Partitions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLunaClientResponseTypeDef = TypedDict(
+    "DescribeLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "Certificate": str,
+        "CertificateFingerprint": str,
+        "LastModifiedTimestamp": str,
+        "Label": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ConfigType": str,
+        "ConfigFile": str,
+        "ConfigCred": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromResourceRequestRequestTypeDef",
+ListAvailableZonesResponseTypeDef = TypedDict(
+    "ListAvailableZonesResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeyList": Sequence[str],
+        "AZList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveTagsFromResourceResponseTypeDef = TypedDict(
-    "RemoveTagsFromResourceResponseTypeDef",
+ListHapgsResponseTypeDef = TypedDict(
+    "ListHapgsResponseTypeDef",
     {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HapgList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+ListHsmsResponseTypeDef = TypedDict(
+    "ListHsmsResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "HsmList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddTagsToResourceRequestRequestTypeDef = TypedDict(
-    "AddTagsToResourceRequestRequestTypeDef",
+ListLunaClientsResponseTypeDef = TypedDict(
+    "ListLunaClientsResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
+        "ClientList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHapgResponseTypeDef = TypedDict(
+    "ModifyHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHsmResponseTypeDef = TypedDict(
+    "ModifyHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyLunaClientResponseTypeDef = TypedDict(
+    "ModifyLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveTagsFromResourceResponseTypeDef = TypedDict(
+    "RemoveTagsFromResourceResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm/type_defs.pyi` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudhsm.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import ClientVersionType, CloudHsmObjectStateType, HsmStatusType
 
@@ -21,93 +21,89 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "TagTypeDef",
-    "AddTagsToResourceResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHapgRequestRequestTypeDef",
-    "CreateHapgResponseTypeDef",
     "CreateHsmRequestRequestTypeDef",
-    "CreateHsmResponseTypeDef",
     "CreateLunaClientRequestRequestTypeDef",
-    "CreateLunaClientResponseTypeDef",
     "DeleteHapgRequestRequestTypeDef",
-    "DeleteHapgResponseTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
     "DeleteLunaClientRequestRequestTypeDef",
-    "DeleteLunaClientResponseTypeDef",
     "DescribeHapgRequestRequestTypeDef",
-    "DescribeHapgResponseTypeDef",
     "DescribeHsmRequestRequestTypeDef",
-    "DescribeHsmResponseTypeDef",
     "DescribeLunaClientRequestRequestTypeDef",
-    "DescribeLunaClientResponseTypeDef",
     "GetConfigRequestRequestTypeDef",
-    "GetConfigResponseTypeDef",
-    "ListAvailableZonesResponseTypeDef",
-    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListHapgsRequestRequestTypeDef",
-    "ListHapgsResponseTypeDef",
-    "ListHsmsRequestListHsmsPaginateTypeDef",
     "ListHsmsRequestRequestTypeDef",
-    "ListHsmsResponseTypeDef",
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
     "ListLunaClientsRequestRequestTypeDef",
-    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyHapgRequestRequestTypeDef",
-    "ModifyHapgResponseTypeDef",
     "ModifyHsmRequestRequestTypeDef",
-    "ModifyHsmResponseTypeDef",
     "ModifyLunaClientRequestRequestTypeDef",
-    "ModifyLunaClientResponseTypeDef",
-    "PaginatorConfigTypeDef",
     "RemoveTagsFromResourceRequestRequestTypeDef",
-    "RemoveTagsFromResourceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "AddTagsToResourceRequestRequestTypeDef",
+    "AddTagsToResourceResponseTypeDef",
+    "CreateHapgResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "CreateLunaClientResponseTypeDef",
+    "DeleteHapgResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "DeleteLunaClientResponseTypeDef",
+    "DescribeHapgResponseTypeDef",
+    "DescribeHsmResponseTypeDef",
+    "DescribeLunaClientResponseTypeDef",
+    "GetConfigResponseTypeDef",
+    "ListAvailableZonesResponseTypeDef",
+    "ListHapgsResponseTypeDef",
+    "ListHsmsResponseTypeDef",
+    "ListLunaClientsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
+    "ModifyHapgResponseTypeDef",
+    "ModifyHsmResponseTypeDef",
+    "ModifyLunaClientResponseTypeDef",
+    "RemoveTagsFromResourceResponseTypeDef",
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-AddTagsToResourceResponseTypeDef = TypedDict(
-    "AddTagsToResourceResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateHapgRequestRequestTypeDef = TypedDict(
     "CreateHapgRequestRequestTypeDef",
     {
         "Label": str,
     },
 )
 
-CreateHapgResponseTypeDef = TypedDict(
-    "CreateHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "SubnetId": str,
         "SshKey": str,
         "IamRoleArn": str,
         "SubscriptionType": Literal["PRODUCTION"],
@@ -120,26 +116,20 @@
         "ExternalId": str,
         "ClientToken": str,
         "SyslogIp": str,
     },
     total=False,
 )
 
+
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
-CreateHsmResponseTypeDef = TypedDict(
-    "CreateHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredCreateLunaClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateLunaClientRequestRequestTypeDef",
     {
         "Certificate": str,
     },
 )
@@ -147,255 +137,110 @@
     "_OptionalCreateLunaClientRequestRequestTypeDef",
     {
         "Label": str,
     },
     total=False,
 )
 
+
 class CreateLunaClientRequestRequestTypeDef(
     _RequiredCreateLunaClientRequestRequestTypeDef, _OptionalCreateLunaClientRequestRequestTypeDef
 ):
     pass
 
-CreateLunaClientResponseTypeDef = TypedDict(
-    "CreateLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DeleteHapgRequestRequestTypeDef = TypedDict(
     "DeleteHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DeleteHapgResponseTypeDef = TypedDict(
-    "DeleteHapgResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteHsmRequestRequestTypeDef = TypedDict(
     "DeleteHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeleteLunaClientRequestRequestTypeDef = TypedDict(
     "DeleteLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
     },
 )
 
-DeleteLunaClientResponseTypeDef = TypedDict(
-    "DeleteLunaClientResponseTypeDef",
-    {
-        "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHapgRequestRequestTypeDef = TypedDict(
     "DescribeHapgRequestRequestTypeDef",
     {
         "HapgArn": str,
     },
 )
 
-DescribeHapgResponseTypeDef = TypedDict(
-    "DescribeHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "HapgSerial": str,
-        "HsmsLastActionFailed": List[str],
-        "HsmsPendingDeletion": List[str],
-        "HsmsPendingRegistration": List[str],
-        "Label": str,
-        "LastModifiedTimestamp": str,
-        "PartitionSerialList": List[str],
-        "State": CloudHsmObjectStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeHsmRequestRequestTypeDef = TypedDict(
     "DescribeHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
         "HsmSerialNumber": str,
     },
     total=False,
 )
 
-DescribeHsmResponseTypeDef = TypedDict(
-    "DescribeHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "Status": HsmStatusType,
-        "StatusDetails": str,
-        "AvailabilityZone": str,
-        "EniId": str,
-        "EniIp": str,
-        "SubscriptionType": Literal["PRODUCTION"],
-        "SubscriptionStartDate": str,
-        "SubscriptionEndDate": str,
-        "VpcId": str,
-        "SubnetId": str,
-        "IamRoleArn": str,
-        "SerialNumber": str,
-        "VendorName": str,
-        "HsmType": str,
-        "SoftwareVersion": str,
-        "SshPublicKey": str,
-        "SshKeyLastUpdated": str,
-        "ServerCertUri": str,
-        "ServerCertLastUpdated": str,
-        "Partitions": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeLunaClientRequestRequestTypeDef = TypedDict(
     "DescribeLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "CertificateFingerprint": str,
     },
     total=False,
 )
 
-DescribeLunaClientResponseTypeDef = TypedDict(
-    "DescribeLunaClientResponseTypeDef",
-    {
-        "ClientArn": str,
-        "Certificate": str,
-        "CertificateFingerprint": str,
-        "LastModifiedTimestamp": str,
-        "Label": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetConfigRequestRequestTypeDef = TypedDict(
     "GetConfigRequestRequestTypeDef",
     {
         "ClientArn": str,
         "ClientVersion": ClientVersionType,
         "HapgList": Sequence[str],
     },
 )
 
-GetConfigResponseTypeDef = TypedDict(
-    "GetConfigResponseTypeDef",
-    {
-        "ConfigType": str,
-        "ConfigFile": str,
-        "ConfigCred": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListAvailableZonesResponseTypeDef = TypedDict(
-    "ListAvailableZonesResponseTypeDef",
-    {
-        "AZList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
-    "ListHapgsRequestListHapgsPaginateTypeDef",
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
 
 ListHapgsRequestRequestTypeDef = TypedDict(
     "ListHapgsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHapgsResponseTypeDef = TypedDict(
-    "ListHapgsResponseTypeDef",
-    {
-        "HapgList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
-    "ListHsmsRequestListHsmsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListHsmsRequestRequestTypeDef = TypedDict(
     "ListHsmsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListHsmsResponseTypeDef = TypedDict(
-    "ListHsmsResponseTypeDef",
-    {
-        "HsmList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
-    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLunaClientsRequestRequestTypeDef = TypedDict(
     "ListLunaClientsRequestRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListLunaClientsResponseTypeDef = TypedDict(
-    "ListLunaClientsResponseTypeDef",
-    {
-        "ClientList": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
@@ -410,26 +255,20 @@
     {
         "Label": str,
         "PartitionSerialList": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyHapgRequestRequestTypeDef(
     _RequiredModifyHapgRequestRequestTypeDef, _OptionalModifyHapgRequestRequestTypeDef
 ):
     pass
 
-ModifyHapgResponseTypeDef = TypedDict(
-    "ModifyHapgResponseTypeDef",
-    {
-        "HapgArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredModifyHsmRequestRequestTypeDef = TypedDict(
     "_RequiredModifyHsmRequestRequestTypeDef",
     {
         "HsmArn": str,
     },
 )
@@ -441,88 +280,258 @@
         "IamRoleArn": str,
         "ExternalId": str,
         "SyslogIp": str,
     },
     total=False,
 )
 
+
 class ModifyHsmRequestRequestTypeDef(
     _RequiredModifyHsmRequestRequestTypeDef, _OptionalModifyHsmRequestRequestTypeDef
 ):
     pass
 
-ModifyHsmResponseTypeDef = TypedDict(
-    "ModifyHsmResponseTypeDef",
-    {
-        "HsmArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ModifyLunaClientRequestRequestTypeDef = TypedDict(
     "ModifyLunaClientRequestRequestTypeDef",
     {
         "ClientArn": str,
         "Certificate": str,
     },
 )
 
-ModifyLunaClientResponseTypeDef = TypedDict(
-    "ModifyLunaClientResponseTypeDef",
+RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
+    "RemoveTagsFromResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagKeyList": Sequence[str],
+    },
+)
+
+AddTagsToResourceRequestRequestTypeDef = TypedDict(
+    "AddTagsToResourceRequestRequestTypeDef",
+    {
+        "ResourceArn": str,
+        "TagList": Sequence[TagTypeDef],
+    },
+)
+
+AddTagsToResourceResponseTypeDef = TypedDict(
+    "AddTagsToResourceResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHapgResponseTypeDef = TypedDict(
+    "CreateHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateHsmResponseTypeDef = TypedDict(
+    "CreateHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateLunaClientResponseTypeDef = TypedDict(
+    "CreateLunaClientResponseTypeDef",
     {
         "ClientArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteHapgResponseTypeDef = TypedDict(
+    "DeleteHapgResponseTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-RemoveTagsFromResourceRequestRequestTypeDef = TypedDict(
-    "RemoveTagsFromResourceRequestRequestTypeDef",
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagKeyList": Sequence[str],
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-RemoveTagsFromResourceResponseTypeDef = TypedDict(
-    "RemoveTagsFromResourceResponseTypeDef",
+DeleteLunaClientResponseTypeDef = TypedDict(
+    "DeleteLunaClientResponseTypeDef",
     {
         "Status": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+DescribeHapgResponseTypeDef = TypedDict(
+    "DescribeHapgResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "HapgArn": str,
+        "HapgSerial": str,
+        "HsmsLastActionFailed": List[str],
+        "HsmsPendingDeletion": List[str],
+        "HsmsPendingRegistration": List[str],
+        "Label": str,
+        "LastModifiedTimestamp": str,
+        "PartitionSerialList": List[str],
+        "State": CloudHsmObjectStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-AddTagsToResourceRequestRequestTypeDef = TypedDict(
-    "AddTagsToResourceRequestRequestTypeDef",
+DescribeHsmResponseTypeDef = TypedDict(
+    "DescribeHsmResponseTypeDef",
     {
-        "ResourceArn": str,
-        "TagList": Sequence[TagTypeDef],
+        "HsmArn": str,
+        "Status": HsmStatusType,
+        "StatusDetails": str,
+        "AvailabilityZone": str,
+        "EniId": str,
+        "EniIp": str,
+        "SubscriptionType": Literal["PRODUCTION"],
+        "SubscriptionStartDate": str,
+        "SubscriptionEndDate": str,
+        "VpcId": str,
+        "SubnetId": str,
+        "IamRoleArn": str,
+        "SerialNumber": str,
+        "VendorName": str,
+        "HsmType": str,
+        "SoftwareVersion": str,
+        "SshPublicKey": str,
+        "SshKeyLastUpdated": str,
+        "ServerCertUri": str,
+        "ServerCertLastUpdated": str,
+        "Partitions": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeLunaClientResponseTypeDef = TypedDict(
+    "DescribeLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "Certificate": str,
+        "CertificateFingerprint": str,
+        "LastModifiedTimestamp": str,
+        "Label": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetConfigResponseTypeDef = TypedDict(
+    "GetConfigResponseTypeDef",
+    {
+        "ConfigType": str,
+        "ConfigFile": str,
+        "ConfigCred": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListAvailableZonesResponseTypeDef = TypedDict(
+    "ListAvailableZonesResponseTypeDef",
+    {
+        "AZList": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHapgsResponseTypeDef = TypedDict(
+    "ListHapgsResponseTypeDef",
+    {
+        "HapgList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHsmsResponseTypeDef = TypedDict(
+    "ListHsmsResponseTypeDef",
+    {
+        "HsmList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListLunaClientsResponseTypeDef = TypedDict(
+    "ListLunaClientsResponseTypeDef",
+    {
+        "ClientList": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "TagList": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHapgResponseTypeDef = TypedDict(
+    "ModifyHapgResponseTypeDef",
+    {
+        "HapgArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyHsmResponseTypeDef = TypedDict(
+    "ModifyHsmResponseTypeDef",
+    {
+        "HsmArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ModifyLunaClientResponseTypeDef = TypedDict(
+    "ModifyLunaClientResponseTypeDef",
+    {
+        "ClientArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RemoveTagsFromResourceResponseTypeDef = TypedDict(
+    "RemoveTagsFromResourceResponseTypeDef",
+    {
+        "Status": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListHapgsRequestListHapgsPaginateTypeDef = TypedDict(
+    "ListHapgsRequestListHapgsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
+)
+
+ListHsmsRequestListHsmsPaginateTypeDef = TypedDict(
+    "ListHsmsRequestListHsmsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLunaClientsRequestListLunaClientsPaginateTypeDef = TypedDict(
+    "ListLunaClientsRequestListLunaClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
 )
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudHSM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudhsm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudhsm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsm"></a>
 
 # types-aiobotocore-cloudhsm
 
 [![PyPI - types-aiobotocore-cloudhsm](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsm?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsm)](https://pepy.tech/project/types-aiobotocore-cloudhsm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudHSM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsm.html#CloudHSM)
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
 [types-aiobotocore-cloudhsm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsm/).
 
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
@@ -318,72 +317,72 @@
 )
 
 
 def check_value(value: ClientVersionType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudhsm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudhsm.type_defs import (
     TagTypeDef,
-    AddTagsToResourceResponseTypeDef,
+    ResponseMetadataTypeDef,
     CreateHapgRequestRequestTypeDef,
-    CreateHapgResponseTypeDef,
     CreateHsmRequestRequestTypeDef,
-    CreateHsmResponseTypeDef,
     CreateLunaClientRequestRequestTypeDef,
-    CreateLunaClientResponseTypeDef,
     DeleteHapgRequestRequestTypeDef,
-    DeleteHapgResponseTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
     DeleteLunaClientRequestRequestTypeDef,
-    DeleteLunaClientResponseTypeDef,
     DescribeHapgRequestRequestTypeDef,
-    DescribeHapgResponseTypeDef,
     DescribeHsmRequestRequestTypeDef,
-    DescribeHsmResponseTypeDef,
     DescribeLunaClientRequestRequestTypeDef,
-    DescribeLunaClientResponseTypeDef,
     GetConfigRequestRequestTypeDef,
-    GetConfigResponseTypeDef,
-    ListAvailableZonesResponseTypeDef,
-    ListHapgsRequestListHapgsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListHapgsRequestRequestTypeDef,
-    ListHapgsResponseTypeDef,
-    ListHsmsRequestListHsmsPaginateTypeDef,
     ListHsmsRequestRequestTypeDef,
-    ListHsmsResponseTypeDef,
-    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
     ListLunaClientsRequestRequestTypeDef,
-    ListLunaClientsResponseTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyHapgRequestRequestTypeDef,
-    ModifyHapgResponseTypeDef,
     ModifyHsmRequestRequestTypeDef,
-    ModifyHsmResponseTypeDef,
     ModifyLunaClientRequestRequestTypeDef,
-    ModifyLunaClientResponseTypeDef,
-    PaginatorConfigTypeDef,
     RemoveTagsFromResourceRequestRequestTypeDef,
-    RemoveTagsFromResourceResponseTypeDef,
-    ResponseMetadataTypeDef,
     AddTagsToResourceRequestRequestTypeDef,
+    AddTagsToResourceResponseTypeDef,
+    CreateHapgResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    CreateLunaClientResponseTypeDef,
+    DeleteHapgResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    DeleteLunaClientResponseTypeDef,
+    DescribeHapgResponseTypeDef,
+    DescribeHsmResponseTypeDef,
+    DescribeLunaClientResponseTypeDef,
+    GetConfigResponseTypeDef,
+    ListAvailableZonesResponseTypeDef,
+    ListHapgsResponseTypeDef,
+    ListHsmsResponseTypeDef,
+    ListLunaClientsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
+    ModifyHapgResponseTypeDef,
+    ModifyHsmResponseTypeDef,
+    ModifyLunaClientResponseTypeDef,
+    RemoveTagsFromResourceResponseTypeDef,
+    ListHapgsRequestListHapgsPaginateTypeDef,
+    ListHsmsRequestListHsmsPaginateTypeDef,
+    ListLunaClientsRequestListLunaClientsPaginateTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudhsm-2.5.2/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsm-2.5.2.post1/types_aiobotocore_cloudhsm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-sagemaker-a2i-runtime-2.5.2.tar.gz` & `tmp/types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sagemaker-a2i-runtime-2.5.2.tar", last modified: Sat Jul  8 01:44:15 2023, max compression
+gzip compressed data, was "types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:57 2023, max compression
```

## Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.tar` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.386834 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14155 2023-07-08 01:44:15.386834 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12537 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:15.386834 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.382833 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8431 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8416 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:19.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:15.386834 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14155 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 01:44:15.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12542 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8088 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-08-02 14:48:58.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:57.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:56.993469 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14113 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-02 14:52:56.000000 types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/LICENSE` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/PKG-INFO` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-a2i-runtime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sagemaker-a2i-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sagemaker-a2i-runtime"></a>
 
 # types-aiobotocore-sagemaker-a2i-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-a2i-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-a2i-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-a2i-runtime)](https://pepy.tech/project/types-aiobotocore-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AugmentedAIRuntime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
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
@@ -307,42 +306,44 @@
 )
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sagemaker_a2i_runtime.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
+    ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
+    StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
+    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
+def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/README.md` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sagemaker-a2i-runtime"></a>
 
 # types-aiobotocore-sagemaker-a2i-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-a2i-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-a2i-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-a2i-runtime)](https://pepy.tech/project/types-aiobotocore-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AugmentedAIRuntime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
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
@@ -274,42 +274,44 @@
 )
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sagemaker_a2i_runtime.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
+    ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
+    StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
+    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
+def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/setup.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sagemaker-a2i-runtime",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sagemaker_a2i_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with"
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
     keywords=(
-        "aiobotocore sagemaker-a2i-runtime type-annotations boto3-stubs mypy typeshed autocomplete"
+        "aiobotocore sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sagemaker_a2i_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/",
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/__init__.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/__main__.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime\nOther"
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

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/client.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,57 +11,53 @@
 
     session = get_session()
     async with session.create_client("sagemaker-a2i-runtime") as client:
         client: AugmentedAIRuntimeClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import SortOrderType
 from .paginator import ListHumanLoopsPaginator
 from .type_defs import (
     DescribeHumanLoopResponseTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     ListHumanLoopsResponseTypeDef,
     StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("AugmentedAIRuntimeClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
-
 class AugmentedAIRuntimeClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/)
     """
 
     meta: ClientMeta
@@ -70,111 +66,100 @@
     def exceptions(self) -> Exceptions:
         """
         AugmentedAIRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#close)
         """
-
     async def delete_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Deletes the specified human loop for a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#delete_human_loop)
         """
-
     async def describe_human_loop(self, *, HumanLoopName: str) -> DescribeHumanLoopResponseTypeDef:
         """
         Returns information about the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#describe_human_loop)
         """
-
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#generate_presigned_url)
         """
-
     async def list_human_loops(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListHumanLoopsResponseTypeDef:
         """
         Returns information about human loops, given the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#list_human_loops)
         """
-
     async def start_human_loop(
         self,
         *,
         HumanLoopName: str,
         FlowDefinitionArn: str,
         HumanLoopInput: HumanLoopInputTypeDef,
         DataAttributes: HumanLoopDataAttributesTypeDef = ...
     ) -> StartHumanLoopResponseTypeDef:
         """
         Starts a human loop, provided that at least one activation condition is met.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#start_human_loop)
         """
-
     async def stop_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Stops the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#stop_human_loop)
         """
-
     def get_paginator(self, operation_name: Literal["list_human_loops"]) -> ListHumanLoopsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#get_paginator)
         """
-
     async def __aenter__(self) -> "AugmentedAIRuntimeClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/client.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,53 +11,57 @@
 
     session = get_session()
     async with session.create_client("sagemaker-a2i-runtime") as client:
         client: AugmentedAIRuntimeClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import SortOrderType
 from .paginator import ListHumanLoopsPaginator
 from .type_defs import (
     DescribeHumanLoopResponseTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     ListHumanLoopsResponseTypeDef,
     StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("AugmentedAIRuntimeClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     ClientError: Type[BotocoreClientError]
     ConflictException: Type[BotocoreClientError]
     InternalServerException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     ServiceQuotaExceededException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
     ValidationException: Type[BotocoreClientError]
 
+
 class AugmentedAIRuntimeClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/)
     """
 
     meta: ClientMeta
@@ -66,100 +70,111 @@
     def exceptions(self) -> Exceptions:
         """
         AugmentedAIRuntimeClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#close)
         """
+
     async def delete_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Deletes the specified human loop for a flow definition.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.delete_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#delete_human_loop)
         """
+
     async def describe_human_loop(self, *, HumanLoopName: str) -> DescribeHumanLoopResponseTypeDef:
         """
         Returns information about the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.describe_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#describe_human_loop)
         """
+
     async def generate_presigned_url(
         self,
         ClientMethod: str,
         Params: Mapping[str, Any] = ...,
         ExpiresIn: int = 3600,
         HttpMethod: str = ...,
     ) -> str:
         """
         Generate a presigned url given a client, its method, and arguments.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#generate_presigned_url)
         """
+
     async def list_human_loops(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
         NextToken: str = ...,
         MaxResults: int = ...
     ) -> ListHumanLoopsResponseTypeDef:
         """
         Returns information about human loops, given the specified parameters.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.list_human_loops)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#list_human_loops)
         """
+
     async def start_human_loop(
         self,
         *,
         HumanLoopName: str,
         FlowDefinitionArn: str,
         HumanLoopInput: HumanLoopInputTypeDef,
         DataAttributes: HumanLoopDataAttributesTypeDef = ...
     ) -> StartHumanLoopResponseTypeDef:
         """
         Starts a human loop, provided that at least one activation condition is met.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.start_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#start_human_loop)
         """
+
     async def stop_human_loop(self, *, HumanLoopName: str) -> Dict[str, Any]:
         """
         Stops the specified human loop.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.stop_human_loop)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#stop_human_loop)
         """
+
     def get_paginator(self, operation_name: Literal["list_human_loops"]) -> ListHumanLoopsPaginator:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client.get_paginator)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/#get_paginator)
         """
+
     async def __aenter__(self) -> "AugmentedAIRuntimeClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/client/)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/literals.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/paginator.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,21 @@
     session = get_session()
     with session.create_client("sagemaker-a2i-runtime") as client:
         client: AugmentedAIRuntimeClient
 
         list_human_loops_paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import SortOrderType
-from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 
@@ -48,16 +47,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
     """
 
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/paginator.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,21 @@
     session = get_session()
     with session.create_client("sagemaker-a2i-runtime") as client:
         client: AugmentedAIRuntimeClient
 
         list_human_loops_paginator: ListHumanLoopsPaginator = client.get_paginator("list_human_loops")
     ```
 """
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import SortOrderType
-from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef
+from .type_defs import ListHumanLoopsResponseTypeDef, PaginatorConfigTypeDef, TimestampTypeDef
 
 __all__ = ("ListHumanLoopsPaginator",)
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
@@ -45,16 +44,16 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
     """
 
     def paginate(
         self,
         *,
         FlowDefinitionArn: str,
-        CreationTimeAfter: Union[datetime, str] = ...,
-        CreationTimeBefore: Union[datetime, str] = ...,
+        CreationTimeAfter: TimestampTypeDef = ...,
+        CreationTimeBefore: TimestampTypeDef = ...,
         SortOrder: SortOrderType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListHumanLoopsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime.Paginator.ListHumanLoops.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/paginators/#listhumanloopspaginator)
         """
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,45 +4,45 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
-    data: DeleteHumanLoopRequestRequestTypeDef = {...}
+    data: DeleteHumanLoopRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ContentClassifierType, HumanLoopStatusType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "DeleteHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
     "HumanLoopSummaryTypeDef",
-    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    "ListHumanLoopsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartHumanLoopResponseTypeDef",
+    "TimestampTypeDef",
     "StopHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopResponseTypeDef",
+    "StartHumanLoopResponseTypeDef",
     "StartHumanLoopRequestRequestTypeDef",
     "ListHumanLoopsResponseTypeDef",
+    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    "ListHumanLoopsRequestRequestTypeDef",
 )
 
 DeleteHumanLoopRequestRequestTypeDef = TypedDict(
     "DeleteHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
@@ -58,14 +58,25 @@
 HumanLoopOutputTypeDef = TypedDict(
     "HumanLoopOutputTypeDef",
     {
         "OutputS3Uri": str,
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
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
 )
 
@@ -84,93 +95,25 @@
         "CreationTime": datetime,
         "FailureReason": str,
         "FlowDefinitionArn": str,
     },
     total=False,
 )
 
-_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
-    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-):
-    pass
-
-
-_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestRequestTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestRequestTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-
-class ListHumanLoopsRequestRequestTypeDef(
-    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
-):
-    pass
-
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
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
-StartHumanLoopResponseTypeDef = TypedDict(
-    "StartHumanLoopResponseTypeDef",
-    {
-        "HumanLoopArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 StopHumanLoopRequestRequestTypeDef = TypedDict(
     "StopHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
 )
 
@@ -181,15 +124,23 @@
         "FailureReason": str,
         "FailureCode": str,
         "HumanLoopStatus": HumanLoopStatusType,
         "HumanLoopName": str,
         "HumanLoopArn": str,
         "FlowDefinitionArn": str,
         "HumanLoopOutput": HumanLoopOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartHumanLoopResponseTypeDef = TypedDict(
+    "StartHumanLoopResponseTypeDef",
+    {
+        "HumanLoopArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartHumanLoopRequestRequestTypeDef = TypedDict(
     "_RequiredStartHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
@@ -201,22 +152,66 @@
     "_OptionalStartHumanLoopRequestRequestTypeDef",
     {
         "DataAttributes": HumanLoopDataAttributesTypeDef,
     },
     total=False,
 )
 
-
 class StartHumanLoopRequestRequestTypeDef(
     _RequiredStartHumanLoopRequestRequestTypeDef, _OptionalStartHumanLoopRequestRequestTypeDef
 ):
     pass
 
-
 ListHumanLoopsResponseTypeDef = TypedDict(
     "ListHumanLoopsResponseTypeDef",
     {
         "HumanLoopSummaries": List[HumanLoopSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
+    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+):
+    pass
+
+_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestRequestTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestRequestTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": SortOrderType,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
+
+class ListHumanLoopsRequestRequestTypeDef(
+    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime/type_defs.pyi` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,44 +4,46 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sagemaker_a2i_runtime.type_defs import DeleteHumanLoopRequestRequestTypeDef
 
-    data: DeleteHumanLoopRequestRequestTypeDef = {...}
+    data: DeleteHumanLoopRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ContentClassifierType, HumanLoopStatusType, SortOrderType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "DeleteHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopRequestRequestTypeDef",
     "HumanLoopOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "HumanLoopDataAttributesTypeDef",
     "HumanLoopInputTypeDef",
     "HumanLoopSummaryTypeDef",
-    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    "ListHumanLoopsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartHumanLoopResponseTypeDef",
+    "TimestampTypeDef",
     "StopHumanLoopRequestRequestTypeDef",
     "DescribeHumanLoopResponseTypeDef",
+    "StartHumanLoopResponseTypeDef",
     "StartHumanLoopRequestRequestTypeDef",
     "ListHumanLoopsResponseTypeDef",
+    "ListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    "ListHumanLoopsRequestRequestTypeDef",
 )
 
 DeleteHumanLoopRequestRequestTypeDef = TypedDict(
     "DeleteHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
@@ -57,14 +59,25 @@
 HumanLoopOutputTypeDef = TypedDict(
     "HumanLoopOutputTypeDef",
     {
         "OutputS3Uri": str,
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
 HumanLoopDataAttributesTypeDef = TypedDict(
     "HumanLoopDataAttributesTypeDef",
     {
         "ContentClassifiers": Sequence[ContentClassifierType],
     },
 )
 
@@ -83,89 +96,25 @@
         "CreationTime": datetime,
         "FailureReason": str,
         "FlowDefinitionArn": str,
     },
     total=False,
 )
 
-_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
-    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-):
-    pass
-
-_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_RequiredListHumanLoopsRequestRequestTypeDef",
-    {
-        "FlowDefinitionArn": str,
-    },
-)
-_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
-    "_OptionalListHumanLoopsRequestRequestTypeDef",
-    {
-        "CreationTimeAfter": Union[datetime, str],
-        "CreationTimeBefore": Union[datetime, str],
-        "SortOrder": SortOrderType,
-        "NextToken": str,
-        "MaxResults": int,
-    },
-    total=False,
-)
-
-class ListHumanLoopsRequestRequestTypeDef(
-    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
-):
-    pass
-
 PaginatorConfigTypeDef = TypedDict(
     "PaginatorConfigTypeDef",
     {
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
-StartHumanLoopResponseTypeDef = TypedDict(
-    "StartHumanLoopResponseTypeDef",
-    {
-        "HumanLoopArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 StopHumanLoopRequestRequestTypeDef = TypedDict(
     "StopHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
     },
 )
 
@@ -176,15 +125,23 @@
         "FailureReason": str,
         "FailureCode": str,
         "HumanLoopStatus": HumanLoopStatusType,
         "HumanLoopName": str,
         "HumanLoopArn": str,
         "FlowDefinitionArn": str,
         "HumanLoopOutput": HumanLoopOutputTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartHumanLoopResponseTypeDef = TypedDict(
+    "StartHumanLoopResponseTypeDef",
+    {
+        "HumanLoopArn": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartHumanLoopRequestRequestTypeDef = TypedDict(
     "_RequiredStartHumanLoopRequestRequestTypeDef",
     {
         "HumanLoopName": str,
@@ -196,20 +153,71 @@
     "_OptionalStartHumanLoopRequestRequestTypeDef",
     {
         "DataAttributes": HumanLoopDataAttributesTypeDef,
     },
     total=False,
 )
 
+
 class StartHumanLoopRequestRequestTypeDef(
     _RequiredStartHumanLoopRequestRequestTypeDef, _OptionalStartHumanLoopRequestRequestTypeDef
 ):
     pass
 
+
 ListHumanLoopsResponseTypeDef = TypedDict(
     "ListHumanLoopsResponseTypeDef",
     {
         "HumanLoopSummaries": List[HumanLoopSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": SortOrderType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListHumanLoopsRequestListHumanLoopsPaginateTypeDef(
+    _RequiredListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    _OptionalListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_RequiredListHumanLoopsRequestRequestTypeDef",
+    {
+        "FlowDefinitionArn": str,
+    },
+)
+_OptionalListHumanLoopsRequestRequestTypeDef = TypedDict(
+    "_OptionalListHumanLoopsRequestRequestTypeDef",
+    {
+        "CreationTimeAfter": TimestampTypeDef,
+        "CreationTimeBefore": TimestampTypeDef,
+        "SortOrder": SortOrderType,
+        "NextToken": str,
+        "MaxResults": int,
     },
+    total=False,
 )
+
+
+class ListHumanLoopsRequestRequestTypeDef(
+    _RequiredListHumanLoopsRequestRequestTypeDef, _OptionalListHumanLoopsRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sagemaker-a2i-runtime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.AugmentedAIRuntime 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sagemaker-a2i-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sagemaker-a2i-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sagemaker-a2i-runtime"></a>
 
 # types-aiobotocore-sagemaker-a2i-runtime
 
 [![PyPI - types-aiobotocore-sagemaker-a2i-runtime](https://img.shields.io/pypi/v/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sagemaker-a2i-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sagemaker-a2i-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sagemaker-a2i-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-sagemaker-a2i-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sagemaker-a2i-runtime)](https://pepy.tech/project/types-aiobotocore-sagemaker-a2i-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.AugmentedAIRuntime 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sagemaker-a2i-runtime.html#AugmentedAIRuntime)
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
 [types-aiobotocore-sagemaker-a2i-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sagemaker_a2i_runtime/).
 
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
@@ -307,42 +306,44 @@
 )
 
 
 def check_value(value: ContentClassifierType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sagemaker_a2i_runtime.type_defs` module contains structures
-and shapes assembled to typed dictionaries for additional type checking.
+and shapes assembled to typed dictionaries and unions for additional type
+checking.
 
 ```python
 from types_aiobotocore_sagemaker_a2i_runtime.type_defs import (
     DeleteHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopRequestRequestTypeDef,
     HumanLoopOutputTypeDef,
+    ResponseMetadataTypeDef,
     HumanLoopDataAttributesTypeDef,
     HumanLoopInputTypeDef,
     HumanLoopSummaryTypeDef,
-    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
-    ListHumanLoopsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartHumanLoopResponseTypeDef,
+    TimestampTypeDef,
     StopHumanLoopRequestRequestTypeDef,
     DescribeHumanLoopResponseTypeDef,
+    StartHumanLoopResponseTypeDef,
     StartHumanLoopRequestRequestTypeDef,
     ListHumanLoopsResponseTypeDef,
+    ListHumanLoopsRequestListHumanLoopsPaginateTypeDef,
+    ListHumanLoopsRequestRequestTypeDef,
 )
 
 
-def get_structure() -> DeleteHumanLoopRequestRequestTypeDef:
+def get_value() -> DeleteHumanLoopRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sagemaker-a2i-runtime-2.5.2/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-sagemaker-a2i-runtime-2.5.2.post1/types_aiobotocore_sagemaker_a2i_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


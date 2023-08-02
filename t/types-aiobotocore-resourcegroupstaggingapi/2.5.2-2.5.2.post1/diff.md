# Comparing `tmp/types-aiobotocore-resourcegroupstaggingapi-2.5.2.tar.gz` & `tmp/types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.5.2.tar", last modified: Sat Jul  8 01:44:11 2023, max compression
+gzip compressed data, was "types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:52 2023, max compression
```

## Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2.tar` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.866771 types-aiobotocore-resourcegroupstaggingapi-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-07-08 01:44:11.866771 types-aiobotocore-resourcegroupstaggingapi-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13578 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:11.866771 types-aiobotocore-resourcegroupstaggingapi-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.862771 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:18.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:11.866771 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15211 2023-07-08 01:44:11.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-08 01:44:11.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:11.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:11.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-08 01:44:11.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.933481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12694 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12673 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8948 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8946 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6296 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6290 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8261 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-08-02 14:47:56.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:55.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:52.937481 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 14:52:52.000000 types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/LICENSE` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resourcegroupstaggingapi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resourcegroupstaggingapi type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resourcegroupstaggingapi"></a>
 
 # types-aiobotocore-resourcegroupstaggingapi
 
 [![PyPI - types-aiobotocore-resourcegroupstaggingapi](https://img.shields.io/pypi/v/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/types-aiobotocore-resourcegroupstaggingapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceGroupsTaggingAPI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
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
@@ -321,54 +320,54 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resourcegroupstaggingapi.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    DescribeReportCreationOutputTypeDef,
+    ResponseMetadataTypeDef,
     FailureInfoTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
-    GetTagValuesOutputTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
+    DescribeReportCreationOutputTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
 
 
-def get_structure() -> ComplianceDetailsTypeDef:
+def get_value() -> ComplianceDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/README.md` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-resourcegroupstaggingapi"></a>
 
 # types-aiobotocore-resourcegroupstaggingapi
 
 [![PyPI - types-aiobotocore-resourcegroupstaggingapi](https://img.shields.io/pypi/v/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/types-aiobotocore-resourcegroupstaggingapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceGroupsTaggingAPI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
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
@@ -288,54 +288,54 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resourcegroupstaggingapi.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    DescribeReportCreationOutputTypeDef,
+    ResponseMetadataTypeDef,
     FailureInfoTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
-    GetTagValuesOutputTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
+    DescribeReportCreationOutputTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
 
 
-def get_structure() -> ComplianceDetailsTypeDef:
+def get_value() -> ComplianceDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/setup.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-resourcegroupstaggingapi",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_resourcegroupstaggingapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with"
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
-        "aiobotocore resourcegroupstaggingapi type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "aiobotocore resourcegroupstaggingapi type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_resourcegroupstaggingapi": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/",
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/__init__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/__main__.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI\nOther"
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

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/client.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/client.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/literals.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/literals.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/paginator.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 
@@ -92,43 +92,43 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 
 class GetTagKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTagKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
         """
 
 
 class GetTagValuesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
     """
 
     def paginate(
-        self, *, Key: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Key: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTagValuesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
         """
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self,
         *,
         TargetIdFilters: Sequence[str] = ...,
         RegionFilters: Sequence[str] = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         TagKeyFilters: Sequence[str] = ...,
         GroupBy: Sequence[GroupByAttributeType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetComplianceSummaryOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetComplianceSummary.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getcompliancesummarypaginator)
         """
 
 class GetResourcesPaginator(AioPaginator):
@@ -88,41 +88,41 @@
         *,
         TagFilters: Sequence[TagFilterTypeDef] = ...,
         TagsPerPage: int = ...,
         ResourceTypeFilters: Sequence[str] = ...,
         IncludeComplianceDetails: bool = ...,
         ExcludeCompliantResources: bool = ...,
         ResourceARNList: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetResourcesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetResources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#getresourcespaginator)
         """
 
 class GetTagKeysPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTagKeysOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagKeys.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagkeyspaginator)
         """
 
 class GetTagValuesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
     """
 
     def paginate(
-        self, *, Key: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Key: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetTagValuesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI.Paginator.GetTagValues.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/paginators/#gettagvaluespaginator)
         """
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/type_defs.py` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_resourcegroupstaggingapi.type_defs import ComplianceDetailsTypeDef
 
-    data: ComplianceDetailsTypeDef = {...}
+    data: ComplianceDetailsTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ErrorCodeType, GroupByAttributeType, TargetIdTypeType
 
@@ -20,34 +20,34 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "ComplianceDetailsTypeDef",
-    "DescribeReportCreationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "FailureInfoTypeDef",
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
     "TagFilterTypeDef",
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
     "GetTagKeysInputRequestTypeDef",
-    "GetTagKeysOutputTypeDef",
-    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetTagValuesInputRequestTypeDef",
-    "GetTagValuesOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "StartReportCreationInputRequestTypeDef",
     "TagResourcesInputRequestTypeDef",
     "UntagResourcesInputRequestTypeDef",
+    "DescribeReportCreationOutputTypeDef",
+    "GetTagKeysOutputTypeDef",
+    "GetTagValuesOutputTypeDef",
     "TagResourcesOutputTypeDef",
     "UntagResourcesOutputTypeDef",
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetComplianceSummaryOutputTypeDef",
     "GetResourcesInputGetResourcesPaginateTypeDef",
     "GetResourcesInputRequestTypeDef",
     "ResourceTagMappingTypeDef",
     "GetResourcesOutputTypeDef",
 )
 
@@ -57,43 +57,41 @@
         "NoncompliantKeys": List[str],
         "KeysWithNoncompliantValues": List[str],
         "ComplianceStatus": bool,
     },
     total=False,
 )
 
-DescribeReportCreationOutputTypeDef = TypedDict(
-    "DescribeReportCreationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "S3Location": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "StatusCode": int,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TargetIdFilters": Sequence[str],
-        "RegionFilters": Sequence[str],
-        "ResourceTypeFilters": Sequence[str],
-        "TagKeyFilters": Sequence[str],
-        "GroupBy": Sequence[GroupByAttributeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetComplianceSummaryInputRequestTypeDef = TypedDict(
     "GetComplianceSummaryInputRequestTypeDef",
     {
@@ -126,61 +124,22 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetTagKeysInputRequestTypeDef = TypedDict(
     "GetTagKeysInputRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
-GetTagKeysOutputTypeDef = TypedDict(
-    "GetTagKeysOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagKeys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetTagValuesInputGetTagValuesPaginateTypeDef(
-    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
-    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetTagValuesInputRequestTypeDef = TypedDict(
     "_RequiredGetTagValuesInputRequestTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalGetTagValuesInputRequestTypeDef = TypedDict(
@@ -194,52 +153,22 @@
 
 class GetTagValuesInputRequestTypeDef(
     _RequiredGetTagValuesInputRequestTypeDef, _OptionalGetTagValuesInputRequestTypeDef
 ):
     pass
 
 
-GetTagValuesOutputTypeDef = TypedDict(
-    "GetTagValuesOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagValues": List[str],
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 StartReportCreationInputRequestTypeDef = TypedDict(
     "StartReportCreationInputRequestTypeDef",
     {
         "S3Bucket": str,
     },
 )
 
@@ -255,49 +184,120 @@
     "UntagResourcesInputRequestTypeDef",
     {
         "ResourceARNList": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeReportCreationOutputTypeDef = TypedDict(
+    "DescribeReportCreationOutputTypeDef",
+    {
+        "Status": str,
+        "S3Location": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagKeysOutputTypeDef = TypedDict(
+    "GetTagKeysOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagKeys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagValuesOutputTypeDef = TypedDict(
+    "GetTagValuesOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourcesOutputTypeDef = TypedDict(
     "TagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UntagResourcesOutputTypeDef = TypedDict(
     "UntagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    {
+        "TargetIdFilters": Sequence[str],
+        "RegionFilters": Sequence[str],
+        "ResourceTypeFilters": Sequence[str],
+        "TagKeyFilters": Sequence[str],
+        "GroupBy": Sequence[GroupByAttributeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "Key": str,
     },
 )
+_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetTagValuesInputGetTagValuesPaginateTypeDef(
+    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
+    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
+):
+    pass
+
 
 GetComplianceSummaryOutputTypeDef = TypedDict(
     "GetComplianceSummaryOutputTypeDef",
     {
         "SummaryList": List[SummaryTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesInputGetResourcesPaginateTypeDef = TypedDict(
     "GetResourcesInputGetResourcesPaginateTypeDef",
     {
         "TagFilters": Sequence[TagFilterTypeDef],
         "TagsPerPage": int,
         "ResourceTypeFilters": Sequence[str],
         "IncludeComplianceDetails": bool,
         "ExcludeCompliantResources": bool,
         "ResourceARNList": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetResourcesInputRequestTypeDef = TypedDict(
     "GetResourcesInputRequestTypeDef",
     {
@@ -324,10 +324,10 @@
 )
 
 GetResourcesOutputTypeDef = TypedDict(
     "GetResourcesOutputTypeDef",
     {
         "PaginationToken": str,
         "ResourceTagMappingList": List[ResourceTagMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,49 +4,49 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_resourcegroupstaggingapi.type_defs import ComplianceDetailsTypeDef
 
-    data: ComplianceDetailsTypeDef = {...}
+    data: ComplianceDetailsTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import ErrorCodeType, GroupByAttributeType, TargetIdTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "ComplianceDetailsTypeDef",
-    "DescribeReportCreationOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "FailureInfoTypeDef",
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetComplianceSummaryInputRequestTypeDef",
     "SummaryTypeDef",
     "TagFilterTypeDef",
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
     "GetTagKeysInputRequestTypeDef",
-    "GetTagKeysOutputTypeDef",
-    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetTagValuesInputRequestTypeDef",
-    "GetTagValuesOutputTypeDef",
-    "PaginatorConfigTypeDef",
     "TagTypeDef",
-    "ResponseMetadataTypeDef",
     "StartReportCreationInputRequestTypeDef",
     "TagResourcesInputRequestTypeDef",
     "UntagResourcesInputRequestTypeDef",
+    "DescribeReportCreationOutputTypeDef",
+    "GetTagKeysOutputTypeDef",
+    "GetTagValuesOutputTypeDef",
     "TagResourcesOutputTypeDef",
     "UntagResourcesOutputTypeDef",
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    "GetTagValuesInputGetTagValuesPaginateTypeDef",
     "GetComplianceSummaryOutputTypeDef",
     "GetResourcesInputGetResourcesPaginateTypeDef",
     "GetResourcesInputRequestTypeDef",
     "ResourceTagMappingTypeDef",
     "GetResourcesOutputTypeDef",
 )
 
@@ -56,43 +56,41 @@
         "NoncompliantKeys": List[str],
         "KeysWithNoncompliantValues": List[str],
         "ComplianceStatus": bool,
     },
     total=False,
 )
 
-DescribeReportCreationOutputTypeDef = TypedDict(
-    "DescribeReportCreationOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "Status": str,
-        "S3Location": str,
-        "ErrorMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 FailureInfoTypeDef = TypedDict(
     "FailureInfoTypeDef",
     {
         "StatusCode": int,
         "ErrorCode": ErrorCodeType,
         "ErrorMessage": str,
     },
     total=False,
 )
 
-GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
-    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "TargetIdFilters": Sequence[str],
-        "RegionFilters": Sequence[str],
-        "ResourceTypeFilters": Sequence[str],
-        "TagKeyFilters": Sequence[str],
-        "GroupBy": Sequence[GroupByAttributeType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 GetComplianceSummaryInputRequestTypeDef = TypedDict(
     "GetComplianceSummaryInputRequestTypeDef",
     {
@@ -125,59 +123,22 @@
     {
         "Key": str,
         "Values": Sequence[str],
     },
     total=False,
 )
 
-GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
-    "GetTagKeysInputGetTagKeysPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 GetTagKeysInputRequestTypeDef = TypedDict(
     "GetTagKeysInputRequestTypeDef",
     {
         "PaginationToken": str,
     },
     total=False,
 )
 
-GetTagKeysOutputTypeDef = TypedDict(
-    "GetTagKeysOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagKeys": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "Key": str,
-    },
-)
-_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
-    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetTagValuesInputGetTagValuesPaginateTypeDef(
-    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
-    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
-):
-    pass
-
 _RequiredGetTagValuesInputRequestTypeDef = TypedDict(
     "_RequiredGetTagValuesInputRequestTypeDef",
     {
         "Key": str,
     },
 )
 _OptionalGetTagValuesInputRequestTypeDef = TypedDict(
@@ -189,52 +150,22 @@
 )
 
 class GetTagValuesInputRequestTypeDef(
     _RequiredGetTagValuesInputRequestTypeDef, _OptionalGetTagValuesInputRequestTypeDef
 ):
     pass
 
-GetTagValuesOutputTypeDef = TypedDict(
-    "GetTagValuesOutputTypeDef",
-    {
-        "PaginationToken": str,
-        "TagValues": List[str],
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
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
 StartReportCreationInputRequestTypeDef = TypedDict(
     "StartReportCreationInputRequestTypeDef",
     {
         "S3Bucket": str,
     },
 )
 
@@ -250,49 +181,118 @@
     "UntagResourcesInputRequestTypeDef",
     {
         "ResourceARNList": Sequence[str],
         "TagKeys": Sequence[str],
     },
 )
 
+DescribeReportCreationOutputTypeDef = TypedDict(
+    "DescribeReportCreationOutputTypeDef",
+    {
+        "Status": str,
+        "S3Location": str,
+        "ErrorMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagKeysOutputTypeDef = TypedDict(
+    "GetTagKeysOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagKeys": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetTagValuesOutputTypeDef = TypedDict(
+    "GetTagValuesOutputTypeDef",
+    {
+        "PaginationToken": str,
+        "TagValues": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 TagResourcesOutputTypeDef = TypedDict(
     "TagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UntagResourcesOutputTypeDef = TypedDict(
     "UntagResourcesOutputTypeDef",
     {
         "FailedResourcesMap": Dict[str, FailureInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef = TypedDict(
+    "GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef",
+    {
+        "TargetIdFilters": Sequence[str],
+        "RegionFilters": Sequence[str],
+        "ResourceTypeFilters": Sequence[str],
+        "TagKeyFilters": Sequence[str],
+        "GroupBy": Sequence[GroupByAttributeType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+GetTagKeysInputGetTagKeysPaginateTypeDef = TypedDict(
+    "GetTagKeysInputGetTagKeysPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_RequiredGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "Key": str,
+    },
+)
+_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef = TypedDict(
+    "_OptionalGetTagValuesInputGetTagValuesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetTagValuesInputGetTagValuesPaginateTypeDef(
+    _RequiredGetTagValuesInputGetTagValuesPaginateTypeDef,
+    _OptionalGetTagValuesInputGetTagValuesPaginateTypeDef,
+):
+    pass
+
 GetComplianceSummaryOutputTypeDef = TypedDict(
     "GetComplianceSummaryOutputTypeDef",
     {
         "SummaryList": List[SummaryTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetResourcesInputGetResourcesPaginateTypeDef = TypedDict(
     "GetResourcesInputGetResourcesPaginateTypeDef",
     {
         "TagFilters": Sequence[TagFilterTypeDef],
         "TagsPerPage": int,
         "ResourceTypeFilters": Sequence[str],
         "IncludeComplianceDetails": bool,
         "ExcludeCompliantResources": bool,
         "ResourceARNList": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 GetResourcesInputRequestTypeDef = TypedDict(
     "GetResourcesInputRequestTypeDef",
     {
@@ -319,10 +319,10 @@
 )
 
 GetResourcesOutputTypeDef = TypedDict(
     "GetResourcesOutputTypeDef",
     {
         "PaginationToken": str,
         "ResourceTagMappingList": List[ResourceTagMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-resourcegroupstaggingapi
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ResourceGroupsTaggingAPI 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore resourcegroupstaggingapi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore resourcegroupstaggingapi type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-resourcegroupstaggingapi"></a>
 
 # types-aiobotocore-resourcegroupstaggingapi
 
 [![PyPI - types-aiobotocore-resourcegroupstaggingapi](https://img.shields.io/pypi/v/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-resourcegroupstaggingapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-resourcegroupstaggingapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-resourcegroupstaggingapi?color=blue)](https://pypistats.org/packages/types-aiobotocore-resourcegroupstaggingapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-resourcegroupstaggingapi)](https://pepy.tech/project/types-aiobotocore-resourcegroupstaggingapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ResourceGroupsTaggingAPI 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/resourcegroupstaggingapi.html#ResourceGroupsTaggingAPI)
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
 [types-aiobotocore-resourcegroupstaggingapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_resourcegroupstaggingapi/).
 
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
@@ -321,54 +320,54 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_resourcegroupstaggingapi.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_resourcegroupstaggingapi.type_defs import (
     ComplianceDetailsTypeDef,
-    DescribeReportCreationOutputTypeDef,
+    ResponseMetadataTypeDef,
     FailureInfoTypeDef,
-    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetComplianceSummaryInputRequestTypeDef,
     SummaryTypeDef,
     TagFilterTypeDef,
-    GetTagKeysInputGetTagKeysPaginateTypeDef,
     GetTagKeysInputRequestTypeDef,
-    GetTagKeysOutputTypeDef,
-    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetTagValuesInputRequestTypeDef,
-    GetTagValuesOutputTypeDef,
-    PaginatorConfigTypeDef,
     TagTypeDef,
-    ResponseMetadataTypeDef,
     StartReportCreationInputRequestTypeDef,
     TagResourcesInputRequestTypeDef,
     UntagResourcesInputRequestTypeDef,
+    DescribeReportCreationOutputTypeDef,
+    GetTagKeysOutputTypeDef,
+    GetTagValuesOutputTypeDef,
     TagResourcesOutputTypeDef,
     UntagResourcesOutputTypeDef,
+    GetComplianceSummaryInputGetComplianceSummaryPaginateTypeDef,
+    GetTagKeysInputGetTagKeysPaginateTypeDef,
+    GetTagValuesInputGetTagValuesPaginateTypeDef,
     GetComplianceSummaryOutputTypeDef,
     GetResourcesInputGetResourcesPaginateTypeDef,
     GetResourcesInputRequestTypeDef,
     ResourceTagMappingTypeDef,
     GetResourcesOutputTypeDef,
 )
 
 
-def get_structure() -> ComplianceDetailsTypeDef:
+def get_value() -> ComplianceDetailsTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-resourcegroupstaggingapi-2.5.2/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt` & `types-aiobotocore-resourcegroupstaggingapi-2.5.2.post1/types_aiobotocore_resourcegroupstaggingapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


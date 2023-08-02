# Comparing `tmp/types-aiobotocore-cloud9-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloud9-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloud9-2.5.2.tar", last modified: Sat Jul  8 01:43:20 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloud9-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:59 2023, max compression
```

## Comparing `types-aiobotocore-cloud9-2.5.2.tar` & `types-aiobotocore-cloud9-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:20.565807 types-aiobotocore-cloud9-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-08 01:43:20.565807 types-aiobotocore-cloud9-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12933 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:20.565807 types-aiobotocore-cloud9-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:20.565807 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-07-08 01:26:50.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-07-08 01:26:50.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9739 2023-07-08 01:26:50.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-07-08 01:26:50.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:49.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:20.565807 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-07-08 01:43:20.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:43:20.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:20.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:20.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:20.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:20.000000 types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12916 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.845637 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13609 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13585 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9453 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9451 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9708 2023-08-02 14:34:19.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:18.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:59.849637 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14430 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:59.000000 types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloud9-2.5.2/LICENSE` & `types-aiobotocore-cloud9-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/PKG-INFO` & `types-aiobotocore-cloud9-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloud9 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloud9 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloud9"></a>
 
 # types-aiobotocore-cloud9
 
 [![PyPI - types-aiobotocore-cloud9](https://img.shields.io/pypi/v/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloud9?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloud9)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Cloud9 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
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
@@ -321,56 +320,56 @@
 )
 
 
 def check_value(value: ConnectionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloud9.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloud9.type_defs import (
     TagTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
+    ListEnvironmentsResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloud9-2.5.2/README.md` & `types-aiobotocore-cloud9-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloud9"></a>
 
 # types-aiobotocore-cloud9
 
 [![PyPI - types-aiobotocore-cloud9](https://img.shields.io/pypi/v/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloud9?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloud9)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Cloud9 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
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
@@ -288,56 +288,56 @@
 )
 
 
 def check_value(value: ConnectionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloud9.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloud9.type_defs import (
     TagTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
+    ListEnvironmentsResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloud9-2.5.2/setup.py` & `types-aiobotocore-cloud9-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloud9",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloud9"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore cloud9 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloud9 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloud9": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/"
```

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/__init__.py` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/__init__.pyi` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/__main__.py` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Cloud9 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Cloud9 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9\nOther"
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

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/client.py` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/client.pyi` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/literals.py` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/literals.pyi` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/paginator.py` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,28 +55,28 @@
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
 
 class ListEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/paginator.pyi` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -52,27 +52,27 @@
 
     def paginate(
         self,
         *,
         userArn: str = ...,
         environmentId: str = ...,
         permissions: Sequence[PermissionsType] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEnvironmentMembershipsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.DescribeEnvironmentMemberships.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#describeenvironmentmembershipspaginator)
         """
 
 class ListEnvironmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#listenvironmentspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListEnvironmentsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9.Paginator.ListEnvironments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/paginators/#listenvironmentspaginator)
         """
```

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/type_defs.py` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloud9.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -30,57 +30,60 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "TagTypeDef",
-    "CreateEnvironmentEC2ResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     "DescribeEnvironmentStatusRequestRequestTypeDef",
-    "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
-    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateEnvironmentEC2ResultTypeDef",
+    "DescribeEnvironmentStatusResultTypeDef",
+    "ListEnvironmentsResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "EnvironmentTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateEnvironmentEC2ResultTypeDef = TypedDict(
-    "CreateEnvironmentEC2ResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -124,21 +127,20 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "userArn": str,
-        "environmentId": str,
-        "permissions": Sequence[PermissionsType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEnvironmentMembershipsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     {
@@ -154,23 +156,14 @@
 DescribeEnvironmentStatusRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentStatusRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentStatusResultTypeDef = TypedDict(
-    "DescribeEnvironmentStatusResultTypeDef",
-    {
-        "status": EnvironmentStatusType,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentsRequestRequestTypeDef",
     {
         "environmentIds": Sequence[str],
     },
 )
 
@@ -180,68 +173,30 @@
         "status": EnvironmentLifecycleStatusType,
         "reason": str,
         "failureResource": str,
     },
     total=False,
 )
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListEnvironmentsResultTypeDef = TypedDict(
-    "ListEnvironmentsResultTypeDef",
-    {
-        "nextToken": str,
-        "environmentIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -305,55 +260,100 @@
 class CreateEnvironmentEC2RequestRequestTypeDef(
     _RequiredCreateEnvironmentEC2RequestRequestTypeDef,
     _OptionalCreateEnvironmentEC2RequestRequestTypeDef,
 ):
     pass
 
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateEnvironmentEC2ResultTypeDef = TypedDict(
+    "CreateEnvironmentEC2ResultTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentStatusResultTypeDef = TypedDict(
+    "DescribeEnvironmentStatusResultTypeDef",
+    {
+        "status": EnvironmentStatusType,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsResultTypeDef = TypedDict(
+    "ListEnvironmentsResultTypeDef",
+    {
+        "nextToken": str,
+        "environmentIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEnvironmentMembershipResultTypeDef = TypedDict(
     "CreateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentMembershipsResultTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsResultTypeDef",
     {
         "memberships": List[EnvironmentMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentMembershipResultTypeDef = TypedDict(
     "UpdateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    {
+        "userArn": str,
+        "environmentId": str,
+        "permissions": Sequence[PermissionsType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEnvironmentTypeDef = TypedDict(
     "_RequiredEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "arn": str,
         "ownerArn": str,
     },
@@ -376,10 +376,10 @@
     pass
 
 
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9/type_defs.pyi` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloud9.type_defs import TagTypeDef
 
-    data: TagTypeDef = {...}
+    data: TagTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -29,57 +29,60 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "TagTypeDef",
-    "CreateEnvironmentEC2ResultTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     "EnvironmentMemberTypeDef",
     "DeleteEnvironmentMembershipRequestRequestTypeDef",
     "DeleteEnvironmentRequestRequestTypeDef",
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     "DescribeEnvironmentStatusRequestRequestTypeDef",
-    "DescribeEnvironmentStatusResultTypeDef",
     "DescribeEnvironmentsRequestRequestTypeDef",
     "EnvironmentLifecycleTypeDef",
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "ListEnvironmentsRequestRequestTypeDef",
-    "ListEnvironmentsResultTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateEnvironmentMembershipRequestRequestTypeDef",
     "UpdateEnvironmentRequestRequestTypeDef",
     "CreateEnvironmentEC2RequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "CreateEnvironmentEC2ResultTypeDef",
+    "DescribeEnvironmentStatusResultTypeDef",
+    "ListEnvironmentsResultTypeDef",
+    "ListTagsForResourceResponseTypeDef",
     "CreateEnvironmentMembershipResultTypeDef",
     "DescribeEnvironmentMembershipsResultTypeDef",
     "UpdateEnvironmentMembershipResultTypeDef",
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
     "EnvironmentTypeDef",
     "DescribeEnvironmentsResultTypeDef",
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateEnvironmentEC2ResultTypeDef = TypedDict(
-    "CreateEnvironmentEC2ResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "environmentId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CreateEnvironmentMembershipRequestRequestTypeDef = TypedDict(
     "CreateEnvironmentMembershipRequestRequestTypeDef",
     {
         "environmentId": str,
@@ -121,21 +124,20 @@
 DeleteEnvironmentRequestRequestTypeDef = TypedDict(
     "DeleteEnvironmentRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
-    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "userArn": str,
-        "environmentId": str,
-        "permissions": Sequence[PermissionsType],
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeEnvironmentMembershipsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsRequestRequestTypeDef",
     {
@@ -151,23 +153,14 @@
 DescribeEnvironmentStatusRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentStatusRequestRequestTypeDef",
     {
         "environmentId": str,
     },
 )
 
-DescribeEnvironmentStatusResultTypeDef = TypedDict(
-    "DescribeEnvironmentStatusResultTypeDef",
-    {
-        "status": EnvironmentStatusType,
-        "message": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeEnvironmentsRequestRequestTypeDef = TypedDict(
     "DescribeEnvironmentsRequestRequestTypeDef",
     {
         "environmentIds": Sequence[str],
     },
 )
 
@@ -177,68 +170,30 @@
         "status": EnvironmentLifecycleStatusType,
         "reason": str,
         "failureResource": str,
     },
     total=False,
 )
 
-ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
-    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListEnvironmentsRequestRequestTypeDef = TypedDict(
     "ListEnvironmentsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-ListEnvironmentsResultTypeDef = TypedDict(
-    "ListEnvironmentsResultTypeDef",
-    {
-        "nextToken": str,
-        "environmentIds": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
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
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -298,55 +253,100 @@
 
 class CreateEnvironmentEC2RequestRequestTypeDef(
     _RequiredCreateEnvironmentEC2RequestRequestTypeDef,
     _OptionalCreateEnvironmentEC2RequestRequestTypeDef,
 ):
     pass
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateEnvironmentEC2ResultTypeDef = TypedDict(
+    "CreateEnvironmentEC2ResultTypeDef",
+    {
+        "environmentId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeEnvironmentStatusResultTypeDef = TypedDict(
+    "DescribeEnvironmentStatusResultTypeDef",
+    {
+        "status": EnvironmentStatusType,
+        "message": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListEnvironmentsResultTypeDef = TypedDict(
+    "ListEnvironmentsResultTypeDef",
+    {
+        "nextToken": str,
+        "environmentIds": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": List[TagTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateEnvironmentMembershipResultTypeDef = TypedDict(
     "CreateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeEnvironmentMembershipsResultTypeDef = TypedDict(
     "DescribeEnvironmentMembershipsResultTypeDef",
     {
         "memberships": List[EnvironmentMemberTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateEnvironmentMembershipResultTypeDef = TypedDict(
     "UpdateEnvironmentMembershipResultTypeDef",
     {
         "membership": EnvironmentMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef = TypedDict(
+    "DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef",
+    {
+        "userArn": str,
+        "environmentId": str,
+        "permissions": Sequence[PermissionsType],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListEnvironmentsRequestListEnvironmentsPaginateTypeDef = TypedDict(
+    "ListEnvironmentsRequestListEnvironmentsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 _RequiredEnvironmentTypeDef = TypedDict(
     "_RequiredEnvironmentTypeDef",
     {
         "type": EnvironmentTypeType,
         "arn": str,
         "ownerArn": str,
     },
@@ -367,10 +367,10 @@
 class EnvironmentTypeDef(_RequiredEnvironmentTypeDef, _OptionalEnvironmentTypeDef):
     pass
 
 DescribeEnvironmentsResultTypeDef = TypedDict(
     "DescribeEnvironmentsResultTypeDef",
     {
         "environments": List[EnvironmentTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/PKG-INFO` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloud9
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Cloud9 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloud9 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloud9 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloud9"></a>
 
 # types-aiobotocore-cloud9
 
 [![PyPI - types-aiobotocore-cloud9](https://img.shields.io/pypi/v/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloud9.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloud9)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloud9?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloud9)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloud9)](https://pepy.tech/project/types-aiobotocore-cloud9)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Cloud9 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloud9.html#Cloud9)
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
 [types-aiobotocore-cloud9 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloud9/).
 
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
@@ -321,56 +320,56 @@
 )
 
 
 def check_value(value: ConnectionTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloud9.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloud9.type_defs import (
     TagTypeDef,
-    CreateEnvironmentEC2ResultTypeDef,
+    ResponseMetadataTypeDef,
     CreateEnvironmentMembershipRequestRequestTypeDef,
     EnvironmentMemberTypeDef,
     DeleteEnvironmentMembershipRequestRequestTypeDef,
     DeleteEnvironmentRequestRequestTypeDef,
-    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeEnvironmentMembershipsRequestRequestTypeDef,
     DescribeEnvironmentStatusRequestRequestTypeDef,
-    DescribeEnvironmentStatusResultTypeDef,
     DescribeEnvironmentsRequestRequestTypeDef,
     EnvironmentLifecycleTypeDef,
-    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     ListEnvironmentsRequestRequestTypeDef,
-    ListEnvironmentsResultTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateEnvironmentMembershipRequestRequestTypeDef,
     UpdateEnvironmentRequestRequestTypeDef,
     CreateEnvironmentEC2RequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    CreateEnvironmentEC2ResultTypeDef,
+    DescribeEnvironmentStatusResultTypeDef,
+    ListEnvironmentsResultTypeDef,
+    ListTagsForResourceResponseTypeDef,
     CreateEnvironmentMembershipResultTypeDef,
     DescribeEnvironmentMembershipsResultTypeDef,
     UpdateEnvironmentMembershipResultTypeDef,
+    DescribeEnvironmentMembershipsRequestDescribeEnvironmentMembershipsPaginateTypeDef,
+    ListEnvironmentsRequestListEnvironmentsPaginateTypeDef,
     EnvironmentTypeDef,
     DescribeEnvironmentsResultTypeDef,
 )
 
 
-def get_structure() -> TagTypeDef:
+def get_value() -> TagTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloud9-2.5.2/types_aiobotocore_cloud9.egg-info/SOURCES.txt` & `types-aiobotocore-cloud9-2.5.2.post1/types_aiobotocore_cloud9.egg-info/SOURCES.txt`

 * *Files identical despite different names*


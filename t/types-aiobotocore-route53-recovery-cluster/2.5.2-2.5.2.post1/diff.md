# Comparing `tmp/types-aiobotocore-route53-recovery-cluster-2.5.2.tar.gz` & `tmp/types-aiobotocore-route53-recovery-cluster-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-route53-recovery-cluster-2.5.2.tar", last modified: Sat Jul  8 01:44:13 2023, max compression
+gzip compressed data, was "types-aiobotocore-route53-recovery-cluster-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:54 2023, max compression
```

## Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2.tar` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.554801 types-aiobotocore-route53-recovery-cluster-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-07-08 01:44:13.554801 types-aiobotocore-route53-recovery-cluster-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12644 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:13.554801 types-aiobotocore-route53-recovery-cluster-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2238 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.554801 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-08 01:39:28.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:27.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:13.554801 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14275 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-08 01:44:13.000000 types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12627 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.673476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8343 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7916 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-02 14:48:06.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:48:05.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:54.677476 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-08-02 14:52:54.000000 types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/LICENSE` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/PKG-INFO` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-cluster
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53-recovery-cluster type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53-recovery-cluster type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53-recovery-cluster"></a>
 
 # types-aiobotocore-route53-recovery-cluster
 
 [![PyPI - types-aiobotocore-route53-recovery-cluster](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-cluster)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-cluster)](https://pepy.tech/project/types-aiobotocore-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53RecoveryCluster 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
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
@@ -307,39 +306,39 @@
 )
 
 
 def check_value(value: ListRoutingControlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53_recovery_cluster.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
+def get_value() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/README.md` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-route53-recovery-cluster"></a>
 
 # types-aiobotocore-route53-recovery-cluster
 
 [![PyPI - types-aiobotocore-route53-recovery-cluster](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-cluster)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-cluster)](https://pepy.tech/project/types-aiobotocore-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53RecoveryCluster 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
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
@@ -274,39 +274,39 @@
 )
 
 
 def check_value(value: ListRoutingControlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53_recovery_cluster.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
+def get_value() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/setup.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,46 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-route53-recovery-cluster",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_route53_recovery_cluster"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with"
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
-        "aiobotocore route53-recovery-cluster type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "aiobotocore route53-recovery-cluster type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_route53_recovery_cluster": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/",
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/__init__.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/__init__.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/__main__.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster\nOther"
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

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/client.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/client.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/literals.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/literals.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/paginator.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -25,31 +25,28 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListRoutingControlsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListRoutingControlsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListRoutingControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
         """
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/paginator.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,28 +25,31 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListRoutingControlsResponseTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListRoutingControlsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListRoutingControlsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
     """
 
     def paginate(
-        self, *, ControlPanelArn: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ControlPanelArn: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListRoutingControlsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster.Paginator.ListRoutingControls.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/paginators/#listroutingcontrolspaginator)
         """
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/type_defs.py` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateRequestRequestTypeDef
 
-    data: GetRoutingControlStateRequestRequestTypeDef = {...}
+    data: GetRoutingControlStateRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import RoutingControlStateType
 
@@ -20,48 +20,50 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "GetRoutingControlStateRequestRequestTypeDef",
-    "GetRoutingControlStateResponseTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
     "UpdateRoutingControlStateRequestRequestTypeDef",
+    "GetRoutingControlStateResponseTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlStatesRequestRequestTypeDef",
 )
 
 GetRoutingControlStateRequestRequestTypeDef = TypedDict(
     "GetRoutingControlStateRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 
-GetRoutingControlStateResponseTypeDef = TypedDict(
-    "GetRoutingControlStateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RoutingControlArn": str,
-        "RoutingControlState": RoutingControlStateType,
-        "RoutingControlName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ControlPanelArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRoutingControlsRequestRequestTypeDef = TypedDict(
     "ListRoutingControlsRequestRequestTypeDef",
     {
@@ -80,35 +82,14 @@
         "RoutingControlArn": str,
         "RoutingControlName": str,
         "RoutingControlState": RoutingControlStateType,
     },
     total=False,
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
 UpdateRoutingControlStateEntryTypeDef = TypedDict(
     "UpdateRoutingControlStateEntryTypeDef",
     {
         "RoutingControlArn": str,
         "RoutingControlState": RoutingControlStateType,
     },
 )
@@ -132,20 +113,39 @@
 class UpdateRoutingControlStateRequestRequestTypeDef(
     _RequiredUpdateRoutingControlStateRequestRequestTypeDef,
     _OptionalUpdateRoutingControlStateRequestRequestTypeDef,
 ):
     pass
 
 
+GetRoutingControlStateResponseTypeDef = TypedDict(
+    "GetRoutingControlStateResponseTypeDef",
+    {
+        "RoutingControlArn": str,
+        "RoutingControlState": RoutingControlStateType,
+        "RoutingControlName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "RoutingControls": List[RoutingControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateRoutingControlStatesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRoutingControlStatesRequestRequestTypeDef",
     {
         "UpdateRoutingControlStateEntries": Sequence[UpdateRoutingControlStateEntryTypeDef],
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster/type_defs.pyi` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,63 +4,65 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_route53_recovery_cluster.type_defs import GetRoutingControlStateRequestRequestTypeDef
 
-    data: GetRoutingControlStateRequestRequestTypeDef = {...}
+    data: GetRoutingControlStateRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import RoutingControlStateType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "GetRoutingControlStateRequestRequestTypeDef",
-    "GetRoutingControlStateResponseTypeDef",
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
     "ListRoutingControlsRequestRequestTypeDef",
     "RoutingControlTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateRoutingControlStateEntryTypeDef",
     "UpdateRoutingControlStateRequestRequestTypeDef",
+    "GetRoutingControlStateResponseTypeDef",
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
     "ListRoutingControlsResponseTypeDef",
     "UpdateRoutingControlStatesRequestRequestTypeDef",
 )
 
 GetRoutingControlStateRequestRequestTypeDef = TypedDict(
     "GetRoutingControlStateRequestRequestTypeDef",
     {
         "RoutingControlArn": str,
     },
 )
 
-GetRoutingControlStateResponseTypeDef = TypedDict(
-    "GetRoutingControlStateResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "RoutingControlArn": str,
-        "RoutingControlState": RoutingControlStateType,
-        "RoutingControlName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
-    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ControlPanelArn": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 ListRoutingControlsRequestRequestTypeDef = TypedDict(
     "ListRoutingControlsRequestRequestTypeDef",
     {
@@ -79,35 +81,14 @@
         "RoutingControlArn": str,
         "RoutingControlName": str,
         "RoutingControlState": RoutingControlStateType,
     },
     total=False,
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
 UpdateRoutingControlStateEntryTypeDef = TypedDict(
     "UpdateRoutingControlStateEntryTypeDef",
     {
         "RoutingControlArn": str,
         "RoutingControlState": RoutingControlStateType,
     },
 )
@@ -129,20 +110,39 @@
 
 class UpdateRoutingControlStateRequestRequestTypeDef(
     _RequiredUpdateRoutingControlStateRequestRequestTypeDef,
     _OptionalUpdateRoutingControlStateRequestRequestTypeDef,
 ):
     pass
 
+GetRoutingControlStateResponseTypeDef = TypedDict(
+    "GetRoutingControlStateResponseTypeDef",
+    {
+        "RoutingControlArn": str,
+        "RoutingControlState": RoutingControlStateType,
+        "RoutingControlName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListRoutingControlsRequestListRoutingControlsPaginateTypeDef = TypedDict(
+    "ListRoutingControlsRequestListRoutingControlsPaginateTypeDef",
+    {
+        "ControlPanelArn": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListRoutingControlsResponseTypeDef = TypedDict(
     "ListRoutingControlsResponseTypeDef",
     {
         "RoutingControls": List[RoutingControlTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateRoutingControlStatesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateRoutingControlStatesRequestRequestTypeDef",
     {
         "UpdateRoutingControlStateEntries": Sequence[UpdateRoutingControlStateEntryTypeDef],
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-route53-recovery-cluster
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Route53RecoveryCluster 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore route53-recovery-cluster type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore route53-recovery-cluster type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-route53-recovery-cluster"></a>
 
 # types-aiobotocore-route53-recovery-cluster
 
 [![PyPI - types-aiobotocore-route53-recovery-cluster](https://img.shields.io/pypi/v/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-route53-recovery-cluster.svg?color=blue)](https://pypi.org/project/types-aiobotocore-route53-recovery-cluster)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-route53-recovery-cluster?color=blue)](https://pypistats.org/packages/types-aiobotocore-route53-recovery-cluster)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-route53-recovery-cluster)](https://pepy.tech/project/types-aiobotocore-route53-recovery-cluster)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Route53RecoveryCluster 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/route53-recovery-cluster.html#Route53RecoveryCluster)
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
 [types-aiobotocore-route53-recovery-cluster docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_route53_recovery_cluster/).
 
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
@@ -307,39 +306,39 @@
 )
 
 
 def check_value(value: ListRoutingControlsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_route53_recovery_cluster.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_route53_recovery_cluster.type_defs import (
     GetRoutingControlStateRequestRequestTypeDef,
-    GetRoutingControlStateResponseTypeDef,
-    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
     ListRoutingControlsRequestRequestTypeDef,
     RoutingControlTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     UpdateRoutingControlStateEntryTypeDef,
     UpdateRoutingControlStateRequestRequestTypeDef,
+    GetRoutingControlStateResponseTypeDef,
+    ListRoutingControlsRequestListRoutingControlsPaginateTypeDef,
     ListRoutingControlsResponseTypeDef,
     UpdateRoutingControlStatesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> GetRoutingControlStateRequestRequestTypeDef:
+def get_value() -> GetRoutingControlStateRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-route53-recovery-cluster-2.5.2/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt` & `types-aiobotocore-route53-recovery-cluster-2.5.2.post1/types_aiobotocore_route53_recovery_cluster.egg-info/SOURCES.txt`

 * *Files identical despite different names*


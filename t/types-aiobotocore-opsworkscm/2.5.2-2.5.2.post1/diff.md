# Comparing `tmp/types-aiobotocore-opsworkscm-2.5.2.tar.gz` & `tmp/types-aiobotocore-opsworkscm-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-opsworkscm-2.5.2.tar", last modified: Sat Jul  8 01:44:04 2023, max compression
+gzip compressed data, was "types-aiobotocore-opsworkscm-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:45 2023, max compression
```

## Comparing `types-aiobotocore-opsworkscm-2.5.2.tar` & `types-aiobotocore-opsworkscm-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.574637 types-aiobotocore-opsworkscm-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-08 01:44:04.574637 types-aiobotocore-opsworkscm-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14656 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:04.574637 types-aiobotocore-opsworkscm-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.566637 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5489 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18816 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18789 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:09.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-07-08 01:36:10.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:04.574637 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-08 01:44:04.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-08 01:44:04.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:04.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:04.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:44:04.000000 types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14639 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.325505 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19181 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9048 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18749 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:44:27.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-08-02 14:44:28.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:45.329505 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:52:45.000000 types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/LICENSE` & `types-aiobotocore-opsworkscm-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/PKG-INFO` & `types-aiobotocore-opsworkscm-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore opsworkscm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opsworkscm?color=blue)](https://pypistats.org/packages/types-aiobotocore-opsworkscm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpsWorksCM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
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
@@ -348,74 +347,74 @@
 )
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_opsworkscm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    AssociateNodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
     DescribeServersRequestRequestTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
     ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
+    AssociateNodeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
+    DisassociateNodeResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAttributeTypeDef:
+def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/README.md` & `types-aiobotocore-opsworkscm-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opsworkscm?color=blue)](https://pypistats.org/packages/types-aiobotocore-opsworkscm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpsWorksCM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
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
@@ -315,74 +315,74 @@
 )
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_opsworkscm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    AssociateNodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
     DescribeServersRequestRequestTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
     ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
+    AssociateNodeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
+    DisassociateNodeResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAttributeTypeDef:
+def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/setup.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-opsworkscm",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_opsworkscm"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with"
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
-    keywords="aiobotocore opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore opsworkscm type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_opsworkscm": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/"
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/__init__.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/__init__.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/__main__.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.OpsWorksCM 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.OpsWorksCM 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM\nOther"
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

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/client.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/client.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/literals.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/literals.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/paginator.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,58 +64,58 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describebackupspaginator)
         """
 
 
 class DescribeEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeeventspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeeventspaginator)
         """
 
 
 class DescribeServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeserverspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeserverspaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/paginator.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -61,55 +61,55 @@
     """
 
     def paginate(
         self,
         *,
         BackupId: str = ...,
         ServerName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describebackupspaginator)
         """
 
 class DescribeEventsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeeventspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeEvents.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeeventspaginator)
         """
 
 class DescribeServersPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeserverspaginator)
     """
 
     def paginate(
-        self, *, ServerName: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ServerName: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.DescribeServers.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#describeserverspaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceArn: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/type_defs.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_opsworkscm.type_defs import AccountAttributeTypeDef
 
-    data: AccountAttributeTypeDef = {...}
+    data: AccountAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -28,51 +28,51 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
-    "AssociateNodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
     "DescribeServersRequestRequestTypeDef",
-    "DisassociateNodeResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
     "AssociateNodeRequestRequestTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
     "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
+    "AssociateNodeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    "DisassociateNodeResponseTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
@@ -94,19 +94,22 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AssociateNodeResponseTypeDef = TypedDict(
-    "AssociateNodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BackupTypeDef = TypedDict(
     "BackupTypeDef",
     {
         "BackupArn": str,
@@ -155,20 +158,20 @@
 DeleteServerRequestRequestTypeDef = TypedDict(
     "DeleteServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "BackupId": str,
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -176,36 +179,14 @@
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "ServerName": str,
-    },
-)
-_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeEventsRequestDescribeEventsPaginateTypeDef(
-    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
-    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventsRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalDescribeEventsRequestRequestTypeDef = TypedDict(
@@ -248,63 +229,24 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
-DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
-    {
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DisassociateNodeResponseTypeDef = TypedDict(
-    "DisassociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -320,35 +262,14 @@
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
         "ServerName": str,
     },
 )
@@ -419,40 +340,23 @@
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
 
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "Attributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNodeRequestRequestTypeDef = TypedDict(
     "AssociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
 )
 
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
     },
 )
@@ -490,23 +394,14 @@
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
 
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BackupRetentionCount": int,
         "ServerName": str,
         "CreatedAt": datetime,
@@ -551,28 +446,70 @@
 
 class StartMaintenanceRequestRequestTypeDef(
     _RequiredStartMaintenanceRequestRequestTypeDef, _OptionalStartMaintenanceRequestRequestTypeDef
 ):
     pass
 
 
+AssociateNodeResponseTypeDef = TypedDict(
+    "AssociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "Attributes": List[AccountAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateNodeResponseTypeDef = TypedDict(
+    "DisassociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackupRequestRequestTypeDef",
     {
         "ServerName": str,
@@ -635,32 +572,95 @@
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "BackupId": str,
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "ServerName": str,
+    },
+)
+_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeEventsRequestDescribeEventsPaginateTypeDef(
+    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
+    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
+):
+    pass
+
+
+DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    {
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "ServerEvents": List[ServerEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "NodeAssociationStatusToken": str,
@@ -683,51 +683,51 @@
     pass
 
 
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServersResponseTypeDef = TypedDict(
     "DescribeServersResponseTypeDef",
     {
         "Servers": List[ServerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreServerResponseTypeDef = TypedDict(
     "RestoreServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMaintenanceResponseTypeDef = TypedDict(
     "StartMaintenanceResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerEngineAttributesResponseTypeDef = TypedDict(
     "UpdateServerEngineAttributesResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerResponseTypeDef = TypedDict(
     "UpdateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/type_defs.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_opsworkscm.type_defs import AccountAttributeTypeDef
 
-    data: AccountAttributeTypeDef = {...}
+    data: AccountAttributeTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
@@ -27,51 +27,51 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountAttributeTypeDef",
     "EngineAttributeTypeDef",
-    "AssociateNodeResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "BackupTypeDef",
     "TagTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteServerRequestRequestTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
     "DescribeEventsRequestRequestTypeDef",
     "ServerEventTypeDef",
     "WaiterConfigTypeDef",
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
     "DescribeServersRequestRequestTypeDef",
-    "DisassociateNodeResponseTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreServerRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateServerEngineAttributesRequestRequestTypeDef",
     "UpdateServerRequestRequestTypeDef",
-    "DescribeAccountAttributesResponseTypeDef",
     "AssociateNodeRequestRequestTypeDef",
-    "DescribeNodeAssociationStatusResponseTypeDef",
     "DisassociateNodeRequestRequestTypeDef",
     "ExportServerEngineAttributeRequestRequestTypeDef",
-    "ExportServerEngineAttributeResponseTypeDef",
     "ServerTypeDef",
     "StartMaintenanceRequestRequestTypeDef",
+    "AssociateNodeResponseTypeDef",
+    "DescribeAccountAttributesResponseTypeDef",
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    "DisassociateNodeResponseTypeDef",
+    "ExportServerEngineAttributeResponseTypeDef",
     "CreateBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "CreateBackupRequestRequestTypeDef",
     "CreateServerRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeEventsRequestDescribeEventsPaginateTypeDef",
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "DescribeEventsResponseTypeDef",
     "DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     "CreateServerResponseTypeDef",
     "DescribeServersResponseTypeDef",
     "RestoreServerResponseTypeDef",
     "StartMaintenanceResponseTypeDef",
     "UpdateServerEngineAttributesResponseTypeDef",
@@ -93,19 +93,22 @@
     {
         "Name": str,
         "Value": str,
     },
     total=False,
 )
 
-AssociateNodeResponseTypeDef = TypedDict(
-    "AssociateNodeResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 BackupTypeDef = TypedDict(
     "BackupTypeDef",
     {
         "BackupArn": str,
@@ -154,20 +157,20 @@
 DeleteServerRequestRequestTypeDef = TypedDict(
     "DeleteServerRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "BackupId": str,
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeBackupsRequestRequestTypeDef = TypedDict(
     "DescribeBackupsRequestRequestTypeDef",
     {
@@ -175,34 +178,14 @@
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "ServerName": str,
-    },
-)
-_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeEventsRequestDescribeEventsPaginateTypeDef(
-    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
-    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeEventsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeEventsRequestRequestTypeDef",
     {
         "ServerName": str,
     },
 )
 _OptionalDescribeEventsRequestRequestTypeDef = TypedDict(
@@ -243,61 +226,24 @@
     "DescribeNodeAssociationStatusRequestRequestTypeDef",
     {
         "NodeAssociationStatusToken": str,
         "ServerName": str,
     },
 )
 
-DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
-    "DescribeServersRequestDescribeServersPaginateTypeDef",
-    {
-        "ServerName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeServersRequestRequestTypeDef = TypedDict(
     "DescribeServersRequestRequestTypeDef",
     {
         "ServerName": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-DisassociateNodeResponseTypeDef = TypedDict(
-    "DisassociateNodeResponseTypeDef",
-    {
-        "NodeAssociationStatusToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceArn": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -311,35 +257,14 @@
 
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
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
 _RequiredRestoreServerRequestRequestTypeDef = TypedDict(
     "_RequiredRestoreServerRequestRequestTypeDef",
     {
         "BackupId": str,
         "ServerName": str,
     },
 )
@@ -404,40 +329,23 @@
 )
 
 class UpdateServerRequestRequestTypeDef(
     _RequiredUpdateServerRequestRequestTypeDef, _OptionalUpdateServerRequestRequestTypeDef
 ):
     pass
 
-DescribeAccountAttributesResponseTypeDef = TypedDict(
-    "DescribeAccountAttributesResponseTypeDef",
-    {
-        "Attributes": List[AccountAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 AssociateNodeRequestRequestTypeDef = TypedDict(
     "AssociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
         "EngineAttributes": Sequence[EngineAttributeTypeDef],
     },
 )
 
-DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
-    "DescribeNodeAssociationStatusResponseTypeDef",
-    {
-        "NodeAssociationStatus": NodeAssociationStatusType,
-        "EngineAttributes": List[EngineAttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDisassociateNodeRequestRequestTypeDef = TypedDict(
     "_RequiredDisassociateNodeRequestRequestTypeDef",
     {
         "ServerName": str,
         "NodeName": str,
     },
 )
@@ -471,23 +379,14 @@
 
 class ExportServerEngineAttributeRequestRequestTypeDef(
     _RequiredExportServerEngineAttributeRequestRequestTypeDef,
     _OptionalExportServerEngineAttributeRequestRequestTypeDef,
 ):
     pass
 
-ExportServerEngineAttributeResponseTypeDef = TypedDict(
-    "ExportServerEngineAttributeResponseTypeDef",
-    {
-        "EngineAttribute": EngineAttributeTypeDef,
-        "ServerName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ServerTypeDef = TypedDict(
     "ServerTypeDef",
     {
         "AssociatePublicIpAddress": bool,
         "BackupRetentionCount": int,
         "ServerName": str,
         "CreatedAt": datetime,
@@ -530,28 +429,70 @@
 )
 
 class StartMaintenanceRequestRequestTypeDef(
     _RequiredStartMaintenanceRequestRequestTypeDef, _OptionalStartMaintenanceRequestRequestTypeDef
 ):
     pass
 
+AssociateNodeResponseTypeDef = TypedDict(
+    "AssociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeAccountAttributesResponseTypeDef = TypedDict(
+    "DescribeAccountAttributesResponseTypeDef",
+    {
+        "Attributes": List[AccountAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeNodeAssociationStatusResponseTypeDef = TypedDict(
+    "DescribeNodeAssociationStatusResponseTypeDef",
+    {
+        "NodeAssociationStatus": NodeAssociationStatusType,
+        "EngineAttributes": List[EngineAttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DisassociateNodeResponseTypeDef = TypedDict(
+    "DisassociateNodeResponseTypeDef",
+    {
+        "NodeAssociationStatusToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExportServerEngineAttributeResponseTypeDef = TypedDict(
+    "ExportServerEngineAttributeResponseTypeDef",
+    {
+        "EngineAttribute": EngineAttributeTypeDef,
+        "ServerName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateBackupResponseTypeDef = TypedDict(
     "CreateBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeBackupsResponseTypeDef = TypedDict(
     "DescribeBackupsResponseTypeDef",
     {
         "Backups": List[BackupTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateBackupRequestRequestTypeDef = TypedDict(
     "_RequiredCreateBackupRequestRequestTypeDef",
     {
         "ServerName": str,
@@ -610,32 +551,91 @@
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "BackupId": str,
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "ServerName": str,
+    },
+)
+_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeEventsRequestDescribeEventsPaginateTypeDef(
+    _RequiredDescribeEventsRequestDescribeEventsPaginateTypeDef,
+    _OptionalDescribeEventsRequestDescribeEventsPaginateTypeDef,
+):
+    pass
+
+DescribeServersRequestDescribeServersPaginateTypeDef = TypedDict(
+    "DescribeServersRequestDescribeServersPaginateTypeDef",
+    {
+        "ServerName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceArn": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 DescribeEventsResponseTypeDef = TypedDict(
     "DescribeEventsResponseTypeDef",
     {
         "ServerEvents": List[ServerEventTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef = TypedDict(
     "_RequiredDescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef",
     {
         "NodeAssociationStatusToken": str,
@@ -656,51 +656,51 @@
 ):
     pass
 
 CreateServerResponseTypeDef = TypedDict(
     "CreateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeServersResponseTypeDef = TypedDict(
     "DescribeServersResponseTypeDef",
     {
         "Servers": List[ServerTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreServerResponseTypeDef = TypedDict(
     "RestoreServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartMaintenanceResponseTypeDef = TypedDict(
     "StartMaintenanceResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerEngineAttributesResponseTypeDef = TypedDict(
     "UpdateServerEngineAttributesResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateServerResponseTypeDef = TypedDict(
     "UpdateServerResponseTypeDef",
     {
         "Server": ServerTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/waiter.py` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm/waiter.pyi` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/PKG-INFO` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-opsworkscm
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.OpsWorksCM 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore opsworkscm type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore opsworkscm type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-opsworkscm"></a>
 
 # types-aiobotocore-opsworkscm
 
 [![PyPI - types-aiobotocore-opsworkscm](https://img.shields.io/pypi/v/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-opsworkscm.svg?color=blue)](https://pypi.org/project/types-aiobotocore-opsworkscm)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-opsworkscm?color=blue)](https://pypistats.org/packages/types-aiobotocore-opsworkscm)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-opsworkscm)](https://pepy.tech/project/types-aiobotocore-opsworkscm)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.OpsWorksCM 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/opsworkscm.html#OpsWorksCM)
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
 [types-aiobotocore-opsworkscm docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_opsworkscm/).
 
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
@@ -348,74 +347,74 @@
 )
 
 
 def check_value(value: BackupStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_opsworkscm.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_opsworkscm.type_defs import (
     AccountAttributeTypeDef,
     EngineAttributeTypeDef,
-    AssociateNodeResponseTypeDef,
+    ResponseMetadataTypeDef,
     BackupTypeDef,
     TagTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteServerRequestRequestTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeEventsRequestDescribeEventsPaginateTypeDef,
     DescribeEventsRequestRequestTypeDef,
     ServerEventTypeDef,
     WaiterConfigTypeDef,
     DescribeNodeAssociationStatusRequestRequestTypeDef,
-    DescribeServersRequestDescribeServersPaginateTypeDef,
     DescribeServersRequestRequestTypeDef,
-    DisassociateNodeResponseTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreServerRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateServerEngineAttributesRequestRequestTypeDef,
     UpdateServerRequestRequestTypeDef,
-    DescribeAccountAttributesResponseTypeDef,
     AssociateNodeRequestRequestTypeDef,
-    DescribeNodeAssociationStatusResponseTypeDef,
     DisassociateNodeRequestRequestTypeDef,
     ExportServerEngineAttributeRequestRequestTypeDef,
-    ExportServerEngineAttributeResponseTypeDef,
     ServerTypeDef,
     StartMaintenanceRequestRequestTypeDef,
+    AssociateNodeResponseTypeDef,
+    DescribeAccountAttributesResponseTypeDef,
+    DescribeNodeAssociationStatusResponseTypeDef,
+    DisassociateNodeResponseTypeDef,
+    ExportServerEngineAttributeResponseTypeDef,
     CreateBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     CreateBackupRequestRequestTypeDef,
     CreateServerRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeEventsRequestDescribeEventsPaginateTypeDef,
+    DescribeServersRequestDescribeServersPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     DescribeEventsResponseTypeDef,
     DescribeNodeAssociationStatusRequestNodeAssociatedWaitTypeDef,
     CreateServerResponseTypeDef,
     DescribeServersResponseTypeDef,
     RestoreServerResponseTypeDef,
     StartMaintenanceResponseTypeDef,
     UpdateServerEngineAttributesResponseTypeDef,
     UpdateServerResponseTypeDef,
 )
 
 
-def get_structure() -> AccountAttributeTypeDef:
+def get_value() -> AccountAttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-opsworkscm-2.5.2/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt` & `types-aiobotocore-opsworkscm-2.5.2.post1/types_aiobotocore_opsworkscm.egg-info/SOURCES.txt`

 * *Files identical despite different names*


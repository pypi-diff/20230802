# Comparing `tmp/types-aiobotocore-cloudhsmv2-2.5.2.tar.gz` & `tmp/types-aiobotocore-cloudhsmv2-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.5.2.tar", last modified: Sat Jul  8 01:43:21 2023, max compression
+gzip compressed data, was "types-aiobotocore-cloudhsmv2-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:00 2023, max compression
```

## Comparing `types-aiobotocore-cloudhsmv2-2.5.2.tar` & `types-aiobotocore-cloudhsmv2-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.569826 types-aiobotocore-cloudhsmv2-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:43:21.565826 types-aiobotocore-cloudhsmv2-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13248 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:21.569826 types-aiobotocore-cloudhsmv2-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.557826 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13065 2023-07-08 01:27:09.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:27:08.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:21.565826 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-08 01:43:21.000000 types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13231 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14707 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14680 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9010 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13048 2023-08-02 14:34:41.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13031 2023-08-02 14:34:41.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:34:40.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:00.145636 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 14:51:59.000000 types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/LICENSE` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudhsmv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudhsmv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsmv2"></a>
 
 # types-aiobotocore-cloudhsmv2
 
 [![PyPI - types-aiobotocore-cloudhsmv2](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsmv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsmv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsmv2)](https://pepy.tech/project/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudHSMV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
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
@@ -320,67 +319,67 @@
 )
 
 
 def check_value(value: BackupPolicyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudhsmv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudhsmv2.type_defs import (
     BackupRetentionPolicyTypeDef,
     TagTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
     DestinationBackupTypeDef,
+    ResponseMetadataTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
     InitializeClusterRequestRequestTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     ModifyBackupAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
     CopyBackupToRegionRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ClusterTypeDef,
-    CreateHsmResponseTypeDef,
     CopyBackupToRegionResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    InitializeClusterResponseTypeDef,
+    ListTagsResponseTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyTypeDef:
+def get_value() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/README.md` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-cloudhsmv2"></a>
 
 # types-aiobotocore-cloudhsmv2
 
 [![PyPI - types-aiobotocore-cloudhsmv2](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsmv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsmv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsmv2)](https://pepy.tech/project/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudHSMV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
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
@@ -287,67 +287,67 @@
 )
 
 
 def check_value(value: BackupPolicyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudhsmv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudhsmv2.type_defs import (
     BackupRetentionPolicyTypeDef,
     TagTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
     DestinationBackupTypeDef,
+    ResponseMetadataTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
     InitializeClusterRequestRequestTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     ModifyBackupAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
     CopyBackupToRegionRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ClusterTypeDef,
-    CreateHsmResponseTypeDef,
     CopyBackupToRegionResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    InitializeClusterResponseTypeDef,
+    ListTagsResponseTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyTypeDef:
+def get_value() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/setup.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-cloudhsmv2",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_cloudhsmv2"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with"
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
-    keywords="aiobotocore cloudhsmv2 type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore cloudhsmv2 type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_cloudhsmv2": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/"
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__init__.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/__main__.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.CloudHSMV2 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.CloudHSMV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2\nOther"
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

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/client.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/literals.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         SortAscending: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describebackupspaginator)
         """
 
 
@@ -74,28 +74,28 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
         """
 
 
 class ListTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#listtagspaginator)
         """
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/paginator.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
         SortAscending: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeBackupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeBackups.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describebackupspaginator)
         """
 
 class DescribeClustersPaginator(AioPaginator):
@@ -70,27 +70,27 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
     """
 
     def paginate(
         self,
         *,
         Filters: Mapping[str, Sequence[str]] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeClustersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.DescribeClusters.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#describeclusterspaginator)
         """
 
 class ListTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#listtagspaginator)
     """
 
     def paginate(
-        self, *, ResourceId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2.Paginator.ListTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/paginators/#listtagspaginator)
         """
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.py` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
 
-    data: BackupRetentionPolicyTypeDef = {...}
+    data: BackupRetentionPolicyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import BackupStateType, ClusterStateType, HsmStateType
@@ -22,48 +22,47 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BackupRetentionPolicyTypeDef",
     "TagTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
     "DestinationBackupTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "InitializeClusterRequestRequestTypeDef",
-    "InitializeClusterResponseTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ModifyBackupAttributesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreBackupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ModifyClusterRequestRequestTypeDef",
     "BackupTypeDef",
     "CopyBackupToRegionRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ClusterTypeDef",
-    "CreateHsmResponseTypeDef",
     "CopyBackupToRegionResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "InitializeClusterResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "DeleteBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "ModifyBackupAttributesResponseTypeDef",
     "RestoreBackupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
@@ -115,30 +114,39 @@
         "EniIp": str,
         "State": HsmStateType,
         "StateMessage": str,
     },
     total=False,
 )
 
-
 class HsmTypeDef(_RequiredHsmTypeDef, _OptionalHsmTypeDef):
     pass
 
-
 DestinationBackupTypeDef = TypedDict(
     "DestinationBackupTypeDef",
     {
         "CreateTimestamp": datetime,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
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
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "ClusterId": str,
         "AvailabilityZone": str,
     },
 )
@@ -146,21 +154,19 @@
     "_OptionalCreateHsmRequestRequestTypeDef",
     {
         "IpAddress": str,
     },
     total=False,
 )
 
-
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
-
 DeleteBackupRequestRequestTypeDef = TypedDict(
     "DeleteBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -183,35 +189,25 @@
         "HsmId": str,
         "EniId": str,
         "EniIp": str,
     },
     total=False,
 )
 
-
 class DeleteHsmRequestRequestTypeDef(
     _RequiredDeleteHsmRequestRequestTypeDef, _OptionalDeleteHsmRequestRequestTypeDef
 ):
     pass
 
-
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "HsmId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filters": Mapping[str, Sequence[str]],
-        "SortAscending": bool,
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
@@ -219,23 +215,14 @@
         "MaxResults": int,
         "Filters": Mapping[str, Sequence[str]],
         "SortAscending": bool,
     },
     total=False,
 )
 
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "Filters": Mapping[str, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -247,44 +234,14 @@
     {
         "ClusterId": str,
         "SignedCert": str,
         "TrustAnchor": str,
     },
 )
 
-InitializeClusterResponseTypeDef = TypedDict(
-    "InitializeClusterResponseTypeDef",
-    {
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -292,50 +249,27 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
-
 ModifyBackupAttributesRequestRequestTypeDef = TypedDict(
     "ModifyBackupAttributesRequestRequestTypeDef",
     {
         "BackupId": str,
         "NeverExpires": bool,
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
 RestoreBackupRequestRequestTypeDef = TypedDict(
     "RestoreBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -374,19 +308,17 @@
         "SourceCluster": str,
         "DeleteTimestamp": datetime,
         "TagList": List[TagTypeDef],
     },
     total=False,
 )
 
-
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
-
 _RequiredCopyBackupToRegionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupToRegionRequestRequestTypeDef",
     {
         "DestinationRegion": str,
         "BackupId": str,
     },
 )
@@ -394,22 +326,20 @@
     "_OptionalCopyBackupToRegionRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CopyBackupToRegionRequestRequestTypeDef(
     _RequiredCopyBackupToRegionRequestRequestTypeDef,
     _OptionalCopyBackupToRegionRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "HsmType": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -419,30 +349,19 @@
         "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
         "SourceBackupId": str,
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagList": Sequence[TagTypeDef],
     },
 )
@@ -465,88 +384,152 @@
         "VpcId": str,
         "Certificates": CertificatesTypeDef,
         "TagList": List[TagTypeDef],
     },
     total=False,
 )
 
+CopyBackupToRegionResponseTypeDef = TypedDict(
+    "CopyBackupToRegionResponseTypeDef",
+    {
+        "DestinationBackup": DestinationBackupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateHsmResponseTypeDef = TypedDict(
     "CreateHsmResponseTypeDef",
     {
         "Hsm": HsmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopyBackupToRegionResponseTypeDef = TypedDict(
-    "CopyBackupToRegionResponseTypeDef",
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
     {
-        "DestinationBackup": DestinationBackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HsmId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitializeClusterResponseTypeDef = TypedDict(
+    "InitializeClusterResponseTypeDef",
+    {
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "SortAscending": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceId": str,
+    },
+)
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
 DeleteBackupResponseTypeDef = TypedDict(
     "DeleteBackupResponseTypeDef",
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
 
 ModifyBackupAttributesResponseTypeDef = TypedDict(
     "ModifyBackupAttributesResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreBackupResponseTypeDef = TypedDict(
     "RestoreBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResponseTypeDef = TypedDict(
     "ModifyClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2/type_defs.pyi` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_cloudhsmv2.type_defs import BackupRetentionPolicyTypeDef
 
-    data: BackupRetentionPolicyTypeDef = {...}
+    data: BackupRetentionPolicyTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence
 
 from .literals import BackupStateType, ClusterStateType, HsmStateType
@@ -22,47 +22,48 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BackupRetentionPolicyTypeDef",
     "TagTypeDef",
     "CertificatesTypeDef",
     "HsmTypeDef",
     "DestinationBackupTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateHsmRequestRequestTypeDef",
     "DeleteBackupRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteHsmRequestRequestTypeDef",
-    "DeleteHsmResponseTypeDef",
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeBackupsRequestRequestTypeDef",
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
     "DescribeClustersRequestRequestTypeDef",
     "InitializeClusterRequestRequestTypeDef",
-    "InitializeClusterResponseTypeDef",
-    "ListTagsRequestListTagsPaginateTypeDef",
     "ListTagsRequestRequestTypeDef",
     "ModifyBackupAttributesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreBackupRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "ModifyClusterRequestRequestTypeDef",
     "BackupTypeDef",
     "CopyBackupToRegionRequestRequestTypeDef",
     "CreateClusterRequestRequestTypeDef",
-    "ListTagsResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ClusterTypeDef",
-    "CreateHsmResponseTypeDef",
     "CopyBackupToRegionResponseTypeDef",
+    "CreateHsmResponseTypeDef",
+    "DeleteHsmResponseTypeDef",
+    "InitializeClusterResponseTypeDef",
+    "ListTagsResponseTypeDef",
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    "ListTagsRequestListTagsPaginateTypeDef",
     "DeleteBackupResponseTypeDef",
     "DescribeBackupsResponseTypeDef",
     "ModifyBackupAttributesResponseTypeDef",
     "RestoreBackupResponseTypeDef",
     "CreateClusterResponseTypeDef",
     "DeleteClusterResponseTypeDef",
     "DescribeClustersResponseTypeDef",
@@ -114,28 +115,41 @@
         "EniIp": str,
         "State": HsmStateType,
         "StateMessage": str,
     },
     total=False,
 )
 
+
 class HsmTypeDef(_RequiredHsmTypeDef, _OptionalHsmTypeDef):
     pass
 
+
 DestinationBackupTypeDef = TypedDict(
     "DestinationBackupTypeDef",
     {
         "CreateTimestamp": datetime,
         "SourceRegion": str,
         "SourceBackup": str,
         "SourceCluster": str,
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
 _RequiredCreateHsmRequestRequestTypeDef = TypedDict(
     "_RequiredCreateHsmRequestRequestTypeDef",
     {
         "ClusterId": str,
         "AvailabilityZone": str,
     },
 )
@@ -143,19 +157,21 @@
     "_OptionalCreateHsmRequestRequestTypeDef",
     {
         "IpAddress": str,
     },
     total=False,
 )
 
+
 class CreateHsmRequestRequestTypeDef(
     _RequiredCreateHsmRequestRequestTypeDef, _OptionalCreateHsmRequestRequestTypeDef
 ):
     pass
 
+
 DeleteBackupRequestRequestTypeDef = TypedDict(
     "DeleteBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -178,33 +194,27 @@
         "HsmId": str,
         "EniId": str,
         "EniIp": str,
     },
     total=False,
 )
 
+
 class DeleteHsmRequestRequestTypeDef(
     _RequiredDeleteHsmRequestRequestTypeDef, _OptionalDeleteHsmRequestRequestTypeDef
 ):
     pass
 
-DeleteHsmResponseTypeDef = TypedDict(
-    "DeleteHsmResponseTypeDef",
-    {
-        "HsmId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
-    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Filters": Mapping[str, Sequence[str]],
-        "SortAscending": bool,
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
@@ -212,23 +222,14 @@
         "MaxResults": int,
         "Filters": Mapping[str, Sequence[str]],
         "SortAscending": bool,
     },
     total=False,
 )
 
-DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
-    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
-    {
-        "Filters": Mapping[str, Sequence[str]],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeClustersRequestRequestTypeDef = TypedDict(
     "DescribeClustersRequestRequestTypeDef",
     {
         "Filters": Mapping[str, Sequence[str]],
         "NextToken": str,
         "MaxResults": int,
     },
@@ -240,42 +241,14 @@
     {
         "ClusterId": str,
         "SignedCert": str,
         "TrustAnchor": str,
     },
 )
 
-InitializeClusterResponseTypeDef = TypedDict(
-    "InitializeClusterResponseTypeDef",
-    {
-        "State": ClusterStateType,
-        "StateMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_RequiredListTagsRequestListTagsPaginateTypeDef",
-    {
-        "ResourceId": str,
-    },
-)
-_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
-    "_OptionalListTagsRequestListTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsRequestListTagsPaginateTypeDef(
-    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
-):
-    pass
-
 _RequiredListTagsRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsRequestRequestTypeDef",
     {
         "ResourceId": str,
     },
 )
 _OptionalListTagsRequestRequestTypeDef = TypedDict(
@@ -283,48 +256,29 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
+
 class ListTagsRequestRequestTypeDef(
     _RequiredListTagsRequestRequestTypeDef, _OptionalListTagsRequestRequestTypeDef
 ):
     pass
 
+
 ModifyBackupAttributesRequestRequestTypeDef = TypedDict(
     "ModifyBackupAttributesRequestRequestTypeDef",
     {
         "BackupId": str,
         "NeverExpires": bool,
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
 RestoreBackupRequestRequestTypeDef = TypedDict(
     "RestoreBackupRequestRequestTypeDef",
     {
         "BackupId": str,
     },
 )
 
@@ -363,17 +317,19 @@
         "SourceCluster": str,
         "DeleteTimestamp": datetime,
         "TagList": List[TagTypeDef],
     },
     total=False,
 )
 
+
 class BackupTypeDef(_RequiredBackupTypeDef, _OptionalBackupTypeDef):
     pass
 
+
 _RequiredCopyBackupToRegionRequestRequestTypeDef = TypedDict(
     "_RequiredCopyBackupToRegionRequestRequestTypeDef",
     {
         "DestinationRegion": str,
         "BackupId": str,
     },
 )
@@ -381,20 +337,22 @@
     "_OptionalCopyBackupToRegionRequestRequestTypeDef",
     {
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CopyBackupToRegionRequestRequestTypeDef(
     _RequiredCopyBackupToRegionRequestRequestTypeDef,
     _OptionalCopyBackupToRegionRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateClusterRequestRequestTypeDef = TypedDict(
     "_RequiredCreateClusterRequestRequestTypeDef",
     {
         "HsmType": str,
         "SubnetIds": Sequence[str],
     },
 )
@@ -404,27 +362,20 @@
         "BackupRetentionPolicy": BackupRetentionPolicyTypeDef,
         "SourceBackupId": str,
         "TagList": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateClusterRequestRequestTypeDef(
     _RequiredCreateClusterRequestRequestTypeDef, _OptionalCreateClusterRequestRequestTypeDef
 ):
     pass
 
-ListTagsResponseTypeDef = TypedDict(
-    "ListTagsResponseTypeDef",
-    {
-        "TagList": List[TagTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagList": Sequence[TagTypeDef],
     },
@@ -448,88 +399,154 @@
         "VpcId": str,
         "Certificates": CertificatesTypeDef,
         "TagList": List[TagTypeDef],
     },
     total=False,
 )
 
+CopyBackupToRegionResponseTypeDef = TypedDict(
+    "CopyBackupToRegionResponseTypeDef",
+    {
+        "DestinationBackup": DestinationBackupTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateHsmResponseTypeDef = TypedDict(
     "CreateHsmResponseTypeDef",
     {
         "Hsm": HsmTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-CopyBackupToRegionResponseTypeDef = TypedDict(
-    "CopyBackupToRegionResponseTypeDef",
+DeleteHsmResponseTypeDef = TypedDict(
+    "DeleteHsmResponseTypeDef",
     {
-        "DestinationBackup": DestinationBackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "HsmId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InitializeClusterResponseTypeDef = TypedDict(
+    "InitializeClusterResponseTypeDef",
+    {
+        "State": ClusterStateType,
+        "StateMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsResponseTypeDef = TypedDict(
+    "ListTagsResponseTypeDef",
+    {
+        "TagList": List[TagTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+DescribeBackupsRequestDescribeBackupsPaginateTypeDef = TypedDict(
+    "DescribeBackupsRequestDescribeBackupsPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "SortAscending": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeClustersRequestDescribeClustersPaginateTypeDef = TypedDict(
+    "DescribeClustersRequestDescribeClustersPaginateTypeDef",
+    {
+        "Filters": Mapping[str, Sequence[str]],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_RequiredListTagsRequestListTagsPaginateTypeDef",
+    {
+        "ResourceId": str,
     },
 )
+_OptionalListTagsRequestListTagsPaginateTypeDef = TypedDict(
+    "_OptionalListTagsRequestListTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsRequestListTagsPaginateTypeDef(
+    _RequiredListTagsRequestListTagsPaginateTypeDef, _OptionalListTagsRequestListTagsPaginateTypeDef
+):
+    pass
+
 
 DeleteBackupResponseTypeDef = TypedDict(
     "DeleteBackupResponseTypeDef",
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
 
 ModifyBackupAttributesResponseTypeDef = TypedDict(
     "ModifyBackupAttributesResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RestoreBackupResponseTypeDef = TypedDict(
     "RestoreBackupResponseTypeDef",
     {
         "Backup": BackupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateClusterResponseTypeDef = TypedDict(
     "CreateClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DeleteClusterResponseTypeDef = TypedDict(
     "DeleteClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeClustersResponseTypeDef = TypedDict(
     "DescribeClustersResponseTypeDef",
     {
         "Clusters": List[ClusterTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ModifyClusterResponseTypeDef = TypedDict(
     "ModifyClusterResponseTypeDef",
     {
         "Cluster": ClusterTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-cloudhsmv2
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.CloudHSMV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore cloudhsmv2 type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore cloudhsmv2 type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-cloudhsmv2"></a>
 
 # types-aiobotocore-cloudhsmv2
 
 [![PyPI - types-aiobotocore-cloudhsmv2](https://img.shields.io/pypi/v/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-cloudhsmv2.svg?color=blue)](https://pypi.org/project/types-aiobotocore-cloudhsmv2)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-cloudhsmv2?color=blue)](https://pypistats.org/packages/types-aiobotocore-cloudhsmv2)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-cloudhsmv2)](https://pepy.tech/project/types-aiobotocore-cloudhsmv2)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.CloudHSMV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cloudhsmv2.html#CloudHSMV2)
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
 [types-aiobotocore-cloudhsmv2 docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_cloudhsmv2/).
 
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
@@ -320,67 +319,67 @@
 )
 
 
 def check_value(value: BackupPolicyType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_cloudhsmv2.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_cloudhsmv2.type_defs import (
     BackupRetentionPolicyTypeDef,
     TagTypeDef,
     CertificatesTypeDef,
     HsmTypeDef,
     DestinationBackupTypeDef,
+    ResponseMetadataTypeDef,
     CreateHsmRequestRequestTypeDef,
     DeleteBackupRequestRequestTypeDef,
     DeleteClusterRequestRequestTypeDef,
     DeleteHsmRequestRequestTypeDef,
-    DeleteHsmResponseTypeDef,
-    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeBackupsRequestRequestTypeDef,
-    DescribeClustersRequestDescribeClustersPaginateTypeDef,
     DescribeClustersRequestRequestTypeDef,
     InitializeClusterRequestRequestTypeDef,
-    InitializeClusterResponseTypeDef,
-    ListTagsRequestListTagsPaginateTypeDef,
     ListTagsRequestRequestTypeDef,
     ModifyBackupAttributesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
     RestoreBackupRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     ModifyClusterRequestRequestTypeDef,
     BackupTypeDef,
     CopyBackupToRegionRequestRequestTypeDef,
     CreateClusterRequestRequestTypeDef,
-    ListTagsResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ClusterTypeDef,
-    CreateHsmResponseTypeDef,
     CopyBackupToRegionResponseTypeDef,
+    CreateHsmResponseTypeDef,
+    DeleteHsmResponseTypeDef,
+    InitializeClusterResponseTypeDef,
+    ListTagsResponseTypeDef,
+    DescribeBackupsRequestDescribeBackupsPaginateTypeDef,
+    DescribeClustersRequestDescribeClustersPaginateTypeDef,
+    ListTagsRequestListTagsPaginateTypeDef,
     DeleteBackupResponseTypeDef,
     DescribeBackupsResponseTypeDef,
     ModifyBackupAttributesResponseTypeDef,
     RestoreBackupResponseTypeDef,
     CreateClusterResponseTypeDef,
     DeleteClusterResponseTypeDef,
     DescribeClustersResponseTypeDef,
     ModifyClusterResponseTypeDef,
 )
 
 
-def get_structure() -> BackupRetentionPolicyTypeDef:
+def get_value() -> BackupRetentionPolicyTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-cloudhsmv2-2.5.2/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt` & `types-aiobotocore-cloudhsmv2-2.5.2.post1/types_aiobotocore_cloudhsmv2.egg-info/SOURCES.txt`

 * *Files identical despite different names*


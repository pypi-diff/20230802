# Comparing `tmp/types-aiobotocore-secretsmanager-2.5.2.tar.gz` & `tmp/types-aiobotocore-secretsmanager-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-secretsmanager-2.5.2.tar", last modified: Sat Jul  8 01:44:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-secretsmanager-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
```

## Comparing `types-aiobotocore-secretsmanager-2.5.2.tar` & `types-aiobotocore-secretsmanager-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.874877 types-aiobotocore-secretsmanager-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-07-08 01:44:17.874877 types-aiobotocore-secretsmanager-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:17.874877 types-aiobotocore-secretsmanager-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.874877 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20417 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20385 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19664 2023-07-08 01:40:31.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19641 2023-07-08 01:40:31.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:30.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.874877 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-07-08 01:44:17.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 01:44:17.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:17.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-08 01:44:17.000000 types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13726 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-02 14:49:08.000000 types-aiobotocore-secretsmanager-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.361462 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20286 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20254 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8579 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    19547 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19524 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:09.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.365462 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15272 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-08-02 14:52:59.000000 types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/LICENSE` & `types-aiobotocore-secretsmanager-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2/PKG-INFO` & `types-aiobotocore-secretsmanager-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore secretsmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore secretsmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-secretsmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-secretsmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecretsManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
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
@@ -308,81 +307,82 @@
 )
 
 
 def check_value(value: FilterNameStringTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_secretsmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_secretsmanager.type_defs import (
+    BlobTypeDef,
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
+    ResponseMetadataTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
     ReplicationStatusTypeTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseTypeDef,
     DescribeSecretRequestRequestTypeDef,
     RotationRulesTypeTypeDef,
-    EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
     SecretVersionsListEntryTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
     ValidationErrorsEntryTypeDef,
+    PutSecretValueRequestRequestTypeDef,
+    UpdateSecretRequestRequestTypeDef,
+    CancelRotateSecretResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteSecretResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRandomPasswordResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSecretValueResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSecretValueResponseTypeDef,
+    RestoreSecretResponseTypeDef,
+    RotateSecretResponseTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
+    UpdateSecretResponseTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecretResponseTypeDef,
     RemoveRegionsFromReplicationResponseTypeDef,
     ReplicateSecretToRegionsResponseTypeDef,
     DescribeSecretResponseTypeDef,
     RotateSecretRequestRequestTypeDef,
     SecretListEntryTypeDef,
-    ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
     ListSecretVersionIdsResponseTypeDef,
+    ListSecretsRequestListSecretsPaginateTypeDef,
     ValidateResourcePolicyResponseTypeDef,
     ListSecretsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/README.md` & `types-aiobotocore-secretsmanager-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-secretsmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-secretsmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecretsManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
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
@@ -275,81 +275,82 @@
 )
 
 
 def check_value(value: FilterNameStringTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_secretsmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_secretsmanager.type_defs import (
+    BlobTypeDef,
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
+    ResponseMetadataTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
     ReplicationStatusTypeTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseTypeDef,
     DescribeSecretRequestRequestTypeDef,
     RotationRulesTypeTypeDef,
-    EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
     SecretVersionsListEntryTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
     ValidationErrorsEntryTypeDef,
+    PutSecretValueRequestRequestTypeDef,
+    UpdateSecretRequestRequestTypeDef,
+    CancelRotateSecretResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteSecretResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRandomPasswordResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSecretValueResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSecretValueResponseTypeDef,
+    RestoreSecretResponseTypeDef,
+    RotateSecretResponseTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
+    UpdateSecretResponseTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecretResponseTypeDef,
     RemoveRegionsFromReplicationResponseTypeDef,
     ReplicateSecretToRegionsResponseTypeDef,
     DescribeSecretResponseTypeDef,
     RotateSecretRequestRequestTypeDef,
     SecretListEntryTypeDef,
-    ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
     ListSecretVersionIdsResponseTypeDef,
+    ListSecretsRequestListSecretsPaginateTypeDef,
     ValidateResourcePolicyResponseTypeDef,
     ListSecretsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/setup.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-secretsmanager",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_secretsmanager"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with"
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
-    keywords="aiobotocore secretsmanager type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore secretsmanager type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_secretsmanager": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/"
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/__init__.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/__init__.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/__main__.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SecretsManager 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SecretsManager 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager\nOther"
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

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/client.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
     session = get_session()
     async with session.create_client("secretsmanager") as client:
         client: SecretsManagerClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import SortOrderTypeType
 from .paginator import ListSecretsPaginator
 from .type_defs import (
+    BlobTypeDef,
     CancelRotateSecretResponseTypeDef,
     CreateSecretResponseTypeDef,
     DeleteResourcePolicyResponseTypeDef,
     DeleteSecretResponseTypeDef,
     DescribeSecretResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
@@ -129,15 +129,15 @@
     async def create_secret(
         self,
         *,
         Name: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
-        SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
         ForceOverwriteReplicaSecret: bool = ...
     ) -> CreateSecretResponseTypeDef:
         """
         Creates a new secret.
@@ -272,15 +272,15 @@
         """
 
     async def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
-        SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
         VersionStages: Sequence[str] = ...
     ) -> PutSecretValueResponseTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
@@ -372,15 +372,15 @@
     async def update_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
-        SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...
     ) -> UpdateSecretResponseTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#update_secret)
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/client.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,23 +11,23 @@
 
     session = get_session()
     async with session.create_client("secretsmanager") as client:
         client: SecretsManagerClient
     ```
 """
 import sys
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .literals import SortOrderTypeType
 from .paginator import ListSecretsPaginator
 from .type_defs import (
+    BlobTypeDef,
     CancelRotateSecretResponseTypeDef,
     CreateSecretResponseTypeDef,
     DeleteResourcePolicyResponseTypeDef,
     DeleteSecretResponseTypeDef,
     DescribeSecretResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     FilterTypeDef,
@@ -121,15 +121,15 @@
     async def create_secret(
         self,
         *,
         Name: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
-        SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         AddReplicaRegions: Sequence[ReplicaRegionTypeTypeDef] = ...,
         ForceOverwriteReplicaSecret: bool = ...
     ) -> CreateSecretResponseTypeDef:
         """
         Creates a new secret.
@@ -253,15 +253,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#put_resource_policy)
         """
     async def put_secret_value(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
-        SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...,
         VersionStages: Sequence[str] = ...
     ) -> PutSecretValueResponseTypeDef:
         """
         Creates a new version with a new encrypted secret value and attaches it to the
         secret.
 
@@ -345,15 +345,15 @@
     async def update_secret(
         self,
         *,
         SecretId: str,
         ClientRequestToken: str = ...,
         Description: str = ...,
         KmsKeyId: str = ...,
-        SecretBinary: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        SecretBinary: BlobTypeDef = ...,
         SecretString: str = ...
     ) -> UpdateSecretResponseTypeDef:
         """
         Modifies the details of a secret, including metadata and the secret value.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Client.update_secret)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/client/#update_secret)
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/literals.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/literals.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/paginator.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,13 +49,13 @@
 
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/paginator.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -46,13 +46,13 @@
 
     def paginate(
         self,
         *,
         IncludePlannedDeletion: bool = ...,
         Filters: Sequence[FilterTypeDef] = ...,
         SortOrder: SortOrderTypeType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSecretsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager.Paginator.ListSecrets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/paginators/#listsecretspaginator)
         """
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/type_defs.py` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for secretsmanager service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_secretsmanager.type_defs import CancelRotateSecretRequestRequestTypeDef
+    from types_aiobotocore_secretsmanager.type_defs import BlobTypeDef
 
-    data: CancelRotateSecretRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -20,86 +20,88 @@
 from .literals import FilterNameStringTypeType, SortOrderTypeType, StatusTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "BlobTypeDef",
     "CancelRotateSecretRequestRequestTypeDef",
-    "CancelRotateSecretResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ReplicaRegionTypeTypeDef",
     "TagTypeDef",
     "ReplicationStatusTypeTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
     "DeleteSecretRequestRequestTypeDef",
-    "DeleteSecretResponseTypeDef",
     "DescribeSecretRequestRequestTypeDef",
     "RotationRulesTypeTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FilterTypeDef",
     "GetRandomPasswordRequestRequestTypeDef",
-    "GetRandomPasswordResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetSecretValueRequestRequestTypeDef",
-    "GetSecretValueResponseTypeDef",
     "ListSecretVersionIdsRequestRequestTypeDef",
     "SecretVersionsListEntryTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "PutSecretValueRequestRequestTypeDef",
-    "PutSecretValueResponseTypeDef",
     "RemoveRegionsFromReplicationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreSecretRequestRequestTypeDef",
-    "RestoreSecretResponseTypeDef",
-    "RotateSecretResponseTypeDef",
     "StopReplicationToReplicaRequestRequestTypeDef",
-    "StopReplicationToReplicaResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateSecretRequestRequestTypeDef",
-    "UpdateSecretResponseTypeDef",
     "UpdateSecretVersionStageRequestRequestTypeDef",
-    "UpdateSecretVersionStageResponseTypeDef",
     "ValidateResourcePolicyRequestRequestTypeDef",
     "ValidationErrorsEntryTypeDef",
+    "PutSecretValueRequestRequestTypeDef",
+    "UpdateSecretRequestRequestTypeDef",
+    "CancelRotateSecretResponseTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteSecretResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetRandomPasswordResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetSecretValueResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "PutSecretValueResponseTypeDef",
+    "RestoreSecretResponseTypeDef",
+    "RotateSecretResponseTypeDef",
+    "StopReplicationToReplicaResponseTypeDef",
+    "UpdateSecretResponseTypeDef",
+    "UpdateSecretVersionStageResponseTypeDef",
     "ReplicateSecretToRegionsRequestRequestTypeDef",
     "CreateSecretRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSecretResponseTypeDef",
     "RemoveRegionsFromReplicationResponseTypeDef",
     "ReplicateSecretToRegionsResponseTypeDef",
     "DescribeSecretResponseTypeDef",
     "RotateSecretRequestRequestTypeDef",
     "SecretListEntryTypeDef",
-    "ListSecretsRequestListSecretsPaginateTypeDef",
     "ListSecretsRequestRequestTypeDef",
     "ListSecretVersionIdsResponseTypeDef",
+    "ListSecretsRequestListSecretsPaginateTypeDef",
     "ValidateResourcePolicyResponseTypeDef",
     "ListSecretsResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelRotateSecretRequestRequestTypeDef = TypedDict(
     "CancelRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-CancelRotateSecretResponseTypeDef = TypedDict(
-    "CancelRotateSecretResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ReplicaRegionTypeTypeDef = TypedDict(
     "ReplicaRegionTypeTypeDef",
     {
         "Region": str,
@@ -132,23 +134,14 @@
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteSecretRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalDeleteSecretRequestRequestTypeDef = TypedDict(
@@ -156,31 +149,19 @@
     {
         "RecoveryWindowInDays": int,
         "ForceDeleteWithoutRecovery": bool,
     },
     total=False,
 )
 
-
 class DeleteSecretRequestRequestTypeDef(
     _RequiredDeleteSecretRequestRequestTypeDef, _OptionalDeleteSecretRequestRequestTypeDef
 ):
     pass
 
-
-DeleteSecretResponseTypeDef = TypedDict(
-    "DeleteSecretResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "DeletionDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DescribeSecretRequestRequestTypeDef = TypedDict(
     "DescribeSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
@@ -190,21 +171,14 @@
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": FilterNameStringTypeType,
         "Values": Sequence[str],
     },
     total=False,
@@ -221,39 +195,21 @@
         "ExcludeLowercase": bool,
         "IncludeSpace": bool,
         "RequireEachIncludedType": bool,
     },
     total=False,
 )
 
-GetRandomPasswordResponseTypeDef = TypedDict(
-    "GetRandomPasswordResponseTypeDef",
-    {
-        "RandomPassword": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSecretValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetSecretValueRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalGetSecretValueRequestRequestTypeDef = TypedDict(
@@ -261,35 +217,19 @@
     {
         "VersionId": str,
         "VersionStage": str,
     },
     total=False,
 )
 
-
 class GetSecretValueRequestRequestTypeDef(
     _RequiredGetSecretValueRequestRequestTypeDef, _OptionalGetSecretValueRequestRequestTypeDef
 ):
     pass
 
-
-GetSecretValueResponseTypeDef = TypedDict(
-    "GetSecretValueResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "SecretBinary": bytes,
-        "SecretString": str,
-        "VersionStages": List[str],
-        "CreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListSecretVersionIdsRequestRequestTypeDef = TypedDict(
     "_RequiredListSecretVersionIdsRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalListSecretVersionIdsRequestRequestTypeDef = TypedDict(
@@ -298,22 +238,20 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeDeprecated": bool,
     },
     total=False,
 )
 
-
 class ListSecretVersionIdsRequestRequestTypeDef(
     _RequiredListSecretVersionIdsRequestRequestTypeDef,
     _OptionalListSecretVersionIdsRequestRequestTypeDef,
 ):
     pass
 
-
 SecretVersionsListEntryTypeDef = TypedDict(
     "SecretVersionsListEntryTypeDef",
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
@@ -343,230 +281,277 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "BlockPublicPolicy": bool,
     },
     total=False,
 )
 
-
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
+RemoveRegionsFromReplicationRequestRequestTypeDef = TypedDict(
+    "RemoveRegionsFromReplicationRequestRequestTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecretId": str,
+        "RemoveReplicaRegions": Sequence[str],
     },
 )
 
-_RequiredPutSecretValueRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSecretValueRequestRequestTypeDef",
+RestoreSecretRequestRequestTypeDef = TypedDict(
+    "RestoreSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
-_OptionalPutSecretValueRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSecretValueRequestRequestTypeDef",
+
+StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
+    "StopReplicationToReplicaRequestRequestTypeDef",
     {
-        "ClientRequestToken": str,
-        "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
-        "SecretString": str,
-        "VersionStages": Sequence[str],
+        "SecretId": str,
     },
-    total=False,
 )
 
-
-class PutSecretValueRequestRequestTypeDef(
-    _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
-):
-    pass
-
-
-PutSecretValueResponseTypeDef = TypedDict(
-    "PutSecretValueResponseTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "VersionStages": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecretId": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-RemoveRegionsFromReplicationRequestRequestTypeDef = TypedDict(
-    "RemoveRegionsFromReplicationRequestRequestTypeDef",
+_RequiredUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecretVersionStageRequestRequestTypeDef",
     {
         "SecretId": str,
-        "RemoveReplicaRegions": Sequence[str],
+        "VersionStage": str,
     },
 )
-
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+_OptionalUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecretVersionStageRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "RemoveFromVersionId": str,
+        "MoveToVersionId": str,
     },
+    total=False,
 )
 
-RestoreSecretRequestRequestTypeDef = TypedDict(
-    "RestoreSecretRequestRequestTypeDef",
+class UpdateSecretVersionStageRequestRequestTypeDef(
+    _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
+    _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
+):
+    pass
+
+_RequiredValidateResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredValidateResourcePolicyRequestRequestTypeDef",
     {
-        "SecretId": str,
+        "ResourcePolicy": str,
     },
 )
-
-RestoreSecretResponseTypeDef = TypedDict(
-    "RestoreSecretResponseTypeDef",
+_OptionalValidateResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalValidateResourcePolicyRequestRequestTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecretId": str,
     },
+    total=False,
 )
 
-RotateSecretResponseTypeDef = TypedDict(
-    "RotateSecretResponseTypeDef",
+class ValidateResourcePolicyRequestRequestTypeDef(
+    _RequiredValidateResourcePolicyRequestRequestTypeDef,
+    _OptionalValidateResourcePolicyRequestRequestTypeDef,
+):
+    pass
+
+ValidationErrorsEntryTypeDef = TypedDict(
+    "ValidationErrorsEntryTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CheckName": str,
+        "ErrorMessage": str,
     },
+    total=False,
 )
 
-StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
-    "StopReplicationToReplicaRequestRequestTypeDef",
+_RequiredPutSecretValueRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSecretValueRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
-
-StopReplicationToReplicaResponseTypeDef = TypedDict(
-    "StopReplicationToReplicaResponseTypeDef",
+_OptionalPutSecretValueRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSecretValueRequestRequestTypeDef",
     {
-        "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ClientRequestToken": str,
+        "SecretBinary": BlobTypeDef,
+        "SecretString": str,
+        "VersionStages": Sequence[str],
     },
+    total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "SecretId": str,
-        "TagKeys": Sequence[str],
-    },
-)
+class PutSecretValueRequestRequestTypeDef(
+    _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
+):
+    pass
 
 _RequiredUpdateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalUpdateSecretRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSecretRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "Description": str,
         "KmsKeyId": str,
-        "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
+        "SecretBinary": BlobTypeDef,
         "SecretString": str,
     },
     total=False,
 )
 
-
 class UpdateSecretRequestRequestTypeDef(
     _RequiredUpdateSecretRequestRequestTypeDef, _OptionalUpdateSecretRequestRequestTypeDef
 ):
     pass
 
-
-UpdateSecretResponseTypeDef = TypedDict(
-    "UpdateSecretResponseTypeDef",
+CancelRotateSecretResponseTypeDef = TypedDict(
+    "CancelRotateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecretVersionStageRequestRequestTypeDef",
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
     {
-        "SecretId": str,
-        "VersionStage": str,
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecretVersionStageRequestRequestTypeDef",
+
+DeleteSecretResponseTypeDef = TypedDict(
+    "DeleteSecretResponseTypeDef",
     {
-        "RemoveFromVersionId": str,
-        "MoveToVersionId": str,
+        "ARN": str,
+        "Name": str,
+        "DeletionDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class UpdateSecretVersionStageRequestRequestTypeDef(
-    _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
-    _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
-):
-    pass
+GetRandomPasswordResponseTypeDef = TypedDict(
+    "GetRandomPasswordResponseTypeDef",
+    {
+        "RandomPassword": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateSecretVersionStageResponseTypeDef = TypedDict(
-    "UpdateSecretVersionStageResponseTypeDef",
+GetSecretValueResponseTypeDef = TypedDict(
+    "GetSecretValueResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "VersionId": str,
+        "SecretBinary": bytes,
+        "SecretString": str,
+        "VersionStages": List[str],
+        "CreatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredValidateResourcePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredValidateResourcePolicyRequestRequestTypeDef",
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "ResourcePolicy": str,
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValidateResourcePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalValidateResourcePolicyRequestRequestTypeDef",
+
+PutSecretValueResponseTypeDef = TypedDict(
+    "PutSecretValueResponseTypeDef",
     {
-        "SecretId": str,
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "VersionStages": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+RestoreSecretResponseTypeDef = TypedDict(
+    "RestoreSecretResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class ValidateResourcePolicyRequestRequestTypeDef(
-    _RequiredValidateResourcePolicyRequestRequestTypeDef,
-    _OptionalValidateResourcePolicyRequestRequestTypeDef,
-):
-    pass
+RotateSecretResponseTypeDef = TypedDict(
+    "RotateSecretResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+StopReplicationToReplicaResponseTypeDef = TypedDict(
+    "StopReplicationToReplicaResponseTypeDef",
+    {
+        "ARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ValidationErrorsEntryTypeDef = TypedDict(
-    "ValidationErrorsEntryTypeDef",
+UpdateSecretResponseTypeDef = TypedDict(
+    "UpdateSecretResponseTypeDef",
     {
-        "CheckName": str,
-        "ErrorMessage": str,
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSecretVersionStageResponseTypeDef = TypedDict(
+    "UpdateSecretVersionStageResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "SecretId": str,
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
@@ -576,50 +561,46 @@
     "_OptionalReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
-
 class ReplicateSecretToRegionsRequestRequestTypeDef(
     _RequiredReplicateSecretToRegionsRequestRequestTypeDef,
     _OptionalReplicateSecretToRegionsRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredCreateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecretRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateSecretRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSecretRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "Description": str,
         "KmsKeyId": str,
-        "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
+        "SecretBinary": BlobTypeDef,
         "SecretString": str,
         "Tags": Sequence[TagTypeDef],
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
-
 class CreateSecretRequestRequestTypeDef(
     _RequiredCreateSecretRequestRequestTypeDef, _OptionalCreateSecretRequestRequestTypeDef
 ):
     pass
 
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "SecretId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -627,33 +608,33 @@
 CreateSecretResponseTypeDef = TypedDict(
     "CreateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveRegionsFromReplicationResponseTypeDef = TypedDict(
     "RemoveRegionsFromReplicationResponseTypeDef",
     {
         "ARN": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicateSecretToRegionsResponseTypeDef = TypedDict(
     "ReplicateSecretToRegionsResponseTypeDef",
     {
         "ARN": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSecretResponseTypeDef = TypedDict(
     "DescribeSecretResponseTypeDef",
     {
         "ARN": str,
@@ -670,15 +651,15 @@
         "NextRotationDate": datetime,
         "Tags": List[TagTypeDef],
         "VersionIdsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
@@ -691,21 +672,19 @@
         "RotationLambdaARN": str,
         "RotationRules": RotationRulesTypeTypeDef,
         "RotateImmediately": bool,
     },
     total=False,
 )
 
-
 class RotateSecretRequestRequestTypeDef(
     _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
 ):
     pass
 
-
 SecretListEntryTypeDef = TypedDict(
     "SecretListEntryTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
@@ -722,25 +701,14 @@
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
     },
     total=False,
 )
 
-ListSecretsRequestListSecretsPaginateTypeDef = TypedDict(
-    "ListSecretsRequestListSecretsPaginateTypeDef",
-    {
-        "IncludePlannedDeletion": bool,
-        "Filters": Sequence[FilterTypeDef],
-        "SortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecretsRequestRequestTypeDef = TypedDict(
     "ListSecretsRequestRequestTypeDef",
     {
         "IncludePlannedDeletion": bool,
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -752,28 +720,39 @@
 ListSecretVersionIdsResponseTypeDef = TypedDict(
     "ListSecretVersionIdsResponseTypeDef",
     {
         "Versions": List[SecretVersionsListEntryTypeDef],
         "NextToken": str,
         "ARN": str,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListSecretsRequestListSecretsPaginateTypeDef = TypedDict(
+    "ListSecretsRequestListSecretsPaginateTypeDef",
+    {
+        "IncludePlannedDeletion": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "SortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ValidateResourcePolicyResponseTypeDef = TypedDict(
     "ValidateResourcePolicyResponseTypeDef",
     {
         "PolicyValidationPassed": bool,
         "ValidationErrors": List[ValidationErrorsEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecretsResponseTypeDef = TypedDict(
     "ListSecretsResponseTypeDef",
     {
         "SecretList": List[SecretListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager/type_defs.pyi` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for secretsmanager service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_secretsmanager.type_defs import CancelRotateSecretRequestRequestTypeDef
+    from types_aiobotocore_secretsmanager.type_defs import BlobTypeDef
 
-    data: CancelRotateSecretRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -20,85 +20,89 @@
 from .literals import FilterNameStringTypeType, SortOrderTypeType, StatusTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "BlobTypeDef",
     "CancelRotateSecretRequestRequestTypeDef",
-    "CancelRotateSecretResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ReplicaRegionTypeTypeDef",
     "TagTypeDef",
     "ReplicationStatusTypeTypeDef",
     "DeleteResourcePolicyRequestRequestTypeDef",
-    "DeleteResourcePolicyResponseTypeDef",
     "DeleteSecretRequestRequestTypeDef",
-    "DeleteSecretResponseTypeDef",
     "DescribeSecretRequestRequestTypeDef",
     "RotationRulesTypeTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FilterTypeDef",
     "GetRandomPasswordRequestRequestTypeDef",
-    "GetRandomPasswordResponseTypeDef",
     "GetResourcePolicyRequestRequestTypeDef",
-    "GetResourcePolicyResponseTypeDef",
     "GetSecretValueRequestRequestTypeDef",
-    "GetSecretValueResponseTypeDef",
     "ListSecretVersionIdsRequestRequestTypeDef",
     "SecretVersionsListEntryTypeDef",
     "PaginatorConfigTypeDef",
     "PutResourcePolicyRequestRequestTypeDef",
-    "PutResourcePolicyResponseTypeDef",
-    "PutSecretValueRequestRequestTypeDef",
-    "PutSecretValueResponseTypeDef",
     "RemoveRegionsFromReplicationRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "RestoreSecretRequestRequestTypeDef",
-    "RestoreSecretResponseTypeDef",
-    "RotateSecretResponseTypeDef",
     "StopReplicationToReplicaRequestRequestTypeDef",
-    "StopReplicationToReplicaResponseTypeDef",
     "UntagResourceRequestRequestTypeDef",
-    "UpdateSecretRequestRequestTypeDef",
-    "UpdateSecretResponseTypeDef",
     "UpdateSecretVersionStageRequestRequestTypeDef",
-    "UpdateSecretVersionStageResponseTypeDef",
     "ValidateResourcePolicyRequestRequestTypeDef",
     "ValidationErrorsEntryTypeDef",
+    "PutSecretValueRequestRequestTypeDef",
+    "UpdateSecretRequestRequestTypeDef",
+    "CancelRotateSecretResponseTypeDef",
+    "DeleteResourcePolicyResponseTypeDef",
+    "DeleteSecretResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetRandomPasswordResponseTypeDef",
+    "GetResourcePolicyResponseTypeDef",
+    "GetSecretValueResponseTypeDef",
+    "PutResourcePolicyResponseTypeDef",
+    "PutSecretValueResponseTypeDef",
+    "RestoreSecretResponseTypeDef",
+    "RotateSecretResponseTypeDef",
+    "StopReplicationToReplicaResponseTypeDef",
+    "UpdateSecretResponseTypeDef",
+    "UpdateSecretVersionStageResponseTypeDef",
     "ReplicateSecretToRegionsRequestRequestTypeDef",
     "CreateSecretRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateSecretResponseTypeDef",
     "RemoveRegionsFromReplicationResponseTypeDef",
     "ReplicateSecretToRegionsResponseTypeDef",
     "DescribeSecretResponseTypeDef",
     "RotateSecretRequestRequestTypeDef",
     "SecretListEntryTypeDef",
-    "ListSecretsRequestListSecretsPaginateTypeDef",
     "ListSecretsRequestRequestTypeDef",
     "ListSecretVersionIdsResponseTypeDef",
+    "ListSecretsRequestListSecretsPaginateTypeDef",
     "ValidateResourcePolicyResponseTypeDef",
     "ListSecretsResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 CancelRotateSecretRequestRequestTypeDef = TypedDict(
     "CancelRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-CancelRotateSecretResponseTypeDef = TypedDict(
-    "CancelRotateSecretResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 ReplicaRegionTypeTypeDef = TypedDict(
     "ReplicaRegionTypeTypeDef",
     {
         "Region": str,
@@ -131,23 +135,14 @@
 DeleteResourcePolicyRequestRequestTypeDef = TypedDict(
     "DeleteResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-DeleteResourcePolicyResponseTypeDef = TypedDict(
-    "DeleteResourcePolicyResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteSecretRequestRequestTypeDef = TypedDict(
     "_RequiredDeleteSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalDeleteSecretRequestRequestTypeDef = TypedDict(
@@ -155,28 +150,20 @@
     {
         "RecoveryWindowInDays": int,
         "ForceDeleteWithoutRecovery": bool,
     },
     total=False,
 )
 
+
 class DeleteSecretRequestRequestTypeDef(
     _RequiredDeleteSecretRequestRequestTypeDef, _OptionalDeleteSecretRequestRequestTypeDef
 ):
     pass
 
-DeleteSecretResponseTypeDef = TypedDict(
-    "DeleteSecretResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "DeletionDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 DescribeSecretRequestRequestTypeDef = TypedDict(
     "DescribeSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
@@ -187,21 +174,14 @@
         "AutomaticallyAfterDays": int,
         "Duration": str,
         "ScheduleExpression": str,
     },
     total=False,
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "Key": FilterNameStringTypeType,
         "Values": Sequence[str],
     },
     total=False,
@@ -218,39 +198,21 @@
         "ExcludeLowercase": bool,
         "IncludeSpace": bool,
         "RequireEachIncludedType": bool,
     },
     total=False,
 )
 
-GetRandomPasswordResponseTypeDef = TypedDict(
-    "GetRandomPasswordResponseTypeDef",
-    {
-        "RandomPassword": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetResourcePolicyRequestRequestTypeDef = TypedDict(
     "GetResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 
-GetResourcePolicyResponseTypeDef = TypedDict(
-    "GetResourcePolicyResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "ResourcePolicy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetSecretValueRequestRequestTypeDef = TypedDict(
     "_RequiredGetSecretValueRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalGetSecretValueRequestRequestTypeDef = TypedDict(
@@ -258,32 +220,20 @@
     {
         "VersionId": str,
         "VersionStage": str,
     },
     total=False,
 )
 
+
 class GetSecretValueRequestRequestTypeDef(
     _RequiredGetSecretValueRequestRequestTypeDef, _OptionalGetSecretValueRequestRequestTypeDef
 ):
     pass
 
-GetSecretValueResponseTypeDef = TypedDict(
-    "GetSecretValueResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "SecretBinary": bytes,
-        "SecretString": str,
-        "VersionStages": List[str],
-        "CreatedDate": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredListSecretVersionIdsRequestRequestTypeDef = TypedDict(
     "_RequiredListSecretVersionIdsRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
@@ -293,20 +243,22 @@
         "MaxResults": int,
         "NextToken": str,
         "IncludeDeprecated": bool,
     },
     total=False,
 )
 
+
 class ListSecretVersionIdsRequestRequestTypeDef(
     _RequiredListSecretVersionIdsRequestRequestTypeDef,
     _OptionalListSecretVersionIdsRequestRequestTypeDef,
 ):
     pass
 
+
 SecretVersionsListEntryTypeDef = TypedDict(
     "SecretVersionsListEntryTypeDef",
     {
         "VersionId": str,
         "VersionStages": List[str],
         "LastAccessedDate": datetime,
         "CreatedDate": datetime,
@@ -336,220 +288,287 @@
     "_OptionalPutResourcePolicyRequestRequestTypeDef",
     {
         "BlockPublicPolicy": bool,
     },
     total=False,
 )
 
+
 class PutResourcePolicyRequestRequestTypeDef(
     _RequiredPutResourcePolicyRequestRequestTypeDef, _OptionalPutResourcePolicyRequestRequestTypeDef
 ):
     pass
 
-PutResourcePolicyResponseTypeDef = TypedDict(
-    "PutResourcePolicyResponseTypeDef",
-    {
-        "ARN": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-_RequiredPutSecretValueRequestRequestTypeDef = TypedDict(
-    "_RequiredPutSecretValueRequestRequestTypeDef",
+RemoveRegionsFromReplicationRequestRequestTypeDef = TypedDict(
+    "RemoveRegionsFromReplicationRequestRequestTypeDef",
     {
         "SecretId": str,
+        "RemoveReplicaRegions": Sequence[str],
     },
 )
-_OptionalPutSecretValueRequestRequestTypeDef = TypedDict(
-    "_OptionalPutSecretValueRequestRequestTypeDef",
-    {
-        "ClientRequestToken": str,
-        "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
-        "SecretString": str,
-        "VersionStages": Sequence[str],
-    },
-    total=False,
-)
 
-class PutSecretValueRequestRequestTypeDef(
-    _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
-):
-    pass
-
-PutSecretValueResponseTypeDef = TypedDict(
-    "PutSecretValueResponseTypeDef",
+RestoreSecretRequestRequestTypeDef = TypedDict(
+    "RestoreSecretRequestRequestTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "VersionStages": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "SecretId": str,
     },
 )
 
-RemoveRegionsFromReplicationRequestRequestTypeDef = TypedDict(
-    "RemoveRegionsFromReplicationRequestRequestTypeDef",
+StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
+    "StopReplicationToReplicaRequestRequestTypeDef",
     {
         "SecretId": str,
-        "RemoveReplicaRegions": Sequence[str],
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "SecretId": str,
+        "TagKeys": Sequence[str],
     },
 )
 
-RestoreSecretRequestRequestTypeDef = TypedDict(
-    "RestoreSecretRequestRequestTypeDef",
+_RequiredUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
+    "_RequiredUpdateSecretVersionStageRequestRequestTypeDef",
     {
         "SecretId": str,
+        "VersionStage": str,
     },
 )
-
-RestoreSecretResponseTypeDef = TypedDict(
-    "RestoreSecretResponseTypeDef",
+_OptionalUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
+    "_OptionalUpdateSecretVersionStageRequestRequestTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RemoveFromVersionId": str,
+        "MoveToVersionId": str,
     },
+    total=False,
 )
 
-RotateSecretResponseTypeDef = TypedDict(
-    "RotateSecretResponseTypeDef",
+
+class UpdateSecretVersionStageRequestRequestTypeDef(
+    _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
+    _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredValidateResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_RequiredValidateResourcePolicyRequestRequestTypeDef",
     {
-        "ARN": str,
-        "Name": str,
-        "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourcePolicy": str,
     },
 )
-
-StopReplicationToReplicaRequestRequestTypeDef = TypedDict(
-    "StopReplicationToReplicaRequestRequestTypeDef",
+_OptionalValidateResourcePolicyRequestRequestTypeDef = TypedDict(
+    "_OptionalValidateResourcePolicyRequestRequestTypeDef",
     {
         "SecretId": str,
     },
+    total=False,
 )
 
-StopReplicationToReplicaResponseTypeDef = TypedDict(
-    "StopReplicationToReplicaResponseTypeDef",
+
+class ValidateResourcePolicyRequestRequestTypeDef(
+    _RequiredValidateResourcePolicyRequestRequestTypeDef,
+    _OptionalValidateResourcePolicyRequestRequestTypeDef,
+):
+    pass
+
+
+ValidationErrorsEntryTypeDef = TypedDict(
+    "ValidationErrorsEntryTypeDef",
     {
-        "ARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CheckName": str,
+        "ErrorMessage": str,
     },
+    total=False,
 )
 
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
+_RequiredPutSecretValueRequestRequestTypeDef = TypedDict(
+    "_RequiredPutSecretValueRequestRequestTypeDef",
     {
         "SecretId": str,
-        "TagKeys": Sequence[str],
     },
 )
+_OptionalPutSecretValueRequestRequestTypeDef = TypedDict(
+    "_OptionalPutSecretValueRequestRequestTypeDef",
+    {
+        "ClientRequestToken": str,
+        "SecretBinary": BlobTypeDef,
+        "SecretString": str,
+        "VersionStages": Sequence[str],
+    },
+    total=False,
+)
+
+
+class PutSecretValueRequestRequestTypeDef(
+    _RequiredPutSecretValueRequestRequestTypeDef, _OptionalPutSecretValueRequestRequestTypeDef
+):
+    pass
+
 
 _RequiredUpdateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
     },
 )
 _OptionalUpdateSecretRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateSecretRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "Description": str,
         "KmsKeyId": str,
-        "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
+        "SecretBinary": BlobTypeDef,
         "SecretString": str,
     },
     total=False,
 )
 
+
 class UpdateSecretRequestRequestTypeDef(
     _RequiredUpdateSecretRequestRequestTypeDef, _OptionalUpdateSecretRequestRequestTypeDef
 ):
     pass
 
-UpdateSecretResponseTypeDef = TypedDict(
-    "UpdateSecretResponseTypeDef",
+
+CancelRotateSecretResponseTypeDef = TypedDict(
+    "CancelRotateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
-    "_RequiredUpdateSecretVersionStageRequestRequestTypeDef",
+DeleteResourcePolicyResponseTypeDef = TypedDict(
+    "DeleteResourcePolicyResponseTypeDef",
     {
-        "SecretId": str,
-        "VersionStage": str,
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalUpdateSecretVersionStageRequestRequestTypeDef = TypedDict(
-    "_OptionalUpdateSecretVersionStageRequestRequestTypeDef",
+
+DeleteSecretResponseTypeDef = TypedDict(
+    "DeleteSecretResponseTypeDef",
     {
-        "RemoveFromVersionId": str,
-        "MoveToVersionId": str,
+        "ARN": str,
+        "Name": str,
+        "DeletionDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class UpdateSecretVersionStageRequestRequestTypeDef(
-    _RequiredUpdateSecretVersionStageRequestRequestTypeDef,
-    _OptionalUpdateSecretVersionStageRequestRequestTypeDef,
-):
-    pass
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-UpdateSecretVersionStageResponseTypeDef = TypedDict(
-    "UpdateSecretVersionStageResponseTypeDef",
+GetRandomPasswordResponseTypeDef = TypedDict(
+    "GetRandomPasswordResponseTypeDef",
+    {
+        "RandomPassword": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetResourcePolicyResponseTypeDef = TypedDict(
+    "GetResourcePolicyResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResourcePolicy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredValidateResourcePolicyRequestRequestTypeDef = TypedDict(
-    "_RequiredValidateResourcePolicyRequestRequestTypeDef",
+GetSecretValueResponseTypeDef = TypedDict(
+    "GetSecretValueResponseTypeDef",
     {
-        "ResourcePolicy": str,
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "SecretBinary": bytes,
+        "SecretString": str,
+        "VersionStages": List[str],
+        "CreatedDate": datetime,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalValidateResourcePolicyRequestRequestTypeDef = TypedDict(
-    "_OptionalValidateResourcePolicyRequestRequestTypeDef",
+
+PutResourcePolicyResponseTypeDef = TypedDict(
+    "PutResourcePolicyResponseTypeDef",
     {
-        "SecretId": str,
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class ValidateResourcePolicyRequestRequestTypeDef(
-    _RequiredValidateResourcePolicyRequestRequestTypeDef,
-    _OptionalValidateResourcePolicyRequestRequestTypeDef,
-):
-    pass
+PutSecretValueResponseTypeDef = TypedDict(
+    "PutSecretValueResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "VersionStages": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-ValidationErrorsEntryTypeDef = TypedDict(
-    "ValidationErrorsEntryTypeDef",
+RestoreSecretResponseTypeDef = TypedDict(
+    "RestoreSecretResponseTypeDef",
     {
-        "CheckName": str,
-        "ErrorMessage": str,
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RotateSecretResponseTypeDef = TypedDict(
+    "RotateSecretResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopReplicationToReplicaResponseTypeDef = TypedDict(
+    "StopReplicationToReplicaResponseTypeDef",
+    {
+        "ARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSecretResponseTypeDef = TypedDict(
+    "UpdateSecretResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "VersionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateSecretVersionStageResponseTypeDef = TypedDict(
+    "UpdateSecretVersionStageResponseTypeDef",
+    {
+        "ARN": str,
+        "Name": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 _RequiredReplicateSecretToRegionsRequestRequestTypeDef = TypedDict(
     "_RequiredReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "SecretId": str,
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
@@ -559,46 +578,50 @@
     "_OptionalReplicateSecretToRegionsRequestRequestTypeDef",
     {
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
+
 class ReplicateSecretToRegionsRequestRequestTypeDef(
     _RequiredReplicateSecretToRegionsRequestRequestTypeDef,
     _OptionalReplicateSecretToRegionsRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredCreateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredCreateSecretRequestRequestTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalCreateSecretRequestRequestTypeDef = TypedDict(
     "_OptionalCreateSecretRequestRequestTypeDef",
     {
         "ClientRequestToken": str,
         "Description": str,
         "KmsKeyId": str,
-        "SecretBinary": Union[str, bytes, IO[Any], StreamingBody],
+        "SecretBinary": BlobTypeDef,
         "SecretString": str,
         "Tags": Sequence[TagTypeDef],
         "AddReplicaRegions": Sequence[ReplicaRegionTypeTypeDef],
         "ForceOverwriteReplicaSecret": bool,
     },
     total=False,
 )
 
+
 class CreateSecretRequestRequestTypeDef(
     _RequiredCreateSecretRequestRequestTypeDef, _OptionalCreateSecretRequestRequestTypeDef
 ):
     pass
 
+
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "SecretId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
@@ -606,33 +629,33 @@
 CreateSecretResponseTypeDef = TypedDict(
     "CreateSecretResponseTypeDef",
     {
         "ARN": str,
         "Name": str,
         "VersionId": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RemoveRegionsFromReplicationResponseTypeDef = TypedDict(
     "RemoveRegionsFromReplicationResponseTypeDef",
     {
         "ARN": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicateSecretToRegionsResponseTypeDef = TypedDict(
     "ReplicateSecretToRegionsResponseTypeDef",
     {
         "ARN": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeSecretResponseTypeDef = TypedDict(
     "DescribeSecretResponseTypeDef",
     {
         "ARN": str,
@@ -649,15 +672,15 @@
         "NextRotationDate": datetime,
         "Tags": List[TagTypeDef],
         "VersionIdsToStages": Dict[str, List[str]],
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
         "ReplicationStatus": List[ReplicationStatusTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredRotateSecretRequestRequestTypeDef = TypedDict(
     "_RequiredRotateSecretRequestRequestTypeDef",
     {
         "SecretId": str,
@@ -670,19 +693,21 @@
         "RotationLambdaARN": str,
         "RotationRules": RotationRulesTypeTypeDef,
         "RotateImmediately": bool,
     },
     total=False,
 )
 
+
 class RotateSecretRequestRequestTypeDef(
     _RequiredRotateSecretRequestRequestTypeDef, _OptionalRotateSecretRequestRequestTypeDef
 ):
     pass
 
+
 SecretListEntryTypeDef = TypedDict(
     "SecretListEntryTypeDef",
     {
         "ARN": str,
         "Name": str,
         "Description": str,
         "KmsKeyId": str,
@@ -699,25 +724,14 @@
         "OwningService": str,
         "CreatedDate": datetime,
         "PrimaryRegion": str,
     },
     total=False,
 )
 
-ListSecretsRequestListSecretsPaginateTypeDef = TypedDict(
-    "ListSecretsRequestListSecretsPaginateTypeDef",
-    {
-        "IncludePlannedDeletion": bool,
-        "Filters": Sequence[FilterTypeDef],
-        "SortOrder": SortOrderTypeType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSecretsRequestRequestTypeDef = TypedDict(
     "ListSecretsRequestRequestTypeDef",
     {
         "IncludePlannedDeletion": bool,
         "MaxResults": int,
         "NextToken": str,
         "Filters": Sequence[FilterTypeDef],
@@ -729,28 +743,39 @@
 ListSecretVersionIdsResponseTypeDef = TypedDict(
     "ListSecretVersionIdsResponseTypeDef",
     {
         "Versions": List[SecretVersionsListEntryTypeDef],
         "NextToken": str,
         "ARN": str,
         "Name": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ListSecretsRequestListSecretsPaginateTypeDef = TypedDict(
+    "ListSecretsRequestListSecretsPaginateTypeDef",
+    {
+        "IncludePlannedDeletion": bool,
+        "Filters": Sequence[FilterTypeDef],
+        "SortOrder": SortOrderTypeType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ValidateResourcePolicyResponseTypeDef = TypedDict(
     "ValidateResourcePolicyResponseTypeDef",
     {
         "PolicyValidationPassed": bool,
         "ValidationErrors": List[ValidationErrorsEntryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSecretsResponseTypeDef = TypedDict(
     "ListSecretsResponseTypeDef",
     {
         "SecretList": List[SecretListEntryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/PKG-INFO` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-secretsmanager
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SecretsManager 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore secretsmanager type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore secretsmanager type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-secretsmanager"></a>
 
 # types-aiobotocore-secretsmanager
 
 [![PyPI - types-aiobotocore-secretsmanager](https://img.shields.io/pypi/v/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-secretsmanager.svg?color=blue)](https://pypi.org/project/types-aiobotocore-secretsmanager)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-secretsmanager?color=blue)](https://pypistats.org/packages/types-aiobotocore-secretsmanager)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-secretsmanager)](https://pepy.tech/project/types-aiobotocore-secretsmanager)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SecretsManager 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/secretsmanager.html#SecretsManager)
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
 [types-aiobotocore-secretsmanager docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_secretsmanager/).
 
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
@@ -308,81 +307,82 @@
 )
 
 
 def check_value(value: FilterNameStringTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_secretsmanager.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_secretsmanager.type_defs import (
+    BlobTypeDef,
     CancelRotateSecretRequestRequestTypeDef,
-    CancelRotateSecretResponseTypeDef,
+    ResponseMetadataTypeDef,
     ReplicaRegionTypeTypeDef,
     TagTypeDef,
     ReplicationStatusTypeTypeDef,
     DeleteResourcePolicyRequestRequestTypeDef,
-    DeleteResourcePolicyResponseTypeDef,
     DeleteSecretRequestRequestTypeDef,
-    DeleteSecretResponseTypeDef,
     DescribeSecretRequestRequestTypeDef,
     RotationRulesTypeTypeDef,
-    EmptyResponseMetadataTypeDef,
     FilterTypeDef,
     GetRandomPasswordRequestRequestTypeDef,
-    GetRandomPasswordResponseTypeDef,
     GetResourcePolicyRequestRequestTypeDef,
-    GetResourcePolicyResponseTypeDef,
     GetSecretValueRequestRequestTypeDef,
-    GetSecretValueResponseTypeDef,
     ListSecretVersionIdsRequestRequestTypeDef,
     SecretVersionsListEntryTypeDef,
     PaginatorConfigTypeDef,
     PutResourcePolicyRequestRequestTypeDef,
-    PutResourcePolicyResponseTypeDef,
-    PutSecretValueRequestRequestTypeDef,
-    PutSecretValueResponseTypeDef,
     RemoveRegionsFromReplicationRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     RestoreSecretRequestRequestTypeDef,
-    RestoreSecretResponseTypeDef,
-    RotateSecretResponseTypeDef,
     StopReplicationToReplicaRequestRequestTypeDef,
-    StopReplicationToReplicaResponseTypeDef,
     UntagResourceRequestRequestTypeDef,
-    UpdateSecretRequestRequestTypeDef,
-    UpdateSecretResponseTypeDef,
     UpdateSecretVersionStageRequestRequestTypeDef,
-    UpdateSecretVersionStageResponseTypeDef,
     ValidateResourcePolicyRequestRequestTypeDef,
     ValidationErrorsEntryTypeDef,
+    PutSecretValueRequestRequestTypeDef,
+    UpdateSecretRequestRequestTypeDef,
+    CancelRotateSecretResponseTypeDef,
+    DeleteResourcePolicyResponseTypeDef,
+    DeleteSecretResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetRandomPasswordResponseTypeDef,
+    GetResourcePolicyResponseTypeDef,
+    GetSecretValueResponseTypeDef,
+    PutResourcePolicyResponseTypeDef,
+    PutSecretValueResponseTypeDef,
+    RestoreSecretResponseTypeDef,
+    RotateSecretResponseTypeDef,
+    StopReplicationToReplicaResponseTypeDef,
+    UpdateSecretResponseTypeDef,
+    UpdateSecretVersionStageResponseTypeDef,
     ReplicateSecretToRegionsRequestRequestTypeDef,
     CreateSecretRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateSecretResponseTypeDef,
     RemoveRegionsFromReplicationResponseTypeDef,
     ReplicateSecretToRegionsResponseTypeDef,
     DescribeSecretResponseTypeDef,
     RotateSecretRequestRequestTypeDef,
     SecretListEntryTypeDef,
-    ListSecretsRequestListSecretsPaginateTypeDef,
     ListSecretsRequestRequestTypeDef,
     ListSecretVersionIdsResponseTypeDef,
+    ListSecretsRequestListSecretsPaginateTypeDef,
     ValidateResourcePolicyResponseTypeDef,
     ListSecretsResponseTypeDef,
 )
 
 
-def get_structure() -> CancelRotateSecretRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-secretsmanager-2.5.2/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt` & `types-aiobotocore-secretsmanager-2.5.2.post1/types_aiobotocore_secretsmanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-efs-2.5.2.tar.gz` & `tmp/types-aiobotocore-efs-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-efs-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-efs-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-efs-2.5.2.tar` & `types-aiobotocore-efs-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.170085 types-aiobotocore-efs-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-07-08 01:43:35.170085 types-aiobotocore-efs-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14484 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.170085 types-aiobotocore-efs-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.162085 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25287 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    25245 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-07-08 01:30:15.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24257 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:14.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.170085 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16033 2023-07-08 01:43:35.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:43:35.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:43:35.000000 types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.505594 types-aiobotocore-efs-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-02 14:52:14.493594 types-aiobotocore-efs-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14496 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.505594 types-aiobotocore-efs-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.493594 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25225 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25183 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9483 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24710 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24679 2023-08-02 14:38:02.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:01.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.493594 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15998 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:14.000000 types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-efs-2.5.2/LICENSE` & `types-aiobotocore-efs-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2/PKG-INFO` & `types-aiobotocore-efs-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-efs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore efs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore efs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-efs"></a>
 
 # types-aiobotocore-efs
 
 [![PyPI - types-aiobotocore-efs](https://img.shields.io/pypi/v/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-efs?color=blue)](https://pypistats.org/packages/types-aiobotocore-efs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EFS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
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
@@ -324,93 +323,95 @@
 )
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_efs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_efs.type_defs import (
-    PosixUserTypeDef,
+    PosixUserOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
+    PosixUserTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
+    MountTargetDescriptionResponseTypeDef,
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    PosixUserUnionTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     AccessPointDescriptionTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserTypeDef:
+def get_value() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-efs-2.5.2/README.md` & `types-aiobotocore-efs-2.5.2.post1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-efs"></a>
 
 # types-aiobotocore-efs
 
 [![PyPI - types-aiobotocore-efs](https://img.shields.io/pypi/v/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-efs?color=blue)](https://pypistats.org/packages/types-aiobotocore-efs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EFS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
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
@@ -291,93 +291,95 @@
 )
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_efs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_efs.type_defs import (
-    PosixUserTypeDef,
+    PosixUserOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
+    PosixUserTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
+    MountTargetDescriptionResponseTypeDef,
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    PosixUserUnionTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     AccessPointDescriptionTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserTypeDef:
+def get_value() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-efs-2.5.2/setup.py` & `types-aiobotocore-efs-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-efs",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_efs"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore efs type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore efs type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_efs": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/__init__.py` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/__init__.pyi` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/__main__.py` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.EFS 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.EFS 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS\nOther"
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

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/client.py` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,35 +23,35 @@
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
     DescribeTagsPaginator,
 )
 from .type_defs import (
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     BackupPolicyDescriptionTypeDef,
     BackupPolicyTypeDef,
     DescribeAccessPointsResponseTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeMountTargetSecurityGroupsResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DestinationToCreateTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PosixUserTypeDef,
+    MountTargetDescriptionResponseTypeDef,
+    PosixUserUnionTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -138,17 +138,17 @@
 
     async def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: PosixUserTypeDef = ...,
+        PosixUser: PosixUserUnionTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
-    ) -> AccessPointDescriptionResponseMetadataTypeDef:
+    ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_access_point)
         """
 
@@ -160,40 +160,40 @@
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...,
         AvailabilityZoneName: str = ...,
         Backup: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Creates a new, empty file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_file_system)
         """
 
     async def create_mount_target(
         self,
         *,
         FileSystemId: str,
         SubnetId: str,
         IpAddress: str = ...,
         SecurityGroups: Sequence[str] = ...
-    ) -> MountTargetDescriptionResponseMetadataTypeDef:
+    ) -> MountTargetDescriptionResponseTypeDef:
         """
         Creates a mount target for a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_mount_target)
         """
 
     async def create_replication_configuration(
         self, *, SourceFileSystemId: str, Destinations: Sequence[DestinationToCreateTypeDef]
-    ) -> ReplicationConfigurationDescriptionResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationDescriptionResponseTypeDef:
         """
         Creates a replication configuration that replicates an existing EFS file system
         to a new, read-only file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_replication_configuration)
         """
@@ -478,15 +478,15 @@
 
     async def update_file_system(
         self,
         *,
         FileSystemId: str,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Updates the throughput mode or the amount of provisioned throughput of an
         existing file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#update_file_system)
         """
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/client.pyi` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -23,35 +23,35 @@
 from .literals import PerformanceModeType, ResourceIdTypeType, ThroughputModeType
 from .paginator import (
     DescribeFileSystemsPaginator,
     DescribeMountTargetsPaginator,
     DescribeTagsPaginator,
 )
 from .type_defs import (
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     BackupPolicyDescriptionTypeDef,
     BackupPolicyTypeDef,
     DescribeAccessPointsResponseTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeMountTargetSecurityGroupsResponseTypeDef,
     DescribeMountTargetsResponseTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeTagsResponseTypeDef,
     DestinationToCreateTypeDef,
     EmptyResponseMetadataTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemPolicyDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceResponseTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PosixUserTypeDef,
+    MountTargetDescriptionResponseTypeDef,
+    PosixUserUnionTypeDef,
     PutAccountPreferencesResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     RootDirectoryTypeDef,
     TagTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
@@ -131,17 +131,17 @@
         """
     async def create_access_point(
         self,
         *,
         ClientToken: str,
         FileSystemId: str,
         Tags: Sequence[TagTypeDef] = ...,
-        PosixUser: PosixUserTypeDef = ...,
+        PosixUser: PosixUserUnionTypeDef = ...,
         RootDirectory: RootDirectoryTypeDef = ...
-    ) -> AccessPointDescriptionResponseMetadataTypeDef:
+    ) -> AccessPointDescriptionResponseTypeDef:
         """
         Creates an EFS access point.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_access_point)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_access_point)
         """
     async def create_file_system(
@@ -152,38 +152,38 @@
         Encrypted: bool = ...,
         KmsKeyId: str = ...,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...,
         AvailabilityZoneName: str = ...,
         Backup: bool = ...,
         Tags: Sequence[TagTypeDef] = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Creates a new, empty file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_file_system)
         """
     async def create_mount_target(
         self,
         *,
         FileSystemId: str,
         SubnetId: str,
         IpAddress: str = ...,
         SecurityGroups: Sequence[str] = ...
-    ) -> MountTargetDescriptionResponseMetadataTypeDef:
+    ) -> MountTargetDescriptionResponseTypeDef:
         """
         Creates a mount target for a file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_mount_target)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_mount_target)
         """
     async def create_replication_configuration(
         self, *, SourceFileSystemId: str, Destinations: Sequence[DestinationToCreateTypeDef]
-    ) -> ReplicationConfigurationDescriptionResponseMetadataTypeDef:
+    ) -> ReplicationConfigurationDescriptionResponseTypeDef:
         """
         Creates a replication configuration that replicates an existing EFS file system
         to a new, read-only file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.create_replication_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#create_replication_configuration)
         """
@@ -441,15 +441,15 @@
         """
     async def update_file_system(
         self,
         *,
         FileSystemId: str,
         ThroughputMode: ThroughputModeType = ...,
         ProvisionedThroughputInMibps: float = ...
-    ) -> FileSystemDescriptionResponseMetadataTypeDef:
+    ) -> FileSystemDescriptionResponseTypeDef:
         """
         Updates the throughput mode or the amount of provisioned throughput of an
         existing file system.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Client.update_file_system)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/client/#update_file_system)
         """
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/literals.py` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/literals.pyi` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/paginator.py` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describefilesystemspaginator)
         """
 
 
@@ -76,28 +76,28 @@
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describemounttargetspaginator)
         """
 
 
 class DescribeTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
-        self, *, FileSystemId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FileSystemId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describetagspaginator)
         """
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/paginator.pyi` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     """
 
     def paginate(
         self,
         *,
         CreationToken: str = ...,
         FileSystemId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeFileSystemsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeFileSystems.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describefilesystemspaginator)
         """
 
 class DescribeMountTargetsPaginator(AioPaginator):
@@ -72,27 +72,27 @@
 
     def paginate(
         self,
         *,
         FileSystemId: str = ...,
         MountTargetId: str = ...,
         AccessPointId: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMountTargetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeMountTargets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describemounttargetspaginator)
         """
 
 class DescribeTagsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describetagspaginator)
     """
 
     def paginate(
-        self, *, FileSystemId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, FileSystemId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTagsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS.Paginator.DescribeTags.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/paginators/#describetagspaginator)
         """
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/type_defs.py` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for efs service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_efs.type_defs import PosixUserTypeDef
+    from types_aiobotocore_efs.type_defs import PosixUserOutputTypeDef
 
-    data: PosixUserTypeDef = {...}
+    data: PosixUserOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     LifeCycleStateType,
     PerformanceModeType,
     ReplicationStatusType,
     ResourceIdTypeType,
     ResourceType,
@@ -31,103 +31,113 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
-    "PosixUserTypeDef",
+    "PosixUserOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "BackupPolicyTypeDef",
+    "PosixUserTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DescribeAccessPointsRequestRequestTypeDef",
     "DescribeAccountPreferencesRequestRequestTypeDef",
     "ResourceIdPreferenceTypeDef",
     "DescribeBackupPolicyRequestRequestTypeDef",
     "DescribeFileSystemPolicyRequestRequestTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
     "DescribeLifecycleConfigurationRequestRequestTypeDef",
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeMountTargetsRequestRequestTypeDef",
     "MountTargetDescriptionTypeDef",
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
-    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
-    "FileSystemPolicyDescriptionTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FileSystemPolicyDescriptionTypeDef",
+    "MountTargetDescriptionResponseTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
+    "PosixUserUnionTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeMountTargetsResponseTypeDef",
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
-    "FileSystemDescriptionResponseMetadataTypeDef",
+    "FileSystemDescriptionResponseTypeDef",
     "FileSystemDescriptionTypeDef",
     "LifecycleConfigurationDescriptionTypeDef",
     "PutLifecycleConfigurationRequestRequestTypeDef",
-    "AccessPointDescriptionResponseMetadataTypeDef",
+    "AccessPointDescriptionResponseTypeDef",
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
-_RequiredPosixUserTypeDef = TypedDict(
-    "_RequiredPosixUserTypeDef",
+_RequiredPosixUserOutputTypeDef = TypedDict(
+    "_RequiredPosixUserOutputTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
-_OptionalPosixUserTypeDef = TypedDict(
-    "_OptionalPosixUserTypeDef",
+_OptionalPosixUserOutputTypeDef = TypedDict(
+    "_OptionalPosixUserOutputTypeDef",
     {
-        "SecondaryGids": Sequence[int],
+        "SecondaryGids": List[int],
     },
     total=False,
 )
 
-
-class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
+class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
     pass
 
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
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
@@ -136,14 +146,32 @@
 BackupPolicyTypeDef = TypedDict(
     "BackupPolicyTypeDef",
     {
         "Status": StatusType,
     },
 )
 
+_RequiredPosixUserTypeDef = TypedDict(
+    "_RequiredPosixUserTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+    },
+)
+_OptionalPosixUserTypeDef = TypedDict(
+    "_OptionalPosixUserTypeDef",
+    {
+        "SecondaryGids": Sequence[int],
+    },
+    total=False,
+)
+
+class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
+    pass
+
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -152,21 +180,19 @@
     {
         "IpAddress": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class CreateMountTargetRequestRequestTypeDef(
     _RequiredCreateMountTargetRequestRequestTypeDef, _OptionalCreateMountTargetRequestRequestTypeDef
 ):
     pass
 
-
 DestinationToCreateTypeDef = TypedDict(
     "DestinationToCreateTypeDef",
     {
         "Region": str,
         "AvailabilityZoneName": str,
         "KmsKeyId": str,
     },
@@ -264,20 +290,20 @@
 DescribeFileSystemPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CreationToken": str,
-        "FileSystemId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
@@ -299,33 +325,14 @@
 DescribeMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 
-DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-        "MountTargetId": str,
-        "AccessPointId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMountTargetsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "Marker": str,
         "FileSystemId": str,
         "MountTargetId": str,
@@ -352,53 +359,29 @@
         "AvailabilityZoneId": str,
         "AvailabilityZoneName": str,
         "VpcId": str,
     },
     total=False,
 )
 
-
 class MountTargetDescriptionTypeDef(
     _RequiredMountTargetDescriptionTypeDef, _OptionalMountTargetDescriptionTypeDef
 ):
     pass
 
-
 DescribeReplicationConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-    },
-)
-_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class DescribeTagsRequestDescribeTagsPaginateTypeDef(
-    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
-    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -406,21 +389,19 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
-
 class DescribeTagsRequestRequestTypeDef(
     _RequiredDescribeTagsRequestRequestTypeDef, _OptionalDescribeTagsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Status": ReplicationStatusType,
         "FileSystemId": str,
         "Region": str,
     },
@@ -429,26 +410,17 @@
     "_OptionalDestinationTypeDef",
     {
         "LastReplicatedTimestamp": datetime,
     },
     total=False,
 )
 
-
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredFileSystemSizeTypeDef = TypedDict(
     "_RequiredFileSystemSizeTypeDef",
     {
         "Value": int,
     },
 )
 _OptionalFileSystemSizeTypeDef = TypedDict(
@@ -457,28 +429,17 @@
         "Timestamp": datetime,
         "ValueInIA": int,
         "ValueInStandard": int,
     },
     total=False,
 )
 
-
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
-
-FileSystemPolicyDescriptionTypeDef = TypedDict(
-    "FileSystemPolicyDescriptionTypeDef",
-    {
-        "FileSystemId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
     total=False,
@@ -495,71 +456,40 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
-
 _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
-
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
-
-MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    {
-        "OwnerId": str,
-        "MountTargetId": str,
-        "FileSystemId": str,
-        "SubnetId": str,
-        "LifeCycleState": LifeCycleStateType,
-        "IpAddress": str,
-        "NetworkInterfaceId": str,
-        "AvailabilityZoneId": str,
-        "AvailabilityZoneName": str,
-        "VpcId": str,
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
 PutAccountPreferencesRequestRequestTypeDef = TypedDict(
     "PutAccountPreferencesRequestRequestTypeDef",
     {
         "ResourceIdType": ResourceIdTypeType,
     },
 )
 
@@ -574,33 +504,20 @@
     "_OptionalPutFileSystemPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
-
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
 ):
     pass
 
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
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -616,20 +533,59 @@
     {
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
     },
     total=False,
 )
 
-
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FileSystemPolicyDescriptionTypeDef = TypedDict(
+    "FileSystemPolicyDescriptionTypeDef",
+    {
+        "FileSystemId": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MountTargetDescriptionResponseTypeDef = TypedDict(
+    "MountTargetDescriptionResponseTypeDef",
+    {
+        "OwnerId": str,
+        "MountTargetId": str,
+        "FileSystemId": str,
+        "SubnetId": str,
+        "LifeCycleState": LifeCycleStateType,
+        "IpAddress": str,
+        "NetworkInterfaceId": str,
+        "AvailabilityZoneId": str,
+        "AvailabilityZoneName": str,
+        "VpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
     },
 )
@@ -644,45 +600,43 @@
         "AvailabilityZoneName": str,
         "Backup": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
-
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "Marker": str,
         "Tags": List[TagTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
         "ResourceId": str,
@@ -690,26 +644,27 @@
     },
 )
 
 BackupPolicyDescriptionTypeDef = TypedDict(
     "BackupPolicyDescriptionTypeDef",
     {
         "BackupPolicy": BackupPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBackupPolicyRequestRequestTypeDef = TypedDict(
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "BackupPolicy": BackupPolicyTypeDef,
     },
 )
 
+PosixUserUnionTypeDef = Union[PosixUserTypeDef, PosixUserOutputTypeDef]
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
@@ -724,46 +679,87 @@
 )
 
 DescribeAccountPreferencesResponseTypeDef = TypedDict(
     "DescribeAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountPreferencesResponseTypeDef = TypedDict(
     "PutAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    {
+        "CreationToken": str,
+        "FileSystemId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+        "MountTargetId": str,
+        "AccessPointId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+    },
+)
+_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTagsRequestDescribeTagsPaginateTypeDef(
+    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
+    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
+):
+    pass
+
 DescribeMountTargetsResponseTypeDef = TypedDict(
     "DescribeMountTargetsResponseTypeDef",
     {
         "Marker": str,
         "MountTargets": List[MountTargetDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationDescriptionResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+ReplicationConfigurationDescriptionResponseTypeDef = TypedDict(
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     {
         "SourceFileSystemId": str,
         "SourceFileSystemRegion": str,
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationConfigurationDescriptionTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionTypeDef",
     {
         "SourceFileSystemId": str,
@@ -771,16 +767,16 @@
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
     },
 )
 
-FileSystemDescriptionResponseMetadataTypeDef = TypedDict(
-    "FileSystemDescriptionResponseMetadataTypeDef",
+FileSystemDescriptionResponseTypeDef = TypedDict(
+    "FileSystemDescriptionResponseTypeDef",
     {
         "OwnerId": str,
         "CreationToken": str,
         "FileSystemId": str,
         "FileSystemArn": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
@@ -791,15 +787,15 @@
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
         "OwnerId": str,
@@ -824,64 +820,62 @@
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
     },
     total=False,
 )
 
-
 class FileSystemDescriptionTypeDef(
     _RequiredFileSystemDescriptionTypeDef, _OptionalFileSystemDescriptionTypeDef
 ):
     pass
 
-
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
         "LifecyclePolicies": List[LifecyclePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "LifecyclePolicies": Sequence[LifecyclePolicyTypeDef],
     },
 )
 
-AccessPointDescriptionResponseMetadataTypeDef = TypedDict(
-    "AccessPointDescriptionResponseMetadataTypeDef",
+AccessPointDescriptionResponseTypeDef = TypedDict(
+    "AccessPointDescriptionResponseTypeDef",
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
 
@@ -898,41 +892,39 @@
         "Tags": Sequence[TagTypeDef],
         "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
     },
     total=False,
 )
 
-
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
-
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemsResponseTypeDef = TypedDict(
     "DescribeFileSystemsResponseTypeDef",
     {
         "Marker": str,
         "FileSystems": List[FileSystemDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsResponseTypeDef = TypedDict(
     "DescribeAccessPointsResponseTypeDef",
     {
         "AccessPoints": List[AccessPointDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs/type_defs.pyi` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 Type annotations for efs service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_efs.type_defs import PosixUserTypeDef
+    from types_aiobotocore_efs.type_defs import PosixUserOutputTypeDef
 
-    data: PosixUserTypeDef = {...}
+    data: PosixUserOutputTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     LifeCycleStateType,
     PerformanceModeType,
     ReplicationStatusType,
     ResourceIdTypeType,
     ResourceType,
@@ -31,101 +31,117 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
-    "PosixUserTypeDef",
+    "PosixUserOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "BackupPolicyTypeDef",
+    "PosixUserTypeDef",
     "CreateMountTargetRequestRequestTypeDef",
     "DestinationToCreateTypeDef",
     "CreationInfoTypeDef",
     "DeleteAccessPointRequestRequestTypeDef",
     "DeleteFileSystemPolicyRequestRequestTypeDef",
     "DeleteFileSystemRequestRequestTypeDef",
     "DeleteMountTargetRequestRequestTypeDef",
     "DeleteReplicationConfigurationRequestRequestTypeDef",
     "DeleteTagsRequestRequestTypeDef",
     "DescribeAccessPointsRequestRequestTypeDef",
     "DescribeAccountPreferencesRequestRequestTypeDef",
     "ResourceIdPreferenceTypeDef",
     "DescribeBackupPolicyRequestRequestTypeDef",
     "DescribeFileSystemPolicyRequestRequestTypeDef",
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeFileSystemsRequestRequestTypeDef",
     "DescribeLifecycleConfigurationRequestRequestTypeDef",
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
     "DescribeMountTargetsRequestRequestTypeDef",
     "MountTargetDescriptionTypeDef",
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
-    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeTagsRequestRequestTypeDef",
     "DestinationTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "FileSystemSizeTypeDef",
-    "FileSystemPolicyDescriptionTypeDef",
     "LifecyclePolicyTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "ModifyMountTargetSecurityGroupsRequestRequestTypeDef",
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    "PaginatorConfigTypeDef",
     "PutAccountPreferencesRequestRequestTypeDef",
     "PutFileSystemPolicyRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateFileSystemRequestRequestTypeDef",
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "FileSystemPolicyDescriptionTypeDef",
+    "MountTargetDescriptionResponseTypeDef",
     "CreateFileSystemRequestRequestTypeDef",
     "CreateTagsRequestRequestTypeDef",
     "DescribeTagsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "BackupPolicyDescriptionTypeDef",
     "PutBackupPolicyRequestRequestTypeDef",
+    "PosixUserUnionTypeDef",
     "CreateReplicationConfigurationRequestRequestTypeDef",
     "RootDirectoryTypeDef",
     "DescribeAccountPreferencesResponseTypeDef",
     "PutAccountPreferencesResponseTypeDef",
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    "DescribeTagsRequestDescribeTagsPaginateTypeDef",
     "DescribeMountTargetsResponseTypeDef",
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     "ReplicationConfigurationDescriptionTypeDef",
-    "FileSystemDescriptionResponseMetadataTypeDef",
+    "FileSystemDescriptionResponseTypeDef",
     "FileSystemDescriptionTypeDef",
     "LifecycleConfigurationDescriptionTypeDef",
     "PutLifecycleConfigurationRequestRequestTypeDef",
-    "AccessPointDescriptionResponseMetadataTypeDef",
+    "AccessPointDescriptionResponseTypeDef",
     "AccessPointDescriptionTypeDef",
     "CreateAccessPointRequestRequestTypeDef",
     "DescribeReplicationConfigurationsResponseTypeDef",
     "DescribeFileSystemsResponseTypeDef",
     "DescribeAccessPointsResponseTypeDef",
 )
 
-_RequiredPosixUserTypeDef = TypedDict(
-    "_RequiredPosixUserTypeDef",
+_RequiredPosixUserOutputTypeDef = TypedDict(
+    "_RequiredPosixUserOutputTypeDef",
     {
         "Uid": int,
         "Gid": int,
     },
 )
-_OptionalPosixUserTypeDef = TypedDict(
-    "_OptionalPosixUserTypeDef",
+_OptionalPosixUserOutputTypeDef = TypedDict(
+    "_OptionalPosixUserOutputTypeDef",
     {
-        "SecondaryGids": Sequence[int],
+        "SecondaryGids": List[int],
     },
     total=False,
 )
 
-class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
+
+class PosixUserOutputTypeDef(_RequiredPosixUserOutputTypeDef, _OptionalPosixUserOutputTypeDef):
     pass
 
+
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
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -133,14 +149,34 @@
 BackupPolicyTypeDef = TypedDict(
     "BackupPolicyTypeDef",
     {
         "Status": StatusType,
     },
 )
 
+_RequiredPosixUserTypeDef = TypedDict(
+    "_RequiredPosixUserTypeDef",
+    {
+        "Uid": int,
+        "Gid": int,
+    },
+)
+_OptionalPosixUserTypeDef = TypedDict(
+    "_OptionalPosixUserTypeDef",
+    {
+        "SecondaryGids": Sequence[int],
+    },
+    total=False,
+)
+
+
+class PosixUserTypeDef(_RequiredPosixUserTypeDef, _OptionalPosixUserTypeDef):
+    pass
+
+
 _RequiredCreateMountTargetRequestRequestTypeDef = TypedDict(
     "_RequiredCreateMountTargetRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "SubnetId": str,
     },
 )
@@ -149,19 +185,21 @@
     {
         "IpAddress": str,
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class CreateMountTargetRequestRequestTypeDef(
     _RequiredCreateMountTargetRequestRequestTypeDef, _OptionalCreateMountTargetRequestRequestTypeDef
 ):
     pass
 
+
 DestinationToCreateTypeDef = TypedDict(
     "DestinationToCreateTypeDef",
     {
         "Region": str,
         "AvailabilityZoneName": str,
         "KmsKeyId": str,
     },
@@ -259,20 +297,20 @@
 DescribeFileSystemPolicyRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 
-DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
-    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "CreationToken": str,
-        "FileSystemId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeFileSystemsRequestRequestTypeDef = TypedDict(
     "DescribeFileSystemsRequestRequestTypeDef",
     {
@@ -294,33 +332,14 @@
 DescribeMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 
-DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
-    "DescribeMountTargetSecurityGroupsResponseTypeDef",
-    {
-        "SecurityGroups": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
-    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-        "MountTargetId": str,
-        "AccessPointId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 DescribeMountTargetsRequestRequestTypeDef = TypedDict(
     "DescribeMountTargetsRequestRequestTypeDef",
     {
         "MaxItems": int,
         "Marker": str,
         "FileSystemId": str,
         "MountTargetId": str,
@@ -347,49 +366,31 @@
         "AvailabilityZoneId": str,
         "AvailabilityZoneName": str,
         "VpcId": str,
     },
     total=False,
 )
 
+
 class MountTargetDescriptionTypeDef(
     _RequiredMountTargetDescriptionTypeDef, _OptionalMountTargetDescriptionTypeDef
 ):
     pass
 
+
 DescribeReplicationConfigurationsRequestRequestTypeDef = TypedDict(
     "DescribeReplicationConfigurationsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "FileSystemId": str,
-    },
-)
-_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
-    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class DescribeTagsRequestDescribeTagsPaginateTypeDef(
-    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
-    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTagsRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
     },
 )
 _OptionalDescribeTagsRequestRequestTypeDef = TypedDict(
@@ -397,19 +398,21 @@
     {
         "MaxItems": int,
         "Marker": str,
     },
     total=False,
 )
 
+
 class DescribeTagsRequestRequestTypeDef(
     _RequiredDescribeTagsRequestRequestTypeDef, _OptionalDescribeTagsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDestinationTypeDef = TypedDict(
     "_RequiredDestinationTypeDef",
     {
         "Status": ReplicationStatusType,
         "FileSystemId": str,
         "Region": str,
     },
@@ -418,23 +421,18 @@
     "_OptionalDestinationTypeDef",
     {
         "LastReplicatedTimestamp": datetime,
     },
     total=False,
 )
 
+
 class DestinationTypeDef(_RequiredDestinationTypeDef, _OptionalDestinationTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredFileSystemSizeTypeDef = TypedDict(
     "_RequiredFileSystemSizeTypeDef",
     {
         "Value": int,
     },
 )
@@ -444,25 +442,18 @@
         "Timestamp": datetime,
         "ValueInIA": int,
         "ValueInStandard": int,
     },
     total=False,
 )
 
+
 class FileSystemSizeTypeDef(_RequiredFileSystemSizeTypeDef, _OptionalFileSystemSizeTypeDef):
     pass
 
-FileSystemPolicyDescriptionTypeDef = TypedDict(
-    "FileSystemPolicyDescriptionTypeDef",
-    {
-        "FileSystemId": str,
-        "Policy": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 LifecyclePolicyTypeDef = TypedDict(
     "LifecyclePolicyTypeDef",
     {
         "TransitionToIA": TransitionToIARulesType,
         "TransitionToPrimaryStorageClass": Literal["AFTER_1_ACCESS"],
     },
@@ -480,66 +471,43 @@
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class ListTagsForResourceRequestRequestTypeDef(
     _RequiredListTagsForResourceRequestRequestTypeDef,
     _OptionalListTagsForResourceRequestRequestTypeDef,
 ):
     pass
 
+
 _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "MountTargetId": str,
     },
 )
 _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef = TypedDict(
     "_OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef",
     {
         "SecurityGroups": Sequence[str],
     },
     total=False,
 )
 
+
 class ModifyMountTargetSecurityGroupsRequestRequestTypeDef(
     _RequiredModifyMountTargetSecurityGroupsRequestRequestTypeDef,
     _OptionalModifyMountTargetSecurityGroupsRequestRequestTypeDef,
 ):
     pass
 
-MountTargetDescriptionResponseMetadataTypeDef = TypedDict(
-    "MountTargetDescriptionResponseMetadataTypeDef",
-    {
-        "OwnerId": str,
-        "MountTargetId": str,
-        "FileSystemId": str,
-        "SubnetId": str,
-        "LifeCycleState": LifeCycleStateType,
-        "IpAddress": str,
-        "NetworkInterfaceId": str,
-        "AvailabilityZoneId": str,
-        "AvailabilityZoneName": str,
-        "VpcId": str,
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
 
 PutAccountPreferencesRequestRequestTypeDef = TypedDict(
     "PutAccountPreferencesRequestRequestTypeDef",
     {
         "ResourceIdType": ResourceIdTypeType,
     },
 )
@@ -555,30 +523,21 @@
     "_OptionalPutFileSystemPolicyRequestRequestTypeDef",
     {
         "BypassPolicyLockoutSafetyCheck": bool,
     },
     total=False,
 )
 
+
 class PutFileSystemPolicyRequestRequestTypeDef(
     _RequiredPutFileSystemPolicyRequestRequestTypeDef,
     _OptionalPutFileSystemPolicyRequestRequestTypeDef,
 ):
     pass
 
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
 
 UntagResourceRequestRequestTypeDef = TypedDict(
     "UntagResourceRequestRequestTypeDef",
     {
         "ResourceId": str,
         "TagKeys": Sequence[str],
     },
@@ -595,19 +554,62 @@
     {
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
     },
     total=False,
 )
 
+
 class UpdateFileSystemRequestRequestTypeDef(
     _RequiredUpdateFileSystemRequestRequestTypeDef, _OptionalUpdateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
+DescribeMountTargetSecurityGroupsResponseTypeDef = TypedDict(
+    "DescribeMountTargetSecurityGroupsResponseTypeDef",
+    {
+        "SecurityGroups": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+FileSystemPolicyDescriptionTypeDef = TypedDict(
+    "FileSystemPolicyDescriptionTypeDef",
+    {
+        "FileSystemId": str,
+        "Policy": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+MountTargetDescriptionResponseTypeDef = TypedDict(
+    "MountTargetDescriptionResponseTypeDef",
+    {
+        "OwnerId": str,
+        "MountTargetId": str,
+        "FileSystemId": str,
+        "SubnetId": str,
+        "LifeCycleState": LifeCycleStateType,
+        "IpAddress": str,
+        "NetworkInterfaceId": str,
+        "AvailabilityZoneId": str,
+        "AvailabilityZoneName": str,
+        "VpcId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredCreateFileSystemRequestRequestTypeDef = TypedDict(
     "_RequiredCreateFileSystemRequestRequestTypeDef",
     {
         "CreationToken": str,
     },
 )
 _OptionalCreateFileSystemRequestRequestTypeDef = TypedDict(
@@ -621,43 +623,45 @@
         "AvailabilityZoneName": str,
         "Backup": bool,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateFileSystemRequestRequestTypeDef(
     _RequiredCreateFileSystemRequestRequestTypeDef, _OptionalCreateFileSystemRequestRequestTypeDef
 ):
     pass
 
+
 CreateTagsRequestRequestTypeDef = TypedDict(
     "CreateTagsRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
 DescribeTagsResponseTypeDef = TypedDict(
     "DescribeTagsResponseTypeDef",
     {
         "Marker": str,
         "Tags": List[TagTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
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
         "ResourceId": str,
@@ -665,26 +669,27 @@
     },
 )
 
 BackupPolicyDescriptionTypeDef = TypedDict(
     "BackupPolicyDescriptionTypeDef",
     {
         "BackupPolicy": BackupPolicyTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutBackupPolicyRequestRequestTypeDef = TypedDict(
     "PutBackupPolicyRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "BackupPolicy": BackupPolicyTypeDef,
     },
 )
 
+PosixUserUnionTypeDef = Union[PosixUserTypeDef, PosixUserOutputTypeDef]
 CreateReplicationConfigurationRequestRequestTypeDef = TypedDict(
     "CreateReplicationConfigurationRequestRequestTypeDef",
     {
         "SourceFileSystemId": str,
         "Destinations": Sequence[DestinationToCreateTypeDef],
     },
 )
@@ -699,46 +704,89 @@
 )
 
 DescribeAccountPreferencesResponseTypeDef = TypedDict(
     "DescribeAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutAccountPreferencesResponseTypeDef = TypedDict(
     "PutAccountPreferencesResponseTypeDef",
     {
         "ResourceIdPreference": ResourceIdPreferenceTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef = TypedDict(
+    "DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef",
+    {
+        "CreationToken": str,
+        "FileSystemId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef = TypedDict(
+    "DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+        "MountTargetId": str,
+        "AccessPointId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "FileSystemId": str,
+    },
+)
+_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef = TypedDict(
+    "_OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTagsRequestDescribeTagsPaginateTypeDef(
+    _RequiredDescribeTagsRequestDescribeTagsPaginateTypeDef,
+    _OptionalDescribeTagsRequestDescribeTagsPaginateTypeDef,
+):
+    pass
+
+
 DescribeMountTargetsResponseTypeDef = TypedDict(
     "DescribeMountTargetsResponseTypeDef",
     {
         "Marker": str,
         "MountTargets": List[MountTargetDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ReplicationConfigurationDescriptionResponseMetadataTypeDef = TypedDict(
-    "ReplicationConfigurationDescriptionResponseMetadataTypeDef",
+ReplicationConfigurationDescriptionResponseTypeDef = TypedDict(
+    "ReplicationConfigurationDescriptionResponseTypeDef",
     {
         "SourceFileSystemId": str,
         "SourceFileSystemRegion": str,
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReplicationConfigurationDescriptionTypeDef = TypedDict(
     "ReplicationConfigurationDescriptionTypeDef",
     {
         "SourceFileSystemId": str,
@@ -746,16 +794,16 @@
         "SourceFileSystemArn": str,
         "OriginalSourceFileSystemArn": str,
         "CreationTime": datetime,
         "Destinations": List[DestinationTypeDef],
     },
 )
 
-FileSystemDescriptionResponseMetadataTypeDef = TypedDict(
-    "FileSystemDescriptionResponseMetadataTypeDef",
+FileSystemDescriptionResponseTypeDef = TypedDict(
+    "FileSystemDescriptionResponseTypeDef",
     {
         "OwnerId": str,
         "CreationToken": str,
         "FileSystemId": str,
         "FileSystemArn": str,
         "CreationTime": datetime,
         "LifeCycleState": LifeCycleStateType,
@@ -766,15 +814,15 @@
         "Encrypted": bool,
         "KmsKeyId": str,
         "ThroughputMode": ThroughputModeType,
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredFileSystemDescriptionTypeDef = TypedDict(
     "_RequiredFileSystemDescriptionTypeDef",
     {
         "OwnerId": str,
@@ -799,62 +847,64 @@
         "ProvisionedThroughputInMibps": float,
         "AvailabilityZoneName": str,
         "AvailabilityZoneId": str,
     },
     total=False,
 )
 
+
 class FileSystemDescriptionTypeDef(
     _RequiredFileSystemDescriptionTypeDef, _OptionalFileSystemDescriptionTypeDef
 ):
     pass
 
+
 LifecycleConfigurationDescriptionTypeDef = TypedDict(
     "LifecycleConfigurationDescriptionTypeDef",
     {
         "LifecyclePolicies": List[LifecyclePolicyTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutLifecycleConfigurationRequestRequestTypeDef = TypedDict(
     "PutLifecycleConfigurationRequestRequestTypeDef",
     {
         "FileSystemId": str,
         "LifecyclePolicies": Sequence[LifecyclePolicyTypeDef],
     },
 )
 
-AccessPointDescriptionResponseMetadataTypeDef = TypedDict(
-    "AccessPointDescriptionResponseMetadataTypeDef",
+AccessPointDescriptionResponseTypeDef = TypedDict(
+    "AccessPointDescriptionResponseTypeDef",
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AccessPointDescriptionTypeDef = TypedDict(
     "AccessPointDescriptionTypeDef",
     {
         "ClientToken": str,
         "Name": str,
         "Tags": List[TagTypeDef],
         "AccessPointId": str,
         "AccessPointArn": str,
         "FileSystemId": str,
-        "PosixUser": PosixUserTypeDef,
+        "PosixUser": PosixUserOutputTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
         "OwnerId": str,
         "LifeCycleState": LifeCycleStateType,
     },
     total=False,
 )
 
@@ -871,39 +921,41 @@
         "Tags": Sequence[TagTypeDef],
         "PosixUser": PosixUserTypeDef,
         "RootDirectory": RootDirectoryTypeDef,
     },
     total=False,
 )
 
+
 class CreateAccessPointRequestRequestTypeDef(
     _RequiredCreateAccessPointRequestRequestTypeDef, _OptionalCreateAccessPointRequestRequestTypeDef
 ):
     pass
 
+
 DescribeReplicationConfigurationsResponseTypeDef = TypedDict(
     "DescribeReplicationConfigurationsResponseTypeDef",
     {
         "Replications": List[ReplicationConfigurationDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeFileSystemsResponseTypeDef = TypedDict(
     "DescribeFileSystemsResponseTypeDef",
     {
         "Marker": str,
         "FileSystems": List[FileSystemDescriptionTypeDef],
         "NextMarker": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeAccessPointsResponseTypeDef = TypedDict(
     "DescribeAccessPointsResponseTypeDef",
     {
         "AccessPoints": List[AccessPointDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/PKG-INFO` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-efs
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.EFS 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore efs type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore efs type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-efs"></a>
 
 # types-aiobotocore-efs
 
 [![PyPI - types-aiobotocore-efs](https://img.shields.io/pypi/v/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-efs.svg?color=blue)](https://pypi.org/project/types-aiobotocore-efs)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-efs?color=blue)](https://pypistats.org/packages/types-aiobotocore-efs)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-efs)](https://pepy.tech/project/types-aiobotocore-efs)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.EFS 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/efs.html#EFS)
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
 [types-aiobotocore-efs docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_efs/).
 
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
@@ -324,93 +323,95 @@
 )
 
 
 def check_value(value: DescribeFileSystemsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_efs.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_efs.type_defs import (
-    PosixUserTypeDef,
+    PosixUserOutputTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     BackupPolicyTypeDef,
+    PosixUserTypeDef,
     CreateMountTargetRequestRequestTypeDef,
     DestinationToCreateTypeDef,
     CreationInfoTypeDef,
     DeleteAccessPointRequestRequestTypeDef,
     DeleteFileSystemPolicyRequestRequestTypeDef,
     DeleteFileSystemRequestRequestTypeDef,
     DeleteMountTargetRequestRequestTypeDef,
     DeleteReplicationConfigurationRequestRequestTypeDef,
     DeleteTagsRequestRequestTypeDef,
     DescribeAccessPointsRequestRequestTypeDef,
     DescribeAccountPreferencesRequestRequestTypeDef,
     ResourceIdPreferenceTypeDef,
     DescribeBackupPolicyRequestRequestTypeDef,
     DescribeFileSystemPolicyRequestRequestTypeDef,
-    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeFileSystemsRequestRequestTypeDef,
     DescribeLifecycleConfigurationRequestRequestTypeDef,
     DescribeMountTargetSecurityGroupsRequestRequestTypeDef,
-    DescribeMountTargetSecurityGroupsResponseTypeDef,
-    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
     DescribeMountTargetsRequestRequestTypeDef,
     MountTargetDescriptionTypeDef,
     DescribeReplicationConfigurationsRequestRequestTypeDef,
-    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeTagsRequestRequestTypeDef,
     DestinationTypeDef,
-    EmptyResponseMetadataTypeDef,
     FileSystemSizeTypeDef,
-    FileSystemPolicyDescriptionTypeDef,
     LifecyclePolicyTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     ModifyMountTargetSecurityGroupsRequestRequestTypeDef,
-    MountTargetDescriptionResponseMetadataTypeDef,
-    PaginatorConfigTypeDef,
     PutAccountPreferencesRequestRequestTypeDef,
     PutFileSystemPolicyRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateFileSystemRequestRequestTypeDef,
+    DescribeMountTargetSecurityGroupsResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    FileSystemPolicyDescriptionTypeDef,
+    MountTargetDescriptionResponseTypeDef,
     CreateFileSystemRequestRequestTypeDef,
     CreateTagsRequestRequestTypeDef,
     DescribeTagsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     BackupPolicyDescriptionTypeDef,
     PutBackupPolicyRequestRequestTypeDef,
+    PosixUserUnionTypeDef,
     CreateReplicationConfigurationRequestRequestTypeDef,
     RootDirectoryTypeDef,
     DescribeAccountPreferencesResponseTypeDef,
     PutAccountPreferencesResponseTypeDef,
+    DescribeFileSystemsRequestDescribeFileSystemsPaginateTypeDef,
+    DescribeMountTargetsRequestDescribeMountTargetsPaginateTypeDef,
+    DescribeTagsRequestDescribeTagsPaginateTypeDef,
     DescribeMountTargetsResponseTypeDef,
-    ReplicationConfigurationDescriptionResponseMetadataTypeDef,
+    ReplicationConfigurationDescriptionResponseTypeDef,
     ReplicationConfigurationDescriptionTypeDef,
-    FileSystemDescriptionResponseMetadataTypeDef,
+    FileSystemDescriptionResponseTypeDef,
     FileSystemDescriptionTypeDef,
     LifecycleConfigurationDescriptionTypeDef,
     PutLifecycleConfigurationRequestRequestTypeDef,
-    AccessPointDescriptionResponseMetadataTypeDef,
+    AccessPointDescriptionResponseTypeDef,
     AccessPointDescriptionTypeDef,
     CreateAccessPointRequestRequestTypeDef,
     DescribeReplicationConfigurationsResponseTypeDef,
     DescribeFileSystemsResponseTypeDef,
     DescribeAccessPointsResponseTypeDef,
 )
 
 
-def get_structure() -> PosixUserTypeDef:
+def get_value() -> PosixUserOutputTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-efs-2.5.2/types_aiobotocore_efs.egg-info/SOURCES.txt` & `types-aiobotocore-efs-2.5.2.post1/types_aiobotocore_efs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


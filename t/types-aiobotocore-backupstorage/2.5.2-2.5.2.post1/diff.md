# Comparing `tmp/types-aiobotocore-backupstorage-2.5.2.tar.gz` & `tmp/types-aiobotocore-backupstorage-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-backupstorage-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-backupstorage-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-backupstorage-2.5.2.tar` & `types-aiobotocore-backupstorage-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.933738 types-aiobotocore-backupstorage-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-07-08 01:43:16.929738 types-aiobotocore-backupstorage-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.933738 types-aiobotocore-backupstorage-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.929738 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11103 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-07-08 01:26:20.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:19.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.929738 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13067 2023-07-08 01:43:16.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 01:43:16.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:16.000000 types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.337648 types-aiobotocore-backupstorage-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-08-02 14:51:55.333648 types-aiobotocore-backupstorage-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.337648 types-aiobotocore-backupstorage-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.329648 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10956 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10938 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8502 2023-08-02 14:33:47.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8490 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:46.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.333648 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:51:55.000000 types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/LICENSE` & `types-aiobotocore-backupstorage-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2/PKG-INFO` & `types-aiobotocore-backupstorage-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore backupstorage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore backupstorage type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backupstorage"></a>
 
 # types-aiobotocore-backupstorage
 
 [![PyPI - types-aiobotocore-backupstorage](https://img.shields.io/pypi/v/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backupstorage?color=blue)](https://pypistats.org/packages/types-aiobotocore-backupstorage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BackupStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -282,48 +281,50 @@
 )
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backupstorage.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backupstorage.type_defs import (
     BackupObjectTypeDef,
+    BlobTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
-    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
-    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
-    ListObjectsInputRequestTypeDef,
+    TimestampTypeDef,
+    StartObjectInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
     PutChunkInputRequestTypeDef,
-    PutChunkOutputTypeDef,
     PutObjectInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChunkOutputTypeDef,
+    GetObjectMetadataOutputTypeDef,
+    ListChunksOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    NotifyObjectCompleteOutputTypeDef,
+    PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartObjectInputRequestTypeDef,
     StartObjectOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListChunksOutputTypeDef,
+    ListObjectsInputRequestTypeDef,
 )
 
 
-def get_structure() -> BackupObjectTypeDef:
+def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/README.md` & `types-aiobotocore-backupstorage-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-backupstorage"></a>
 
 # types-aiobotocore-backupstorage
 
 [![PyPI - types-aiobotocore-backupstorage](https://img.shields.io/pypi/v/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backupstorage?color=blue)](https://pypistats.org/packages/types-aiobotocore-backupstorage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BackupStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -40,15 +40,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -249,48 +249,50 @@
 )
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backupstorage.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backupstorage.type_defs import (
     BackupObjectTypeDef,
+    BlobTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
-    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
-    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
-    ListObjectsInputRequestTypeDef,
+    TimestampTypeDef,
+    StartObjectInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
     PutChunkInputRequestTypeDef,
-    PutChunkOutputTypeDef,
     PutObjectInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChunkOutputTypeDef,
+    GetObjectMetadataOutputTypeDef,
+    ListChunksOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    NotifyObjectCompleteOutputTypeDef,
+    PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartObjectInputRequestTypeDef,
     StartObjectOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListChunksOutputTypeDef,
+    ListObjectsInputRequestTypeDef,
 )
 
 
-def get_structure() -> BackupObjectTypeDef:
+def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/setup.py` & `types-aiobotocore-backupstorage-2.5.2.post1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-backupstorage",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_backupstorage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with"
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
-    keywords="aiobotocore backupstorage type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore backupstorage type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_backupstorage": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/"
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/client.py` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -11,64 +11,60 @@
 
     session = get_session()
     async with session.create_client("backupstorage") as client:
         client: BackupStorageClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
+    BlobTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("BackupStorageClient",)
 
-
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
-
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     DataAlreadyExistsException: Type[BotocoreClientError]
     IllegalArgumentException: Type[BotocoreClientError]
     KMSInvalidKeyUsageException: Type[BotocoreClientError]
     NotReadableInputStreamException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     RetryableException: Type[BotocoreClientError]
     ServiceInternalException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
-
 class BackupStorageClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/)
     """
 
     meta: ClientMeta
@@ -77,177 +73,163 @@
     def exceptions(self) -> Exceptions:
         """
         BackupStorageClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#exceptions)
         """
-
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#can_paginate)
         """
-
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#close)
         """
-
     async def delete_object(
         self, *, BackupJobId: str, ObjectName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete Object from the incremental base Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.delete_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#delete_object)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#generate_presigned_url)
         """
-
     async def get_chunk(self, *, StorageJobId: str, ChunkToken: str) -> GetChunkOutputTypeDef:
         """
         Gets the specified object's chunk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.get_chunk)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#get_chunk)
         """
-
     async def get_object_metadata(
         self, *, StorageJobId: str, ObjectToken: str
     ) -> GetObjectMetadataOutputTypeDef:
         """
         Get metadata associated with an Object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.get_object_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#get_object_metadata)
         """
-
     async def list_chunks(
         self, *, StorageJobId: str, ObjectToken: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChunksOutputTypeDef:
         """
         List chunks in a given Object See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/ListChunks).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_chunks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#list_chunks)
         """
-
     async def list_objects(
         self,
         *,
         StorageJobId: str,
         StartingObjectName: str = ...,
         StartingObjectPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        CreatedBefore: Union[datetime, str] = ...,
-        CreatedAfter: Union[datetime, str] = ...
+        CreatedBefore: TimestampTypeDef = ...,
+        CreatedAfter: TimestampTypeDef = ...
     ) -> ListObjectsOutputTypeDef:
         """
         List all Objects in a given Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#list_objects)
         """
-
     async def notify_object_complete(
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ObjectChecksum: str,
         ObjectChecksumAlgorithm: Literal["SUMMARY"],
         MetadataString: str = ...,
-        MetadataBlob: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        MetadataBlob: BlobTypeDef = ...,
         MetadataBlobLength: int = ...,
         MetadataBlobChecksum: str = ...,
         MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...
     ) -> NotifyObjectCompleteOutputTypeDef:
         """
         Complete upload See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/NotifyObjectComplete).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.notify_object_complete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#notify_object_complete)
         """
-
     async def put_chunk(
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ChunkIndex: int,
-        Data: Union[str, bytes, IO[Any], StreamingBody],
+        Data: BlobTypeDef,
         Length: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"]
     ) -> PutChunkOutputTypeDef:
         """
         Upload chunk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_chunk)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#put_chunk)
         """
-
     async def put_object(
         self,
         *,
         BackupJobId: str,
         ObjectName: str,
         MetadataString: str = ...,
-        InlineChunk: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        InlineChunk: BlobTypeDef = ...,
         InlineChunkLength: int = ...,
         InlineChunkChecksum: str = ...,
         InlineChunkChecksumAlgorithm: str = ...,
         ObjectChecksum: str = ...,
         ObjectChecksumAlgorithm: Literal["SUMMARY"] = ...,
         ThrowOnDuplicate: bool = ...
     ) -> PutObjectOutputTypeDef:
         """
         Upload object that can store object metadata String and data blob in single API
         call using inline chunk field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#put_object)
         """
-
     async def start_object(
         self, *, BackupJobId: str, ObjectName: str, ThrowOnDuplicate: bool = ...
     ) -> StartObjectOutputTypeDef:
         """
         Start upload containing one or many chunks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.start_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#start_object)
         """
-
     async def __aenter__(self) -> "BackupStorageClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/)
         """
-
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/)
         """
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/client.pyi` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,60 +11,64 @@
 
     session = get_session()
     async with session.create_client("backupstorage") as client:
         client: BackupStorageClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
+    BlobTypeDef,
     EmptyResponseMetadataTypeDef,
     GetChunkOutputTypeDef,
     GetObjectMetadataOutputTypeDef,
     ListChunksOutputTypeDef,
     ListObjectsOutputTypeDef,
     NotifyObjectCompleteOutputTypeDef,
     PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
     StartObjectOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("BackupStorageClient",)
 
+
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
         self.response: Dict[str, Any]
         self.operation_name: str
 
+
 class Exceptions:
     AccessDeniedException: Type[BotocoreClientError]
     ClientError: Type[BotocoreClientError]
     DataAlreadyExistsException: Type[BotocoreClientError]
     IllegalArgumentException: Type[BotocoreClientError]
     KMSInvalidKeyUsageException: Type[BotocoreClientError]
     NotReadableInputStreamException: Type[BotocoreClientError]
     ResourceNotFoundException: Type[BotocoreClientError]
     RetryableException: Type[BotocoreClientError]
     ServiceInternalException: Type[BotocoreClientError]
     ServiceUnavailableException: Type[BotocoreClientError]
     ThrottlingException: Type[BotocoreClientError]
 
+
 class BackupStorageClient(AioBaseClient):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/)
     """
 
     meta: ClientMeta
@@ -73,163 +77,177 @@
     def exceptions(self) -> Exceptions:
         """
         BackupStorageClient exceptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.exceptions)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#exceptions)
         """
+
     def can_paginate(self, operation_name: str) -> bool:
         """
         Check if an operation can be paginated.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.can_paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#can_paginate)
         """
+
     async def close(self) -> None:
         """
         Closes underlying endpoint connections.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#close)
         """
+
     async def delete_object(
         self, *, BackupJobId: str, ObjectName: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Delete Object from the incremental base Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.delete_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#delete_object)
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
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.generate_presigned_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#generate_presigned_url)
         """
+
     async def get_chunk(self, *, StorageJobId: str, ChunkToken: str) -> GetChunkOutputTypeDef:
         """
         Gets the specified object's chunk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.get_chunk)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#get_chunk)
         """
+
     async def get_object_metadata(
         self, *, StorageJobId: str, ObjectToken: str
     ) -> GetObjectMetadataOutputTypeDef:
         """
         Get metadata associated with an Object.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.get_object_metadata)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#get_object_metadata)
         """
+
     async def list_chunks(
         self, *, StorageJobId: str, ObjectToken: str, MaxResults: int = ..., NextToken: str = ...
     ) -> ListChunksOutputTypeDef:
         """
         List chunks in a given Object See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/ListChunks).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_chunks)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#list_chunks)
         """
+
     async def list_objects(
         self,
         *,
         StorageJobId: str,
         StartingObjectName: str = ...,
         StartingObjectPrefix: str = ...,
         MaxResults: int = ...,
         NextToken: str = ...,
-        CreatedBefore: Union[datetime, str] = ...,
-        CreatedAfter: Union[datetime, str] = ...
+        CreatedBefore: TimestampTypeDef = ...,
+        CreatedAfter: TimestampTypeDef = ...
     ) -> ListObjectsOutputTypeDef:
         """
         List all Objects in a given Backup.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.list_objects)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#list_objects)
         """
+
     async def notify_object_complete(
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ObjectChecksum: str,
         ObjectChecksumAlgorithm: Literal["SUMMARY"],
         MetadataString: str = ...,
-        MetadataBlob: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        MetadataBlob: BlobTypeDef = ...,
         MetadataBlobLength: int = ...,
         MetadataBlobChecksum: str = ...,
         MetadataBlobChecksumAlgorithm: Literal["SHA256"] = ...
     ) -> NotifyObjectCompleteOutputTypeDef:
         """
         Complete upload See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/backupstorage-2018-04-10/NotifyObjectComplete).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.notify_object_complete)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#notify_object_complete)
         """
+
     async def put_chunk(
         self,
         *,
         BackupJobId: str,
         UploadId: str,
         ChunkIndex: int,
-        Data: Union[str, bytes, IO[Any], StreamingBody],
+        Data: BlobTypeDef,
         Length: int,
         Checksum: str,
         ChecksumAlgorithm: Literal["SHA256"]
     ) -> PutChunkOutputTypeDef:
         """
         Upload chunk.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_chunk)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#put_chunk)
         """
+
     async def put_object(
         self,
         *,
         BackupJobId: str,
         ObjectName: str,
         MetadataString: str = ...,
-        InlineChunk: Union[str, bytes, IO[Any], StreamingBody] = ...,
+        InlineChunk: BlobTypeDef = ...,
         InlineChunkLength: int = ...,
         InlineChunkChecksum: str = ...,
         InlineChunkChecksumAlgorithm: str = ...,
         ObjectChecksum: str = ...,
         ObjectChecksumAlgorithm: Literal["SUMMARY"] = ...,
         ThrowOnDuplicate: bool = ...
     ) -> PutObjectOutputTypeDef:
         """
         Upload object that can store object metadata String and data blob in single API
         call using inline chunk field.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.put_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#put_object)
         """
+
     async def start_object(
         self, *, BackupJobId: str, ObjectName: str, ThrowOnDuplicate: bool = ...
     ) -> StartObjectOutputTypeDef:
         """
         Start upload containing one or many chunks.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client.start_object)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/#start_object)
         """
+
     async def __aenter__(self) -> "BackupStorageClient":
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/)
         """
+
     async def __aexit__(self, exc_type: Any, exc_val: Any, exc_tb: Any) -> Any:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage.Client)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/client/)
         """
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/literals.py` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/literals.pyi` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/type_defs.py` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_backupstorage.type_defs import BackupObjectTypeDef
 
-    data: BackupObjectTypeDef = {...}
+    data: BackupObjectTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from aiobotocore.response import StreamingBody
@@ -25,34 +25,36 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BackupObjectTypeDef",
+    "BlobTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
-    "GetChunkOutputTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
-    "GetObjectMetadataOutputTypeDef",
     "ListChunksInputRequestTypeDef",
-    "ListObjectsInputRequestTypeDef",
+    "TimestampTypeDef",
+    "StartObjectInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
-    "NotifyObjectCompleteOutputTypeDef",
     "PutChunkInputRequestTypeDef",
-    "PutChunkOutputTypeDef",
     "PutObjectInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetChunkOutputTypeDef",
+    "GetObjectMetadataOutputTypeDef",
+    "ListChunksOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "NotifyObjectCompleteOutputTypeDef",
+    "PutChunkOutputTypeDef",
     "PutObjectOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartObjectInputRequestTypeDef",
     "StartObjectOutputTypeDef",
-    "ListObjectsOutputTypeDef",
-    "ListChunksOutputTypeDef",
+    "ListObjectsInputRequestTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -70,14 +72,15 @@
 )
 
 
 class BackupObjectTypeDef(_RequiredBackupObjectTypeDef, _OptionalBackupObjectTypeDef):
     pass
 
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChunkTypeDef = TypedDict(
     "ChunkTypeDef",
     {
         "Index": int,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
@@ -89,60 +92,41 @@
     "DeleteObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetChunkInputRequestTypeDef = TypedDict(
     "GetChunkInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ChunkToken": str,
     },
 )
 
-GetChunkOutputTypeDef = TypedDict(
-    "GetChunkOutputTypeDef",
-    {
-        "Data": StreamingBody,
-        "Length": int,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectMetadataInputRequestTypeDef = TypedDict(
     "GetObjectMetadataInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
 
-GetObjectMetadataOutputTypeDef = TypedDict(
-    "GetObjectMetadataOutputTypeDef",
-    {
-        "MetadataString": str,
-        "MetadataBlob": StreamingBody,
-        "MetadataBlobLength": int,
-        "MetadataBlobChecksum": str,
-        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChunksInputRequestTypeDef = TypedDict(
     "_RequiredListChunksInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
@@ -158,36 +142,33 @@
 
 class ListChunksInputRequestTypeDef(
     _RequiredListChunksInputRequestTypeDef, _OptionalListChunksInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListObjectsInputRequestTypeDef = TypedDict(
-    "_RequiredListObjectsInputRequestTypeDef",
+TimestampTypeDef = Union[datetime, str]
+_RequiredStartObjectInputRequestTypeDef = TypedDict(
+    "_RequiredStartObjectInputRequestTypeDef",
     {
-        "StorageJobId": str,
+        "BackupJobId": str,
+        "ObjectName": str,
     },
 )
-_OptionalListObjectsInputRequestTypeDef = TypedDict(
-    "_OptionalListObjectsInputRequestTypeDef",
+_OptionalStartObjectInputRequestTypeDef = TypedDict(
+    "_OptionalStartObjectInputRequestTypeDef",
     {
-        "StartingObjectName": str,
-        "StartingObjectPrefix": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
+        "ThrowOnDuplicate": bool,
     },
     total=False,
 )
 
 
-class ListObjectsInputRequestTypeDef(
-    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+class StartObjectInputRequestTypeDef(
+    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
 
 _RequiredNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_RequiredNotifyObjectCompleteInputRequestTypeDef",
     {
@@ -197,15 +178,15 @@
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
     },
 )
 _OptionalNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_OptionalNotifyObjectCompleteInputRequestTypeDef",
     {
         "MetadataString": str,
-        "MetadataBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "MetadataBlob": BlobTypeDef,
         "MetadataBlobLength": int,
         "MetadataBlobChecksum": str,
         "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
     },
     total=False,
 )
 
@@ -213,57 +194,39 @@
 class NotifyObjectCompleteInputRequestTypeDef(
     _RequiredNotifyObjectCompleteInputRequestTypeDef,
     _OptionalNotifyObjectCompleteInputRequestTypeDef,
 ):
     pass
 
 
-NotifyObjectCompleteOutputTypeDef = TypedDict(
-    "NotifyObjectCompleteOutputTypeDef",
-    {
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
-PutChunkOutputTypeDef = TypedDict(
-    "PutChunkOutputTypeDef",
-    {
-        "ChunkChecksum": str,
-        "ChunkChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
     "_RequiredPutObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
 _OptionalPutObjectInputRequestTypeDef = TypedDict(
     "_OptionalPutObjectInputRequestTypeDef",
     {
         "MetadataString": str,
-        "InlineChunk": Union[str, bytes, IO[Any], StreamingBody],
+        "InlineChunk": BlobTypeDef,
         "InlineChunkLength": int,
         "InlineChunkChecksum": str,
         "InlineChunkChecksumAlgorithm": str,
         "ObjectChecksum": str,
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
         "ThrowOnDuplicate": bool,
     },
@@ -273,76 +236,116 @@
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "InlineChunkChecksum": str,
-        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetChunkOutputTypeDef = TypedDict(
+    "GetChunkOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Data": StreamingBody,
+        "Length": int,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartObjectInputRequestTypeDef = TypedDict(
-    "_RequiredStartObjectInputRequestTypeDef",
+GetObjectMetadataOutputTypeDef = TypedDict(
+    "GetObjectMetadataOutputTypeDef",
     {
-        "BackupJobId": str,
-        "ObjectName": str,
+        "MetadataString": str,
+        "MetadataBlob": StreamingBody,
+        "MetadataBlobLength": int,
+        "MetadataBlobChecksum": str,
+        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartObjectInputRequestTypeDef = TypedDict(
-    "_OptionalStartObjectInputRequestTypeDef",
+
+ListChunksOutputTypeDef = TypedDict(
+    "ListChunksOutputTypeDef",
     {
-        "ThrowOnDuplicate": bool,
+        "ChunkList": List[ChunkTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
+    {
+        "ObjectList": List[BackupObjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class StartObjectInputRequestTypeDef(
-    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
-):
-    pass
+NotifyObjectCompleteOutputTypeDef = TypedDict(
+    "NotifyObjectCompleteOutputTypeDef",
+    {
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
+PutChunkOutputTypeDef = TypedDict(
+    "PutChunkOutputTypeDef",
+    {
+        "ChunkChecksum": str,
+        "ChunkChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "InlineChunkChecksum": str,
+        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 StartObjectOutputTypeDef = TypedDict(
     "StartObjectOutputTypeDef",
     {
         "UploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+_RequiredListObjectsInputRequestTypeDef = TypedDict(
+    "_RequiredListObjectsInputRequestTypeDef",
     {
-        "ObjectList": List[BackupObjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StorageJobId": str,
     },
 )
-
-ListChunksOutputTypeDef = TypedDict(
-    "ListChunksOutputTypeDef",
+_OptionalListObjectsInputRequestTypeDef = TypedDict(
+    "_OptionalListObjectsInputRequestTypeDef",
     {
-        "ChunkList": List[ChunkTypeDef],
+        "StartingObjectName": str,
+        "StartingObjectPrefix": str,
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
     },
+    total=False,
 )
+
+
+class ListObjectsInputRequestTypeDef(
+    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage/type_defs.pyi` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_backupstorage.type_defs import BackupObjectTypeDef
 
-    data: BackupObjectTypeDef = {...}
+    data: BackupObjectTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, List, Union
 
 from aiobotocore.response import StreamingBody
@@ -24,34 +24,36 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BackupObjectTypeDef",
+    "BlobTypeDef",
     "ChunkTypeDef",
     "DeleteObjectInputRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetChunkInputRequestTypeDef",
-    "GetChunkOutputTypeDef",
     "GetObjectMetadataInputRequestTypeDef",
-    "GetObjectMetadataOutputTypeDef",
     "ListChunksInputRequestTypeDef",
-    "ListObjectsInputRequestTypeDef",
+    "TimestampTypeDef",
+    "StartObjectInputRequestTypeDef",
     "NotifyObjectCompleteInputRequestTypeDef",
-    "NotifyObjectCompleteOutputTypeDef",
     "PutChunkInputRequestTypeDef",
-    "PutChunkOutputTypeDef",
     "PutObjectInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetChunkOutputTypeDef",
+    "GetObjectMetadataOutputTypeDef",
+    "ListChunksOutputTypeDef",
+    "ListObjectsOutputTypeDef",
+    "NotifyObjectCompleteOutputTypeDef",
+    "PutChunkOutputTypeDef",
     "PutObjectOutputTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartObjectInputRequestTypeDef",
     "StartObjectOutputTypeDef",
-    "ListObjectsOutputTypeDef",
-    "ListChunksOutputTypeDef",
+    "ListObjectsInputRequestTypeDef",
 )
 
 _RequiredBackupObjectTypeDef = TypedDict(
     "_RequiredBackupObjectTypeDef",
     {
         "Name": str,
         "ObjectChecksum": str,
@@ -67,14 +69,15 @@
     },
     total=False,
 )
 
 class BackupObjectTypeDef(_RequiredBackupObjectTypeDef, _OptionalBackupObjectTypeDef):
     pass
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ChunkTypeDef = TypedDict(
     "ChunkTypeDef",
     {
         "Index": int,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
@@ -86,60 +89,41 @@
     "DeleteObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetChunkInputRequestTypeDef = TypedDict(
     "GetChunkInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ChunkToken": str,
     },
 )
 
-GetChunkOutputTypeDef = TypedDict(
-    "GetChunkOutputTypeDef",
-    {
-        "Data": StreamingBody,
-        "Length": int,
-        "Checksum": str,
-        "ChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetObjectMetadataInputRequestTypeDef = TypedDict(
     "GetObjectMetadataInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
 
-GetObjectMetadataOutputTypeDef = TypedDict(
-    "GetObjectMetadataOutputTypeDef",
-    {
-        "MetadataString": str,
-        "MetadataBlob": StreamingBody,
-        "MetadataBlobLength": int,
-        "MetadataBlobChecksum": str,
-        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListChunksInputRequestTypeDef = TypedDict(
     "_RequiredListChunksInputRequestTypeDef",
     {
         "StorageJobId": str,
         "ObjectToken": str,
     },
 )
@@ -153,35 +137,32 @@
 )
 
 class ListChunksInputRequestTypeDef(
     _RequiredListChunksInputRequestTypeDef, _OptionalListChunksInputRequestTypeDef
 ):
     pass
 
-_RequiredListObjectsInputRequestTypeDef = TypedDict(
-    "_RequiredListObjectsInputRequestTypeDef",
+TimestampTypeDef = Union[datetime, str]
+_RequiredStartObjectInputRequestTypeDef = TypedDict(
+    "_RequiredStartObjectInputRequestTypeDef",
     {
-        "StorageJobId": str,
+        "BackupJobId": str,
+        "ObjectName": str,
     },
 )
-_OptionalListObjectsInputRequestTypeDef = TypedDict(
-    "_OptionalListObjectsInputRequestTypeDef",
+_OptionalStartObjectInputRequestTypeDef = TypedDict(
+    "_OptionalStartObjectInputRequestTypeDef",
     {
-        "StartingObjectName": str,
-        "StartingObjectPrefix": str,
-        "MaxResults": int,
-        "NextToken": str,
-        "CreatedBefore": Union[datetime, str],
-        "CreatedAfter": Union[datetime, str],
+        "ThrowOnDuplicate": bool,
     },
     total=False,
 )
 
-class ListObjectsInputRequestTypeDef(
-    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+class StartObjectInputRequestTypeDef(
+    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
 ):
     pass
 
 _RequiredNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_RequiredNotifyObjectCompleteInputRequestTypeDef",
     {
         "BackupJobId": str,
@@ -190,71 +171,53 @@
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
     },
 )
 _OptionalNotifyObjectCompleteInputRequestTypeDef = TypedDict(
     "_OptionalNotifyObjectCompleteInputRequestTypeDef",
     {
         "MetadataString": str,
-        "MetadataBlob": Union[str, bytes, IO[Any], StreamingBody],
+        "MetadataBlob": BlobTypeDef,
         "MetadataBlobLength": int,
         "MetadataBlobChecksum": str,
         "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
     },
     total=False,
 )
 
 class NotifyObjectCompleteInputRequestTypeDef(
     _RequiredNotifyObjectCompleteInputRequestTypeDef,
     _OptionalNotifyObjectCompleteInputRequestTypeDef,
 ):
     pass
 
-NotifyObjectCompleteOutputTypeDef = TypedDict(
-    "NotifyObjectCompleteOutputTypeDef",
-    {
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 PutChunkInputRequestTypeDef = TypedDict(
     "PutChunkInputRequestTypeDef",
     {
         "BackupJobId": str,
         "UploadId": str,
         "ChunkIndex": int,
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "Length": int,
         "Checksum": str,
         "ChecksumAlgorithm": Literal["SHA256"],
     },
 )
 
-PutChunkOutputTypeDef = TypedDict(
-    "PutChunkOutputTypeDef",
-    {
-        "ChunkChecksum": str,
-        "ChunkChecksumAlgorithm": Literal["SHA256"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredPutObjectInputRequestTypeDef = TypedDict(
     "_RequiredPutObjectInputRequestTypeDef",
     {
         "BackupJobId": str,
         "ObjectName": str,
     },
 )
 _OptionalPutObjectInputRequestTypeDef = TypedDict(
     "_OptionalPutObjectInputRequestTypeDef",
     {
         "MetadataString": str,
-        "InlineChunk": Union[str, bytes, IO[Any], StreamingBody],
+        "InlineChunk": BlobTypeDef,
         "InlineChunkLength": int,
         "InlineChunkChecksum": str,
         "InlineChunkChecksumAlgorithm": str,
         "ObjectChecksum": str,
         "ObjectChecksumAlgorithm": Literal["SUMMARY"],
         "ThrowOnDuplicate": bool,
     },
@@ -262,74 +225,115 @@
 )
 
 class PutObjectInputRequestTypeDef(
     _RequiredPutObjectInputRequestTypeDef, _OptionalPutObjectInputRequestTypeDef
 ):
     pass
 
-PutObjectOutputTypeDef = TypedDict(
-    "PutObjectOutputTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "InlineChunkChecksum": str,
-        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
-        "ObjectChecksum": str,
-        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+GetChunkOutputTypeDef = TypedDict(
+    "GetChunkOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Data": StreamingBody,
+        "Length": int,
+        "Checksum": str,
+        "ChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredStartObjectInputRequestTypeDef = TypedDict(
-    "_RequiredStartObjectInputRequestTypeDef",
+GetObjectMetadataOutputTypeDef = TypedDict(
+    "GetObjectMetadataOutputTypeDef",
     {
-        "BackupJobId": str,
-        "ObjectName": str,
+        "MetadataString": str,
+        "MetadataBlob": StreamingBody,
+        "MetadataBlobLength": int,
+        "MetadataBlobChecksum": str,
+        "MetadataBlobChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-_OptionalStartObjectInputRequestTypeDef = TypedDict(
-    "_OptionalStartObjectInputRequestTypeDef",
+
+ListChunksOutputTypeDef = TypedDict(
+    "ListChunksOutputTypeDef",
     {
-        "ThrowOnDuplicate": bool,
+        "ChunkList": List[ChunkTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class StartObjectInputRequestTypeDef(
-    _RequiredStartObjectInputRequestTypeDef, _OptionalStartObjectInputRequestTypeDef
-):
-    pass
+ListObjectsOutputTypeDef = TypedDict(
+    "ListObjectsOutputTypeDef",
+    {
+        "ObjectList": List[BackupObjectTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+NotifyObjectCompleteOutputTypeDef = TypedDict(
+    "NotifyObjectCompleteOutputTypeDef",
+    {
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutChunkOutputTypeDef = TypedDict(
+    "PutChunkOutputTypeDef",
+    {
+        "ChunkChecksum": str,
+        "ChunkChecksumAlgorithm": Literal["SHA256"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutObjectOutputTypeDef = TypedDict(
+    "PutObjectOutputTypeDef",
+    {
+        "InlineChunkChecksum": str,
+        "InlineChunkChecksumAlgorithm": Literal["SHA256"],
+        "ObjectChecksum": str,
+        "ObjectChecksumAlgorithm": Literal["SUMMARY"],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 StartObjectOutputTypeDef = TypedDict(
     "StartObjectOutputTypeDef",
     {
         "UploadId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ListObjectsOutputTypeDef = TypedDict(
-    "ListObjectsOutputTypeDef",
+_RequiredListObjectsInputRequestTypeDef = TypedDict(
+    "_RequiredListObjectsInputRequestTypeDef",
     {
-        "ObjectList": List[BackupObjectTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "StorageJobId": str,
     },
 )
-
-ListChunksOutputTypeDef = TypedDict(
-    "ListChunksOutputTypeDef",
+_OptionalListObjectsInputRequestTypeDef = TypedDict(
+    "_OptionalListObjectsInputRequestTypeDef",
     {
-        "ChunkList": List[ChunkTypeDef],
+        "StartingObjectName": str,
+        "StartingObjectPrefix": str,
+        "MaxResults": int,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "CreatedBefore": TimestampTypeDef,
+        "CreatedAfter": TimestampTypeDef,
     },
+    total=False,
 )
+
+class ListObjectsInputRequestTypeDef(
+    _RequiredListObjectsInputRequestTypeDef, _OptionalListObjectsInputRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/PKG-INFO` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-backupstorage
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.BackupStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore backupstorage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore backupstorage type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-backupstorage"></a>
 
 # types-aiobotocore-backupstorage
 
 [![PyPI - types-aiobotocore-backupstorage](https://img.shields.io/pypi/v/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-backupstorage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-backupstorage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-backupstorage?color=blue)](https://pypistats.org/packages/types-aiobotocore-backupstorage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-backupstorage)](https://pepy.tech/project/types-aiobotocore-backupstorage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.BackupStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/backupstorage.html#BackupStorage)
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
 [types-aiobotocore-backupstorage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_backupstorage/).
 
 See how it helps to find and fix potential bugs:
 
@@ -73,15 +72,15 @@
     - [Sublime Text](#sublime-text)
     - [Other IDEs](#other-ides)
     - [mypy](#mypy)
     - [pyright](#pyright)
   - [Explicit type annotations](#explicit-type-annotations)
     - [Client annotations](#client-annotations)
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
@@ -282,48 +281,50 @@
 )
 
 
 def check_value(value: DataChecksumAlgorithmType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_backupstorage.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_backupstorage.type_defs import (
     BackupObjectTypeDef,
+    BlobTypeDef,
     ChunkTypeDef,
     DeleteObjectInputRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetChunkInputRequestTypeDef,
-    GetChunkOutputTypeDef,
     GetObjectMetadataInputRequestTypeDef,
-    GetObjectMetadataOutputTypeDef,
     ListChunksInputRequestTypeDef,
-    ListObjectsInputRequestTypeDef,
+    TimestampTypeDef,
+    StartObjectInputRequestTypeDef,
     NotifyObjectCompleteInputRequestTypeDef,
-    NotifyObjectCompleteOutputTypeDef,
     PutChunkInputRequestTypeDef,
-    PutChunkOutputTypeDef,
     PutObjectInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetChunkOutputTypeDef,
+    GetObjectMetadataOutputTypeDef,
+    ListChunksOutputTypeDef,
+    ListObjectsOutputTypeDef,
+    NotifyObjectCompleteOutputTypeDef,
+    PutChunkOutputTypeDef,
     PutObjectOutputTypeDef,
-    ResponseMetadataTypeDef,
-    StartObjectInputRequestTypeDef,
     StartObjectOutputTypeDef,
-    ListObjectsOutputTypeDef,
-    ListChunksOutputTypeDef,
+    ListObjectsInputRequestTypeDef,
 )
 
 
-def get_structure() -> BackupObjectTypeDef:
+def get_value() -> BackupObjectTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-backupstorage-2.5.2/types_aiobotocore_backupstorage.egg-info/SOURCES.txt` & `types-aiobotocore-backupstorage-2.5.2.post1/types_aiobotocore_backupstorage.egg-info/SOURCES.txt`

 * *Files identical despite different names*


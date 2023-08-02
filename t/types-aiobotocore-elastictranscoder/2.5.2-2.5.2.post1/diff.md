# Comparing `tmp/types-aiobotocore-elastictranscoder-2.5.2.tar.gz` & `tmp/types-aiobotocore-elastictranscoder-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-elastictranscoder-2.5.2.tar", last modified: Sat Jul  8 01:43:35 2023, max compression
+gzip compressed data, was "types-aiobotocore-elastictranscoder-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:14 2023, max compression
```

## Comparing `types-aiobotocore-elastictranscoder-2.5.2.tar` & `types-aiobotocore-elastictranscoder-2.5.2.post1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.542092 types-aiobotocore-elastictranscoder-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-07-08 01:43:35.534092 types-aiobotocore-elastictranscoder-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15315 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:35.542092 types-aiobotocore-elastictranscoder-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.526092 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    18529 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22891 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22872 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:30:28.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-08 01:30:29.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:35.534092 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16920 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-08 01:43:35.000000 types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-08-02 14:38:16.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18610 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8426 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25515 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25497 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-08-02 14:38:17.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:14.825593 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17171 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 14:52:14.000000 types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/LICENSE` & `types-aiobotocore-elastictranscoder-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elastictranscoder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elastictranscoder"></a>
 
 # types-aiobotocore-elastictranscoder
 
 [![PyPI - types-aiobotocore-elastictranscoder](https://img.shields.io/pypi/v/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastictranscoder?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastictranscoder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastictranscoder)](https://pepy.tech/project/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticTranscoder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
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
@@ -345,97 +344,107 @@
 )
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elastictranscoder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DetectedPropertiesTypeDef,
     TimingTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PermissionOutputTypeDef,
     PermissionTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
     AudioParametersTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
     PlaylistTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
+    VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
+    JobAlbumArtOutputTypeDef,
     JobAlbumArtTypeDef,
+    CaptionsOutputTypeDef,
     CaptionsTypeDef,
+    InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
-    CreateJobOutputTypeDef,
+    CreatePresetRequestRequestTypeDef,
+    VideoParametersUnionTypeDef,
     JobOutputTypeDef,
+    CreateJobOutputTypeDef,
+    JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
+    JobInputUnionTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/README.md` & `types-aiobotocore-elastictranscoder-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-elastictranscoder"></a>
 
 # types-aiobotocore-elastictranscoder
 
 [![PyPI - types-aiobotocore-elastictranscoder](https://img.shields.io/pypi/v/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastictranscoder?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastictranscoder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastictranscoder)](https://pepy.tech/project/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticTranscoder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
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
@@ -312,97 +312,107 @@
 )
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elastictranscoder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DetectedPropertiesTypeDef,
     TimingTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PermissionOutputTypeDef,
     PermissionTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
     AudioParametersTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
     PlaylistTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
+    VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
+    JobAlbumArtOutputTypeDef,
     JobAlbumArtTypeDef,
+    CaptionsOutputTypeDef,
     CaptionsTypeDef,
+    InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
-    CreateJobOutputTypeDef,
+    CreatePresetRequestRequestTypeDef,
+    VideoParametersUnionTypeDef,
     JobOutputTypeDef,
+    CreateJobOutputTypeDef,
+    JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
+    JobInputUnionTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/setup.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-elastictranscoder",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_elastictranscoder"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with"
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
-    keywords=(
-        "aiobotocore elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore elastictranscoder type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_elastictranscoder": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/"
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__init__.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/__main__.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ElasticTranscoder 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ElasticTranscoder 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder\nOther"
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

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 from .type_defs import (
     AudioParametersTypeDef,
     CreateJobOutputTypeDef,
     CreateJobPlaylistTypeDef,
     CreateJobResponseTypeDef,
     CreatePipelineResponseTypeDef,
     CreatePresetResponseTypeDef,
-    JobInputTypeDef,
+    JobInputUnionTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListPresetsResponseTypeDef,
     NotificationsTypeDef,
-    PipelineOutputConfigTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     ReadJobResponseTypeDef,
     ReadPipelineResponseTypeDef,
     ReadPresetResponseTypeDef,
     TestRoleResponseTypeDef,
     ThumbnailsTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
-    VideoParametersTypeDef,
+    VideoParametersUnionTypeDef,
 )
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -121,16 +121,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#close)
         """
 
     async def create_job(
         self,
         *,
         PipelineId: str,
-        Input: JobInputTypeDef = ...,
-        Inputs: Sequence[JobInputTypeDef] = ...,
+        Input: JobInputUnionTypeDef = ...,
+        Inputs: Sequence[JobInputUnionTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
         UserMetadata: Mapping[str, str] = ...
     ) -> CreateJobResponseTypeDef:
         """
@@ -146,31 +146,31 @@
         *,
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_pipeline)
         """
 
     async def create_preset(
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
-        Video: VideoParametersTypeDef = ...,
+        Video: VideoParametersUnionTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
         Thumbnails: ThumbnailsTypeDef = ...
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
@@ -289,16 +289,16 @@
         *,
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/client.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/client.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -29,30 +29,30 @@
 from .type_defs import (
     AudioParametersTypeDef,
     CreateJobOutputTypeDef,
     CreateJobPlaylistTypeDef,
     CreateJobResponseTypeDef,
     CreatePipelineResponseTypeDef,
     CreatePresetResponseTypeDef,
-    JobInputTypeDef,
+    JobInputUnionTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ListPresetsResponseTypeDef,
     NotificationsTypeDef,
-    PipelineOutputConfigTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     ReadJobResponseTypeDef,
     ReadPipelineResponseTypeDef,
     ReadPresetResponseTypeDef,
     TestRoleResponseTypeDef,
     ThumbnailsTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
-    VideoParametersTypeDef,
+    VideoParametersUnionTypeDef,
 )
 from .waiter import JobCompleteWaiter
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
@@ -113,16 +113,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.close)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#close)
         """
     async def create_job(
         self,
         *,
         PipelineId: str,
-        Input: JobInputTypeDef = ...,
-        Inputs: Sequence[JobInputTypeDef] = ...,
+        Input: JobInputUnionTypeDef = ...,
+        Inputs: Sequence[JobInputUnionTypeDef] = ...,
         Output: CreateJobOutputTypeDef = ...,
         Outputs: Sequence[CreateJobOutputTypeDef] = ...,
         OutputKeyPrefix: str = ...,
         Playlists: Sequence[CreateJobPlaylistTypeDef] = ...,
         UserMetadata: Mapping[str, str] = ...
     ) -> CreateJobResponseTypeDef:
         """
@@ -137,30 +137,30 @@
         *,
         Name: str,
         InputBucket: str,
         Role: str,
         OutputBucket: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> CreatePipelineResponseTypeDef:
         """
         The CreatePipeline operation creates a pipeline with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#create_pipeline)
         """
     async def create_preset(
         self,
         *,
         Name: str,
         Container: str,
         Description: str = ...,
-        Video: VideoParametersTypeDef = ...,
+        Video: VideoParametersUnionTypeDef = ...,
         Audio: AudioParametersTypeDef = ...,
         Thumbnails: ThumbnailsTypeDef = ...
     ) -> CreatePresetResponseTypeDef:
         """
         The CreatePreset operation creates a preset with settings that you specify.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.create_preset)
@@ -267,16 +267,16 @@
         *,
         Id: str,
         Name: str = ...,
         InputBucket: str = ...,
         Role: str = ...,
         AwsKmsKeyArn: str = ...,
         Notifications: NotificationsTypeDef = ...,
-        ContentConfig: PipelineOutputConfigTypeDef = ...,
-        ThumbnailConfig: PipelineOutputConfigTypeDef = ...
+        ContentConfig: PipelineOutputConfigUnionTypeDef = ...,
+        ThumbnailConfig: PipelineOutputConfigUnionTypeDef = ...
     ) -> UpdatePipelineResponseTypeDef:
         """
         Use the `UpdatePipeline` operation to update settings for a pipeline.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Client.update_pipeline)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/client/#update_pipeline)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/literals.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,58 +64,58 @@
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsByPipelineResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
 
 class ListJobsByStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbystatuspaginator)
     """
 
     def paginate(
-        self, *, Status: str, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: str, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsByStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbystatuspaginator)
         """
 
 
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpipelinespaginator)
         """
 
 
 class ListPresetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpresetspaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpresetspaginator)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/paginator.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -61,55 +61,55 @@
     """
 
     def paginate(
         self,
         *,
         PipelineId: str,
         Ascending: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsByPipelineResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByPipeline.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbypipelinepaginator)
         """
 
 class ListJobsByStatusPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbystatuspaginator)
     """
 
     def paginate(
-        self, *, Status: str, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: str, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListJobsByStatusResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListJobsByStatus.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listjobsbystatuspaginator)
         """
 
 class ListPipelinesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpipelinespaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPipelinesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPipelines.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpipelinespaginator)
         """
 
 class ListPresetsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpresetspaginator)
     """
 
     def paginate(
-        self, *, Ascending: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Ascending: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListPresetsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder.Paginator.ListPresets.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/paginators/#listpresetspaginator)
         """
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,97 +4,107 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef
 
-    data: EncryptionTypeDef = {...}
+    data: EncryptionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "EncryptionTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DetectedPropertiesTypeDef",
     "TimingTypeDef",
-    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
-    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "PermissionOutputTypeDef",
     "PermissionTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
-    "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
     "AudioParametersTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
     "PlaylistTypeDef",
+    "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
+    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
+    "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
+    "JobAlbumArtOutputTypeDef",
     "JobAlbumArtTypeDef",
+    "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
+    "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
+    "PipelineOutputConfigUnionTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "CreatePresetRequestRequestTypeDef",
     "PresetTypeDef",
-    "CreateJobOutputTypeDef",
+    "CreatePresetRequestRequestTypeDef",
+    "VideoParametersUnionTypeDef",
     "JobOutputTypeDef",
+    "CreateJobOutputTypeDef",
+    "JobInputOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
+    "JobInputUnionTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
 )
 
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
@@ -153,14 +163,25 @@
         "KeyId": str,
         "InitializationVector": str,
         "LicenseAcquisitionUrl": str,
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
 NotificationsTypeDef = TypedDict(
     "NotificationsTypeDef",
     {
         "Progressing": str,
         "Completed": str,
         "Warning": str,
         "Error": str,
@@ -224,37 +245,24 @@
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
     total=False,
 )
 
-_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
-    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobsByPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByPipelineRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalListJobsByPipelineRequestRequestTypeDef = TypedDict(
@@ -270,37 +278,14 @@
 class ListJobsByPipelineRequestRequestTypeDef(
     _RequiredListJobsByPipelineRequestRequestTypeDef,
     _OptionalListJobsByPipelineRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Status": str,
-    },
-)
-_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
-    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListJobsByStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByStatusRequestRequestTypeDef",
     {
         "Status": str,
     },
 )
 _OptionalListJobsByStatusRequestRequestTypeDef = TypedDict(
@@ -315,56 +300,38 @@
 
 class ListJobsByStatusRequestRequestTypeDef(
     _RequiredListJobsByStatusRequestRequestTypeDef, _OptionalListJobsByStatusRequestRequestTypeDef
 ):
     pass
 
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PermissionOutputTypeDef = TypedDict(
+    "PermissionOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "GranteeType": str,
+        "Grantee": str,
+        "Access": List[str],
     },
     total=False,
 )
 
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
@@ -418,44 +385,24 @@
 ReadPresetRequestRequestTypeDef = TypedDict(
     "ReadPresetRequestRequestTypeDef",
     {
         "Id": str,
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
 TestRoleRequestRequestTypeDef = TypedDict(
     "TestRoleRequestRequestTypeDef",
     {
         "Role": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Topics": Sequence[str],
     },
 )
 
-TestRoleResponseTypeDef = TypedDict(
-    "TestRoleResponseTypeDef",
-    {
-        "Success": str,
-        "Messages": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePipelineStatusRequestRequestTypeDef = TypedDict(
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
@@ -549,32 +496,137 @@
         "PlayReadyDrm": PlayReadyDrmTypeDef,
         "Status": str,
         "StatusDetail": str,
     },
     total=False,
 )
 
+TestRoleResponseTypeDef = TypedDict(
+    "TestRoleResponseTypeDef",
+    {
+        "Success": str,
+        "Messages": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
+_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
+    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+):
+    pass
+
+
+_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Status": str,
+    },
+)
+_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
+    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+):
+    pass
+
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+PipelineOutputConfigOutputTypeDef = TypedDict(
+    "PipelineOutputConfigOutputTypeDef",
+    {
+        "Bucket": str,
+        "StorageClass": str,
+        "Permissions": List[PermissionOutputTypeDef],
+    },
+    total=False,
+)
+
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
+VideoParametersOutputTypeDef = TypedDict(
+    "VideoParametersOutputTypeDef",
+    {
+        "Codec": str,
+        "CodecOptions": Dict[str, str],
+        "KeyframesMaxDist": str,
+        "FixedGOP": str,
+        "BitRate": str,
+        "FrameRate": str,
+        "MaxFrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "DisplayAspectRatio": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+        "Watermarks": List[PresetWatermarkTypeDef],
+    },
+    total=False,
+)
+
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
         "Codec": str,
         "CodecOptions": Mapping[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -610,42 +662,88 @@
 
 class ReadJobRequestJobCompleteWaitTypeDef(
     _RequiredReadJobRequestJobCompleteWaitTypeDef, _OptionalReadJobRequestJobCompleteWaitTypeDef
 ):
     pass
 
 
+JobAlbumArtOutputTypeDef = TypedDict(
+    "JobAlbumArtOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "Artwork": List[ArtworkTypeDef],
+    },
+    total=False,
+)
+
 JobAlbumArtTypeDef = TypedDict(
     "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
         "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
 )
 
+CaptionsOutputTypeDef = TypedDict(
+    "CaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceTypeDef],
+        "CaptionFormats": List[CaptionFormatTypeDef],
+    },
+    total=False,
+)
+
 CaptionsTypeDef = TypedDict(
     "CaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
         "CaptionFormats": Sequence[CaptionFormatTypeDef],
     },
     total=False,
 )
 
+InputCaptionsOutputTypeDef = TypedDict(
+    "InputCaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceTypeDef],
+    },
+    total=False,
+)
+
 InputCaptionsTypeDef = TypedDict(
     "InputCaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
     },
     total=False,
 )
 
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Status": str,
+        "InputBucket": str,
+        "OutputBucket": str,
+        "Role": str,
+        "AwsKmsKeyArn": str,
+        "Notifications": NotificationsTypeDef,
+        "ContentConfig": PipelineOutputConfigOutputTypeDef,
+        "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "Name": str,
         "InputBucket": str,
         "Role": str,
     },
@@ -665,32 +763,17 @@
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Status": str,
-        "InputBucket": str,
-        "OutputBucket": str,
-        "Role": str,
-        "AwsKmsKeyArn": str,
-        "Notifications": NotificationsTypeDef,
-        "ContentConfig": PipelineOutputConfigTypeDef,
-        "ThumbnailConfig": PipelineOutputConfigTypeDef,
-    },
-    total=False,
-)
-
+PipelineOutputConfigUnionTypeDef = Union[
+    PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef
+]
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -710,14 +793,30 @@
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Container": str,
+        "Audio": AudioParametersTypeDef,
+        "Video": VideoParametersOutputTypeDef,
+        "Thumbnails": ThumbnailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Container": str,
     },
 )
@@ -735,26 +834,39 @@
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
 
-PresetTypeDef = TypedDict(
-    "PresetTypeDef",
+VideoParametersUnionTypeDef = Union[VideoParametersTypeDef, VideoParametersOutputTypeDef]
+JobOutputTypeDef = TypedDict(
+    "JobOutputTypeDef",
     {
         "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Container": str,
-        "Audio": AudioParametersTypeDef,
-        "Video": VideoParametersTypeDef,
-        "Thumbnails": ThumbnailsTypeDef,
-        "Type": str,
+        "Key": str,
+        "ThumbnailPattern": str,
+        "ThumbnailEncryption": EncryptionTypeDef,
+        "Rotate": str,
+        "PresetId": str,
+        "SegmentDuration": str,
+        "Status": str,
+        "StatusDetail": str,
+        "Duration": int,
+        "Width": int,
+        "Height": int,
+        "FrameRate": str,
+        "FileSize": int,
+        "DurationMillis": int,
+        "Watermarks": List[JobWatermarkTypeDef],
+        "AlbumArt": JobAlbumArtOutputTypeDef,
+        "Composition": List[ClipTypeDef],
+        "Captions": CaptionsOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
+        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
@@ -769,38 +881,27 @@
         "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-JobOutputTypeDef = TypedDict(
-    "JobOutputTypeDef",
+JobInputOutputTypeDef = TypedDict(
+    "JobInputOutputTypeDef",
     {
-        "Id": str,
         "Key": str,
-        "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionTypeDef,
-        "Rotate": str,
-        "PresetId": str,
-        "SegmentDuration": str,
-        "Status": str,
-        "StatusDetail": str,
-        "Duration": int,
-        "Width": int,
-        "Height": int,
         "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-        "Watermarks": List[JobWatermarkTypeDef],
-        "AlbumArt": JobAlbumArtTypeDef,
-        "Composition": List[ClipTypeDef],
-        "Captions": CaptionsTypeDef,
+        "Resolution": str,
+        "AspectRatio": str,
+        "Interlaced": str,
+        "Container": str,
         "Encryption": EncryptionTypeDef,
-        "AppliedColorSpaceConversion": str,
+        "TimeSpan": TimeSpanTypeDef,
+        "InputCaptions": InputCaptionsOutputTypeDef,
+        "DetectedProperties": DetectedPropertiesTypeDef,
     },
     total=False,
 )
 
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
@@ -819,159 +920,159 @@
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "Pipelines": List[PipelineTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPipelineResponseTypeDef = TypedDict(
     "ReadPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineNotificationsResponseTypeDef = TypedDict(
     "UpdatePipelineNotificationsResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineStatusResponseTypeDef = TypedDict(
     "UpdatePipelineStatusResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "Presets": List[PresetTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPresetResponseTypeDef = TypedDict(
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Input": JobInputTypeDef,
-        "Inputs": Sequence[JobInputTypeDef],
-        "Output": CreateJobOutputTypeDef,
-        "Outputs": Sequence[CreateJobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": Sequence[CreateJobPlaylistTypeDef],
-        "UserMetadata": Mapping[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
-
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PipelineId": str,
-        "Input": JobInputTypeDef,
-        "Inputs": List[JobInputTypeDef],
+        "Input": JobInputOutputTypeDef,
+        "Inputs": List[JobInputOutputTypeDef],
         "Output": JobOutputTypeDef,
         "Outputs": List[JobOutputTypeDef],
         "OutputKeyPrefix": str,
         "Playlists": List[PlaylistTypeDef],
         "Status": str,
         "UserMetadata": Dict[str, str],
         "Timing": TimingTypeDef,
     },
     total=False,
 )
 
+JobInputUnionTypeDef = Union[JobInputTypeDef, JobInputOutputTypeDef]
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByPipelineResponseTypeDef = TypedDict(
     "ListJobsByPipelineResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByStatusResponseTypeDef = TypedDict(
     "ListJobsByStatusResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Input": JobInputTypeDef,
+        "Inputs": Sequence[JobInputUnionTypeDef],
+        "Output": CreateJobOutputTypeDef,
+        "Outputs": Sequence[CreateJobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": Sequence[CreateJobPlaylistTypeDef],
+        "UserMetadata": Mapping[str, str],
     },
+    total=False,
 )
+
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/type_defs.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -4,96 +4,106 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_elastictranscoder.type_defs import EncryptionTypeDef
 
-    data: EncryptionTypeDef = {...}
+    data: EncryptionTypeDef = ...
     ```
 """
 import sys
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "EncryptionTypeDef",
     "AudioCodecOptionsTypeDef",
     "CancelJobRequestRequestTypeDef",
     "TimeSpanTypeDef",
     "HlsContentProtectionTypeDef",
     "PlayReadyDrmTypeDef",
+    "ResponseMetadataTypeDef",
     "NotificationsTypeDef",
     "WarningTypeDef",
     "ThumbnailsTypeDef",
     "DeletePipelineRequestRequestTypeDef",
     "DeletePresetRequestRequestTypeDef",
     "DetectedPropertiesTypeDef",
     "TimingTypeDef",
-    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListJobsByPipelineRequestRequestTypeDef",
-    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
     "ListJobsByStatusRequestRequestTypeDef",
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
     "ListPipelinesRequestRequestTypeDef",
-    "ListPresetsRequestListPresetsPaginateTypeDef",
     "ListPresetsRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
+    "PermissionOutputTypeDef",
     "PermissionTypeDef",
     "PresetWatermarkTypeDef",
     "WaiterConfigTypeDef",
     "ReadJobRequestRequestTypeDef",
     "ReadPipelineRequestRequestTypeDef",
     "ReadPresetRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "TestRoleRequestRequestTypeDef",
-    "TestRoleResponseTypeDef",
     "UpdatePipelineStatusRequestRequestTypeDef",
     "ArtworkTypeDef",
     "CaptionFormatTypeDef",
     "CaptionSourceTypeDef",
     "JobWatermarkTypeDef",
     "AudioParametersTypeDef",
     "ClipTypeDef",
     "CreateJobPlaylistTypeDef",
     "PlaylistTypeDef",
+    "TestRoleResponseTypeDef",
     "UpdatePipelineNotificationsRequestRequestTypeDef",
+    "ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    "ListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    "PipelineOutputConfigOutputTypeDef",
     "PipelineOutputConfigTypeDef",
+    "VideoParametersOutputTypeDef",
     "VideoParametersTypeDef",
     "ReadJobRequestJobCompleteWaitTypeDef",
+    "JobAlbumArtOutputTypeDef",
     "JobAlbumArtTypeDef",
+    "CaptionsOutputTypeDef",
     "CaptionsTypeDef",
+    "InputCaptionsOutputTypeDef",
     "InputCaptionsTypeDef",
-    "CreatePipelineRequestRequestTypeDef",
     "PipelineTypeDef",
+    "CreatePipelineRequestRequestTypeDef",
+    "PipelineOutputConfigUnionTypeDef",
     "UpdatePipelineRequestRequestTypeDef",
-    "CreatePresetRequestRequestTypeDef",
     "PresetTypeDef",
-    "CreateJobOutputTypeDef",
+    "CreatePresetRequestRequestTypeDef",
+    "VideoParametersUnionTypeDef",
     "JobOutputTypeDef",
+    "CreateJobOutputTypeDef",
+    "JobInputOutputTypeDef",
     "JobInputTypeDef",
     "CreatePipelineResponseTypeDef",
     "ListPipelinesResponseTypeDef",
     "ReadPipelineResponseTypeDef",
     "UpdatePipelineNotificationsResponseTypeDef",
     "UpdatePipelineResponseTypeDef",
     "UpdatePipelineStatusResponseTypeDef",
     "CreatePresetResponseTypeDef",
     "ListPresetsResponseTypeDef",
     "ReadPresetResponseTypeDef",
-    "CreateJobRequestRequestTypeDef",
     "JobTypeDef",
+    "JobInputUnionTypeDef",
     "CreateJobResponseTypeDef",
     "ListJobsByPipelineResponseTypeDef",
     "ListJobsByStatusResponseTypeDef",
     "ReadJobResponseTypeDef",
+    "CreateJobRequestRequestTypeDef",
 )
 
 EncryptionTypeDef = TypedDict(
     "EncryptionTypeDef",
     {
         "Mode": str,
         "Key": str,
@@ -152,14 +162,25 @@
         "KeyId": str,
         "InitializationVector": str,
         "LicenseAcquisitionUrl": str,
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
 NotificationsTypeDef = TypedDict(
     "NotificationsTypeDef",
     {
         "Progressing": str,
         "Completed": str,
         "Warning": str,
         "Error": str,
@@ -223,35 +244,24 @@
         "SubmitTimeMillis": int,
         "StartTimeMillis": int,
         "FinishTimeMillis": int,
     },
     total=False,
 )
 
-_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
-    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
-    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
-):
-    pass
-
 _RequiredListJobsByPipelineRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByPipelineRequestRequestTypeDef",
     {
         "PipelineId": str,
     },
 )
 _OptionalListJobsByPipelineRequestRequestTypeDef = TypedDict(
@@ -265,35 +275,14 @@
 
 class ListJobsByPipelineRequestRequestTypeDef(
     _RequiredListJobsByPipelineRequestRequestTypeDef,
     _OptionalListJobsByPipelineRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Status": str,
-    },
-)
-_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
-    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
-    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
-):
-    pass
-
 _RequiredListJobsByStatusRequestRequestTypeDef = TypedDict(
     "_RequiredListJobsByStatusRequestRequestTypeDef",
     {
         "Status": str,
     },
 )
 _OptionalListJobsByStatusRequestRequestTypeDef = TypedDict(
@@ -306,56 +295,38 @@
 )
 
 class ListJobsByStatusRequestRequestTypeDef(
     _RequiredListJobsByStatusRequestRequestTypeDef, _OptionalListJobsByStatusRequestRequestTypeDef
 ):
     pass
 
-ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
-    "ListPipelinesRequestListPipelinesPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPipelinesRequestRequestTypeDef = TypedDict(
     "ListPipelinesRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
-    "ListPresetsRequestListPresetsPaginateTypeDef",
-    {
-        "Ascending": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListPresetsRequestRequestTypeDef = TypedDict(
     "ListPresetsRequestRequestTypeDef",
     {
         "Ascending": str,
         "PageToken": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+PermissionOutputTypeDef = TypedDict(
+    "PermissionOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "GranteeType": str,
+        "Grantee": str,
+        "Access": List[str],
     },
     total=False,
 )
 
 PermissionTypeDef = TypedDict(
     "PermissionTypeDef",
     {
@@ -409,44 +380,24 @@
 ReadPresetRequestRequestTypeDef = TypedDict(
     "ReadPresetRequestRequestTypeDef",
     {
         "Id": str,
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
 TestRoleRequestRequestTypeDef = TypedDict(
     "TestRoleRequestRequestTypeDef",
     {
         "Role": str,
         "InputBucket": str,
         "OutputBucket": str,
         "Topics": Sequence[str],
     },
 )
 
-TestRoleResponseTypeDef = TypedDict(
-    "TestRoleResponseTypeDef",
-    {
-        "Success": str,
-        "Messages": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UpdatePipelineStatusRequestRequestTypeDef = TypedDict(
     "UpdatePipelineStatusRequestRequestTypeDef",
     {
         "Id": str,
         "Status": str,
     },
 )
@@ -540,32 +491,133 @@
         "PlayReadyDrm": PlayReadyDrmTypeDef,
         "Status": str,
         "StatusDetail": str,
     },
     total=False,
 )
 
+TestRoleResponseTypeDef = TypedDict(
+    "TestRoleResponseTypeDef",
+    {
+        "Success": str,
+        "Messages": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 UpdatePipelineNotificationsRequestRequestTypeDef = TypedDict(
     "UpdatePipelineNotificationsRequestRequestTypeDef",
     {
         "Id": str,
         "Notifications": NotificationsTypeDef,
     },
 )
 
+_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef = TypedDict(
+    "_OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef(
+    _RequiredListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    _OptionalListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+):
+    pass
+
+_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Status": str,
+    },
+)
+_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef = TypedDict(
+    "_OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListJobsByStatusRequestListJobsByStatusPaginateTypeDef(
+    _RequiredListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    _OptionalListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+):
+    pass
+
+ListPipelinesRequestListPipelinesPaginateTypeDef = TypedDict(
+    "ListPipelinesRequestListPipelinesPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListPresetsRequestListPresetsPaginateTypeDef = TypedDict(
+    "ListPresetsRequestListPresetsPaginateTypeDef",
+    {
+        "Ascending": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+PipelineOutputConfigOutputTypeDef = TypedDict(
+    "PipelineOutputConfigOutputTypeDef",
+    {
+        "Bucket": str,
+        "StorageClass": str,
+        "Permissions": List[PermissionOutputTypeDef],
+    },
+    total=False,
+)
+
 PipelineOutputConfigTypeDef = TypedDict(
     "PipelineOutputConfigTypeDef",
     {
         "Bucket": str,
         "StorageClass": str,
         "Permissions": Sequence[PermissionTypeDef],
     },
     total=False,
 )
 
+VideoParametersOutputTypeDef = TypedDict(
+    "VideoParametersOutputTypeDef",
+    {
+        "Codec": str,
+        "CodecOptions": Dict[str, str],
+        "KeyframesMaxDist": str,
+        "FixedGOP": str,
+        "BitRate": str,
+        "FrameRate": str,
+        "MaxFrameRate": str,
+        "Resolution": str,
+        "AspectRatio": str,
+        "MaxWidth": str,
+        "MaxHeight": str,
+        "DisplayAspectRatio": str,
+        "SizingPolicy": str,
+        "PaddingPolicy": str,
+        "Watermarks": List[PresetWatermarkTypeDef],
+    },
+    total=False,
+)
+
 VideoParametersTypeDef = TypedDict(
     "VideoParametersTypeDef",
     {
         "Codec": str,
         "CodecOptions": Mapping[str, str],
         "KeyframesMaxDist": str,
         "FixedGOP": str,
@@ -599,42 +651,88 @@
 )
 
 class ReadJobRequestJobCompleteWaitTypeDef(
     _RequiredReadJobRequestJobCompleteWaitTypeDef, _OptionalReadJobRequestJobCompleteWaitTypeDef
 ):
     pass
 
+JobAlbumArtOutputTypeDef = TypedDict(
+    "JobAlbumArtOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "Artwork": List[ArtworkTypeDef],
+    },
+    total=False,
+)
+
 JobAlbumArtTypeDef = TypedDict(
     "JobAlbumArtTypeDef",
     {
         "MergePolicy": str,
         "Artwork": Sequence[ArtworkTypeDef],
     },
     total=False,
 )
 
+CaptionsOutputTypeDef = TypedDict(
+    "CaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceTypeDef],
+        "CaptionFormats": List[CaptionFormatTypeDef],
+    },
+    total=False,
+)
+
 CaptionsTypeDef = TypedDict(
     "CaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
         "CaptionFormats": Sequence[CaptionFormatTypeDef],
     },
     total=False,
 )
 
+InputCaptionsOutputTypeDef = TypedDict(
+    "InputCaptionsOutputTypeDef",
+    {
+        "MergePolicy": str,
+        "CaptionSources": List[CaptionSourceTypeDef],
+    },
+    total=False,
+)
+
 InputCaptionsTypeDef = TypedDict(
     "InputCaptionsTypeDef",
     {
         "MergePolicy": str,
         "CaptionSources": Sequence[CaptionSourceTypeDef],
     },
     total=False,
 )
 
+PipelineTypeDef = TypedDict(
+    "PipelineTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Status": str,
+        "InputBucket": str,
+        "OutputBucket": str,
+        "Role": str,
+        "AwsKmsKeyArn": str,
+        "Notifications": NotificationsTypeDef,
+        "ContentConfig": PipelineOutputConfigOutputTypeDef,
+        "ThumbnailConfig": PipelineOutputConfigOutputTypeDef,
+    },
+    total=False,
+)
+
 _RequiredCreatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePipelineRequestRequestTypeDef",
     {
         "Name": str,
         "InputBucket": str,
         "Role": str,
     },
@@ -652,32 +750,17 @@
 )
 
 class CreatePipelineRequestRequestTypeDef(
     _RequiredCreatePipelineRequestRequestTypeDef, _OptionalCreatePipelineRequestRequestTypeDef
 ):
     pass
 
-PipelineTypeDef = TypedDict(
-    "PipelineTypeDef",
-    {
-        "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Status": str,
-        "InputBucket": str,
-        "OutputBucket": str,
-        "Role": str,
-        "AwsKmsKeyArn": str,
-        "Notifications": NotificationsTypeDef,
-        "ContentConfig": PipelineOutputConfigTypeDef,
-        "ThumbnailConfig": PipelineOutputConfigTypeDef,
-    },
-    total=False,
-)
-
+PipelineOutputConfigUnionTypeDef = Union[
+    PipelineOutputConfigTypeDef, PipelineOutputConfigOutputTypeDef
+]
 _RequiredUpdatePipelineRequestRequestTypeDef = TypedDict(
     "_RequiredUpdatePipelineRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalUpdatePipelineRequestRequestTypeDef = TypedDict(
@@ -695,14 +778,30 @@
 )
 
 class UpdatePipelineRequestRequestTypeDef(
     _RequiredUpdatePipelineRequestRequestTypeDef, _OptionalUpdatePipelineRequestRequestTypeDef
 ):
     pass
 
+PresetTypeDef = TypedDict(
+    "PresetTypeDef",
+    {
+        "Id": str,
+        "Arn": str,
+        "Name": str,
+        "Description": str,
+        "Container": str,
+        "Audio": AudioParametersTypeDef,
+        "Video": VideoParametersOutputTypeDef,
+        "Thumbnails": ThumbnailsTypeDef,
+        "Type": str,
+    },
+    total=False,
+)
+
 _RequiredCreatePresetRequestRequestTypeDef = TypedDict(
     "_RequiredCreatePresetRequestRequestTypeDef",
     {
         "Name": str,
         "Container": str,
     },
 )
@@ -718,26 +817,39 @@
 )
 
 class CreatePresetRequestRequestTypeDef(
     _RequiredCreatePresetRequestRequestTypeDef, _OptionalCreatePresetRequestRequestTypeDef
 ):
     pass
 
-PresetTypeDef = TypedDict(
-    "PresetTypeDef",
+VideoParametersUnionTypeDef = Union[VideoParametersTypeDef, VideoParametersOutputTypeDef]
+JobOutputTypeDef = TypedDict(
+    "JobOutputTypeDef",
     {
         "Id": str,
-        "Arn": str,
-        "Name": str,
-        "Description": str,
-        "Container": str,
-        "Audio": AudioParametersTypeDef,
-        "Video": VideoParametersTypeDef,
-        "Thumbnails": ThumbnailsTypeDef,
-        "Type": str,
+        "Key": str,
+        "ThumbnailPattern": str,
+        "ThumbnailEncryption": EncryptionTypeDef,
+        "Rotate": str,
+        "PresetId": str,
+        "SegmentDuration": str,
+        "Status": str,
+        "StatusDetail": str,
+        "Duration": int,
+        "Width": int,
+        "Height": int,
+        "FrameRate": str,
+        "FileSize": int,
+        "DurationMillis": int,
+        "Watermarks": List[JobWatermarkTypeDef],
+        "AlbumArt": JobAlbumArtOutputTypeDef,
+        "Composition": List[ClipTypeDef],
+        "Captions": CaptionsOutputTypeDef,
+        "Encryption": EncryptionTypeDef,
+        "AppliedColorSpaceConversion": str,
     },
     total=False,
 )
 
 CreateJobOutputTypeDef = TypedDict(
     "CreateJobOutputTypeDef",
     {
@@ -752,38 +864,27 @@
         "Composition": Sequence[ClipTypeDef],
         "Captions": CaptionsTypeDef,
         "Encryption": EncryptionTypeDef,
     },
     total=False,
 )
 
-JobOutputTypeDef = TypedDict(
-    "JobOutputTypeDef",
+JobInputOutputTypeDef = TypedDict(
+    "JobInputOutputTypeDef",
     {
-        "Id": str,
         "Key": str,
-        "ThumbnailPattern": str,
-        "ThumbnailEncryption": EncryptionTypeDef,
-        "Rotate": str,
-        "PresetId": str,
-        "SegmentDuration": str,
-        "Status": str,
-        "StatusDetail": str,
-        "Duration": int,
-        "Width": int,
-        "Height": int,
         "FrameRate": str,
-        "FileSize": int,
-        "DurationMillis": int,
-        "Watermarks": List[JobWatermarkTypeDef],
-        "AlbumArt": JobAlbumArtTypeDef,
-        "Composition": List[ClipTypeDef],
-        "Captions": CaptionsTypeDef,
+        "Resolution": str,
+        "AspectRatio": str,
+        "Interlaced": str,
+        "Container": str,
         "Encryption": EncryptionTypeDef,
-        "AppliedColorSpaceConversion": str,
+        "TimeSpan": TimeSpanTypeDef,
+        "InputCaptions": InputCaptionsOutputTypeDef,
+        "DetectedProperties": DetectedPropertiesTypeDef,
     },
     total=False,
 )
 
 JobInputTypeDef = TypedDict(
     "JobInputTypeDef",
     {
@@ -802,157 +903,158 @@
 )
 
 CreatePipelineResponseTypeDef = TypedDict(
     "CreatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPipelinesResponseTypeDef = TypedDict(
     "ListPipelinesResponseTypeDef",
     {
         "Pipelines": List[PipelineTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPipelineResponseTypeDef = TypedDict(
     "ReadPipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineNotificationsResponseTypeDef = TypedDict(
     "UpdatePipelineNotificationsResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineResponseTypeDef = TypedDict(
     "UpdatePipelineResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
         "Warnings": List[WarningTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdatePipelineStatusResponseTypeDef = TypedDict(
     "UpdatePipelineStatusResponseTypeDef",
     {
         "Pipeline": PipelineTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreatePresetResponseTypeDef = TypedDict(
     "CreatePresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
         "Warning": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPresetsResponseTypeDef = TypedDict(
     "ListPresetsResponseTypeDef",
     {
         "Presets": List[PresetTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadPresetResponseTypeDef = TypedDict(
     "ReadPresetResponseTypeDef",
     {
         "Preset": PresetTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredCreateJobRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateJobRequestRequestTypeDef",
-    {
-        "PipelineId": str,
-    },
-)
-_OptionalCreateJobRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateJobRequestRequestTypeDef",
-    {
-        "Input": JobInputTypeDef,
-        "Inputs": Sequence[JobInputTypeDef],
-        "Output": CreateJobOutputTypeDef,
-        "Outputs": Sequence[CreateJobOutputTypeDef],
-        "OutputKeyPrefix": str,
-        "Playlists": Sequence[CreateJobPlaylistTypeDef],
-        "UserMetadata": Mapping[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class CreateJobRequestRequestTypeDef(
-    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
-):
-    pass
-
 JobTypeDef = TypedDict(
     "JobTypeDef",
     {
         "Id": str,
         "Arn": str,
         "PipelineId": str,
-        "Input": JobInputTypeDef,
-        "Inputs": List[JobInputTypeDef],
+        "Input": JobInputOutputTypeDef,
+        "Inputs": List[JobInputOutputTypeDef],
         "Output": JobOutputTypeDef,
         "Outputs": List[JobOutputTypeDef],
         "OutputKeyPrefix": str,
         "Playlists": List[PlaylistTypeDef],
         "Status": str,
         "UserMetadata": Dict[str, str],
         "Timing": TimingTypeDef,
     },
     total=False,
 )
 
+JobInputUnionTypeDef = Union[JobInputTypeDef, JobInputOutputTypeDef]
 CreateJobResponseTypeDef = TypedDict(
     "CreateJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByPipelineResponseTypeDef = TypedDict(
     "ListJobsByPipelineResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListJobsByStatusResponseTypeDef = TypedDict(
     "ListJobsByStatusResponseTypeDef",
     {
         "Jobs": List[JobTypeDef],
         "NextPageToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReadJobResponseTypeDef = TypedDict(
     "ReadJobResponseTypeDef",
     {
         "Job": JobTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+
+_RequiredCreateJobRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateJobRequestRequestTypeDef",
+    {
+        "PipelineId": str,
+    },
+)
+_OptionalCreateJobRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateJobRequestRequestTypeDef",
+    {
+        "Input": JobInputTypeDef,
+        "Inputs": Sequence[JobInputUnionTypeDef],
+        "Output": CreateJobOutputTypeDef,
+        "Outputs": Sequence[CreateJobOutputTypeDef],
+        "OutputKeyPrefix": str,
+        "Playlists": Sequence[CreateJobPlaylistTypeDef],
+        "UserMetadata": Mapping[str, str],
+    },
+    total=False,
+)
+
+class CreateJobRequestRequestTypeDef(
+    _RequiredCreateJobRequestRequestTypeDef, _OptionalCreateJobRequestRequestTypeDef
+):
+    pass
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.py` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder/waiter.pyi` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder/waiter.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-elastictranscoder
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ElasticTranscoder 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore elastictranscoder type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore elastictranscoder type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-elastictranscoder"></a>
 
 # types-aiobotocore-elastictranscoder
 
 [![PyPI - types-aiobotocore-elastictranscoder](https://img.shields.io/pypi/v/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-elastictranscoder.svg?color=blue)](https://pypi.org/project/types-aiobotocore-elastictranscoder)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-elastictranscoder?color=blue)](https://pypistats.org/packages/types-aiobotocore-elastictranscoder)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-elastictranscoder)](https://pepy.tech/project/types-aiobotocore-elastictranscoder)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ElasticTranscoder 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/elastictranscoder.html#ElasticTranscoder)
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
 [types-aiobotocore-elastictranscoder docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_elastictranscoder/).
 
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
@@ -345,97 +344,107 @@
 )
 
 
 def check_value(value: JobCompleteWaiterName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_elastictranscoder.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_elastictranscoder.type_defs import (
     EncryptionTypeDef,
     AudioCodecOptionsTypeDef,
     CancelJobRequestRequestTypeDef,
     TimeSpanTypeDef,
     HlsContentProtectionTypeDef,
     PlayReadyDrmTypeDef,
+    ResponseMetadataTypeDef,
     NotificationsTypeDef,
     WarningTypeDef,
     ThumbnailsTypeDef,
     DeletePipelineRequestRequestTypeDef,
     DeletePresetRequestRequestTypeDef,
     DetectedPropertiesTypeDef,
     TimingTypeDef,
-    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListJobsByPipelineRequestRequestTypeDef,
-    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
     ListJobsByStatusRequestRequestTypeDef,
-    ListPipelinesRequestListPipelinesPaginateTypeDef,
     ListPipelinesRequestRequestTypeDef,
-    ListPresetsRequestListPresetsPaginateTypeDef,
     ListPresetsRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
+    PermissionOutputTypeDef,
     PermissionTypeDef,
     PresetWatermarkTypeDef,
     WaiterConfigTypeDef,
     ReadJobRequestRequestTypeDef,
     ReadPipelineRequestRequestTypeDef,
     ReadPresetRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
     TestRoleRequestRequestTypeDef,
-    TestRoleResponseTypeDef,
     UpdatePipelineStatusRequestRequestTypeDef,
     ArtworkTypeDef,
     CaptionFormatTypeDef,
     CaptionSourceTypeDef,
     JobWatermarkTypeDef,
     AudioParametersTypeDef,
     ClipTypeDef,
     CreateJobPlaylistTypeDef,
     PlaylistTypeDef,
+    TestRoleResponseTypeDef,
     UpdatePipelineNotificationsRequestRequestTypeDef,
+    ListJobsByPipelineRequestListJobsByPipelinePaginateTypeDef,
+    ListJobsByStatusRequestListJobsByStatusPaginateTypeDef,
+    ListPipelinesRequestListPipelinesPaginateTypeDef,
+    ListPresetsRequestListPresetsPaginateTypeDef,
+    PipelineOutputConfigOutputTypeDef,
     PipelineOutputConfigTypeDef,
+    VideoParametersOutputTypeDef,
     VideoParametersTypeDef,
     ReadJobRequestJobCompleteWaitTypeDef,
+    JobAlbumArtOutputTypeDef,
     JobAlbumArtTypeDef,
+    CaptionsOutputTypeDef,
     CaptionsTypeDef,
+    InputCaptionsOutputTypeDef,
     InputCaptionsTypeDef,
-    CreatePipelineRequestRequestTypeDef,
     PipelineTypeDef,
+    CreatePipelineRequestRequestTypeDef,
+    PipelineOutputConfigUnionTypeDef,
     UpdatePipelineRequestRequestTypeDef,
-    CreatePresetRequestRequestTypeDef,
     PresetTypeDef,
-    CreateJobOutputTypeDef,
+    CreatePresetRequestRequestTypeDef,
+    VideoParametersUnionTypeDef,
     JobOutputTypeDef,
+    CreateJobOutputTypeDef,
+    JobInputOutputTypeDef,
     JobInputTypeDef,
     CreatePipelineResponseTypeDef,
     ListPipelinesResponseTypeDef,
     ReadPipelineResponseTypeDef,
     UpdatePipelineNotificationsResponseTypeDef,
     UpdatePipelineResponseTypeDef,
     UpdatePipelineStatusResponseTypeDef,
     CreatePresetResponseTypeDef,
     ListPresetsResponseTypeDef,
     ReadPresetResponseTypeDef,
-    CreateJobRequestRequestTypeDef,
     JobTypeDef,
+    JobInputUnionTypeDef,
     CreateJobResponseTypeDef,
     ListJobsByPipelineResponseTypeDef,
     ListJobsByStatusResponseTypeDef,
     ReadJobResponseTypeDef,
+    CreateJobRequestRequestTypeDef,
 )
 
 
-def get_structure() -> EncryptionTypeDef:
+def get_value() -> EncryptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-elastictranscoder-2.5.2/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt` & `types-aiobotocore-elastictranscoder-2.5.2.post1/types_aiobotocore_elastictranscoder.egg-info/SOURCES.txt`

 * *Files identical despite different names*


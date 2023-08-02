# Comparing `tmp/types-aiobotocore-kinesis-video-archived-media-2.5.2.tar.gz` & `tmp/types-aiobotocore-kinesis-video-archived-media-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-archived-media-2.5.2.tar", last modified: Sat Jul  8 01:43:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-archived-media-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2.tar` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.082385 types-aiobotocore-kinesis-video-archived-media-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15424 2023-07-08 01:43:51.082385 types-aiobotocore-kinesis-video-archived-media-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:51.082385 types-aiobotocore-kinesis-video-archived-media-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.082385 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12159 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-07-08 01:33:24.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-07-08 01:33:24.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4145 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-07-08 01:33:24.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-07-08 01:33:24.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:23.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.082385 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15424 2023-07-08 01:43:50.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 01:43:50.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:50.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:50.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:50.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-08 01:43:50.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13774 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.189549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12136 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9695 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9693 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-02 14:41:30.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:29.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.193549 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15373 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/LICENSE` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/PKG-INFO` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-archived-media
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesis-video-archived-media type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesis-video-archived-media"></a>
 
 # types-aiobotocore-kinesis-video-archived-media
 
 [![PyPI - types-aiobotocore-kinesis-video-archived-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-archived-media?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-archived-media)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-archived-media)](https://pepy.tech/project/types-aiobotocore-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideoArchivedMedia 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
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
@@ -329,54 +328,55 @@
 )
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesis_video_archived_media.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_archived_media.type_defs import (
+    TimestampTypeDef,
+    FragmentTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ImageTypeDef,
+    GetMediaForFragmentListInputRequestTypeDef,
     ClipTimestampRangeTypeDef,
     DASHTimestampRangeTypeDef,
+    GetImagesInputRequestTypeDef,
+    HLSTimestampRangeTypeDef,
     TimestampRangeTypeDef,
-    FragmentTypeDef,
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesInputRequestTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
     GetMediaForFragmentListOutputTypeDef,
-    HLSTimestampRangeTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
+    ClipFragmentSelectorTypeDef,
+    DASHFragmentSelectorTypeDef,
     HLSFragmentSelectorTypeDef,
+    FragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
+    GetHLSStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
 )
 
 
-def get_structure() -> ClipTimestampRangeTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/README.md` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kinesis-video-archived-media"></a>
 
 # types-aiobotocore-kinesis-video-archived-media
 
 [![PyPI - types-aiobotocore-kinesis-video-archived-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-archived-media?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-archived-media)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-archived-media)](https://pepy.tech/project/types-aiobotocore-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideoArchivedMedia 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
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
@@ -296,54 +296,55 @@
 )
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesis_video_archived_media.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_archived_media.type_defs import (
+    TimestampTypeDef,
+    FragmentTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ImageTypeDef,
+    GetMediaForFragmentListInputRequestTypeDef,
     ClipTimestampRangeTypeDef,
     DASHTimestampRangeTypeDef,
+    GetImagesInputRequestTypeDef,
+    HLSTimestampRangeTypeDef,
     TimestampRangeTypeDef,
-    FragmentTypeDef,
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesInputRequestTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
     GetMediaForFragmentListOutputTypeDef,
-    HLSTimestampRangeTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
+    ClipFragmentSelectorTypeDef,
+    DASHFragmentSelectorTypeDef,
     HLSFragmentSelectorTypeDef,
+    FragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
+    GetHLSStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
 )
 
 
-def get_structure() -> ClipTimestampRangeTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/setup.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-archived-media",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_kinesis_video_archived_media"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with"
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
-        "aiobotocore kinesis-video-archived-media type-annotations boto3-stubs mypy typeshed"
+        "aiobotocore kinesis-video-archived-media type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesis_video_archived_media": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/__init__.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/__init__.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/__main__.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/client.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("kinesis-video-archived-media") as client:
         client: KinesisVideoArchivedMediaClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ContainerFormatType,
     DASHDisplayFragmentNumberType,
@@ -40,14 +39,15 @@
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetImagesOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -178,16 +178,16 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/client/#get_hls_streaming_session_url)
         """
 
     async def get_images(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/client.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("kinesis-video-archived-media") as client:
         client: KinesisVideoArchivedMediaClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import (
     ContainerFormatType,
     DASHDisplayFragmentNumberType,
@@ -40,14 +39,15 @@
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
     GetImagesOutputTypeDef,
     GetMediaForFragmentListOutputTypeDef,
     HLSFragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -167,16 +167,16 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Client.get_hls_streaming_session_url)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/client/#get_hls_streaming_session_url)
         """
     async def get_images(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/literals.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/literals.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/paginator.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -19,85 +19,80 @@
         client: KinesisVideoArchivedMediaClient
 
         get_images_paginator: GetImagesPaginator = client.get_paginator("get_images")
         list_fragments_paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Mapping, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Mapping, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import FormatType, ImageSelectorTypeType
 from .type_defs import (
     FragmentSelectorTypeDef,
     GetImagesOutputTypeDef,
     ListFragmentsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetImagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#getimagespaginator)
     """
 
     def paginate(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
-
 class ListFragmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#listfragmentspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         FragmentSelector: FragmentSelectorTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFragmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#listfragmentspaginator)
         """
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/paginator.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,80 +19,85 @@
         client: KinesisVideoArchivedMediaClient
 
         get_images_paginator: GetImagesPaginator = client.get_paginator("get_images")
         list_fragments_paginator: ListFragmentsPaginator = client.get_paginator("list_fragments")
     ```
 """
 import sys
-from datetime import datetime
-from typing import AsyncIterator, Generic, Iterator, Mapping, TypeVar, Union
+from typing import AsyncIterator, Generic, Iterator, Mapping, TypeVar
 
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .literals import FormatType, ImageSelectorTypeType
 from .type_defs import (
     FragmentSelectorTypeDef,
     GetImagesOutputTypeDef,
     ListFragmentsOutputTypeDef,
     PaginatorConfigTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = ("GetImagesPaginator", "ListFragmentsPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetImagesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#getimagespaginator)
     """
 
     def paginate(
         self,
         *,
         ImageSelectorType: ImageSelectorTypeType,
-        StartTimestamp: Union[datetime, str],
-        EndTimestamp: Union[datetime, str],
+        StartTimestamp: TimestampTypeDef,
+        EndTimestamp: TimestampTypeDef,
         SamplingInterval: int,
         Format: FormatType,
         StreamName: str = ...,
         StreamARN: str = ...,
         FormatConfig: Mapping[Literal["JPEGQuality"], str] = ...,
         WidthPixels: int = ...,
         HeightPixels: int = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetImagesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.GetImages.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#getimagespaginator)
         """
 
+
 class ListFragmentsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#listfragmentspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
         FragmentSelector: FragmentSelectorTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListFragmentsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia.Paginator.ListFragments.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/paginators/#listfragmentspaginator)
         """
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/type_defs.py` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesis-video-archived-media service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_kinesis_video_archived_media.type_defs import ClipTimestampRangeTypeDef
+    from types_aiobotocore_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
-    data: ClipTimestampRangeTypeDef = {...}
+    data: TimestampTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,142 +39,132 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
+    "TimestampTypeDef",
+    "FragmentTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ImageTypeDef",
+    "GetMediaForFragmentListInputRequestTypeDef",
     "ClipTimestampRangeTypeDef",
     "DASHTimestampRangeTypeDef",
+    "GetImagesInputRequestTypeDef",
+    "HLSTimestampRangeTypeDef",
     "TimestampRangeTypeDef",
-    "FragmentTypeDef",
     "GetClipOutputTypeDef",
     "GetDASHStreamingSessionURLOutputTypeDef",
     "GetHLSStreamingSessionURLOutputTypeDef",
-    "GetImagesInputGetImagesPaginateTypeDef",
-    "GetImagesInputRequestTypeDef",
-    "ImageTypeDef",
-    "GetMediaForFragmentListInputRequestTypeDef",
     "GetMediaForFragmentListOutputTypeDef",
-    "HLSTimestampRangeTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "ClipFragmentSelectorTypeDef",
-    "DASHFragmentSelectorTypeDef",
-    "FragmentSelectorTypeDef",
     "ListFragmentsOutputTypeDef",
+    "GetImagesInputGetImagesPaginateTypeDef",
     "GetImagesOutputTypeDef",
+    "ClipFragmentSelectorTypeDef",
+    "DASHFragmentSelectorTypeDef",
     "HLSFragmentSelectorTypeDef",
+    "FragmentSelectorTypeDef",
     "GetClipInputRequestTypeDef",
     "GetDASHStreamingSessionURLInputRequestTypeDef",
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     "ListFragmentsInputRequestTypeDef",
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
-)
-
-ClipTimestampRangeTypeDef = TypedDict(
-    "ClipTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-)
-
-DASHTimestampRangeTypeDef = TypedDict(
-    "DASHTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
 )
 
+TimestampTypeDef = Union[datetime, str]
 FragmentTypeDef = TypedDict(
     "FragmentTypeDef",
     {
         "FragmentNumber": str,
         "FragmentSizeInBytes": int,
         "ProducerTimestamp": datetime,
         "ServerTimestamp": datetime,
         "FragmentLengthInMilliseconds": int,
     },
     total=False,
 )
 
-GetClipOutputTypeDef = TypedDict(
-    "GetClipOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetDASHStreamingSessionURLOutputTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DASHStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLOutputTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
-        "HLSStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeStamp": datetime,
+        "Error": ImageErrorType,
+        "ImageContent": str,
     },
+    total=False,
 )
 
-_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
+_RequiredGetMediaForFragmentListInputRequestTypeDef = TypedDict(
+    "_RequiredGetMediaForFragmentListInputRequestTypeDef",
     {
-        "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-        "SamplingInterval": int,
-        "Format": FormatType,
+        "Fragments": Sequence[str],
     },
 )
-_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+_OptionalGetMediaForFragmentListInputRequestTypeDef = TypedDict(
+    "_OptionalGetMediaForFragmentListInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-
-class GetImagesInputGetImagesPaginateTypeDef(
-    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
+class GetMediaForFragmentListInputRequestTypeDef(
+    _RequiredGetMediaForFragmentListInputRequestTypeDef,
+    _OptionalGetMediaForFragmentListInputRequestTypeDef,
 ):
     pass
 
+ClipTimestampRangeTypeDef = TypedDict(
+    "ClipTimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
+DASHTimestampRangeTypeDef = TypedDict(
+    "DASHTimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+    total=False,
+)
 
 _RequiredGetImagesInputRequestTypeDef = TypedDict(
     "_RequiredGetImagesInputRequestTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputRequestTypeDef = TypedDict(
     "_OptionalGetImagesInputRequestTypeDef",
     {
@@ -185,90 +175,113 @@
         "HeightPixels": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-
 class GetImagesInputRequestTypeDef(
     _RequiredGetImagesInputRequestTypeDef, _OptionalGetImagesInputRequestTypeDef
 ):
     pass
 
-
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
+HLSTimestampRangeTypeDef = TypedDict(
+    "HLSTimestampRangeTypeDef",
     {
-        "TimeStamp": datetime,
-        "Error": ImageErrorType,
-        "ImageContent": str,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-_RequiredGetMediaForFragmentListInputRequestTypeDef = TypedDict(
-    "_RequiredGetMediaForFragmentListInputRequestTypeDef",
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
     {
-        "Fragments": Sequence[str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
 )
-_OptionalGetMediaForFragmentListInputRequestTypeDef = TypedDict(
-    "_OptionalGetMediaForFragmentListInputRequestTypeDef",
+
+GetClipOutputTypeDef = TypedDict(
+    "GetClipOutputTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetDASHStreamingSessionURLOutputTypeDef",
+    {
+        "DASHStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-class GetMediaForFragmentListInputRequestTypeDef(
-    _RequiredGetMediaForFragmentListInputRequestTypeDef,
-    _OptionalGetMediaForFragmentListInputRequestTypeDef,
-):
-    pass
-
+GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLOutputTypeDef",
+    {
+        "HLSStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetMediaForFragmentListOutputTypeDef = TypedDict(
     "GetMediaForFragmentListOutputTypeDef",
     {
         "ContentType": str,
         "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HLSTimestampRangeTypeDef = TypedDict(
-    "HLSTimestampRangeTypeDef",
+ListFragmentsOutputTypeDef = TypedDict(
+    "ListFragmentsOutputTypeDef",
     {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "Fragments": List[FragmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+class GetImagesInputGetImagesPaginateTypeDef(
+    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
+):
+    pass
+
+GetImagesOutputTypeDef = TypedDict(
+    "GetImagesOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Images": List[ImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClipFragmentSelectorTypeDef = TypedDict(
     "ClipFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": ClipFragmentSelectorTypeType,
@@ -281,49 +294,31 @@
     {
         "FragmentSelectorType": DASHFragmentSelectorTypeType,
         "TimestampRange": DASHTimestampRangeTypeDef,
     },
     total=False,
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
-    {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
-    },
-)
-
-ListFragmentsOutputTypeDef = TypedDict(
-    "ListFragmentsOutputTypeDef",
-    {
-        "Fragments": List[FragmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetImagesOutputTypeDef = TypedDict(
-    "GetImagesOutputTypeDef",
-    {
-        "Images": List[ImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HLSFragmentSelectorTypeDef = TypedDict(
     "HLSFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": HLSFragmentSelectorTypeType,
         "TimestampRange": HLSTimestampRangeTypeDef,
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
 _RequiredGetClipInputRequestTypeDef = TypedDict(
     "_RequiredGetClipInputRequestTypeDef",
     {
         "ClipFragmentSelector": ClipFragmentSelectorTypeDef,
     },
 )
 _OptionalGetClipInputRequestTypeDef = TypedDict(
@@ -331,21 +326,19 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-
 class GetClipInputRequestTypeDef(
     _RequiredGetClipInputRequestTypeDef, _OptionalGetClipInputRequestTypeDef
 ):
     pass
 
-
 GetDASHStreamingSessionURLInputRequestTypeDef = TypedDict(
     "GetDASHStreamingSessionURLInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "PlaybackMode": DASHPlaybackModeType,
         "DisplayFragmentTimestamp": DASHDisplayFragmentTimestampType,
@@ -353,45 +346,45 @@
         "DASHFragmentSelector": DASHFragmentSelectorTypeDef,
         "Expires": int,
         "MaxManifestFragmentResults": int,
     },
     total=False,
 )
 
-ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
-    "ListFragmentsInputListFragmentsPaginateTypeDef",
+GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "FragmentSelector": FragmentSelectorTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PlaybackMode": HLSPlaybackModeType,
+        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
+        "ContainerFormat": ContainerFormatType,
+        "DiscontinuityMode": HLSDiscontinuityModeType,
+        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
+        "Expires": int,
+        "MaxMediaPlaylistFragmentResults": int,
     },
     total=False,
 )
 
-ListFragmentsInputRequestTypeDef = TypedDict(
-    "ListFragmentsInputRequestTypeDef",
+ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
+    "ListFragmentsInputListFragmentsPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "MaxResults": int,
-        "NextToken": str,
         "FragmentSelector": FragmentSelectorTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
+ListFragmentsInputRequestTypeDef = TypedDict(
+    "ListFragmentsInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "PlaybackMode": HLSPlaybackModeType,
-        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
-        "ContainerFormat": ContainerFormatType,
-        "DiscontinuityMode": HLSDiscontinuityModeType,
-        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
-        "Expires": int,
-        "MaxMediaPlaylistFragmentResults": int,
+        "MaxResults": int,
+        "NextToken": str,
+        "FragmentSelector": FragmentSelectorTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media/type_defs.pyi` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for kinesis-video-archived-media service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_kinesis_video_archived_media.type_defs import ClipTimestampRangeTypeDef
+    from types_aiobotocore_kinesis_video_archived_media.type_defs import TimestampTypeDef
 
-    data: ClipTimestampRangeTypeDef = {...}
+    data: TimestampTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
@@ -39,139 +39,135 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
+    "TimestampTypeDef",
+    "FragmentTypeDef",
+    "ResponseMetadataTypeDef",
+    "PaginatorConfigTypeDef",
+    "ImageTypeDef",
+    "GetMediaForFragmentListInputRequestTypeDef",
     "ClipTimestampRangeTypeDef",
     "DASHTimestampRangeTypeDef",
+    "GetImagesInputRequestTypeDef",
+    "HLSTimestampRangeTypeDef",
     "TimestampRangeTypeDef",
-    "FragmentTypeDef",
     "GetClipOutputTypeDef",
     "GetDASHStreamingSessionURLOutputTypeDef",
     "GetHLSStreamingSessionURLOutputTypeDef",
-    "GetImagesInputGetImagesPaginateTypeDef",
-    "GetImagesInputRequestTypeDef",
-    "ImageTypeDef",
-    "GetMediaForFragmentListInputRequestTypeDef",
     "GetMediaForFragmentListOutputTypeDef",
-    "HLSTimestampRangeTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "ClipFragmentSelectorTypeDef",
-    "DASHFragmentSelectorTypeDef",
-    "FragmentSelectorTypeDef",
     "ListFragmentsOutputTypeDef",
+    "GetImagesInputGetImagesPaginateTypeDef",
     "GetImagesOutputTypeDef",
+    "ClipFragmentSelectorTypeDef",
+    "DASHFragmentSelectorTypeDef",
     "HLSFragmentSelectorTypeDef",
+    "FragmentSelectorTypeDef",
     "GetClipInputRequestTypeDef",
     "GetDASHStreamingSessionURLInputRequestTypeDef",
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
     "ListFragmentsInputListFragmentsPaginateTypeDef",
     "ListFragmentsInputRequestTypeDef",
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
-)
-
-ClipTimestampRangeTypeDef = TypedDict(
-    "ClipTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-)
-
-DASHTimestampRangeTypeDef = TypedDict(
-    "DASHTimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
-    total=False,
-)
-
-TimestampRangeTypeDef = TypedDict(
-    "TimestampRangeTypeDef",
-    {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-    },
 )
 
+TimestampTypeDef = Union[datetime, str]
 FragmentTypeDef = TypedDict(
     "FragmentTypeDef",
     {
         "FragmentNumber": str,
         "FragmentSizeInBytes": int,
         "ProducerTimestamp": datetime,
         "ServerTimestamp": datetime,
         "FragmentLengthInMilliseconds": int,
     },
     total=False,
 )
 
-GetClipOutputTypeDef = TypedDict(
-    "GetClipOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ContentType": str,
-        "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
-GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetDASHStreamingSessionURLOutputTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "DASHStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
+    total=False,
 )
 
-GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLOutputTypeDef",
+ImageTypeDef = TypedDict(
+    "ImageTypeDef",
     {
-        "HLSStreamingSessionURL": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "TimeStamp": datetime,
+        "Error": ImageErrorType,
+        "ImageContent": str,
     },
+    total=False,
 )
 
-_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
+_RequiredGetMediaForFragmentListInputRequestTypeDef = TypedDict(
+    "_RequiredGetMediaForFragmentListInputRequestTypeDef",
     {
-        "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
-        "SamplingInterval": int,
-        "Format": FormatType,
+        "Fragments": Sequence[str],
     },
 )
-_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
-    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+_OptionalGetMediaForFragmentListInputRequestTypeDef = TypedDict(
+    "_OptionalGetMediaForFragmentListInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
-        "WidthPixels": int,
-        "HeightPixels": int,
-        "PaginationConfig": "PaginatorConfigTypeDef",
     },
     total=False,
 )
 
-class GetImagesInputGetImagesPaginateTypeDef(
-    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
+
+class GetMediaForFragmentListInputRequestTypeDef(
+    _RequiredGetMediaForFragmentListInputRequestTypeDef,
+    _OptionalGetMediaForFragmentListInputRequestTypeDef,
 ):
     pass
 
+
+ClipTimestampRangeTypeDef = TypedDict(
+    "ClipTimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+)
+
+DASHTimestampRangeTypeDef = TypedDict(
+    "DASHTimestampRangeTypeDef",
+    {
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+    },
+    total=False,
+)
+
 _RequiredGetImagesInputRequestTypeDef = TypedDict(
     "_RequiredGetImagesInputRequestTypeDef",
     {
         "ImageSelectorType": ImageSelectorTypeType,
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalGetImagesInputRequestTypeDef = TypedDict(
     "_OptionalGetImagesInputRequestTypeDef",
     {
@@ -182,86 +178,117 @@
         "HeightPixels": int,
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
+
 class GetImagesInputRequestTypeDef(
     _RequiredGetImagesInputRequestTypeDef, _OptionalGetImagesInputRequestTypeDef
 ):
     pass
 
-ImageTypeDef = TypedDict(
-    "ImageTypeDef",
+
+HLSTimestampRangeTypeDef = TypedDict(
+    "HLSTimestampRangeTypeDef",
     {
-        "TimeStamp": datetime,
-        "Error": ImageErrorType,
-        "ImageContent": str,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
     total=False,
 )
 
-_RequiredGetMediaForFragmentListInputRequestTypeDef = TypedDict(
-    "_RequiredGetMediaForFragmentListInputRequestTypeDef",
+TimestampRangeTypeDef = TypedDict(
+    "TimestampRangeTypeDef",
     {
-        "Fragments": Sequence[str],
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
     },
 )
-_OptionalGetMediaForFragmentListInputRequestTypeDef = TypedDict(
-    "_OptionalGetMediaForFragmentListInputRequestTypeDef",
+
+GetClipOutputTypeDef = TypedDict(
+    "GetClipOutputTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
+        "ContentType": str,
+        "Payload": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-class GetMediaForFragmentListInputRequestTypeDef(
-    _RequiredGetMediaForFragmentListInputRequestTypeDef,
-    _OptionalGetMediaForFragmentListInputRequestTypeDef,
-):
-    pass
+GetDASHStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetDASHStreamingSessionURLOutputTypeDef",
+    {
+        "DASHStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetHLSStreamingSessionURLOutputTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLOutputTypeDef",
+    {
+        "HLSStreamingSessionURL": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 GetMediaForFragmentListOutputTypeDef = TypedDict(
     "GetMediaForFragmentListOutputTypeDef",
     {
         "ContentType": str,
         "Payload": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-HLSTimestampRangeTypeDef = TypedDict(
-    "HLSTimestampRangeTypeDef",
+ListFragmentsOutputTypeDef = TypedDict(
+    "ListFragmentsOutputTypeDef",
     {
-        "StartTimestamp": Union[datetime, str],
-        "EndTimestamp": Union[datetime, str],
+        "Fragments": List[FragmentTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+_RequiredGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_RequiredGetImagesInputGetImagesPaginateTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "StartTimestamp": TimestampTypeDef,
+        "EndTimestamp": TimestampTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalGetImagesInputGetImagesPaginateTypeDef = TypedDict(
+    "_OptionalGetImagesInputGetImagesPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+
+class GetImagesInputGetImagesPaginateTypeDef(
+    _RequiredGetImagesInputGetImagesPaginateTypeDef, _OptionalGetImagesInputGetImagesPaginateTypeDef
+):
+    pass
+
+
+GetImagesOutputTypeDef = TypedDict(
+    "GetImagesOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Images": List[ImageTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ClipFragmentSelectorTypeDef = TypedDict(
     "ClipFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": ClipFragmentSelectorTypeType,
@@ -274,49 +301,31 @@
     {
         "FragmentSelectorType": DASHFragmentSelectorTypeType,
         "TimestampRange": DASHTimestampRangeTypeDef,
     },
     total=False,
 )
 
-FragmentSelectorTypeDef = TypedDict(
-    "FragmentSelectorTypeDef",
-    {
-        "FragmentSelectorType": FragmentSelectorTypeType,
-        "TimestampRange": TimestampRangeTypeDef,
-    },
-)
-
-ListFragmentsOutputTypeDef = TypedDict(
-    "ListFragmentsOutputTypeDef",
-    {
-        "Fragments": List[FragmentTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-GetImagesOutputTypeDef = TypedDict(
-    "GetImagesOutputTypeDef",
-    {
-        "Images": List[ImageTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 HLSFragmentSelectorTypeDef = TypedDict(
     "HLSFragmentSelectorTypeDef",
     {
         "FragmentSelectorType": HLSFragmentSelectorTypeType,
         "TimestampRange": HLSTimestampRangeTypeDef,
     },
     total=False,
 )
 
+FragmentSelectorTypeDef = TypedDict(
+    "FragmentSelectorTypeDef",
+    {
+        "FragmentSelectorType": FragmentSelectorTypeType,
+        "TimestampRange": TimestampRangeTypeDef,
+    },
+)
+
 _RequiredGetClipInputRequestTypeDef = TypedDict(
     "_RequiredGetClipInputRequestTypeDef",
     {
         "ClipFragmentSelector": ClipFragmentSelectorTypeDef,
     },
 )
 _OptionalGetClipInputRequestTypeDef = TypedDict(
@@ -324,19 +333,21 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
+
 class GetClipInputRequestTypeDef(
     _RequiredGetClipInputRequestTypeDef, _OptionalGetClipInputRequestTypeDef
 ):
     pass
 
+
 GetDASHStreamingSessionURLInputRequestTypeDef = TypedDict(
     "GetDASHStreamingSessionURLInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "PlaybackMode": DASHPlaybackModeType,
         "DisplayFragmentTimestamp": DASHDisplayFragmentTimestampType,
@@ -344,45 +355,45 @@
         "DASHFragmentSelector": DASHFragmentSelectorTypeDef,
         "Expires": int,
         "MaxManifestFragmentResults": int,
     },
     total=False,
 )
 
-ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
-    "ListFragmentsInputListFragmentsPaginateTypeDef",
+GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
+    "GetHLSStreamingSessionURLInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "FragmentSelector": FragmentSelectorTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PlaybackMode": HLSPlaybackModeType,
+        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
+        "ContainerFormat": ContainerFormatType,
+        "DiscontinuityMode": HLSDiscontinuityModeType,
+        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
+        "Expires": int,
+        "MaxMediaPlaylistFragmentResults": int,
     },
     total=False,
 )
 
-ListFragmentsInputRequestTypeDef = TypedDict(
-    "ListFragmentsInputRequestTypeDef",
+ListFragmentsInputListFragmentsPaginateTypeDef = TypedDict(
+    "ListFragmentsInputListFragmentsPaginateTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "MaxResults": int,
-        "NextToken": str,
         "FragmentSelector": FragmentSelectorTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
-GetHLSStreamingSessionURLInputRequestTypeDef = TypedDict(
-    "GetHLSStreamingSessionURLInputRequestTypeDef",
+ListFragmentsInputRequestTypeDef = TypedDict(
+    "ListFragmentsInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
-        "PlaybackMode": HLSPlaybackModeType,
-        "HLSFragmentSelector": HLSFragmentSelectorTypeDef,
-        "ContainerFormat": ContainerFormatType,
-        "DiscontinuityMode": HLSDiscontinuityModeType,
-        "DisplayFragmentTimestamp": HLSDisplayFragmentTimestampType,
-        "Expires": int,
-        "MaxMediaPlaylistFragmentResults": int,
+        "MaxResults": int,
+        "NextToken": str,
+        "FragmentSelector": FragmentSelectorTypeDef,
     },
     total=False,
 )
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-archived-media
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisVideoArchivedMedia 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesis-video-archived-media type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesis-video-archived-media type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesis-video-archived-media"></a>
 
 # types-aiobotocore-kinesis-video-archived-media
 
 [![PyPI - types-aiobotocore-kinesis-video-archived-media](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-archived-media.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-archived-media)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-archived-media?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-archived-media)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-archived-media)](https://pepy.tech/project/types-aiobotocore-kinesis-video-archived-media)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideoArchivedMedia 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-archived-media.html#KinesisVideoArchivedMedia)
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
 [types-aiobotocore-kinesis-video-archived-media docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_archived_media/).
 
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
@@ -329,54 +328,55 @@
 )
 
 
 def check_value(value: ClipFragmentSelectorTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesis_video_archived_media.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_archived_media.type_defs import (
+    TimestampTypeDef,
+    FragmentTypeDef,
+    ResponseMetadataTypeDef,
+    PaginatorConfigTypeDef,
+    ImageTypeDef,
+    GetMediaForFragmentListInputRequestTypeDef,
     ClipTimestampRangeTypeDef,
     DASHTimestampRangeTypeDef,
+    GetImagesInputRequestTypeDef,
+    HLSTimestampRangeTypeDef,
     TimestampRangeTypeDef,
-    FragmentTypeDef,
     GetClipOutputTypeDef,
     GetDASHStreamingSessionURLOutputTypeDef,
     GetHLSStreamingSessionURLOutputTypeDef,
-    GetImagesInputGetImagesPaginateTypeDef,
-    GetImagesInputRequestTypeDef,
-    ImageTypeDef,
-    GetMediaForFragmentListInputRequestTypeDef,
     GetMediaForFragmentListOutputTypeDef,
-    HLSTimestampRangeTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    ClipFragmentSelectorTypeDef,
-    DASHFragmentSelectorTypeDef,
-    FragmentSelectorTypeDef,
     ListFragmentsOutputTypeDef,
+    GetImagesInputGetImagesPaginateTypeDef,
     GetImagesOutputTypeDef,
+    ClipFragmentSelectorTypeDef,
+    DASHFragmentSelectorTypeDef,
     HLSFragmentSelectorTypeDef,
+    FragmentSelectorTypeDef,
     GetClipInputRequestTypeDef,
     GetDASHStreamingSessionURLInputRequestTypeDef,
+    GetHLSStreamingSessionURLInputRequestTypeDef,
     ListFragmentsInputListFragmentsPaginateTypeDef,
     ListFragmentsInputRequestTypeDef,
-    GetHLSStreamingSessionURLInputRequestTypeDef,
 )
 
 
-def get_structure() -> ClipTimestampRangeTypeDef:
+def get_value() -> TimestampTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesis-video-archived-media-2.5.2/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-archived-media-2.5.2.post1/types_aiobotocore_kinesis_video_archived_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*


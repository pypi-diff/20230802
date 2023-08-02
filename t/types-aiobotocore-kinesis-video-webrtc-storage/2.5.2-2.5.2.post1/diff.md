# Comparing `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.tar.gz` & `tmp/types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.tar", last modified: Sat Jul  8 01:43:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
```

## Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.tar` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.270388 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-08 01:43:51.270388 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11531 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:51.270388 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.270388 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-08 01:33:26.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-08 01:33:26.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:25.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.270388 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13177 2023-07-08 01:43:51.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-08 01:43:51.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:51.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-08 01:43:51.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.385549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-08-02 14:52:31.381549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11509 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.385549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.381549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5274 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8039 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.381549 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-02 14:52:31.000000 types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/LICENSE` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesis-video-webrtc-storage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesis-video-webrtc-storage type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesis-video-webrtc-storage"></a>
 
 # types-aiobotocore-kinesis-video-webrtc-storage
 
 [![PyPI - types-aiobotocore-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-webrtc-storage?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-webrtc-storage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideoWebRTCStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
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
@@ -284,31 +283,31 @@
 )
 
 
 def check_value(value: KinesisVideoWebRTCStorageServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesis_video_webrtc_storage.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import (
-    EmptyResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    JoinStorageSessionInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
 )
 
 
-def get_structure() -> EmptyResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/README.md` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kinesis-video-webrtc-storage"></a>
 
 # types-aiobotocore-kinesis-video-webrtc-storage
 
 [![PyPI - types-aiobotocore-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-webrtc-storage?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-webrtc-storage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideoWebRTCStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
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
@@ -251,31 +251,31 @@
 )
 
 
 def check_value(value: KinesisVideoWebRTCStorageServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesis_video_webrtc_storage.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import (
-    EmptyResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    JoinStorageSessionInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
 )
 
 
-def get_structure() -> EmptyResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/setup.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,45 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesis-video-webrtc-storage",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_kinesis_video_webrtc_storage"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with"
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
-        "aiobotocore kinesis-video-webrtc-storage type-annotations boto3-stubs mypy typeshed"
+        "aiobotocore kinesis-video-webrtc-storage type-annotations botocore mypy typeshed"
         " autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesis_video_webrtc_storage": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage\nOther"
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

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/client.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/literals.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 Type annotations for kinesis-video-webrtc-storage service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import EmptyResponseMetadataTypeDef
+    from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
 
-    data: EmptyResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
-    "EmptyResponseMetadataTypeDef",
-    "JoinStorageSessionInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "JoinStorageSessionInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
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
 
 JoinStorageSessionInputRequestTypeDef = TypedDict(
     "JoinStorageSessionInputRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -2,50 +2,50 @@
 Type annotations for kinesis-video-webrtc-storage service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import EmptyResponseMetadataTypeDef
+    from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import ResponseMetadataTypeDef
 
-    data: EmptyResponseMetadataTypeDef = {...}
+    data: ResponseMetadataTypeDef = ...
     ```
 """
 import sys
 from typing import Dict
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
-    "EmptyResponseMetadataTypeDef",
-    "JoinStorageSessionInputRequestTypeDef",
     "ResponseMetadataTypeDef",
+    "JoinStorageSessionInputRequestTypeDef",
+    "EmptyResponseMetadataTypeDef",
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
 
 JoinStorageSessionInputRequestTypeDef = TypedDict(
     "JoinStorageSessionInputRequestTypeDef",
     {
         "channelArn": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesis-video-webrtc-storage
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisVideoWebRTCStorage 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesis-video-webrtc-storage type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesis-video-webrtc-storage type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesis-video-webrtc-storage"></a>
 
 # types-aiobotocore-kinesis-video-webrtc-storage
 
 [![PyPI - types-aiobotocore-kinesis-video-webrtc-storage](https://img.shields.io/pypi/v/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesis-video-webrtc-storage.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesis-video-webrtc-storage)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesis-video-webrtc-storage?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesis-video-webrtc-storage)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesis-video-webrtc-storage)](https://pepy.tech/project/types-aiobotocore-kinesis-video-webrtc-storage)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideoWebRTCStorage 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesis-video-webrtc-storage.html#KinesisVideoWebRTCStorage)
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
 [types-aiobotocore-kinesis-video-webrtc-storage docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesis_video_webrtc_storage/).
 
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
@@ -284,31 +283,31 @@
 )
 
 
 def check_value(value: KinesisVideoWebRTCStorageServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesis_video_webrtc_storage.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_kinesis_video_webrtc_storage.type_defs import (
-    EmptyResponseMetadataTypeDef,
-    JoinStorageSessionInputRequestTypeDef,
     ResponseMetadataTypeDef,
+    JoinStorageSessionInputRequestTypeDef,
+    EmptyResponseMetadataTypeDef,
 )
 
 
-def get_structure() -> EmptyResponseMetadataTypeDef:
+def get_value() -> ResponseMetadataTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt` & `types-aiobotocore-kinesis-video-webrtc-storage-2.5.2.post1/types_aiobotocore_kinesis_video_webrtc_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*


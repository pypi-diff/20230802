# Comparing `tmp/types-aiobotocore-kinesisvideo-2.5.2.tar.gz` & `tmp/types-aiobotocore-kinesisvideo-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisvideo-2.5.2.tar", last modified: Sat Jul  8 01:43:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisvideo-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:32 2023, max compression
```

## Comparing `types-aiobotocore-kinesisvideo-2.5.2.tar` & `types-aiobotocore-kinesisvideo-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.514393 types-aiobotocore-kinesisvideo-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-07-08 01:43:51.514393 types-aiobotocore-kinesisvideo-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15277 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:51.514393 types-aiobotocore-kinesisvideo-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.510393 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24842 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24802 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-07-08 01:33:32.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25198 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:31.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.514393 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16862 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15353 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24852 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9887 2023-08-02 14:41:38.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26253 2023-08-02 14:41:38.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26216 2023-08-02 14:41:38.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:37.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:32.197547 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16891 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 14:52:32.000000 types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/LICENSE` & `types-aiobotocore-kinesisvideo-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.5.2.post1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesisvideo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesisvideo type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisvideo"></a>
 
 # types-aiobotocore-kinesisvideo
 
 [![PyPI - types-aiobotocore-kinesisvideo](https://img.shields.io/pypi/v/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisvideo?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisvideo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideo 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
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
@@ -332,97 +331,99 @@
 )
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisvideo.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
-    CreateSignalingChannelOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
-    CreateStreamOutputTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
     MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     GetDataEndpointInputRequestTypeDef,
-    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
-    ListTagsForStreamOutputTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
     ScheduleConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateSignalingChannelOutputTypeDef,
+    CreateStreamOutputTypeDef,
+    GetDataEndpointOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
     UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/README.md` & `types-aiobotocore-kinesisvideo-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kinesisvideo"></a>
 
 # types-aiobotocore-kinesisvideo
 
 [![PyPI - types-aiobotocore-kinesisvideo](https://img.shields.io/pypi/v/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisvideo?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisvideo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideo 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
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
@@ -299,97 +299,99 @@
 )
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisvideo.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
-    CreateSignalingChannelOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
-    CreateStreamOutputTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
     MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     GetDataEndpointInputRequestTypeDef,
-    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
-    ListTagsForStreamOutputTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
     ScheduleConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateSignalingChannelOutputTypeDef,
+    CreateStreamOutputTypeDef,
+    GetDataEndpointOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
     UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/setup.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisvideo",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_kinesisvideo"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with"
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
-    keywords="aiobotocore kinesisvideo type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore kinesisvideo type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesisvideo": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/"
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/__init__.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/__init__.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/__main__.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisVideo 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.KinesisVideo 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo\nOther"
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

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/client.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
@@ -401,15 +401,15 @@
         """
 
     async def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/client.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     DescribeMediaStorageConfigurationOutputTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     DescribeStreamOutputTypeDef,
     EdgeConfigTypeDef,
     GetDataEndpointOutputTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
-    ImageGenerationConfigurationTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     ListSignalingChannelsOutputTypeDef,
     ListStreamsOutputTypeDef,
     ListTagsForResourceOutputTypeDef,
     ListTagsForStreamOutputTypeDef,
     MediaStorageConfigurationTypeDef,
     NotificationConfigurationTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
@@ -370,15 +370,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_data_retention)
         """
     async def update_image_generation_configuration(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        ImageGenerationConfiguration: ImageGenerationConfigurationTypeDef = ...
+        ImageGenerationConfiguration: ImageGenerationConfigurationUnionTypeDef = ...
     ) -> Dict[str, Any]:
         """
         Updates the `StreamInfo` and `ImageProcessingConfiguration` fields.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Client.update_image_generation_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/client/#update_image_generation_configuration)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/literals.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/literals.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/paginator.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 
@@ -80,15 +80,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 
@@ -98,13 +98,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/paginator.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/paginator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
 
     def paginate(
         self,
         *,
         StreamName: str = ...,
         StreamARN: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeMappedResourceConfigurationOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.DescribeMappedResourceConfiguration.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#describemappedresourceconfigurationpaginator)
         """
 
 class ListSignalingChannelsPaginator(AioPaginator):
@@ -76,15 +76,15 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
     """
 
     def paginate(
         self,
         *,
         ChannelNameCondition: ChannelNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSignalingChannelsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListSignalingChannels.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#listsignalingchannelspaginator)
         """
 
 class ListStreamsPaginator(AioPaginator):
@@ -93,13 +93,13 @@
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
     """
 
     def paginate(
         self,
         *,
         StreamNameCondition: StreamNameConditionTypeDef = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStreamsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo.Paginator.ListStreams.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/paginators/#liststreamspaginator)
         """
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/type_defs.py` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
-    data: SingleMasterConfigurationTypeDef = {...}
+    data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
@@ -41,74 +41,76 @@
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
-    "CreateSignalingChannelOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
-    "CreateStreamOutputTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
     "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "GetDataEndpointInputRequestTypeDef",
-    "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
-    "ListTagsForStreamOutputTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "ScheduleConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
     "UpdateSignalingChannelInputRequestTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListSignalingChannelsInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateSignalingChannelOutputTypeDef",
+    "CreateStreamOutputTypeDef",
+    "GetDataEndpointOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
+    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
+    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
@@ -135,19 +137,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateSignalingChannelOutputTypeDef = TypedDict(
-    "CreateSignalingChannelOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChannelARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
@@ -168,22 +173,14 @@
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
 
-CreateStreamOutputTypeDef = TypedDict(
-    "CreateStreamOutputTypeDef",
-    {
-        "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredDeleteSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalDeleteSignalingChannelInputRequestTypeDef = TypedDict(
@@ -246,20 +243,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     {
@@ -371,22 +368,14 @@
 
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
 
-GetDataEndpointOutputTypeDef = TypedDict(
-    "GetDataEndpointOutputTypeDef",
-    {
-        "DataEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -435,42 +424,24 @@
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
@@ -478,43 +449,22 @@
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
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
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
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
 _RequiredTagStreamInputRequestTypeDef = TypedDict(
     "_RequiredTagStreamInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
 )
 _OptionalTagStreamInputRequestTypeDef = TypedDict(
@@ -644,23 +594,14 @@
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSignalingChannelsInputRequestTypeDef = TypedDict(
     "ListSignalingChannelsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ChannelNameCondition": ChannelNameConditionTypeDef,
     },
@@ -695,38 +636,99 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateSignalingChannelOutputTypeDef = TypedDict(
+    "CreateSignalingChannelOutputTypeDef",
+    {
+        "ChannelARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamOutputTypeDef = TypedDict(
+    "CreateStreamOutputTypeDef",
+    {
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataEndpointOutputTypeDef = TypedDict(
+    "GetDataEndpointOutputTypeDef",
+    {
+        "DataEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationOutputTypeDef",
     {
         "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
         "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     {
         "ChannelARN": str,
@@ -734,24 +736,24 @@
     },
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "ChannelARN": str,
@@ -773,32 +775,60 @@
     pass
 
 
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredImageGenerationConfigurationOutputTypeDef",
+    {
+        "Status": ConfigurationStatusType,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalImageGenerationConfigurationOutputTypeDef",
+    {
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+    },
+    total=False,
+)
+
+
+class ImageGenerationConfigurationOutputTypeDef(
+    _RequiredImageGenerationConfigurationOutputTypeDef,
+    _OptionalImageGenerationConfigurationOutputTypeDef,
+):
+    pass
+
+
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
 
@@ -808,15 +838,15 @@
     pass
 
 
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
@@ -861,50 +891,53 @@
     },
 )
 
 DescribeSignalingChannelOutputTypeDef = TypedDict(
     "DescribeSignalingChannelOutputTypeDef",
     {
         "ChannelInfo": ChannelInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalingChannelsOutputTypeDef = TypedDict(
     "ListSignalingChannelsOutputTypeDef",
     {
         "ChannelInfoList": List[ChannelInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImageGenerationConfigurationUnionTypeDef = Union[
+    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
+]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -941,15 +974,15 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
@@ -978,10 +1011,10 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo/type_defs.pyi` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo/type_defs.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kinesisvideo.type_defs import SingleMasterConfigurationTypeDef
 
-    data: SingleMasterConfigurationTypeDef = {...}
+    data: SingleMasterConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     APINameType,
     ChannelProtocolType,
     ChannelRoleType,
     ChannelTypeType,
     ConfigurationStatusType,
@@ -40,74 +40,76 @@
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "SingleMasterConfigurationTypeDef",
     "ChannelNameConditionTypeDef",
     "TagTypeDef",
-    "CreateSignalingChannelOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CreateStreamInputRequestTypeDef",
-    "CreateStreamOutputTypeDef",
     "DeleteSignalingChannelInputRequestTypeDef",
     "DeleteStreamInputRequestTypeDef",
     "LocalSizeConfigTypeDef",
     "DescribeEdgeConfigurationInputRequestTypeDef",
     "DescribeImageGenerationConfigurationInputRequestTypeDef",
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     "MappedResourceConfigurationListItemTypeDef",
     "DescribeMediaStorageConfigurationInputRequestTypeDef",
     "MediaStorageConfigurationTypeDef",
     "DescribeNotificationConfigurationInputRequestTypeDef",
     "DescribeSignalingChannelInputRequestTypeDef",
     "DescribeStreamInputRequestTypeDef",
     "StreamInfoTypeDef",
     "GetDataEndpointInputRequestTypeDef",
-    "GetDataEndpointOutputTypeDef",
     "SingleMasterChannelEndpointConfigurationTypeDef",
     "ResourceEndpointListItemTypeDef",
     "ImageGenerationDestinationConfigTypeDef",
     "StreamNameConditionTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
-    "ListTagsForResourceOutputTypeDef",
     "ListTagsForStreamInputRequestTypeDef",
-    "ListTagsForStreamOutputTypeDef",
     "MediaSourceConfigTypeDef",
     "NotificationDestinationConfigTypeDef",
-    "PaginatorConfigTypeDef",
     "ScheduleConfigTypeDef",
-    "ResponseMetadataTypeDef",
     "TagStreamInputRequestTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UntagStreamInputRequestTypeDef",
     "UpdateDataRetentionInputRequestTypeDef",
     "UpdateStreamInputRequestTypeDef",
     "ChannelInfoTypeDef",
     "UpdateSignalingChannelInputRequestTypeDef",
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "ListSignalingChannelsInputRequestTypeDef",
     "CreateSignalingChannelInputRequestTypeDef",
     "TagResourceInputRequestTypeDef",
+    "CreateSignalingChannelOutputTypeDef",
+    "CreateStreamOutputTypeDef",
+    "GetDataEndpointOutputTypeDef",
+    "ListTagsForResourceOutputTypeDef",
+    "ListTagsForStreamOutputTypeDef",
     "DeletionConfigTypeDef",
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
     "DescribeMappedResourceConfigurationOutputTypeDef",
     "DescribeMediaStorageConfigurationOutputTypeDef",
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     "DescribeStreamOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "GetSignalingChannelEndpointInputRequestTypeDef",
     "GetSignalingChannelEndpointOutputTypeDef",
+    "ImageGenerationConfigurationOutputTypeDef",
     "ImageGenerationConfigurationTypeDef",
     "ListStreamsInputListStreamsPaginateTypeDef",
     "ListStreamsInputRequestTypeDef",
     "NotificationConfigurationTypeDef",
     "RecorderConfigTypeDef",
     "UploaderConfigTypeDef",
     "DescribeSignalingChannelOutputTypeDef",
     "ListSignalingChannelsOutputTypeDef",
     "DescribeImageGenerationConfigurationOutputTypeDef",
+    "ImageGenerationConfigurationUnionTypeDef",
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     "DescribeNotificationConfigurationOutputTypeDef",
     "UpdateNotificationConfigurationInputRequestTypeDef",
     "EdgeConfigTypeDef",
     "DescribeEdgeConfigurationOutputTypeDef",
     "StartEdgeConfigurationUpdateInputRequestTypeDef",
     "StartEdgeConfigurationUpdateOutputTypeDef",
@@ -134,19 +136,22 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateSignalingChannelOutputTypeDef = TypedDict(
-    "CreateSignalingChannelOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ChannelARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredCreateStreamInputRequestTypeDef = TypedDict(
     "_RequiredCreateStreamInputRequestTypeDef",
     {
         "StreamName": str,
@@ -165,22 +170,14 @@
 )
 
 class CreateStreamInputRequestTypeDef(
     _RequiredCreateStreamInputRequestTypeDef, _OptionalCreateStreamInputRequestTypeDef
 ):
     pass
 
-CreateStreamOutputTypeDef = TypedDict(
-    "CreateStreamOutputTypeDef",
-    {
-        "StreamARN": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredDeleteSignalingChannelInputRequestTypeDef = TypedDict(
     "_RequiredDeleteSignalingChannelInputRequestTypeDef",
     {
         "ChannelARN": str,
     },
 )
 _OptionalDeleteSignalingChannelInputRequestTypeDef = TypedDict(
@@ -239,20 +236,20 @@
     {
         "StreamName": str,
         "StreamARN": str,
     },
     total=False,
 )
 
-DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
-    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "StreamName": str,
-        "StreamARN": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeMappedResourceConfigurationInputRequestTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationInputRequestTypeDef",
     {
@@ -360,22 +357,14 @@
 )
 
 class GetDataEndpointInputRequestTypeDef(
     _RequiredGetDataEndpointInputRequestTypeDef, _OptionalGetDataEndpointInputRequestTypeDef
 ):
     pass
 
-GetDataEndpointOutputTypeDef = TypedDict(
-    "GetDataEndpointOutputTypeDef",
-    {
-        "DataEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 SingleMasterChannelEndpointConfigurationTypeDef = TypedDict(
     "SingleMasterChannelEndpointConfigurationTypeDef",
     {
         "Protocols": Sequence[ChannelProtocolType],
         "Role": ChannelRoleType,
     },
     total=False,
@@ -422,42 +411,24 @@
 )
 
 class ListTagsForResourceInputRequestTypeDef(
     _RequiredListTagsForResourceInputRequestTypeDef, _OptionalListTagsForResourceInputRequestTypeDef
 ):
     pass
 
-ListTagsForResourceOutputTypeDef = TypedDict(
-    "ListTagsForResourceOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListTagsForStreamInputRequestTypeDef = TypedDict(
     "ListTagsForStreamInputRequestTypeDef",
     {
         "NextToken": str,
         "StreamARN": str,
         "StreamName": str,
     },
     total=False,
 )
 
-ListTagsForStreamOutputTypeDef = TypedDict(
-    "ListTagsForStreamOutputTypeDef",
-    {
-        "NextToken": str,
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 MediaSourceConfigTypeDef = TypedDict(
     "MediaSourceConfigTypeDef",
     {
         "MediaUriSecretArn": str,
         "MediaUriType": MediaUriTypeType,
     },
 )
@@ -465,43 +436,22 @@
 NotificationDestinationConfigTypeDef = TypedDict(
     "NotificationDestinationConfigTypeDef",
     {
         "Uri": str,
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
 ScheduleConfigTypeDef = TypedDict(
     "ScheduleConfigTypeDef",
     {
         "ScheduleExpression": str,
         "DurationInSeconds": int,
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
 _RequiredTagStreamInputRequestTypeDef = TypedDict(
     "_RequiredTagStreamInputRequestTypeDef",
     {
         "Tags": Mapping[str, str],
     },
 )
 _OptionalTagStreamInputRequestTypeDef = TypedDict(
@@ -621,23 +571,14 @@
 
 class UpdateSignalingChannelInputRequestTypeDef(
     _RequiredUpdateSignalingChannelInputRequestTypeDef,
     _OptionalUpdateSignalingChannelInputRequestTypeDef,
 ):
     pass
 
-ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
-    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
-    {
-        "ChannelNameCondition": ChannelNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSignalingChannelsInputRequestTypeDef = TypedDict(
     "ListSignalingChannelsInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "ChannelNameCondition": ChannelNameConditionTypeDef,
     },
@@ -670,38 +611,99 @@
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "Tags": Sequence[TagTypeDef],
     },
 )
 
+CreateSignalingChannelOutputTypeDef = TypedDict(
+    "CreateSignalingChannelOutputTypeDef",
+    {
+        "ChannelARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateStreamOutputTypeDef = TypedDict(
+    "CreateStreamOutputTypeDef",
+    {
+        "StreamARN": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetDataEndpointOutputTypeDef = TypedDict(
+    "GetDataEndpointOutputTypeDef",
+    {
+        "DataEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceOutputTypeDef = TypedDict(
+    "ListTagsForResourceOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForStreamOutputTypeDef = TypedDict(
+    "ListTagsForStreamOutputTypeDef",
+    {
+        "NextToken": str,
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 DeletionConfigTypeDef = TypedDict(
     "DeletionConfigTypeDef",
     {
         "EdgeRetentionInHours": int,
         "LocalSizeConfig": LocalSizeConfigTypeDef,
         "DeleteAfterUpload": bool,
     },
     total=False,
 )
 
+DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef = TypedDict(
+    "DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef",
+    {
+        "StreamName": str,
+        "StreamARN": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef = TypedDict(
+    "ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef",
+    {
+        "ChannelNameCondition": ChannelNameConditionTypeDef,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 DescribeMappedResourceConfigurationOutputTypeDef = TypedDict(
     "DescribeMappedResourceConfigurationOutputTypeDef",
     {
         "MappedResourceConfigurationList": List[MappedResourceConfigurationListItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeMediaStorageConfigurationOutputTypeDef = TypedDict(
     "DescribeMediaStorageConfigurationOutputTypeDef",
     {
         "MediaStorageConfiguration": MediaStorageConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateMediaStorageConfigurationInputRequestTypeDef = TypedDict(
     "UpdateMediaStorageConfigurationInputRequestTypeDef",
     {
         "ChannelARN": str,
@@ -709,24 +711,24 @@
     },
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamInfo": StreamInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "StreamInfoList": List[StreamInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetSignalingChannelEndpointInputRequestTypeDef = TypedDict(
     "_RequiredGetSignalingChannelEndpointInputRequestTypeDef",
     {
         "ChannelARN": str,
@@ -746,32 +748,58 @@
 ):
     pass
 
 GetSignalingChannelEndpointOutputTypeDef = TypedDict(
     "GetSignalingChannelEndpointOutputTypeDef",
     {
         "ResourceEndpointList": List[ResourceEndpointListItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_RequiredImageGenerationConfigurationOutputTypeDef",
+    {
+        "Status": ConfigurationStatusType,
+        "ImageSelectorType": ImageSelectorTypeType,
+        "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
+        "SamplingInterval": int,
+        "Format": FormatType,
+    },
+)
+_OptionalImageGenerationConfigurationOutputTypeDef = TypedDict(
+    "_OptionalImageGenerationConfigurationOutputTypeDef",
+    {
+        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "WidthPixels": int,
+        "HeightPixels": int,
+    },
+    total=False,
+)
+
+class ImageGenerationConfigurationOutputTypeDef(
+    _RequiredImageGenerationConfigurationOutputTypeDef,
+    _OptionalImageGenerationConfigurationOutputTypeDef,
+):
+    pass
+
 _RequiredImageGenerationConfigurationTypeDef = TypedDict(
     "_RequiredImageGenerationConfigurationTypeDef",
     {
         "Status": ConfigurationStatusType,
         "ImageSelectorType": ImageSelectorTypeType,
         "DestinationConfig": ImageGenerationDestinationConfigTypeDef,
         "SamplingInterval": int,
         "Format": FormatType,
     },
 )
 _OptionalImageGenerationConfigurationTypeDef = TypedDict(
     "_OptionalImageGenerationConfigurationTypeDef",
     {
-        "FormatConfig": Dict[Literal["JPEGQuality"], str],
+        "FormatConfig": Mapping[Literal["JPEGQuality"], str],
         "WidthPixels": int,
         "HeightPixels": int,
     },
     total=False,
 )
 
 class ImageGenerationConfigurationTypeDef(
@@ -779,15 +807,15 @@
 ):
     pass
 
 ListStreamsInputListStreamsPaginateTypeDef = TypedDict(
     "ListStreamsInputListStreamsPaginateTypeDef",
     {
         "StreamNameCondition": StreamNameConditionTypeDef,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
     total=False,
 )
 
 ListStreamsInputRequestTypeDef = TypedDict(
     "ListStreamsInputRequestTypeDef",
     {
@@ -830,50 +858,53 @@
     },
 )
 
 DescribeSignalingChannelOutputTypeDef = TypedDict(
     "DescribeSignalingChannelOutputTypeDef",
     {
         "ChannelInfo": ChannelInfoTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSignalingChannelsOutputTypeDef = TypedDict(
     "ListSignalingChannelsOutputTypeDef",
     {
         "ChannelInfoList": List[ChannelInfoTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeImageGenerationConfigurationOutputTypeDef = TypedDict(
     "DescribeImageGenerationConfigurationOutputTypeDef",
     {
-        "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ImageGenerationConfiguration": ImageGenerationConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ImageGenerationConfigurationUnionTypeDef = Union[
+    ImageGenerationConfigurationTypeDef, ImageGenerationConfigurationOutputTypeDef
+]
 UpdateImageGenerationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateImageGenerationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
         "StreamARN": str,
         "ImageGenerationConfiguration": ImageGenerationConfigurationTypeDef,
     },
     total=False,
 )
 
 DescribeNotificationConfigurationOutputTypeDef = TypedDict(
     "DescribeNotificationConfigurationOutputTypeDef",
     {
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateNotificationConfigurationInputRequestTypeDef = TypedDict(
     "UpdateNotificationConfigurationInputRequestTypeDef",
     {
         "StreamName": str,
@@ -908,15 +939,15 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartEdgeConfigurationUpdateInputRequestTypeDef = TypedDict(
     "_RequiredStartEdgeConfigurationUpdateInputRequestTypeDef",
     {
         "EdgeConfig": EdgeConfigTypeDef,
@@ -943,10 +974,10 @@
         "StreamName": str,
         "StreamARN": str,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "SyncStatus": SyncStatusType,
         "FailedStatusDetails": str,
         "EdgeConfig": EdgeConfigTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisvideo
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisVideo 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesisvideo type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesisvideo type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisvideo"></a>
 
 # types-aiobotocore-kinesisvideo
 
 [![PyPI - types-aiobotocore-kinesisvideo](https://img.shields.io/pypi/v/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisvideo.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisvideo)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisvideo?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisvideo)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisvideo)](https://pepy.tech/project/types-aiobotocore-kinesisvideo)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisVideo 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisvideo.html#KinesisVideo)
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
 [types-aiobotocore-kinesisvideo docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisvideo/).
 
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
@@ -332,97 +331,99 @@
 )
 
 
 def check_value(value: APINameType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisvideo.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisvideo.type_defs import (
     SingleMasterConfigurationTypeDef,
     ChannelNameConditionTypeDef,
     TagTypeDef,
-    CreateSignalingChannelOutputTypeDef,
+    ResponseMetadataTypeDef,
     CreateStreamInputRequestTypeDef,
-    CreateStreamOutputTypeDef,
     DeleteSignalingChannelInputRequestTypeDef,
     DeleteStreamInputRequestTypeDef,
     LocalSizeConfigTypeDef,
     DescribeEdgeConfigurationInputRequestTypeDef,
     DescribeImageGenerationConfigurationInputRequestTypeDef,
-    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeMappedResourceConfigurationInputRequestTypeDef,
     MappedResourceConfigurationListItemTypeDef,
     DescribeMediaStorageConfigurationInputRequestTypeDef,
     MediaStorageConfigurationTypeDef,
     DescribeNotificationConfigurationInputRequestTypeDef,
     DescribeSignalingChannelInputRequestTypeDef,
     DescribeStreamInputRequestTypeDef,
     StreamInfoTypeDef,
     GetDataEndpointInputRequestTypeDef,
-    GetDataEndpointOutputTypeDef,
     SingleMasterChannelEndpointConfigurationTypeDef,
     ResourceEndpointListItemTypeDef,
     ImageGenerationDestinationConfigTypeDef,
     StreamNameConditionTypeDef,
     ListTagsForResourceInputRequestTypeDef,
-    ListTagsForResourceOutputTypeDef,
     ListTagsForStreamInputRequestTypeDef,
-    ListTagsForStreamOutputTypeDef,
     MediaSourceConfigTypeDef,
     NotificationDestinationConfigTypeDef,
-    PaginatorConfigTypeDef,
     ScheduleConfigTypeDef,
-    ResponseMetadataTypeDef,
     TagStreamInputRequestTypeDef,
     UntagResourceInputRequestTypeDef,
     UntagStreamInputRequestTypeDef,
     UpdateDataRetentionInputRequestTypeDef,
     UpdateStreamInputRequestTypeDef,
     ChannelInfoTypeDef,
     UpdateSignalingChannelInputRequestTypeDef,
-    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     ListSignalingChannelsInputRequestTypeDef,
     CreateSignalingChannelInputRequestTypeDef,
     TagResourceInputRequestTypeDef,
+    CreateSignalingChannelOutputTypeDef,
+    CreateStreamOutputTypeDef,
+    GetDataEndpointOutputTypeDef,
+    ListTagsForResourceOutputTypeDef,
+    ListTagsForStreamOutputTypeDef,
     DeletionConfigTypeDef,
+    DescribeMappedResourceConfigurationInputDescribeMappedResourceConfigurationPaginateTypeDef,
+    ListSignalingChannelsInputListSignalingChannelsPaginateTypeDef,
     DescribeMappedResourceConfigurationOutputTypeDef,
     DescribeMediaStorageConfigurationOutputTypeDef,
     UpdateMediaStorageConfigurationInputRequestTypeDef,
     DescribeStreamOutputTypeDef,
     ListStreamsOutputTypeDef,
     GetSignalingChannelEndpointInputRequestTypeDef,
     GetSignalingChannelEndpointOutputTypeDef,
+    ImageGenerationConfigurationOutputTypeDef,
     ImageGenerationConfigurationTypeDef,
     ListStreamsInputListStreamsPaginateTypeDef,
     ListStreamsInputRequestTypeDef,
     NotificationConfigurationTypeDef,
     RecorderConfigTypeDef,
     UploaderConfigTypeDef,
     DescribeSignalingChannelOutputTypeDef,
     ListSignalingChannelsOutputTypeDef,
     DescribeImageGenerationConfigurationOutputTypeDef,
+    ImageGenerationConfigurationUnionTypeDef,
     UpdateImageGenerationConfigurationInputRequestTypeDef,
     DescribeNotificationConfigurationOutputTypeDef,
     UpdateNotificationConfigurationInputRequestTypeDef,
     EdgeConfigTypeDef,
     DescribeEdgeConfigurationOutputTypeDef,
     StartEdgeConfigurationUpdateInputRequestTypeDef,
     StartEdgeConfigurationUpdateOutputTypeDef,
 )
 
 
-def get_structure() -> SingleMasterConfigurationTypeDef:
+def get_value() -> SingleMasterConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisvideo-2.5.2/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisvideo-2.5.2.post1/types_aiobotocore_kinesisvideo.egg-info/SOURCES.txt`

 * *Files identical despite different names*


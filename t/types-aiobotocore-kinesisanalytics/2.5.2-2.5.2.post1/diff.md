# Comparing `tmp/types-aiobotocore-kinesisanalytics-2.5.2.tar.gz` & `tmp/types-aiobotocore-kinesisanalytics-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.5.2.tar", last modified: Sat Jul  8 01:43:51 2023, max compression
+gzip compressed data, was "types-aiobotocore-kinesisanalytics-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:31 2023, max compression
```

## Comparing `types-aiobotocore-kinesisanalytics-2.5.2.tar` & `types-aiobotocore-kinesisanalytics-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.382391 types-aiobotocore-kinesisanalytics-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-07-08 01:43:51.382391 types-aiobotocore-kinesisanalytics-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:51.382391 types-aiobotocore-kinesisanalytics-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.378390 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17044 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17016 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    25973 2023-07-08 01:33:27.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    25942 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:26.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:51.382391 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15621 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:43:51.000000 types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14056 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2135 2023-08-02 14:41:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    26551 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26518 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:32.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:31.405549 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15610 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:52:31.000000 types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/LICENSE` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesisanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesisanalytics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisanalytics"></a>
 
 # types-aiobotocore-kinesisanalytics
 
 [![PyPI - types-aiobotocore-kinesisanalytics](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisanalytics?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
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
@@ -283,34 +282,35 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisanalytics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
@@ -334,55 +334,56 @@
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
     InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
+    ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ApplicationDetailTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/README.md` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-kinesisanalytics"></a>
 
 # types-aiobotocore-kinesisanalytics
 
 [![PyPI - types-aiobotocore-kinesisanalytics](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisanalytics?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
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
@@ -250,34 +250,35 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisanalytics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
@@ -301,55 +302,56 @@
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
     InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
+    ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ApplicationDetailTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/setup.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-kinesisanalytics",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_kinesisanalytics"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with"
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
-    keywords="aiobotocore kinesisanalytics type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore kinesisanalytics type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_kinesisanalytics": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/"
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/__init__.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/__init__.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/__main__.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.KinesisAnalytics 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.KinesisAnalytics 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics\nOther"
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

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/client.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_kinesisanalytics.client import KinesisAnalyticsClient
 
     session = get_session()
     async with session.create_client("kinesisanalytics") as client:
         client: KinesisAnalyticsClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     ApplicationUpdateTypeDef,
     CloudWatchLoggingOptionTypeDef,
@@ -32,14 +31,15 @@
     InputTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("KinesisAnalyticsClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -176,15 +176,15 @@
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#create_application)
         """
 
     async def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#delete_application)
         """
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/client.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,15 @@
     from types_aiobotocore_kinesisanalytics.client import KinesisAnalyticsClient
 
     session = get_session()
     async with session.create_client("kinesisanalytics") as client:
         client: KinesisAnalyticsClient
     ```
 """
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .type_defs import (
     ApplicationUpdateTypeDef,
     CloudWatchLoggingOptionTypeDef,
@@ -32,14 +31,15 @@
     InputTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     OutputTypeDef,
     ReferenceDataSourceTypeDef,
     S3ConfigurationTypeDef,
     TagTypeDef,
+    TimestampTypeDef,
 )
 
 __all__ = ("KinesisAnalyticsClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -164,15 +164,15 @@
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.create_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#create_application)
         """
     async def delete_application(
-        self, *, ApplicationName: str, CreateTimestamp: Union[datetime, str]
+        self, *, ApplicationName: str, CreateTimestamp: TimestampTypeDef
     ) -> Dict[str, Any]:
         """
         .
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics.Client.delete_application)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/client/#delete_application)
         """
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/literals.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/literals.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/type_defs.py` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,41 +4,41 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kinesisanalytics.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplicationStatusType, InputStartingPositionType, RecordFormatTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "InputParallelismTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
@@ -62,47 +62,48 @@
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
+    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "InputTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
+    "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
+    "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ApplicationDetailTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "ApplicationUpdateTypeDef",
     "DescribeApplicationResponseTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
 )
 
 CloudWatchLoggingOptionTypeDef = TypedDict(
@@ -124,22 +125,20 @@
     "_OptionalCloudWatchLoggingOptionDescriptionTypeDef",
     {
         "CloudWatchLoggingOptionId": str,
     },
     total=False,
 )
 
-
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
-
 ApplicationSummaryTypeDef = TypedDict(
     "ApplicationSummaryTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
     },
@@ -156,21 +155,19 @@
     {
         "LogStreamARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
 )
 
-
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
-
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -185,18 +182,27 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
-
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
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
 
 DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOptionId": str,
@@ -226,22 +232,15 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CreateTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -340,19 +339,17 @@
     "_OptionalRecordColumnTypeDef",
     {
         "Mapping": str,
     },
     total=False,
 )
 
-
 class RecordColumnTypeDef(_RequiredRecordColumnTypeDef, _OptionalRecordColumnTypeDef):
     pass
 
-
 KinesisFirehoseInputTypeDef = TypedDict(
     "KinesisFirehoseInputTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
 )
@@ -508,25 +505,14 @@
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
         "ReferenceRoleARNUpdate": str,
     },
     total=False,
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
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -543,44 +529,52 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOption": CloudWatchLoggingOptionTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationSummary": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "HasMoreApplications": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
     },
 )
 
 InputConfigurationTypeDef = TypedDict(
     "InputConfigurationTypeDef",
     {
         "Id": str,
@@ -645,19 +639,17 @@
         "KinesisStreamsOutput": KinesisStreamsOutputTypeDef,
         "KinesisFirehoseOutput": KinesisFirehoseOutputTypeDef,
         "LambdaOutput": LambdaOutputTypeDef,
     },
     total=False,
 )
 
-
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
-
 _RequiredOutputUpdateTypeDef = TypedDict(
     "_RequiredOutputUpdateTypeDef",
     {
         "OutputId": str,
     },
 )
 _OptionalOutputUpdateTypeDef = TypedDict(
@@ -668,19 +660,17 @@
         "KinesisFirehoseOutputUpdate": KinesisFirehoseOutputUpdateTypeDef,
         "LambdaOutputUpdate": LambdaOutputUpdateTypeDef,
         "DestinationSchemaUpdate": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
-
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
-
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "InputConfigurations": Sequence[InputConfigurationTypeDef],
     },
 )
@@ -717,19 +707,17 @@
     "_OptionalRecordFormatTypeDef",
     {
         "MappingParameters": MappingParametersTypeDef,
     },
     total=False,
 )
 
-
 class RecordFormatTypeDef(_RequiredRecordFormatTypeDef, _OptionalRecordFormatTypeDef):
     pass
 
-
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Output": OutputTypeDef,
     },
@@ -741,14 +729,34 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
+_RequiredSourceSchemaOutputTypeDef = TypedDict(
+    "_RequiredSourceSchemaOutputTypeDef",
+    {
+        "RecordFormat": RecordFormatTypeDef,
+        "RecordColumns": List[RecordColumnTypeDef],
+    },
+)
+_OptionalSourceSchemaOutputTypeDef = TypedDict(
+    "_OptionalSourceSchemaOutputTypeDef",
+    {
+        "RecordEncoding": str,
+    },
+    total=False,
+)
+
+class SourceSchemaOutputTypeDef(
+    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
+):
+    pass
+
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -756,19 +764,17 @@
     "_OptionalSourceSchemaTypeDef",
     {
         "RecordEncoding": str,
     },
     total=False,
 )
 
-
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
-
 _RequiredInputUpdateTypeDef = TypedDict(
     "_RequiredInputUpdateTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalInputUpdateTypeDef = TypedDict(
@@ -780,91 +786,85 @@
         "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
         "InputSchemaUpdate": InputSchemaUpdateTypeDef,
         "InputParallelismUpdate": InputParallelismUpdateTypeDef,
     },
     total=False,
 )
 
-
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
-
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDescriptionTypeDef = TypedDict(
     "InputDescriptionTypeDef",
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
-_RequiredInputTypeDef = TypedDict(
-    "_RequiredInputTypeDef",
-    {
-        "NamePrefix": str,
-        "InputSchema": SourceSchemaTypeDef,
-    },
-)
-_OptionalInputTypeDef = TypedDict(
-    "_OptionalInputTypeDef",
-    {
-        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
-        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
-        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
-        "InputParallelism": InputParallelismTypeDef,
-    },
-    total=False,
-)
-
-
-class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
-    pass
-
-
 _RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_RequiredReferenceDataSourceDescriptionTypeDef",
     {
         "ReferenceId": str,
         "TableName": str,
         "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
     },
 )
 _OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
     "_OptionalReferenceDataSourceDescriptionTypeDef",
     {
-        "ReferenceSchema": SourceSchemaTypeDef,
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceDescriptionTypeDef(
     _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
 ):
     pass
 
+_RequiredInputTypeDef = TypedDict(
+    "_RequiredInputTypeDef",
+    {
+        "NamePrefix": str,
+        "InputSchema": SourceSchemaTypeDef,
+    },
+)
+_OptionalInputTypeDef = TypedDict(
+    "_OptionalInputTypeDef",
+    {
+        "InputProcessingConfiguration": InputProcessingConfigurationTypeDef,
+        "KinesisStreamsInput": KinesisStreamsInputTypeDef,
+        "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
+        "InputParallelism": InputParallelismTypeDef,
+    },
+    total=False,
+)
+
+class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
+    pass
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
@@ -873,21 +873,19 @@
     "_OptionalReferenceDataSourceTypeDef",
     {
         "S3ReferenceDataSource": S3ReferenceDataSourceTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceTypeDef(
     _RequiredReferenceDataSourceTypeDef, _OptionalReferenceDataSourceTypeDef
 ):
     pass
 
-
 _RequiredReferenceDataSourceUpdateTypeDef = TypedDict(
     "_RequiredReferenceDataSourceUpdateTypeDef",
     {
         "ReferenceId": str,
     },
 )
 _OptionalReferenceDataSourceUpdateTypeDef = TypedDict(
@@ -896,20 +894,47 @@
         "TableNameUpdate": str,
         "S3ReferenceDataSourceUpdate": S3ReferenceDataSourceUpdateTypeDef,
         "ReferenceSchemaUpdate": SourceSchemaTypeDef,
     },
     total=False,
 )
 
-
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
+_RequiredApplicationDetailTypeDef = TypedDict(
+    "_RequiredApplicationDetailTypeDef",
+    {
+        "ApplicationName": str,
+        "ApplicationARN": str,
+        "ApplicationStatus": ApplicationStatusType,
+        "ApplicationVersionId": int,
+    },
+)
+_OptionalApplicationDetailTypeDef = TypedDict(
+    "_OptionalApplicationDetailTypeDef",
+    {
+        "ApplicationDescription": str,
+        "CreateTimestamp": datetime,
+        "LastUpdateTimestamp": datetime,
+        "InputDescriptions": List[InputDescriptionTypeDef],
+        "OutputDescriptions": List[OutputDescriptionTypeDef],
+        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
+        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
+        "ApplicationCode": str,
+    },
+    total=False,
+)
+
+class ApplicationDetailTypeDef(
+    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
+):
+    pass
 
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
@@ -931,52 +956,19 @@
         "CloudWatchLoggingOptions": Sequence[CloudWatchLoggingOptionTypeDef],
         "ApplicationCode": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-
-_RequiredApplicationDetailTypeDef = TypedDict(
-    "_RequiredApplicationDetailTypeDef",
-    {
-        "ApplicationName": str,
-        "ApplicationARN": str,
-        "ApplicationStatus": ApplicationStatusType,
-        "ApplicationVersionId": int,
-    },
-)
-_OptionalApplicationDetailTypeDef = TypedDict(
-    "_OptionalApplicationDetailTypeDef",
-    {
-        "ApplicationDescription": str,
-        "CreateTimestamp": datetime,
-        "LastUpdateTimestamp": datetime,
-        "InputDescriptions": List[InputDescriptionTypeDef],
-        "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ApplicationCode": str,
-    },
-    total=False,
-)
-
-
-class ApplicationDetailTypeDef(
-    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
-):
-    pass
-
-
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
     },
@@ -994,15 +986,15 @@
     total=False,
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics/type_defs.pyi` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics/type_defs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,40 +4,42 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_kinesisanalytics.type_defs import CloudWatchLoggingOptionTypeDef
 
-    data: CloudWatchLoggingOptionTypeDef = {...}
+    data: CloudWatchLoggingOptionTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence, Union
 
 from .literals import ApplicationStatusType, InputStartingPositionType, RecordFormatTypeType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CloudWatchLoggingOptionTypeDef",
     "CloudWatchLoggingOptionDescriptionTypeDef",
     "ApplicationSummaryTypeDef",
     "CloudWatchLoggingOptionUpdateTypeDef",
     "CSVMappingParametersTypeDef",
     "TagTypeDef",
+    "ResponseMetadataTypeDef",
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     "DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DeleteApplicationOutputRequestRequestTypeDef",
     "DeleteApplicationReferenceDataSourceRequestRequestTypeDef",
-    "DeleteApplicationRequestRequestTypeDef",
+    "TimestampTypeDef",
     "DescribeApplicationRequestRequestTypeDef",
     "DestinationSchemaTypeDef",
     "InputStartingPositionConfigurationTypeDef",
     "S3ConfigurationTypeDef",
     "InputParallelismTypeDef",
     "KinesisFirehoseInputDescriptionTypeDef",
     "KinesisStreamsInputDescriptionTypeDef",
@@ -61,47 +63,48 @@
     "LambdaOutputTypeDef",
     "LambdaOutputUpdateTypeDef",
     "ListApplicationsRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ReferenceDataSourceDescriptionTypeDef",
     "S3ReferenceDataSourceTypeDef",
     "S3ReferenceDataSourceUpdateTypeDef",
-    "ResponseMetadataTypeDef",
     "StopApplicationRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
+    "TagResourceRequestRequestTypeDef",
     "CreateApplicationResponseTypeDef",
     "ListApplicationsResponseTypeDef",
     "ListTagsForResourceResponseTypeDef",
-    "TagResourceRequestRequestTypeDef",
+    "DeleteApplicationRequestRequestTypeDef",
     "InputConfigurationTypeDef",
     "InputProcessingConfigurationDescriptionTypeDef",
     "InputProcessingConfigurationTypeDef",
     "InputProcessingConfigurationUpdateTypeDef",
     "MappingParametersTypeDef",
     "OutputDescriptionTypeDef",
     "OutputTypeDef",
     "OutputUpdateTypeDef",
     "StartApplicationRequestRequestTypeDef",
     "AddApplicationInputProcessingConfigurationRequestRequestTypeDef",
     "DiscoverInputSchemaRequestRequestTypeDef",
     "RecordFormatTypeDef",
     "AddApplicationOutputRequestRequestTypeDef",
     "InputSchemaUpdateTypeDef",
+    "SourceSchemaOutputTypeDef",
     "SourceSchemaTypeDef",
     "InputUpdateTypeDef",
     "DiscoverInputSchemaResponseTypeDef",
     "InputDescriptionTypeDef",
-    "InputTypeDef",
     "ReferenceDataSourceDescriptionTypeDef",
+    "InputTypeDef",
     "ReferenceDataSourceTypeDef",
     "ReferenceDataSourceUpdateTypeDef",
+    "ApplicationDetailTypeDef",
     "AddApplicationInputRequestRequestTypeDef",
     "CreateApplicationRequestRequestTypeDef",
-    "ApplicationDetailTypeDef",
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     "ApplicationUpdateTypeDef",
     "DescribeApplicationResponseTypeDef",
     "UpdateApplicationRequestRequestTypeDef",
 )
 
 CloudWatchLoggingOptionTypeDef = TypedDict(
@@ -123,20 +126,22 @@
     "_OptionalCloudWatchLoggingOptionDescriptionTypeDef",
     {
         "CloudWatchLoggingOptionId": str,
     },
     total=False,
 )
 
+
 class CloudWatchLoggingOptionDescriptionTypeDef(
     _RequiredCloudWatchLoggingOptionDescriptionTypeDef,
     _OptionalCloudWatchLoggingOptionDescriptionTypeDef,
 ):
     pass
 
+
 ApplicationSummaryTypeDef = TypedDict(
     "ApplicationSummaryTypeDef",
     {
         "ApplicationName": str,
         "ApplicationARN": str,
         "ApplicationStatus": ApplicationStatusType,
     },
@@ -153,19 +158,21 @@
     {
         "LogStreamARNUpdate": str,
         "RoleARNUpdate": str,
     },
     total=False,
 )
 
+
 class CloudWatchLoggingOptionUpdateTypeDef(
     _RequiredCloudWatchLoggingOptionUpdateTypeDef, _OptionalCloudWatchLoggingOptionUpdateTypeDef
 ):
     pass
 
+
 CSVMappingParametersTypeDef = TypedDict(
     "CSVMappingParametersTypeDef",
     {
         "RecordRowDelimiter": str,
         "RecordColumnDelimiter": str,
     },
 )
@@ -180,17 +187,30 @@
     "_OptionalTagTypeDef",
     {
         "Value": str,
     },
     total=False,
 )
 
+
 class TagTypeDef(_RequiredTagTypeDef, _OptionalTagTypeDef):
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
 DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef = TypedDict(
     "DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOptionId": str,
     },
@@ -219,22 +239,15 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceId": str,
     },
 )
 
-DeleteApplicationRequestRequestTypeDef = TypedDict(
-    "DeleteApplicationRequestRequestTypeDef",
-    {
-        "ApplicationName": str,
-        "CreateTimestamp": Union[datetime, str],
-    },
-)
-
+TimestampTypeDef = Union[datetime, str]
 DescribeApplicationRequestRequestTypeDef = TypedDict(
     "DescribeApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -333,17 +346,19 @@
     "_OptionalRecordColumnTypeDef",
     {
         "Mapping": str,
     },
     total=False,
 )
 
+
 class RecordColumnTypeDef(_RequiredRecordColumnTypeDef, _OptionalRecordColumnTypeDef):
     pass
 
+
 KinesisFirehoseInputTypeDef = TypedDict(
     "KinesisFirehoseInputTypeDef",
     {
         "ResourceARN": str,
         "RoleARN": str,
     },
 )
@@ -499,25 +514,14 @@
         "BucketARNUpdate": str,
         "FileKeyUpdate": str,
         "ReferenceRoleARNUpdate": str,
     },
     total=False,
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
 StopApplicationRequestRequestTypeDef = TypedDict(
     "StopApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
     },
 )
 
@@ -534,44 +538,52 @@
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "CloudWatchLoggingOption": CloudWatchLoggingOptionTypeDef,
     },
 )
 
+TagResourceRequestRequestTypeDef = TypedDict(
+    "TagResourceRequestRequestTypeDef",
+    {
+        "ResourceARN": str,
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+
 CreateApplicationResponseTypeDef = TypedDict(
     "CreateApplicationResponseTypeDef",
     {
         "ApplicationSummary": ApplicationSummaryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListApplicationsResponseTypeDef = TypedDict(
     "ListApplicationsResponseTypeDef",
     {
         "ApplicationSummaries": List[ApplicationSummaryTypeDef],
         "HasMoreApplications": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-TagResourceRequestRequestTypeDef = TypedDict(
-    "TagResourceRequestRequestTypeDef",
+DeleteApplicationRequestRequestTypeDef = TypedDict(
+    "DeleteApplicationRequestRequestTypeDef",
     {
-        "ResourceARN": str,
-        "Tags": Sequence[TagTypeDef],
+        "ApplicationName": str,
+        "CreateTimestamp": TimestampTypeDef,
     },
 )
 
 InputConfigurationTypeDef = TypedDict(
     "InputConfigurationTypeDef",
     {
         "Id": str,
@@ -636,17 +648,19 @@
         "KinesisStreamsOutput": KinesisStreamsOutputTypeDef,
         "KinesisFirehoseOutput": KinesisFirehoseOutputTypeDef,
         "LambdaOutput": LambdaOutputTypeDef,
     },
     total=False,
 )
 
+
 class OutputTypeDef(_RequiredOutputTypeDef, _OptionalOutputTypeDef):
     pass
 
+
 _RequiredOutputUpdateTypeDef = TypedDict(
     "_RequiredOutputUpdateTypeDef",
     {
         "OutputId": str,
     },
 )
 _OptionalOutputUpdateTypeDef = TypedDict(
@@ -657,17 +671,19 @@
         "KinesisFirehoseOutputUpdate": KinesisFirehoseOutputUpdateTypeDef,
         "LambdaOutputUpdate": LambdaOutputUpdateTypeDef,
         "DestinationSchemaUpdate": DestinationSchemaTypeDef,
     },
     total=False,
 )
 
+
 class OutputUpdateTypeDef(_RequiredOutputUpdateTypeDef, _OptionalOutputUpdateTypeDef):
     pass
 
+
 StartApplicationRequestRequestTypeDef = TypedDict(
     "StartApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "InputConfigurations": Sequence[InputConfigurationTypeDef],
     },
 )
@@ -704,17 +720,19 @@
     "_OptionalRecordFormatTypeDef",
     {
         "MappingParameters": MappingParametersTypeDef,
     },
     total=False,
 )
 
+
 class RecordFormatTypeDef(_RequiredRecordFormatTypeDef, _OptionalRecordFormatTypeDef):
     pass
 
+
 AddApplicationOutputRequestRequestTypeDef = TypedDict(
     "AddApplicationOutputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Output": OutputTypeDef,
     },
@@ -726,14 +744,36 @@
         "RecordFormatUpdate": RecordFormatTypeDef,
         "RecordEncodingUpdate": str,
         "RecordColumnUpdates": Sequence[RecordColumnTypeDef],
     },
     total=False,
 )
 
+_RequiredSourceSchemaOutputTypeDef = TypedDict(
+    "_RequiredSourceSchemaOutputTypeDef",
+    {
+        "RecordFormat": RecordFormatTypeDef,
+        "RecordColumns": List[RecordColumnTypeDef],
+    },
+)
+_OptionalSourceSchemaOutputTypeDef = TypedDict(
+    "_OptionalSourceSchemaOutputTypeDef",
+    {
+        "RecordEncoding": str,
+    },
+    total=False,
+)
+
+
+class SourceSchemaOutputTypeDef(
+    _RequiredSourceSchemaOutputTypeDef, _OptionalSourceSchemaOutputTypeDef
+):
+    pass
+
+
 _RequiredSourceSchemaTypeDef = TypedDict(
     "_RequiredSourceSchemaTypeDef",
     {
         "RecordFormat": RecordFormatTypeDef,
         "RecordColumns": Sequence[RecordColumnTypeDef],
     },
 )
@@ -741,17 +781,19 @@
     "_OptionalSourceSchemaTypeDef",
     {
         "RecordEncoding": str,
     },
     total=False,
 )
 
+
 class SourceSchemaTypeDef(_RequiredSourceSchemaTypeDef, _OptionalSourceSchemaTypeDef):
     pass
 
+
 _RequiredInputUpdateTypeDef = TypedDict(
     "_RequiredInputUpdateTypeDef",
     {
         "InputId": str,
     },
 )
 _OptionalInputUpdateTypeDef = TypedDict(
@@ -763,44 +805,69 @@
         "KinesisFirehoseInputUpdate": KinesisFirehoseInputUpdateTypeDef,
         "InputSchemaUpdate": InputSchemaUpdateTypeDef,
         "InputParallelismUpdate": InputParallelismUpdateTypeDef,
     },
     total=False,
 )
 
+
 class InputUpdateTypeDef(_RequiredInputUpdateTypeDef, _OptionalInputUpdateTypeDef):
     pass
 
+
 DiscoverInputSchemaResponseTypeDef = TypedDict(
     "DiscoverInputSchemaResponseTypeDef",
     {
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "ParsedInputRecords": List[List[str]],
         "ProcessedInputRecords": List[str],
         "RawInputRecords": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InputDescriptionTypeDef = TypedDict(
     "InputDescriptionTypeDef",
     {
         "InputId": str,
         "NamePrefix": str,
         "InAppStreamNames": List[str],
         "InputProcessingConfigurationDescription": InputProcessingConfigurationDescriptionTypeDef,
         "KinesisStreamsInputDescription": KinesisStreamsInputDescriptionTypeDef,
         "KinesisFirehoseInputDescription": KinesisFirehoseInputDescriptionTypeDef,
-        "InputSchema": SourceSchemaTypeDef,
+        "InputSchema": SourceSchemaOutputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
         "InputStartingPositionConfiguration": InputStartingPositionConfigurationTypeDef,
     },
     total=False,
 )
 
+_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_RequiredReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceId": str,
+        "TableName": str,
+        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
+    },
+)
+_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
+    "_OptionalReferenceDataSourceDescriptionTypeDef",
+    {
+        "ReferenceSchema": SourceSchemaOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class ReferenceDataSourceDescriptionTypeDef(
+    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
+):
+    pass
+
+
 _RequiredInputTypeDef = TypedDict(
     "_RequiredInputTypeDef",
     {
         "NamePrefix": str,
         "InputSchema": SourceSchemaTypeDef,
     },
 )
@@ -811,37 +878,18 @@
         "KinesisStreamsInput": KinesisStreamsInputTypeDef,
         "KinesisFirehoseInput": KinesisFirehoseInputTypeDef,
         "InputParallelism": InputParallelismTypeDef,
     },
     total=False,
 )
 
+
 class InputTypeDef(_RequiredInputTypeDef, _OptionalInputTypeDef):
     pass
 
-_RequiredReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_RequiredReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceId": str,
-        "TableName": str,
-        "S3ReferenceDataSourceDescription": S3ReferenceDataSourceDescriptionTypeDef,
-    },
-)
-_OptionalReferenceDataSourceDescriptionTypeDef = TypedDict(
-    "_OptionalReferenceDataSourceDescriptionTypeDef",
-    {
-        "ReferenceSchema": SourceSchemaTypeDef,
-    },
-    total=False,
-)
-
-class ReferenceDataSourceDescriptionTypeDef(
-    _RequiredReferenceDataSourceDescriptionTypeDef, _OptionalReferenceDataSourceDescriptionTypeDef
-):
-    pass
 
 _RequiredReferenceDataSourceTypeDef = TypedDict(
     "_RequiredReferenceDataSourceTypeDef",
     {
         "TableName": str,
         "ReferenceSchema": SourceSchemaTypeDef,
     },
@@ -850,19 +898,21 @@
     "_OptionalReferenceDataSourceTypeDef",
     {
         "S3ReferenceDataSource": S3ReferenceDataSourceTypeDef,
     },
     total=False,
 )
 
+
 class ReferenceDataSourceTypeDef(
     _RequiredReferenceDataSourceTypeDef, _OptionalReferenceDataSourceTypeDef
 ):
     pass
 
+
 _RequiredReferenceDataSourceUpdateTypeDef = TypedDict(
     "_RequiredReferenceDataSourceUpdateTypeDef",
     {
         "ReferenceId": str,
     },
 )
 _OptionalReferenceDataSourceUpdateTypeDef = TypedDict(
@@ -871,19 +921,52 @@
         "TableNameUpdate": str,
         "S3ReferenceDataSourceUpdate": S3ReferenceDataSourceUpdateTypeDef,
         "ReferenceSchemaUpdate": SourceSchemaTypeDef,
     },
     total=False,
 )
 
+
 class ReferenceDataSourceUpdateTypeDef(
     _RequiredReferenceDataSourceUpdateTypeDef, _OptionalReferenceDataSourceUpdateTypeDef
 ):
     pass
 
+
+_RequiredApplicationDetailTypeDef = TypedDict(
+    "_RequiredApplicationDetailTypeDef",
+    {
+        "ApplicationName": str,
+        "ApplicationARN": str,
+        "ApplicationStatus": ApplicationStatusType,
+        "ApplicationVersionId": int,
+    },
+)
+_OptionalApplicationDetailTypeDef = TypedDict(
+    "_OptionalApplicationDetailTypeDef",
+    {
+        "ApplicationDescription": str,
+        "CreateTimestamp": datetime,
+        "LastUpdateTimestamp": datetime,
+        "InputDescriptions": List[InputDescriptionTypeDef],
+        "OutputDescriptions": List[OutputDescriptionTypeDef],
+        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
+        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
+        "ApplicationCode": str,
+    },
+    total=False,
+)
+
+
+class ApplicationDetailTypeDef(
+    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
+):
+    pass
+
+
 AddApplicationInputRequestRequestTypeDef = TypedDict(
     "AddApplicationInputRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "Input": InputTypeDef,
     },
@@ -904,47 +987,20 @@
         "CloudWatchLoggingOptions": Sequence[CloudWatchLoggingOptionTypeDef],
         "ApplicationCode": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateApplicationRequestRequestTypeDef(
     _RequiredCreateApplicationRequestRequestTypeDef, _OptionalCreateApplicationRequestRequestTypeDef
 ):
     pass
 
-_RequiredApplicationDetailTypeDef = TypedDict(
-    "_RequiredApplicationDetailTypeDef",
-    {
-        "ApplicationName": str,
-        "ApplicationARN": str,
-        "ApplicationStatus": ApplicationStatusType,
-        "ApplicationVersionId": int,
-    },
-)
-_OptionalApplicationDetailTypeDef = TypedDict(
-    "_OptionalApplicationDetailTypeDef",
-    {
-        "ApplicationDescription": str,
-        "CreateTimestamp": datetime,
-        "LastUpdateTimestamp": datetime,
-        "InputDescriptions": List[InputDescriptionTypeDef],
-        "OutputDescriptions": List[OutputDescriptionTypeDef],
-        "ReferenceDataSourceDescriptions": List[ReferenceDataSourceDescriptionTypeDef],
-        "CloudWatchLoggingOptionDescriptions": List[CloudWatchLoggingOptionDescriptionTypeDef],
-        "ApplicationCode": str,
-    },
-    total=False,
-)
-
-class ApplicationDetailTypeDef(
-    _RequiredApplicationDetailTypeDef, _OptionalApplicationDetailTypeDef
-):
-    pass
 
 AddApplicationReferenceDataSourceRequestRequestTypeDef = TypedDict(
     "AddApplicationReferenceDataSourceRequestRequestTypeDef",
     {
         "ApplicationName": str,
         "CurrentApplicationVersionId": int,
         "ReferenceDataSource": ReferenceDataSourceTypeDef,
@@ -963,15 +1019,15 @@
     total=False,
 )
 
 DescribeApplicationResponseTypeDef = TypedDict(
     "DescribeApplicationResponseTypeDef",
     {
         "ApplicationDetail": ApplicationDetailTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateApplicationRequestRequestTypeDef = TypedDict(
     "UpdateApplicationRequestRequestTypeDef",
     {
         "ApplicationName": str,
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-kinesisanalytics
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.KinesisAnalytics 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore kinesisanalytics type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore kinesisanalytics type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-kinesisanalytics"></a>
 
 # types-aiobotocore-kinesisanalytics
 
 [![PyPI - types-aiobotocore-kinesisanalytics](https://img.shields.io/pypi/v/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-kinesisanalytics.svg?color=blue)](https://pypi.org/project/types-aiobotocore-kinesisanalytics)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-kinesisanalytics?color=blue)](https://pypistats.org/packages/types-aiobotocore-kinesisanalytics)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-kinesisanalytics)](https://pepy.tech/project/types-aiobotocore-kinesisanalytics)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.KinesisAnalytics 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kinesisanalytics.html#KinesisAnalytics)
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
 [types-aiobotocore-kinesisanalytics docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_kinesisanalytics/).
 
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
@@ -283,34 +282,35 @@
 )
 
 
 def check_value(value: ApplicationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_kinesisanalytics.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_kinesisanalytics.type_defs import (
     CloudWatchLoggingOptionTypeDef,
     CloudWatchLoggingOptionDescriptionTypeDef,
     ApplicationSummaryTypeDef,
     CloudWatchLoggingOptionUpdateTypeDef,
     CSVMappingParametersTypeDef,
     TagTypeDef,
+    ResponseMetadataTypeDef,
     DeleteApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
     DeleteApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DeleteApplicationOutputRequestRequestTypeDef,
     DeleteApplicationReferenceDataSourceRequestRequestTypeDef,
-    DeleteApplicationRequestRequestTypeDef,
+    TimestampTypeDef,
     DescribeApplicationRequestRequestTypeDef,
     DestinationSchemaTypeDef,
     InputStartingPositionConfigurationTypeDef,
     S3ConfigurationTypeDef,
     InputParallelismTypeDef,
     KinesisFirehoseInputDescriptionTypeDef,
     KinesisStreamsInputDescriptionTypeDef,
@@ -334,55 +334,56 @@
     LambdaOutputTypeDef,
     LambdaOutputUpdateTypeDef,
     ListApplicationsRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ReferenceDataSourceDescriptionTypeDef,
     S3ReferenceDataSourceTypeDef,
     S3ReferenceDataSourceUpdateTypeDef,
-    ResponseMetadataTypeDef,
     StopApplicationRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     AddApplicationCloudWatchLoggingOptionRequestRequestTypeDef,
+    TagResourceRequestRequestTypeDef,
     CreateApplicationResponseTypeDef,
     ListApplicationsResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
-    TagResourceRequestRequestTypeDef,
+    DeleteApplicationRequestRequestTypeDef,
     InputConfigurationTypeDef,
     InputProcessingConfigurationDescriptionTypeDef,
     InputProcessingConfigurationTypeDef,
     InputProcessingConfigurationUpdateTypeDef,
     MappingParametersTypeDef,
     OutputDescriptionTypeDef,
     OutputTypeDef,
     OutputUpdateTypeDef,
     StartApplicationRequestRequestTypeDef,
     AddApplicationInputProcessingConfigurationRequestRequestTypeDef,
     DiscoverInputSchemaRequestRequestTypeDef,
     RecordFormatTypeDef,
     AddApplicationOutputRequestRequestTypeDef,
     InputSchemaUpdateTypeDef,
+    SourceSchemaOutputTypeDef,
     SourceSchemaTypeDef,
     InputUpdateTypeDef,
     DiscoverInputSchemaResponseTypeDef,
     InputDescriptionTypeDef,
-    InputTypeDef,
     ReferenceDataSourceDescriptionTypeDef,
+    InputTypeDef,
     ReferenceDataSourceTypeDef,
     ReferenceDataSourceUpdateTypeDef,
+    ApplicationDetailTypeDef,
     AddApplicationInputRequestRequestTypeDef,
     CreateApplicationRequestRequestTypeDef,
-    ApplicationDetailTypeDef,
     AddApplicationReferenceDataSourceRequestRequestTypeDef,
     ApplicationUpdateTypeDef,
     DescribeApplicationResponseTypeDef,
     UpdateApplicationRequestRequestTypeDef,
 )
 
 
-def get_structure() -> CloudWatchLoggingOptionTypeDef:
+def get_value() -> CloudWatchLoggingOptionTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-kinesisanalytics-2.5.2/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt` & `types-aiobotocore-kinesisanalytics-2.5.2.post1/types_aiobotocore_kinesisanalytics.egg-info/SOURCES.txt`

 * *Files identical despite different names*


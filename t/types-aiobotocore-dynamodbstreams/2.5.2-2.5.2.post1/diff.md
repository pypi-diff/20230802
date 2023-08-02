# Comparing `tmp/types-aiobotocore-dynamodbstreams-2.5.2.tar.gz` & `tmp/types-aiobotocore-dynamodbstreams-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.5.2.tar", last modified: Sat Jul  8 01:43:33 2023, max compression
+gzip compressed data, was "types-aiobotocore-dynamodbstreams-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:12 2023, max compression
```

## Comparing `types-aiobotocore-dynamodbstreams-2.5.2.tar` & `types-aiobotocore-dynamodbstreams-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.062045 types-aiobotocore-dynamodbstreams-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-08 01:43:33.062045 types-aiobotocore-dynamodbstreams-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11450 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:33.062045 types-aiobotocore-dynamodbstreams-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.062045 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-07-08 01:29:15.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-07-08 01:29:15.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-08 01:29:15.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:29:14.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:33.062045 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-08 01:43:32.000000 types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodbstreams-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-08-02 14:52:12.245600 types-aiobotocore-dynamodbstreams-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11433 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:12.249600 types-aiobotocore-dynamodbstreams-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.245600 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     6300 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:36:54.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:12.245600 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12983 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 14:52:12.000000 types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/LICENSE` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dynamodbstreams type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dynamodbstreams type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dynamodbstreams"></a>
 
 # types-aiobotocore-dynamodbstreams
 
 [![PyPI - types-aiobotocore-dynamodbstreams](https://img.shields.io/pypi/v/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodbstreams?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodbstreams)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DynamoDBStreams 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
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
@@ -285,45 +284,45 @@
 )
 
 
 def check_value(value: KeyTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dynamodbstreams.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AttributeValueTypeDef:
+def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/README.md` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-dynamodbstreams"></a>
 
 # types-aiobotocore-dynamodbstreams
 
 [![PyPI - types-aiobotocore-dynamodbstreams](https://img.shields.io/pypi/v/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodbstreams?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodbstreams)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DynamoDBStreams 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
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
@@ -252,45 +252,45 @@
 )
 
 
 def check_value(value: KeyTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dynamodbstreams.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AttributeValueTypeDef:
+def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/setup.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-dynamodbstreams",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_dynamodbstreams"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with"
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
-    keywords="aiobotocore dynamodbstreams type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore dynamodbstreams type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_dynamodbstreams": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/"
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/__main__.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.DynamoDBStreams 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.DynamoDBStreams 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams\nOther"
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

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/client.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/client.pyi` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/literals.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/literals.pyi` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/type_defs.py` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dynamodbstreams.type_defs import AttributeValueTypeDef
 
-    data: AttributeValueTypeDef = {...}
+    data: AttributeValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List
 
 from .literals import (
@@ -28,24 +28,24 @@
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IdentityTypeDef",
     "KeySchemaElementTypeDef",
     "ListStreamsInputRequestTypeDef",
     "StreamTypeDef",
     "StreamRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "RecordTypeDef",
     "ShardTypeDef",
     "GetRecordsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "DescribeStreamOutputTypeDef",
 )
@@ -85,14 +85,25 @@
 
 class DescribeStreamInputRequestTypeDef(
     _RequiredDescribeStreamInputRequestTypeDef, _OptionalDescribeStreamInputRequestTypeDef
 ):
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
+
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -129,22 +140,14 @@
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "PrincipalId": str,
         "Type": str,
     },
     total=False,
@@ -188,40 +191,37 @@
         "SequenceNumber": str,
         "SizeBytes": int,
         "StreamViewType": StreamViewTypeType,
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
 SequenceNumberRangeTypeDef = TypedDict(
     "SequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
         "EndingSequenceNumber": str,
     },
     total=False,
 )
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "Streams": List[StreamTypeDef],
         "LastEvaluatedStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "eventID": str,
@@ -246,15 +246,15 @@
 )
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamDescriptionTypeDef = TypedDict(
     "StreamDescriptionTypeDef",
     {
         "StreamArn": str,
@@ -270,10 +270,10 @@
     total=False,
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams/type_defs.pyi` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_dynamodbstreams.type_defs import AttributeValueTypeDef
 
-    data: AttributeValueTypeDef = {...}
+    data: AttributeValueTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List
 
 from .literals import (
@@ -27,24 +27,24 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttributeValueTypeDef",
     "DescribeStreamInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRecordsInputRequestTypeDef",
     "GetShardIteratorInputRequestTypeDef",
-    "GetShardIteratorOutputTypeDef",
     "IdentityTypeDef",
     "KeySchemaElementTypeDef",
     "ListStreamsInputRequestTypeDef",
     "StreamTypeDef",
     "StreamRecordTypeDef",
-    "ResponseMetadataTypeDef",
     "SequenceNumberRangeTypeDef",
+    "GetShardIteratorOutputTypeDef",
     "ListStreamsOutputTypeDef",
     "RecordTypeDef",
     "ShardTypeDef",
     "GetRecordsOutputTypeDef",
     "StreamDescriptionTypeDef",
     "DescribeStreamOutputTypeDef",
 )
@@ -82,14 +82,25 @@
 )
 
 class DescribeStreamInputRequestTypeDef(
     _RequiredDescribeStreamInputRequestTypeDef, _OptionalDescribeStreamInputRequestTypeDef
 ):
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
+
 _RequiredGetRecordsInputRequestTypeDef = TypedDict(
     "_RequiredGetRecordsInputRequestTypeDef",
     {
         "ShardIterator": str,
     },
 )
 _OptionalGetRecordsInputRequestTypeDef = TypedDict(
@@ -122,22 +133,14 @@
 )
 
 class GetShardIteratorInputRequestTypeDef(
     _RequiredGetShardIteratorInputRequestTypeDef, _OptionalGetShardIteratorInputRequestTypeDef
 ):
     pass
 
-GetShardIteratorOutputTypeDef = TypedDict(
-    "GetShardIteratorOutputTypeDef",
-    {
-        "ShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 IdentityTypeDef = TypedDict(
     "IdentityTypeDef",
     {
         "PrincipalId": str,
         "Type": str,
     },
     total=False,
@@ -181,40 +184,37 @@
         "SequenceNumber": str,
         "SizeBytes": int,
         "StreamViewType": StreamViewTypeType,
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
 SequenceNumberRangeTypeDef = TypedDict(
     "SequenceNumberRangeTypeDef",
     {
         "StartingSequenceNumber": str,
         "EndingSequenceNumber": str,
     },
     total=False,
 )
 
+GetShardIteratorOutputTypeDef = TypedDict(
+    "GetShardIteratorOutputTypeDef",
+    {
+        "ShardIterator": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListStreamsOutputTypeDef = TypedDict(
     "ListStreamsOutputTypeDef",
     {
         "Streams": List[StreamTypeDef],
         "LastEvaluatedStreamArn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RecordTypeDef = TypedDict(
     "RecordTypeDef",
     {
         "eventID": str,
@@ -239,15 +239,15 @@
 )
 
 GetRecordsOutputTypeDef = TypedDict(
     "GetRecordsOutputTypeDef",
     {
         "Records": List[RecordTypeDef],
         "NextShardIterator": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StreamDescriptionTypeDef = TypedDict(
     "StreamDescriptionTypeDef",
     {
         "StreamArn": str,
@@ -263,10 +263,10 @@
     total=False,
 )
 
 DescribeStreamOutputTypeDef = TypedDict(
     "DescribeStreamOutputTypeDef",
     {
         "StreamDescription": StreamDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-dynamodbstreams
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.DynamoDBStreams 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore dynamodbstreams type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore dynamodbstreams type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-dynamodbstreams"></a>
 
 # types-aiobotocore-dynamodbstreams
 
 [![PyPI - types-aiobotocore-dynamodbstreams](https://img.shields.io/pypi/v/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-dynamodbstreams.svg?color=blue)](https://pypi.org/project/types-aiobotocore-dynamodbstreams)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-dynamodbstreams?color=blue)](https://pypistats.org/packages/types-aiobotocore-dynamodbstreams)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-dynamodbstreams)](https://pepy.tech/project/types-aiobotocore-dynamodbstreams)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.DynamoDBStreams 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodbstreams.html#DynamoDBStreams)
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
 [types-aiobotocore-dynamodbstreams docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_dynamodbstreams/).
 
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
@@ -285,45 +284,45 @@
 )
 
 
 def check_value(value: KeyTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_dynamodbstreams.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_dynamodbstreams.type_defs import (
     AttributeValueTypeDef,
     DescribeStreamInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     GetRecordsInputRequestTypeDef,
     GetShardIteratorInputRequestTypeDef,
-    GetShardIteratorOutputTypeDef,
     IdentityTypeDef,
     KeySchemaElementTypeDef,
     ListStreamsInputRequestTypeDef,
     StreamTypeDef,
     StreamRecordTypeDef,
-    ResponseMetadataTypeDef,
     SequenceNumberRangeTypeDef,
+    GetShardIteratorOutputTypeDef,
     ListStreamsOutputTypeDef,
     RecordTypeDef,
     ShardTypeDef,
     GetRecordsOutputTypeDef,
     StreamDescriptionTypeDef,
     DescribeStreamOutputTypeDef,
 )
 
 
-def get_structure() -> AttributeValueTypeDef:
+def get_value() -> AttributeValueTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-dynamodbstreams-2.5.2/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt` & `types-aiobotocore-dynamodbstreams-2.5.2.post1/types_aiobotocore_dynamodbstreams.egg-info/SOURCES.txt`

 * *Files identical despite different names*


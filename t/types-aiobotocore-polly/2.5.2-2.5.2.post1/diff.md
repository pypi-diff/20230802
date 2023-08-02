# Comparing `tmp/types-aiobotocore-polly-2.5.2.tar.gz` & `tmp/types-aiobotocore-polly-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-polly-2.5.2.tar", last modified: Sat Jul  8 01:44:08 2023, max compression
+gzip compressed data, was "types-aiobotocore-polly-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:49 2023, max compression
```

## Comparing `types-aiobotocore-polly-2.5.2.tar` & `types-aiobotocore-polly-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12651 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:08.378708 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8938 2023-07-08 01:36:45.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:36:43.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:08.386708 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:44:08.000000 types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12634 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:45:02.000000 types-aiobotocore-polly-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.625493 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12645 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12624 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-08-02 14:45:05.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10607 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-08-02 14:45:05.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-08-02 14:45:05.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:45:04.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:49.629493 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14144 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:49.000000 types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-polly-2.5.2/LICENSE` & `types-aiobotocore-polly-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/PKG-INFO` & `types-aiobotocore-polly-2.5.2.post1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,29 @@
-Metadata-Version: 2.1
-Name: types-aiobotocore-polly
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.14.5
-Home-page: https://github.com/youtype/mypy_boto3_builder
-Author: Vlad Emelianov
-Author-email: vlad.emelianov.nz@gmail.com
-License: MIT License
-Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
-Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
-Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore polly type-annotations boto3-stubs mypy typeshed autocomplete
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Console
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-polly?color=blue)](https://pypistats.org/packages/types-aiobotocore-polly)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -74,15 +41,15 @@
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
@@ -321,53 +288,53 @@
 )
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_polly.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
     ListLexiconsOutputTypeDef,
 )
 
 
-def get_structure() -> DeleteLexiconInputRequestTypeDef:
+def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-polly-2.5.2/README.md` & `types-aiobotocore-polly-2.5.2.post1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,61 @@
+Metadata-Version: 2.1
+Name: types-aiobotocore-polly
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.1
+Home-page: https://github.com/youtype/mypy_boto3_builder
+Author: Vlad Emelianov
+Author-email: vlad.emelianov.nz@gmail.com
+License: MIT License
+Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
+Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
+Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
+Keywords: aiobotocore polly type-annotations botocore mypy typeshed autocomplete
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-polly?color=blue)](https://pypistats.org/packages/types-aiobotocore-polly)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
 See how it helps to find and fix potential bugs:
 
@@ -41,15 +73,15 @@
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
@@ -288,53 +320,53 @@
 )
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_polly.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
     ListLexiconsOutputTypeDef,
 )
 
 
-def get_structure() -> DeleteLexiconInputRequestTypeDef:
+def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-polly-2.5.2/setup.py` & `types-aiobotocore-polly-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-polly",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_polly"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore polly type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore polly type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_polly": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/"
```

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.py` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__init__.pyi` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/__main__.py` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Polly 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Polly 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly\nOther"
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

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.py` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/client.pyi` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.py` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/literals.pyi` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.py` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,43 +58,43 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#describevoicespaginator)
         """
 
 
 class ListLexiconsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listlexiconspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLexiconsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listlexiconspaginator)
         """
 
 
 class ListSpeechSynthesisTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listspeechsynthesistaskspaginator)
     """
 
     def paginate(
-        self, *, Status: TaskStatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: TaskStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpeechSynthesisTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listspeechsynthesistaskspaginator)
         """
```

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/paginator.pyi` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -55,41 +55,41 @@
 
     def paginate(
         self,
         *,
         Engine: EngineType = ...,
         LanguageCode: LanguageCodeType = ...,
         IncludeAdditionalLanguageCodes: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeVoicesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.DescribeVoices.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#describevoicespaginator)
         """
 
 class ListLexiconsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listlexiconspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListLexiconsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListLexicons.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listlexiconspaginator)
         """
 
 class ListSpeechSynthesisTasksPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listspeechsynthesistaskspaginator)
     """
 
     def paginate(
-        self, *, Status: TaskStatusType = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Status: TaskStatusType = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSpeechSynthesisTasksOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly.Paginator.ListSpeechSynthesisTasks.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/paginators/#listspeechsynthesistaskspaginator)
         """
```

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.py` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
-    data: DeleteLexiconInputRequestTypeDef = {...}
+    data: DeleteLexiconInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from aiobotocore.response import StreamingBody
@@ -32,31 +32,31 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteLexiconInputRequestTypeDef",
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeVoicesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
     "LexiconAttributesTypeDef",
     "LexiconTypeDef",
     "GetSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesisTaskTypeDef",
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
     "ListLexiconsInputRequestTypeDef",
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "ListSpeechSynthesisTasksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLexiconInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesizeSpeechInputRequestTypeDef",
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "SynthesizeSpeechOutputTypeDef",
     "DescribeVoicesOutputTypeDef",
     "LexiconDescriptionTypeDef",
     "GetLexiconOutputTypeDef",
     "GetSpeechSynthesisTaskOutputTypeDef",
     "ListSpeechSynthesisTasksOutputTypeDef",
     "StartSpeechSynthesisTaskOutputTypeDef",
@@ -66,21 +66,20 @@
 DeleteLexiconInputRequestTypeDef = TypedDict(
     "DeleteLexiconInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Engine": EngineType,
-        "LanguageCode": LanguageCodeType,
-        "IncludeAdditionalLanguageCodes": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeVoicesInputRequestTypeDef = TypedDict(
     "DescribeVoicesInputRequestTypeDef",
     {
@@ -88,14 +87,25 @@
         "LanguageCode": LanguageCodeType,
         "IncludeAdditionalLanguageCodes": bool,
         "NextToken": str,
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
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": GenderType,
         "Id": VoiceIdType,
         "LanguageCode": LanguageCodeType,
         "LanguageName": str,
@@ -160,78 +170,40 @@
         "TextType": TextTypeType,
         "VoiceId": VoiceIdType,
         "LanguageCode": LanguageCodeType,
     },
     total=False,
 )
 
-ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLexiconsInputRequestTypeDef = TypedDict(
     "ListLexiconsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
-    {
-        "Status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpeechSynthesisTasksInputRequestTypeDef = TypedDict(
     "ListSpeechSynthesisTasksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Status": TaskStatusType,
     },
     total=False,
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
 PutLexiconInputRequestTypeDef = TypedDict(
     "PutLexiconInputRequestTypeDef",
     {
         "Name": str,
         "Content": str,
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
 _RequiredStartSpeechSynthesisTaskInputRequestTypeDef = TypedDict(
     "_RequiredStartSpeechSynthesisTaskInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "OutputS3BucketName": str,
         "Text": str,
         "VoiceId": VoiceIdType,
@@ -284,30 +256,58 @@
 
 class SynthesizeSpeechInputRequestTypeDef(
     _RequiredSynthesizeSpeechInputRequestTypeDef, _OptionalSynthesizeSpeechInputRequestTypeDef
 ):
     pass
 
 
+DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    {
+        "Engine": EngineType,
+        "LanguageCode": LanguageCodeType,
+        "IncludeAdditionalLanguageCodes": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
+    {
+        "Status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 SynthesizeSpeechOutputTypeDef = TypedDict(
     "SynthesizeSpeechOutputTypeDef",
     {
         "AudioStream": StreamingBody,
         "ContentType": str,
         "RequestCharacters": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": str,
@@ -317,44 +317,44 @@
 )
 
 GetLexiconOutputTypeDef = TypedDict(
     "GetLexiconOutputTypeDef",
     {
         "Lexicon": LexiconTypeDef,
         "LexiconAttributes": LexiconAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "GetSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
         "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly/type_defs.pyi` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_polly.type_defs import DeleteLexiconInputRequestTypeDef
 
-    data: DeleteLexiconInputRequestTypeDef = {...}
+    data: DeleteLexiconInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from aiobotocore.response import StreamingBody
@@ -31,31 +31,31 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteLexiconInputRequestTypeDef",
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeVoicesInputRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "VoiceTypeDef",
     "GetLexiconInputRequestTypeDef",
     "LexiconAttributesTypeDef",
     "LexiconTypeDef",
     "GetSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesisTaskTypeDef",
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
     "ListLexiconsInputRequestTypeDef",
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "ListSpeechSynthesisTasksInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "PutLexiconInputRequestTypeDef",
-    "ResponseMetadataTypeDef",
     "StartSpeechSynthesisTaskInputRequestTypeDef",
     "SynthesizeSpeechInputRequestTypeDef",
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
     "SynthesizeSpeechOutputTypeDef",
     "DescribeVoicesOutputTypeDef",
     "LexiconDescriptionTypeDef",
     "GetLexiconOutputTypeDef",
     "GetSpeechSynthesisTaskOutputTypeDef",
     "ListSpeechSynthesisTasksOutputTypeDef",
     "StartSpeechSynthesisTaskOutputTypeDef",
@@ -65,21 +65,20 @@
 DeleteLexiconInputRequestTypeDef = TypedDict(
     "DeleteLexiconInputRequestTypeDef",
     {
         "Name": str,
     },
 )
 
-DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
-    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "Engine": EngineType,
-        "LanguageCode": LanguageCodeType,
-        "IncludeAdditionalLanguageCodes": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
 DescribeVoicesInputRequestTypeDef = TypedDict(
     "DescribeVoicesInputRequestTypeDef",
     {
@@ -87,14 +86,25 @@
         "LanguageCode": LanguageCodeType,
         "IncludeAdditionalLanguageCodes": bool,
         "NextToken": str,
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
 VoiceTypeDef = TypedDict(
     "VoiceTypeDef",
     {
         "Gender": GenderType,
         "Id": VoiceIdType,
         "LanguageCode": LanguageCodeType,
         "LanguageName": str,
@@ -159,78 +169,40 @@
         "TextType": TextTypeType,
         "VoiceId": VoiceIdType,
         "LanguageCode": LanguageCodeType,
     },
     total=False,
 )
 
-ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
-    "ListLexiconsInputListLexiconsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListLexiconsInputRequestTypeDef = TypedDict(
     "ListLexiconsInputRequestTypeDef",
     {
         "NextToken": str,
     },
     total=False,
 )
 
-ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
-    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
-    {
-        "Status": TaskStatusType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListSpeechSynthesisTasksInputRequestTypeDef = TypedDict(
     "ListSpeechSynthesisTasksInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "Status": TaskStatusType,
     },
     total=False,
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
 PutLexiconInputRequestTypeDef = TypedDict(
     "PutLexiconInputRequestTypeDef",
     {
         "Name": str,
         "Content": str,
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
 _RequiredStartSpeechSynthesisTaskInputRequestTypeDef = TypedDict(
     "_RequiredStartSpeechSynthesisTaskInputRequestTypeDef",
     {
         "OutputFormat": OutputFormatType,
         "OutputS3BucketName": str,
         "Text": str,
         "VoiceId": VoiceIdType,
@@ -279,30 +251,58 @@
 )
 
 class SynthesizeSpeechInputRequestTypeDef(
     _RequiredSynthesizeSpeechInputRequestTypeDef, _OptionalSynthesizeSpeechInputRequestTypeDef
 ):
     pass
 
+DescribeVoicesInputDescribeVoicesPaginateTypeDef = TypedDict(
+    "DescribeVoicesInputDescribeVoicesPaginateTypeDef",
+    {
+        "Engine": EngineType,
+        "LanguageCode": LanguageCodeType,
+        "IncludeAdditionalLanguageCodes": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListLexiconsInputListLexiconsPaginateTypeDef = TypedDict(
+    "ListLexiconsInputListLexiconsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef = TypedDict(
+    "ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef",
+    {
+        "Status": TaskStatusType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 SynthesizeSpeechOutputTypeDef = TypedDict(
     "SynthesizeSpeechOutputTypeDef",
     {
         "AudioStream": StreamingBody,
         "ContentType": str,
         "RequestCharacters": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeVoicesOutputTypeDef = TypedDict(
     "DescribeVoicesOutputTypeDef",
     {
         "Voices": List[VoiceTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 LexiconDescriptionTypeDef = TypedDict(
     "LexiconDescriptionTypeDef",
     {
         "Name": str,
@@ -312,44 +312,44 @@
 )
 
 GetLexiconOutputTypeDef = TypedDict(
     "GetLexiconOutputTypeDef",
     {
         "Lexicon": LexiconTypeDef,
         "LexiconAttributes": LexiconAttributesTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "GetSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSpeechSynthesisTasksOutputTypeDef = TypedDict(
     "ListSpeechSynthesisTasksOutputTypeDef",
     {
         "NextToken": str,
         "SynthesisTasks": List[SynthesisTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartSpeechSynthesisTaskOutputTypeDef = TypedDict(
     "StartSpeechSynthesisTaskOutputTypeDef",
     {
         "SynthesisTask": SynthesisTaskTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListLexiconsOutputTypeDef = TypedDict(
     "ListLexiconsOutputTypeDef",
     {
         "Lexicons": List[LexiconDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/PKG-INFO` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-polly
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Polly 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore polly type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore polly type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-polly"></a>
 
 # types-aiobotocore-polly
 
 [![PyPI - types-aiobotocore-polly](https://img.shields.io/pypi/v/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-polly.svg?color=blue)](https://pypi.org/project/types-aiobotocore-polly)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-polly?color=blue)](https://pypistats.org/packages/types-aiobotocore-polly)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-polly)](https://pepy.tech/project/types-aiobotocore-polly)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Polly 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/polly.html#Polly)
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
 [types-aiobotocore-polly docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_polly/).
 
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
@@ -321,53 +320,53 @@
 )
 
 
 def check_value(value: DescribeVoicesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_polly.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_polly.type_defs import (
     DeleteLexiconInputRequestTypeDef,
-    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeVoicesInputRequestTypeDef,
+    ResponseMetadataTypeDef,
     VoiceTypeDef,
     GetLexiconInputRequestTypeDef,
     LexiconAttributesTypeDef,
     LexiconTypeDef,
     GetSpeechSynthesisTaskInputRequestTypeDef,
     SynthesisTaskTypeDef,
-    ListLexiconsInputListLexiconsPaginateTypeDef,
     ListLexiconsInputRequestTypeDef,
-    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     ListSpeechSynthesisTasksInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     PutLexiconInputRequestTypeDef,
-    ResponseMetadataTypeDef,
     StartSpeechSynthesisTaskInputRequestTypeDef,
     SynthesizeSpeechInputRequestTypeDef,
+    DescribeVoicesInputDescribeVoicesPaginateTypeDef,
+    ListLexiconsInputListLexiconsPaginateTypeDef,
+    ListSpeechSynthesisTasksInputListSpeechSynthesisTasksPaginateTypeDef,
     SynthesizeSpeechOutputTypeDef,
     DescribeVoicesOutputTypeDef,
     LexiconDescriptionTypeDef,
     GetLexiconOutputTypeDef,
     GetSpeechSynthesisTaskOutputTypeDef,
     ListSpeechSynthesisTasksOutputTypeDef,
     StartSpeechSynthesisTaskOutputTypeDef,
     ListLexiconsOutputTypeDef,
 )
 
 
-def get_structure() -> DeleteLexiconInputRequestTypeDef:
+def get_value() -> DeleteLexiconInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-polly-2.5.2/types_aiobotocore_polly.egg-info/SOURCES.txt` & `types-aiobotocore-polly-2.5.2.post1/types_aiobotocore_polly.egg-info/SOURCES.txt`

 * *Files identical despite different names*


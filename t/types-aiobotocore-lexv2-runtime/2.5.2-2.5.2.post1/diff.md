# Comparing `tmp/types-aiobotocore-lexv2-runtime-2.5.2.tar.gz` & `tmp/types-aiobotocore-lexv2-runtime-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lexv2-runtime-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-lexv2-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-lexv2-runtime-2.5.2.tar` & `types-aiobotocore-lexv2-runtime-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.542431 types-aiobotocore-lexv2-runtime-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-08 01:43:53.542431 types-aiobotocore-lexv2-runtime-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11776 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.542431 types-aiobotocore-lexv2-runtime-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.522431 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11323 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:01.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.542431 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13364 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:43:53.000000 types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.669542 types-aiobotocore-lexv2-runtime-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-08-02 14:52:33.665542 types-aiobotocore-lexv2-runtime-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.669542 types-aiobotocore-lexv2-runtime-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.665542 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8577 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    14980 2023-08-02 14:42:11.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14952 2023-08-02 14:42:11.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:10.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.665542 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13637 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:33.000000 types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/LICENSE` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/PKG-INFO` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lexv2-runtime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lexv2-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lexv2-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-runtime"></a>
 
 # types-aiobotocore-lexv2-runtime
 
 [![PyPI - types-aiobotocore-lexv2-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lexv2-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lexv2-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-runtime)](https://pepy.tech/project/types-aiobotocore-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexRuntimeV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [types-aiobotocore-lexv2-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/).
 
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
@@ -287,57 +286,69 @@
 )
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lexv2_runtime.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
+    IntentOutputTypeDef,
     IntentTypeDef,
-    PutSessionResponseTypeDef,
     RecognizedBotMemberTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    RecognizeUtteranceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
+    RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
+    ValueOutputTypeDef,
     ValueTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
+    DeleteSessionResponseTypeDef,
+    PutSessionResponseTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
     RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
+    SessionStateOutputTypeDef,
     SessionStateTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
+    SessionStateUnionTypeDef,
+    MessageUnionTypeDef,
     GetSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
+    PutSessionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/README.md` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-lexv2-runtime"></a>
 
 # types-aiobotocore-lexv2-runtime
 
 [![PyPI - types-aiobotocore-lexv2-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lexv2-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lexv2-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-runtime)](https://pepy.tech/project/types-aiobotocore-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexRuntimeV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [types-aiobotocore-lexv2-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/).
 
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
@@ -254,57 +254,69 @@
 )
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lexv2_runtime.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
+    IntentOutputTypeDef,
     IntentTypeDef,
-    PutSessionResponseTypeDef,
     RecognizedBotMemberTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    RecognizeUtteranceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
+    RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
+    ValueOutputTypeDef,
     ValueTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
+    DeleteSessionResponseTypeDef,
+    PutSessionResponseTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
     RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
+    SessionStateOutputTypeDef,
     SessionStateTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
+    SessionStateUnionTypeDef,
+    MessageUnionTypeDef,
     GetSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
+    PutSessionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/setup.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lexv2-runtime",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_lexv2_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with"
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
-    keywords="aiobotocore lexv2-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore lexv2-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lexv2_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/"
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/__main__.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexRuntimeV2 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.LexRuntimeV2 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2\nOther"
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

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/client.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client
 
     session = get_session()
     async with session.create_client("lexv2-runtime") as client:
         client: LexRuntimeV2Client
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
     GetSessionResponseTypeDef,
-    MessageTypeDef,
+    MessageUnionTypeDef,
     PutSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
-    SessionStateTypeDef,
+    SessionStateUnionTypeDef,
 )
 
 __all__ = ("LexRuntimeV2Client",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
@@ -123,16 +123,16 @@
     async def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: SessionStateTypeDef,
-        messages: Sequence[MessageTypeDef] = ...,
+        sessionState: SessionStateUnionTypeDef,
+        messages: Sequence[MessageUnionTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -143,15 +143,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: SessionStateTypeDef = ...,
+        sessionState: SessionStateUnionTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/client/#recognize_text)
@@ -164,15 +164,15 @@
         botAliasId: str,
         localeId: str,
         sessionId: str,
         requestContentType: str,
         sessionState: str = ...,
         requestAttributes: str = ...,
         responseContentType: str = ...,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody] = ...
+        inputStream: BlobTypeDef = ...
     ) -> RecognizeUtteranceResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_utterance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/client/#recognize_utterance)
         """
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/client.pyi` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -10,28 +10,28 @@
     from types_aiobotocore_lexv2_runtime.client import LexRuntimeV2Client
 
     session = get_session()
     async with session.create_client("lexv2-runtime") as client:
         client: LexRuntimeV2Client
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
     GetSessionResponseTypeDef,
-    MessageTypeDef,
+    MessageUnionTypeDef,
     PutSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
     RecognizeUtteranceResponseTypeDef,
-    SessionStateTypeDef,
+    SessionStateUnionTypeDef,
 )
 
 __all__ = ("LexRuntimeV2Client",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -114,16 +114,16 @@
     async def put_session(
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
-        sessionState: SessionStateTypeDef,
-        messages: Sequence[MessageTypeDef] = ...,
+        sessionState: SessionStateUnionTypeDef,
+        messages: Sequence[MessageUnionTypeDef] = ...,
         requestAttributes: Mapping[str, str] = ...,
         responseContentType: str = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex V2 bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.put_session)
@@ -133,15 +133,15 @@
         self,
         *,
         botId: str,
         botAliasId: str,
         localeId: str,
         sessionId: str,
         text: str,
-        sessionState: SessionStateTypeDef = ...,
+        sessionState: SessionStateUnionTypeDef = ...,
         requestAttributes: Mapping[str, str] = ...
     ) -> RecognizeTextResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/client/#recognize_text)
@@ -153,15 +153,15 @@
         botAliasId: str,
         localeId: str,
         sessionId: str,
         requestContentType: str,
         sessionState: str = ...,
         requestAttributes: str = ...,
         responseContentType: str = ...,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody] = ...
+        inputStream: BlobTypeDef = ...
     ) -> RecognizeUtteranceResponseTypeDef:
         """
         Sends user input to Amazon Lex V2.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2.Client.recognize_utterance)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/client/#recognize_utterance)
         """
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/literals.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/literals.pyi` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/type_defs.py` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
@@ -27,56 +27,68 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
+    "IntentOutputTypeDef",
     "IntentTypeDef",
-    "PutSessionResponseTypeDef",
     "RecognizedBotMemberTypeDef",
-    "RecognizeUtteranceRequestRequestTypeDef",
-    "RecognizeUtteranceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
+    "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
+    "ValueOutputTypeDef",
     "ValueTypeDef",
+    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "RecognizeUtteranceRequestRequestTypeDef",
+    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "RecognizeUtteranceResponseTypeDef",
+    "RuntimeHintDetailsOutputTypeDef",
     "RuntimeHintDetailsTypeDef",
     "SentimentResponseTypeDef",
+    "SlotOutputTypeDef",
     "SlotTypeDef",
+    "SessionStateOutputTypeDef",
     "SessionStateTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
-    "PutSessionRequestRequestTypeDef",
+    "SessionStateUnionTypeDef",
+    "MessageUnionTypeDef",
     "GetSessionResponseTypeDef",
     "RecognizeTextResponseTypeDef",
+    "PutSessionRequestRequestTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -95,22 +107,22 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
@@ -122,171 +134,120 @@
         "slotToElicit": str,
         "slotElicitationStyle": StyleTypeType,
         "subSlotToElicit": "ElicitSubSlotTypeDef",
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-
 _RequiredElicitSubSlotTypeDef = TypedDict(
     "_RequiredElicitSubSlotTypeDef",
     {
         "name": str,
     },
 )
 _OptionalElicitSubSlotTypeDef = TypedDict(
     "_OptionalElicitSubSlotTypeDef",
     {
         "subSlotToElicit": Dict[str, Any],
     },
     total=False,
 )
 
-
 class ElicitSubSlotTypeDef(_RequiredElicitSubSlotTypeDef, _OptionalElicitSubSlotTypeDef):
     pass
 
-
 GetSessionRequestRequestTypeDef = TypedDict(
     "GetSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
+_RequiredIntentOutputTypeDef = TypedDict(
+    "_RequiredIntentOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalIntentOutputTypeDef = TypedDict(
+    "_OptionalIntentOutputTypeDef",
+    {
+        "slots": Dict[str, "SlotOutputTypeDef"],
+        "state": IntentStateType,
+        "confirmationState": ConfirmationStateType,
+    },
+    total=False,
+)
+
+class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
+    pass
+
 _RequiredIntentTypeDef = TypedDict(
     "_RequiredIntentTypeDef",
     {
         "name": str,
     },
 )
 _OptionalIntentTypeDef = TypedDict(
     "_OptionalIntentTypeDef",
     {
-        "slots": Dict[str, "SlotTypeDef"],
+        "slots": Mapping[str, "SlotTypeDef"],
         "state": IntentStateType,
         "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
-
 class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
     pass
 
-
-PutSessionResponseTypeDef = TypedDict(
-    "PutSessionResponseTypeDef",
-    {
-        "contentType": str,
-        "messages": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "audioStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredRecognizedBotMemberTypeDef = TypedDict(
     "_RequiredRecognizedBotMemberTypeDef",
     {
         "botId": str,
     },
 )
 _OptionalRecognizedBotMemberTypeDef = TypedDict(
     "_OptionalRecognizedBotMemberTypeDef",
     {
         "botName": str,
     },
     total=False,
 )
 
-
 class RecognizedBotMemberTypeDef(
     _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
 ):
     pass
 
-
-_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "requestContentType": str,
-    },
-)
-_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "sessionState": str,
-        "requestAttributes": str,
-        "responseContentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-
-class RecognizeUtteranceRequestRequestTypeDef(
-    _RequiredRecognizeUtteranceRequestRequestTypeDef,
-    _OptionalRecognizeUtteranceRequestRequestTypeDef,
-):
-    pass
-
-
-RecognizeUtteranceResponseTypeDef = TypedDict(
-    "RecognizeUtteranceResponseTypeDef",
+RuntimeHintValueTypeDef = TypedDict(
+    "RuntimeHintValueTypeDef",
     {
-        "inputMode": str,
-        "contentType": str,
-        "messages": str,
-        "interpretations": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "inputTranscript": str,
-        "audioStream": StreamingBody,
-        "recognizedBotMember": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "phrase": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RuntimeHintsOutputTypeDef = TypedDict(
+    "RuntimeHintsOutputTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
-RuntimeHintValueTypeDef = TypedDict(
-    "RuntimeHintValueTypeDef",
-    {
-        "phrase": str,
+        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
     },
+    total=False,
 )
 
 RuntimeHintsTypeDef = TypedDict(
     "RuntimeHintsTypeDef",
     {
-        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsTypeDef"]],
+        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
     },
     total=False,
 )
 
 SentimentScoreTypeDef = TypedDict(
     "SentimentScoreTypeDef",
     {
@@ -294,108 +255,271 @@
         "negative": float,
         "neutral": float,
         "mixed": float,
     },
     total=False,
 )
 
+_RequiredValueOutputTypeDef = TypedDict(
+    "_RequiredValueOutputTypeDef",
+    {
+        "interpretedValue": str,
+    },
+)
+_OptionalValueOutputTypeDef = TypedDict(
+    "_OptionalValueOutputTypeDef",
+    {
+        "originalValue": str,
+        "resolvedValues": List[str],
+    },
+    total=False,
+)
+
+class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
+    pass
+
 _RequiredValueTypeDef = TypedDict(
     "_RequiredValueTypeDef",
     {
         "interpretedValue": str,
     },
 )
 _OptionalValueTypeDef = TypedDict(
     "_OptionalValueTypeDef",
     {
         "originalValue": str,
-        "resolvedValues": List[str],
+        "resolvedValues": Sequence[str],
     },
     total=False,
 )
 
-
 class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
     pass
 
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "contextAttributes": Dict[str, str],
+    },
+)
 
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "contextAttributes": Dict[str, str],
+        "contextAttributes": Mapping[str, str],
+    },
+)
+
+_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "requestContentType": str,
+    },
+)
+_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "sessionState": str,
+        "requestAttributes": str,
+        "responseContentType": str,
+        "inputStream": BlobTypeDef,
+    },
+    total=False,
+)
+
+class RecognizeUtteranceRequestRequestTypeDef(
+    _RequiredRecognizeUtteranceRequestRequestTypeDef,
+    _OptionalRecognizeUtteranceRequestRequestTypeDef,
+):
+    pass
+
+_RequiredImageResponseCardOutputTypeDef = TypedDict(
+    "_RequiredImageResponseCardOutputTypeDef",
+    {
+        "title": str,
     },
 )
+_OptionalImageResponseCardOutputTypeDef = TypedDict(
+    "_OptionalImageResponseCardOutputTypeDef",
+    {
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+class ImageResponseCardOutputTypeDef(
+    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
+):
+    pass
 
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
     "_OptionalImageResponseCardTypeDef",
     {
         "subtitle": str,
         "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
+        "buttons": Sequence[ButtonTypeDef],
     },
     total=False,
 )
 
-
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSessionResponseTypeDef = TypedDict(
+    "PutSessionResponseTypeDef",
+    {
+        "contentType": str,
+        "messages": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "audioStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
-RuntimeHintDetailsTypeDef = TypedDict(
-    "RuntimeHintDetailsTypeDef",
+RecognizeUtteranceResponseTypeDef = TypedDict(
+    "RecognizeUtteranceResponseTypeDef",
+    {
+        "inputMode": str,
+        "contentType": str,
+        "messages": str,
+        "interpretations": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "inputTranscript": str,
+        "audioStream": StreamingBody,
+        "recognizedBotMember": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RuntimeHintDetailsOutputTypeDef = TypedDict(
+    "RuntimeHintDetailsOutputTypeDef",
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
+RuntimeHintDetailsTypeDef = TypedDict(
+    "RuntimeHintDetailsTypeDef",
+    {
+        "runtimeHintValues": Sequence[RuntimeHintValueTypeDef],
+        "subSlotHints": Mapping[str, Dict[str, Any]],
+    },
+    total=False,
+)
+
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentiment": SentimentTypeType,
         "sentimentScore": SentimentScoreTypeDef,
     },
     total=False,
 )
 
+SlotOutputTypeDef = TypedDict(
+    "SlotOutputTypeDef",
+    {
+        "value": ValueOutputTypeDef,
+        "shape": ShapeType,
+        "values": List[Dict[str, Any]],
+        "subSlots": Dict[str, Dict[str, Any]],
+    },
+    total=False,
+)
+
 SlotTypeDef = TypedDict(
     "SlotTypeDef",
     {
         "value": ValueTypeDef,
         "shape": ShapeType,
-        "values": List[Dict[str, Any]],
-        "subSlots": Dict[str, Dict[str, Any]],
+        "values": Sequence[Dict[str, Any]],
+        "subSlots": Mapping[str, Dict[str, Any]],
+    },
+    total=False,
+)
+
+SessionStateOutputTypeDef = TypedDict(
+    "SessionStateOutputTypeDef",
+    {
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "sessionAttributes": Dict[str, str],
+        "originatingRequestId": str,
+        "runtimeHints": RuntimeHintsOutputTypeDef,
     },
     total=False,
 )
 
 SessionStateTypeDef = TypedDict(
     "SessionStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentTypeDef,
-        "activeContexts": List[ActiveContextTypeDef],
-        "sessionAttributes": Dict[str, str],
+        "activeContexts": Sequence[ActiveContextTypeDef],
+        "sessionAttributes": Mapping[str, str],
         "originatingRequestId": str,
         "runtimeHints": RuntimeHintsTypeDef,
     },
     total=False,
 )
 
+_RequiredMessageOutputTypeDef = TypedDict(
+    "_RequiredMessageOutputTypeDef",
+    {
+        "contentType": MessageContentTypeType,
+    },
+)
+_OptionalMessageOutputTypeDef = TypedDict(
+    "_OptionalMessageOutputTypeDef",
+    {
+        "content": str,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
+    total=False,
+)
+
+class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+    pass
+
 _RequiredMessageTypeDef = TypedDict(
     "_RequiredMessageTypeDef",
     {
         "contentType": MessageContentTypeType,
     },
 )
 _OptionalMessageTypeDef = TypedDict(
@@ -403,25 +527,23 @@
     {
         "content": str,
         "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
-
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
-
 InterpretationTypeDef = TypedDict(
     "InterpretationTypeDef",
     {
         "nluConfidence": ConfidenceScoreTypeDef,
         "sentimentResponse": SentimentResponseTypeDef,
-        "intent": IntentTypeDef,
+        "intent": IntentOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
     "_RequiredRecognizeTextRequestRequestTypeDef",
     {
@@ -437,64 +559,62 @@
     {
         "sessionState": SessionStateTypeDef,
         "requestAttributes": Mapping[str, str],
     },
     total=False,
 )
 
-
 class RecognizeTextRequestRequestTypeDef(
     _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
 ):
     pass
 
+SessionStateUnionTypeDef = Union[SessionStateTypeDef, SessionStateOutputTypeDef]
+MessageUnionTypeDef = Union[MessageTypeDef, MessageOutputTypeDef]
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageOutputTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageOutputTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
         "sessionState": SessionStateTypeDef,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": Sequence[MessageUnionTypeDef],
         "requestAttributes": Mapping[str, str],
         "responseContentType": str,
     },
     total=False,
 )
 
-
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
-
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "sessionId": str,
-        "messages": List[MessageTypeDef],
-        "interpretations": List[InterpretationTypeDef],
-        "sessionState": SessionStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
-    {
-        "messages": List[MessageTypeDef],
-        "sessionState": SessionStateTypeDef,
-        "interpretations": List[InterpretationTypeDef],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime/type_defs.pyi` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lexv2_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
@@ -27,55 +27,69 @@
 )
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "ConfidenceScoreTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "DialogActionTypeDef",
     "ElicitSubSlotTypeDef",
     "GetSessionRequestRequestTypeDef",
+    "IntentOutputTypeDef",
     "IntentTypeDef",
-    "PutSessionResponseTypeDef",
     "RecognizedBotMemberTypeDef",
-    "RecognizeUtteranceRequestRequestTypeDef",
-    "RecognizeUtteranceResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RuntimeHintValueTypeDef",
+    "RuntimeHintsOutputTypeDef",
     "RuntimeHintsTypeDef",
     "SentimentScoreTypeDef",
+    "ValueOutputTypeDef",
     "ValueTypeDef",
+    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "RecognizeUtteranceRequestRequestTypeDef",
+    "ImageResponseCardOutputTypeDef",
     "ImageResponseCardTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "RecognizeUtteranceResponseTypeDef",
+    "RuntimeHintDetailsOutputTypeDef",
     "RuntimeHintDetailsTypeDef",
     "SentimentResponseTypeDef",
+    "SlotOutputTypeDef",
     "SlotTypeDef",
+    "SessionStateOutputTypeDef",
     "SessionStateTypeDef",
+    "MessageOutputTypeDef",
     "MessageTypeDef",
     "InterpretationTypeDef",
     "RecognizeTextRequestRequestTypeDef",
-    "PutSessionRequestRequestTypeDef",
+    "SessionStateUnionTypeDef",
+    "MessageUnionTypeDef",
     "GetSessionResponseTypeDef",
     "RecognizeTextResponseTypeDef",
+    "PutSessionRequestRequestTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -94,22 +108,22 @@
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
@@ -121,75 +135,89 @@
         "slotToElicit": str,
         "slotElicitationStyle": StyleTypeType,
         "subSlotToElicit": "ElicitSubSlotTypeDef",
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+
 _RequiredElicitSubSlotTypeDef = TypedDict(
     "_RequiredElicitSubSlotTypeDef",
     {
         "name": str,
     },
 )
 _OptionalElicitSubSlotTypeDef = TypedDict(
     "_OptionalElicitSubSlotTypeDef",
     {
         "subSlotToElicit": Dict[str, Any],
     },
     total=False,
 )
 
+
 class ElicitSubSlotTypeDef(_RequiredElicitSubSlotTypeDef, _OptionalElicitSubSlotTypeDef):
     pass
 
+
 GetSessionRequestRequestTypeDef = TypedDict(
     "GetSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
     },
 )
 
+_RequiredIntentOutputTypeDef = TypedDict(
+    "_RequiredIntentOutputTypeDef",
+    {
+        "name": str,
+    },
+)
+_OptionalIntentOutputTypeDef = TypedDict(
+    "_OptionalIntentOutputTypeDef",
+    {
+        "slots": Dict[str, "SlotOutputTypeDef"],
+        "state": IntentStateType,
+        "confirmationState": ConfirmationStateType,
+    },
+    total=False,
+)
+
+
+class IntentOutputTypeDef(_RequiredIntentOutputTypeDef, _OptionalIntentOutputTypeDef):
+    pass
+
+
 _RequiredIntentTypeDef = TypedDict(
     "_RequiredIntentTypeDef",
     {
         "name": str,
     },
 )
 _OptionalIntentTypeDef = TypedDict(
     "_OptionalIntentTypeDef",
     {
-        "slots": Dict[str, "SlotTypeDef"],
+        "slots": Mapping[str, "SlotTypeDef"],
         "state": IntentStateType,
         "confirmationState": ConfirmationStateType,
     },
     total=False,
 )
 
+
 class IntentTypeDef(_RequiredIntentTypeDef, _OptionalIntentTypeDef):
     pass
 
-PutSessionResponseTypeDef = TypedDict(
-    "PutSessionResponseTypeDef",
-    {
-        "contentType": str,
-        "messages": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "audioStream": StreamingBody,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 _RequiredRecognizedBotMemberTypeDef = TypedDict(
     "_RequiredRecognizedBotMemberTypeDef",
     {
         "botId": str,
     },
 )
@@ -197,85 +225,40 @@
     "_OptionalRecognizedBotMemberTypeDef",
     {
         "botName": str,
     },
     total=False,
 )
 
+
 class RecognizedBotMemberTypeDef(
     _RequiredRecognizedBotMemberTypeDef, _OptionalRecognizedBotMemberTypeDef
 ):
     pass
 
-_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "botId": str,
-        "botAliasId": str,
-        "localeId": str,
-        "sessionId": str,
-        "requestContentType": str,
-    },
-)
-_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
-    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
-    {
-        "sessionState": str,
-        "requestAttributes": str,
-        "responseContentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
-    },
-    total=False,
-)
-
-class RecognizeUtteranceRequestRequestTypeDef(
-    _RequiredRecognizeUtteranceRequestRequestTypeDef,
-    _OptionalRecognizeUtteranceRequestRequestTypeDef,
-):
-    pass
-
-RecognizeUtteranceResponseTypeDef = TypedDict(
-    "RecognizeUtteranceResponseTypeDef",
-    {
-        "inputMode": str,
-        "contentType": str,
-        "messages": str,
-        "interpretations": str,
-        "sessionState": str,
-        "requestAttributes": str,
-        "sessionId": str,
-        "inputTranscript": str,
-        "audioStream": StreamingBody,
-        "recognizedBotMember": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+RuntimeHintValueTypeDef = TypedDict(
+    "RuntimeHintValueTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "phrase": str,
     },
 )
 
-RuntimeHintValueTypeDef = TypedDict(
-    "RuntimeHintValueTypeDef",
+RuntimeHintsOutputTypeDef = TypedDict(
+    "RuntimeHintsOutputTypeDef",
     {
-        "phrase": str,
+        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsOutputTypeDef"]],
     },
+    total=False,
 )
 
 RuntimeHintsTypeDef = TypedDict(
     "RuntimeHintsTypeDef",
     {
-        "slotHints": Dict[str, Dict[str, "RuntimeHintDetailsTypeDef"]],
+        "slotHints": Mapping[str, Mapping[str, "RuntimeHintDetailsTypeDef"]],
     },
     total=False,
 )
 
 SentimentScoreTypeDef = TypedDict(
     "SentimentScoreTypeDef",
     {
@@ -283,104 +266,283 @@
         "negative": float,
         "neutral": float,
         "mixed": float,
     },
     total=False,
 )
 
+_RequiredValueOutputTypeDef = TypedDict(
+    "_RequiredValueOutputTypeDef",
+    {
+        "interpretedValue": str,
+    },
+)
+_OptionalValueOutputTypeDef = TypedDict(
+    "_OptionalValueOutputTypeDef",
+    {
+        "originalValue": str,
+        "resolvedValues": List[str],
+    },
+    total=False,
+)
+
+
+class ValueOutputTypeDef(_RequiredValueOutputTypeDef, _OptionalValueOutputTypeDef):
+    pass
+
+
 _RequiredValueTypeDef = TypedDict(
     "_RequiredValueTypeDef",
     {
         "interpretedValue": str,
     },
 )
 _OptionalValueTypeDef = TypedDict(
     "_OptionalValueTypeDef",
     {
         "originalValue": str,
-        "resolvedValues": List[str],
+        "resolvedValues": Sequence[str],
     },
     total=False,
 )
 
+
 class ValueTypeDef(_RequiredValueTypeDef, _OptionalValueTypeDef):
     pass
 
+
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "contextAttributes": Dict[str, str],
+    },
+)
+
 ActiveContextTypeDef = TypedDict(
     "ActiveContextTypeDef",
     {
         "name": str,
         "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "contextAttributes": Dict[str, str],
+        "contextAttributes": Mapping[str, str],
     },
 )
 
+_RequiredRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_RequiredRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "requestContentType": str,
+    },
+)
+_OptionalRecognizeUtteranceRequestRequestTypeDef = TypedDict(
+    "_OptionalRecognizeUtteranceRequestRequestTypeDef",
+    {
+        "sessionState": str,
+        "requestAttributes": str,
+        "responseContentType": str,
+        "inputStream": BlobTypeDef,
+    },
+    total=False,
+)
+
+
+class RecognizeUtteranceRequestRequestTypeDef(
+    _RequiredRecognizeUtteranceRequestRequestTypeDef,
+    _OptionalRecognizeUtteranceRequestRequestTypeDef,
+):
+    pass
+
+
+_RequiredImageResponseCardOutputTypeDef = TypedDict(
+    "_RequiredImageResponseCardOutputTypeDef",
+    {
+        "title": str,
+    },
+)
+_OptionalImageResponseCardOutputTypeDef = TypedDict(
+    "_OptionalImageResponseCardOutputTypeDef",
+    {
+        "subtitle": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+
+class ImageResponseCardOutputTypeDef(
+    _RequiredImageResponseCardOutputTypeDef, _OptionalImageResponseCardOutputTypeDef
+):
+    pass
+
+
 _RequiredImageResponseCardTypeDef = TypedDict(
     "_RequiredImageResponseCardTypeDef",
     {
         "title": str,
     },
 )
 _OptionalImageResponseCardTypeDef = TypedDict(
     "_OptionalImageResponseCardTypeDef",
     {
         "subtitle": str,
         "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
+        "buttons": Sequence[ButtonTypeDef],
     },
     total=False,
 )
 
+
 class ImageResponseCardTypeDef(
     _RequiredImageResponseCardTypeDef, _OptionalImageResponseCardTypeDef
 ):
     pass
 
-RuntimeHintDetailsTypeDef = TypedDict(
-    "RuntimeHintDetailsTypeDef",
+
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "botId": str,
+        "botAliasId": str,
+        "localeId": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutSessionResponseTypeDef = TypedDict(
+    "PutSessionResponseTypeDef",
+    {
+        "contentType": str,
+        "messages": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "audioStream": StreamingBody,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeUtteranceResponseTypeDef = TypedDict(
+    "RecognizeUtteranceResponseTypeDef",
+    {
+        "inputMode": str,
+        "contentType": str,
+        "messages": str,
+        "interpretations": str,
+        "sessionState": str,
+        "requestAttributes": str,
+        "sessionId": str,
+        "inputTranscript": str,
+        "audioStream": StreamingBody,
+        "recognizedBotMember": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RuntimeHintDetailsOutputTypeDef = TypedDict(
+    "RuntimeHintDetailsOutputTypeDef",
     {
         "runtimeHintValues": List[RuntimeHintValueTypeDef],
         "subSlotHints": Dict[str, Dict[str, Any]],
     },
     total=False,
 )
 
+RuntimeHintDetailsTypeDef = TypedDict(
+    "RuntimeHintDetailsTypeDef",
+    {
+        "runtimeHintValues": Sequence[RuntimeHintValueTypeDef],
+        "subSlotHints": Mapping[str, Dict[str, Any]],
+    },
+    total=False,
+)
+
 SentimentResponseTypeDef = TypedDict(
     "SentimentResponseTypeDef",
     {
         "sentiment": SentimentTypeType,
         "sentimentScore": SentimentScoreTypeDef,
     },
     total=False,
 )
 
+SlotOutputTypeDef = TypedDict(
+    "SlotOutputTypeDef",
+    {
+        "value": ValueOutputTypeDef,
+        "shape": ShapeType,
+        "values": List[Dict[str, Any]],
+        "subSlots": Dict[str, Dict[str, Any]],
+    },
+    total=False,
+)
+
 SlotTypeDef = TypedDict(
     "SlotTypeDef",
     {
         "value": ValueTypeDef,
         "shape": ShapeType,
-        "values": List[Dict[str, Any]],
-        "subSlots": Dict[str, Dict[str, Any]],
+        "values": Sequence[Dict[str, Any]],
+        "subSlots": Mapping[str, Dict[str, Any]],
+    },
+    total=False,
+)
+
+SessionStateOutputTypeDef = TypedDict(
+    "SessionStateOutputTypeDef",
+    {
+        "dialogAction": DialogActionTypeDef,
+        "intent": IntentOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "sessionAttributes": Dict[str, str],
+        "originatingRequestId": str,
+        "runtimeHints": RuntimeHintsOutputTypeDef,
     },
     total=False,
 )
 
 SessionStateTypeDef = TypedDict(
     "SessionStateTypeDef",
     {
         "dialogAction": DialogActionTypeDef,
         "intent": IntentTypeDef,
-        "activeContexts": List[ActiveContextTypeDef],
-        "sessionAttributes": Dict[str, str],
+        "activeContexts": Sequence[ActiveContextTypeDef],
+        "sessionAttributes": Mapping[str, str],
         "originatingRequestId": str,
         "runtimeHints": RuntimeHintsTypeDef,
     },
     total=False,
 )
 
+_RequiredMessageOutputTypeDef = TypedDict(
+    "_RequiredMessageOutputTypeDef",
+    {
+        "contentType": MessageContentTypeType,
+    },
+)
+_OptionalMessageOutputTypeDef = TypedDict(
+    "_OptionalMessageOutputTypeDef",
+    {
+        "content": str,
+        "imageResponseCard": ImageResponseCardOutputTypeDef,
+    },
+    total=False,
+)
+
+
+class MessageOutputTypeDef(_RequiredMessageOutputTypeDef, _OptionalMessageOutputTypeDef):
+    pass
+
+
 _RequiredMessageTypeDef = TypedDict(
     "_RequiredMessageTypeDef",
     {
         "contentType": MessageContentTypeType,
     },
 )
 _OptionalMessageTypeDef = TypedDict(
@@ -388,23 +550,25 @@
     {
         "content": str,
         "imageResponseCard": ImageResponseCardTypeDef,
     },
     total=False,
 )
 
+
 class MessageTypeDef(_RequiredMessageTypeDef, _OptionalMessageTypeDef):
     pass
 
+
 InterpretationTypeDef = TypedDict(
     "InterpretationTypeDef",
     {
         "nluConfidence": ConfidenceScoreTypeDef,
         "sentimentResponse": SentimentResponseTypeDef,
-        "intent": IntentTypeDef,
+        "intent": IntentOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredRecognizeTextRequestRequestTypeDef = TypedDict(
     "_RequiredRecognizeTextRequestRequestTypeDef",
     {
@@ -420,60 +584,65 @@
     {
         "sessionState": SessionStateTypeDef,
         "requestAttributes": Mapping[str, str],
     },
     total=False,
 )
 
+
 class RecognizeTextRequestRequestTypeDef(
     _RequiredRecognizeTextRequestRequestTypeDef, _OptionalRecognizeTextRequestRequestTypeDef
 ):
     pass
 
+
+SessionStateUnionTypeDef = Union[SessionStateTypeDef, SessionStateOutputTypeDef]
+MessageUnionTypeDef = Union[MessageTypeDef, MessageOutputTypeDef]
+GetSessionResponseTypeDef = TypedDict(
+    "GetSessionResponseTypeDef",
+    {
+        "sessionId": str,
+        "messages": List[MessageOutputTypeDef],
+        "interpretations": List[InterpretationTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+RecognizeTextResponseTypeDef = TypedDict(
+    "RecognizeTextResponseTypeDef",
+    {
+        "messages": List[MessageOutputTypeDef],
+        "sessionState": SessionStateOutputTypeDef,
+        "interpretations": List[InterpretationTypeDef],
+        "requestAttributes": Dict[str, str],
+        "sessionId": str,
+        "recognizedBotMember": RecognizedBotMemberTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botId": str,
         "botAliasId": str,
         "localeId": str,
         "sessionId": str,
         "sessionState": SessionStateTypeDef,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
-        "messages": Sequence[MessageTypeDef],
+        "messages": Sequence[MessageUnionTypeDef],
         "requestAttributes": Mapping[str, str],
         "responseContentType": str,
     },
     total=False,
 )
 
+
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
-
-GetSessionResponseTypeDef = TypedDict(
-    "GetSessionResponseTypeDef",
-    {
-        "sessionId": str,
-        "messages": List[MessageTypeDef],
-        "interpretations": List[InterpretationTypeDef],
-        "sessionState": SessionStateTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-RecognizeTextResponseTypeDef = TypedDict(
-    "RecognizeTextResponseTypeDef",
-    {
-        "messages": List[MessageTypeDef],
-        "sessionState": SessionStateTypeDef,
-        "interpretations": List[InterpretationTypeDef],
-        "requestAttributes": Dict[str, str],
-        "sessionId": str,
-        "recognizedBotMember": RecognizedBotMemberTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lexv2-runtime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexRuntimeV2 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lexv2-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lexv2-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lexv2-runtime"></a>
 
 # types-aiobotocore-lexv2-runtime
 
 [![PyPI - types-aiobotocore-lexv2-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lexv2-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lexv2-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lexv2-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lexv2-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lexv2-runtime)](https://pepy.tech/project/types-aiobotocore-lexv2-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexRuntimeV2 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lexv2-runtime.html#LexRuntimeV2)
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
 [types-aiobotocore-lexv2-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lexv2_runtime/).
 
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
@@ -287,57 +286,69 @@
 )
 
 
 def check_value(value: ConfirmationStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lexv2_runtime.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lexv2_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     ConfidenceScoreTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
     DialogActionTypeDef,
     ElicitSubSlotTypeDef,
     GetSessionRequestRequestTypeDef,
+    IntentOutputTypeDef,
     IntentTypeDef,
-    PutSessionResponseTypeDef,
     RecognizedBotMemberTypeDef,
-    RecognizeUtteranceRequestRequestTypeDef,
-    RecognizeUtteranceResponseTypeDef,
-    ResponseMetadataTypeDef,
     RuntimeHintValueTypeDef,
+    RuntimeHintsOutputTypeDef,
     RuntimeHintsTypeDef,
     SentimentScoreTypeDef,
+    ValueOutputTypeDef,
     ValueTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    RecognizeUtteranceRequestRequestTypeDef,
+    ImageResponseCardOutputTypeDef,
     ImageResponseCardTypeDef,
+    DeleteSessionResponseTypeDef,
+    PutSessionResponseTypeDef,
+    RecognizeUtteranceResponseTypeDef,
+    RuntimeHintDetailsOutputTypeDef,
     RuntimeHintDetailsTypeDef,
     SentimentResponseTypeDef,
+    SlotOutputTypeDef,
     SlotTypeDef,
+    SessionStateOutputTypeDef,
     SessionStateTypeDef,
+    MessageOutputTypeDef,
     MessageTypeDef,
     InterpretationTypeDef,
     RecognizeTextRequestRequestTypeDef,
-    PutSessionRequestRequestTypeDef,
+    SessionStateUnionTypeDef,
+    MessageUnionTypeDef,
     GetSessionResponseTypeDef,
     RecognizeTextResponseTypeDef,
+    PutSessionRequestRequestTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lexv2-runtime-2.5.2/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lexv2-runtime-2.5.2.post1/types_aiobotocore_lexv2_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


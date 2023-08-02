# Comparing `tmp/types-aiobotocore-lex-runtime-2.5.2.tar.gz` & `tmp/types-aiobotocore-lex-runtime-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.2.tar", last modified: Sat Jul  8 01:43:53 2023, max compression
+gzip compressed data, was "types-aiobotocore-lex-runtime-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:33 2023, max compression
```

## Comparing `types-aiobotocore-lex-runtime-2.5.2.tar` & `types-aiobotocore-lex-runtime-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11484 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9683 2023-07-08 01:33:46.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:33:45.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:53.354428 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13071 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-08 01:43:53.000000 types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11671 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8287 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8439 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11661 2023-08-02 14:41:53.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11644 2023-08-02 14:41:53.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:41:52.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:33.581543 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 14:52:33.000000 types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/LICENSE` & `types-aiobotocore-lex-runtime-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lex-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lex-runtime"></a>
 
 # types-aiobotocore-lex-runtime
 
 [![PyPI - types-aiobotocore-lex-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
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
@@ -286,48 +285,55 @@
 )
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lex_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
-    PostContentRequestRequestTypeDef,
-    PostContentResponseTypeDef,
+    IntentSummaryTypeDef,
     SentimentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    ResponseMetadataTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    PostContentRequestRequestTypeDef,
     GenericAttachmentTypeDef,
+    DeleteSessionResponseTypeDef,
+    PostContentResponseTypeDef,
+    PutSessionResponseTypeDef,
+    DialogActionUnionTypeDef,
     PredictedIntentTypeDef,
+    IntentSummaryUnionTypeDef,
     GetSessionResponseTypeDef,
+    ActiveContextUnionTypeDef,
+    ResponseCardTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
-    ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/README.md` & `types-aiobotocore-lex-runtime-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-lex-runtime"></a>
 
 # types-aiobotocore-lex-runtime
 
 [![PyPI - types-aiobotocore-lex-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
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
@@ -253,48 +253,55 @@
 )
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lex_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
-    PostContentRequestRequestTypeDef,
-    PostContentResponseTypeDef,
+    IntentSummaryTypeDef,
     SentimentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    ResponseMetadataTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    PostContentRequestRequestTypeDef,
     GenericAttachmentTypeDef,
+    DeleteSessionResponseTypeDef,
+    PostContentResponseTypeDef,
+    PutSessionResponseTypeDef,
+    DialogActionUnionTypeDef,
     PredictedIntentTypeDef,
+    IntentSummaryUnionTypeDef,
     GetSessionResponseTypeDef,
+    ActiveContextUnionTypeDef,
+    ResponseCardTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
-    ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/setup.py` & `types-aiobotocore-lex-runtime-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-lex-runtime",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_lex_runtime"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with"
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
-    keywords="aiobotocore lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore lex-runtime type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_lex_runtime": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/"
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/__main__.py` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.LexRuntimeService 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.LexRuntimeService 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService\nOther"
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

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.py` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient
 
     session = get_session()
     async with session.create_client("lex-runtime") as client:
         client: LexRuntimeServiceClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
-    ActiveContextTypeDef,
+    ActiveContextUnionTypeDef,
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
-    DialogActionTypeDef,
+    DialogActionUnionTypeDef,
     GetSessionResponseTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryUnionTypeDef,
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
@@ -127,15 +127,15 @@
     async def post_content(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         contentType: str,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody],
+        inputStream: BlobTypeDef,
         sessionAttributes: str = ...,
         requestAttributes: str = ...,
         accept: str = ...,
         activeContexts: str = ...
     ) -> PostContentResponseTypeDef:
         """
         Sends user input (text or speech) to Amazon Lex.
@@ -149,15 +149,15 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_text)
         """
@@ -165,18 +165,18 @@
     async def put_session(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
-        dialogAction: DialogActionTypeDef = ...,
-        recentIntentSummaryView: Sequence[IntentSummaryTypeDef] = ...,
+        dialogAction: DialogActionUnionTypeDef = ...,
+        recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#put_session)
         """
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/client.pyi` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -10,26 +10,26 @@
     from types_aiobotocore_lex_runtime.client import LexRuntimeServiceClient
 
     session = get_session()
     async with session.create_client("lex-runtime") as client:
         client: LexRuntimeServiceClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Sequence, Type, Union
+from typing import Any, Dict, Mapping, Sequence, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
 from .type_defs import (
-    ActiveContextTypeDef,
+    ActiveContextUnionTypeDef,
+    BlobTypeDef,
     DeleteSessionResponseTypeDef,
-    DialogActionTypeDef,
+    DialogActionUnionTypeDef,
     GetSessionResponseTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryUnionTypeDef,
     PostContentResponseTypeDef,
     PostTextResponseTypeDef,
     PutSessionResponseTypeDef,
 )
 
 __all__ = ("LexRuntimeServiceClient",)
 
@@ -118,15 +118,15 @@
     async def post_content(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         contentType: str,
-        inputStream: Union[str, bytes, IO[Any], StreamingBody],
+        inputStream: BlobTypeDef,
         sessionAttributes: str = ...,
         requestAttributes: str = ...,
         accept: str = ...,
         activeContexts: str = ...
     ) -> PostContentResponseTypeDef:
         """
         Sends user input (text or speech) to Amazon Lex.
@@ -139,33 +139,33 @@
         *,
         botName: str,
         botAlias: str,
         userId: str,
         inputText: str,
         sessionAttributes: Mapping[str, str] = ...,
         requestAttributes: Mapping[str, str] = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PostTextResponseTypeDef:
         """
         Sends user input to Amazon Lex.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.post_text)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#post_text)
         """
     async def put_session(
         self,
         *,
         botName: str,
         botAlias: str,
         userId: str,
         sessionAttributes: Mapping[str, str] = ...,
-        dialogAction: DialogActionTypeDef = ...,
-        recentIntentSummaryView: Sequence[IntentSummaryTypeDef] = ...,
+        dialogAction: DialogActionUnionTypeDef = ...,
+        recentIntentSummaryView: Sequence[IntentSummaryUnionTypeDef] = ...,
         accept: str = ...,
-        activeContexts: Sequence[ActiveContextTypeDef] = ...
+        activeContexts: Sequence[ActiveContextUnionTypeDef] = ...
     ) -> PutSessionResponseTypeDef:
         """
         Creates a new session or modifies an existing session with an Amazon Lex bot.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService.Client.put_session)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/client/#put_session)
         """
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.py` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/literals.pyi` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.py` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
@@ -29,48 +29,55 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentSummaryTypeDef",
+    "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
-    "PostContentRequestRequestTypeDef",
-    "PostContentResponseTypeDef",
+    "IntentSummaryTypeDef",
     "SentimentResponseTypeDef",
-    "PutSessionResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "PostContentRequestRequestTypeDef",
     "GenericAttachmentTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PostContentResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "DialogActionUnionTypeDef",
     "PredictedIntentTypeDef",
+    "IntentSummaryUnionTypeDef",
     "GetSessionResponseTypeDef",
+    "ActiveContextUnionTypeDef",
+    "ResponseCardTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
-    "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -80,49 +87,71 @@
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
+_RequiredDialogActionOutputTypeDef = TypedDict(
+    "_RequiredDialogActionOutputTypeDef",
+    {
+        "type": DialogActionTypeType,
+    },
+)
+_OptionalDialogActionOutputTypeDef = TypedDict(
+    "_OptionalDialogActionOutputTypeDef",
+    {
+        "intentName": str,
+        "slots": Dict[str, str],
+        "slotToElicit": str,
+        "fulfillmentState": FulfillmentStateType,
+        "message": str,
+        "messageFormat": MessageFormatTypeType,
+    },
+    total=False,
+)
+
+class DialogActionOutputTypeDef(
+    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
+):
+    pass
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
     "_OptionalDialogActionTypeDef",
     {
         "intentName": str,
-        "slots": Dict[str, str],
+        "slots": Mapping[str, str],
         "slotToElicit": str,
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
-
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
-
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -131,80 +160,148 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
-
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+_RequiredIntentSummaryOutputTypeDef = TypedDict(
+    "_RequiredIntentSummaryOutputTypeDef",
+    {
+        "dialogActionType": DialogActionTypeType,
+    },
+)
+_OptionalIntentSummaryOutputTypeDef = TypedDict(
+    "_OptionalIntentSummaryOutputTypeDef",
+    {
+        "intentName": str,
+        "checkpointLabel": str,
+        "slots": Dict[str, str],
+        "confirmationStatus": ConfirmationStatusType,
+        "fulfillmentState": FulfillmentStateType,
+        "slotToElicit": str,
+    },
+    total=False,
+)
+
+class IntentSummaryOutputTypeDef(
+    _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
+):
+    pass
+
+IntentConfidenceTypeDef = TypedDict(
+    "IntentConfidenceTypeDef",
+    {
+        "score": float,
+    },
+    total=False,
+)
 
 _RequiredIntentSummaryTypeDef = TypedDict(
     "_RequiredIntentSummaryTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryTypeDef = TypedDict(
     "_OptionalIntentSummaryTypeDef",
     {
         "intentName": str,
         "checkpointLabel": str,
-        "slots": Dict[str, str],
+        "slots": Mapping[str, str],
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
-
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
-
-IntentConfidenceTypeDef = TypedDict(
-    "IntentConfidenceTypeDef",
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
     {
-        "score": float,
+        "sentimentLabel": str,
+        "sentimentScore": str,
     },
     total=False,
 )
 
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Mapping[str, str],
+    },
+)
+
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "contentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
+        "inputStream": BlobTypeDef,
     },
 )
 _OptionalPostContentRequestRequestTypeDef = TypedDict(
     "_OptionalPostContentRequestRequestTypeDef",
     {
         "sessionAttributes": str,
         "requestAttributes": str,
         "accept": str,
         "activeContexts": str,
     },
     total=False,
 )
 
-
 class PostContentRequestRequestTypeDef(
     _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
 ):
     pass
 
+GenericAttachmentTypeDef = TypedDict(
+    "GenericAttachmentTypeDef",
+    {
+        "title": str,
+        "subTitle": str,
+        "attachmentLinkUrl": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 
 PostContentResponseTypeDef = TypedDict(
     "PostContentResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "nluIntentConfidence": str,
@@ -219,27 +316,18 @@
         "slotToElicit": str,
         "inputTranscript": str,
         "encodedInputTranscript": str,
         "audioStream": StreamingBody,
         "botVersion": str,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
-    {
-        "sentimentLabel": str,
-        "sentimentScore": str,
-    },
-    total=False,
-)
-
 PutSessionResponseTypeDef = TypedDict(
     "PutSessionResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "slots": str,
         "sessionAttributes": str,
@@ -247,135 +335,102 @@
         "encodedMessage": str,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
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
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
-GenericAttachmentTypeDef = TypedDict(
-    "GenericAttachmentTypeDef",
-    {
-        "title": str,
-        "subTitle": str,
-        "attachmentLinkUrl": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
+DialogActionUnionTypeDef = Union[DialogActionTypeDef, DialogActionOutputTypeDef]
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
     total=False,
 )
 
+IntentSummaryUnionTypeDef = Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
-        "recentIntentSummaryView": List[IntentSummaryTypeDef],
+        "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
-        "dialogAction": DialogActionTypeDef,
-        "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "dialogAction": DialogActionOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+ActiveContextUnionTypeDef = Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]
+ResponseCardTypeDef = TypedDict(
+    "ResponseCardTypeDef",
+    {
+        "version": str,
+        "contentType": Literal["application/vnd.amazonaws.card.generic"],
+        "genericAttachments": List[GenericAttachmentTypeDef],
+    },
+    total=False,
+)
+
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "inputText": str,
     },
 )
 _OptionalPostTextRequestRequestTypeDef = TypedDict(
     "_OptionalPostTextRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
-        "activeContexts": Sequence[ActiveContextTypeDef],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
-
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "dialogAction": DialogActionTypeDef,
-        "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
+        "recentIntentSummaryView": Sequence[IntentSummaryUnionTypeDef],
         "accept": str,
-        "activeContexts": Sequence[ActiveContextTypeDef],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
-
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
-
-ResponseCardTypeDef = TypedDict(
-    "ResponseCardTypeDef",
-    {
-        "version": str,
-        "contentType": Literal["application/vnd.amazonaws.card.generic"],
-        "genericAttachments": List[GenericAttachmentTypeDef],
-    },
-    total=False,
-)
-
 PostTextResponseTypeDef = TypedDict(
     "PostTextResponseTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "alternativeIntents": List[PredictedIntentTypeDef],
         "slots": Dict[str, str],
@@ -384,11 +439,11 @@
         "sentimentResponse": SentimentResponseTypeDef,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
-        "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime/type_defs.pyi` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime/type_defs.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_lex_runtime.type_defs import ActiveContextTimeToLiveTypeDef
 
-    data: ActiveContextTimeToLiveTypeDef = {...}
+    data: ActiveContextTimeToLiveTypeDef = ...
     ```
 """
 import sys
 from typing import IO, Any, Dict, List, Mapping, Sequence, Union
 
 from aiobotocore.response import StreamingBody
 
@@ -29,47 +29,56 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "ActiveContextTimeToLiveTypeDef",
+    "BlobTypeDef",
     "ButtonTypeDef",
     "DeleteSessionRequestRequestTypeDef",
-    "DeleteSessionResponseTypeDef",
+    "ResponseMetadataTypeDef",
+    "DialogActionOutputTypeDef",
     "DialogActionTypeDef",
     "GetSessionRequestRequestTypeDef",
-    "IntentSummaryTypeDef",
+    "IntentSummaryOutputTypeDef",
     "IntentConfidenceTypeDef",
-    "PostContentRequestRequestTypeDef",
-    "PostContentResponseTypeDef",
+    "IntentSummaryTypeDef",
     "SentimentResponseTypeDef",
-    "PutSessionResponseTypeDef",
-    "ResponseMetadataTypeDef",
+    "ActiveContextOutputTypeDef",
     "ActiveContextTypeDef",
+    "PostContentRequestRequestTypeDef",
     "GenericAttachmentTypeDef",
+    "DeleteSessionResponseTypeDef",
+    "PostContentResponseTypeDef",
+    "PutSessionResponseTypeDef",
+    "DialogActionUnionTypeDef",
     "PredictedIntentTypeDef",
+    "IntentSummaryUnionTypeDef",
     "GetSessionResponseTypeDef",
+    "ActiveContextUnionTypeDef",
+    "ResponseCardTypeDef",
     "PostTextRequestRequestTypeDef",
     "PutSessionRequestRequestTypeDef",
-    "ResponseCardTypeDef",
     "PostTextResponseTypeDef",
 )
 
 ActiveContextTimeToLiveTypeDef = TypedDict(
     "ActiveContextTimeToLiveTypeDef",
     {
         "timeToLiveInSeconds": int,
         "turnsToLive": int,
     },
     total=False,
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 ButtonTypeDef = TypedDict(
     "ButtonTypeDef",
     {
         "text": str,
         "value": str,
     },
 )
@@ -79,47 +88,75 @@
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 
-DeleteSessionResponseTypeDef = TypedDict(
-    "DeleteSessionResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "botName": str,
-        "botAlias": str,
-        "userId": str,
-        "sessionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
+_RequiredDialogActionOutputTypeDef = TypedDict(
+    "_RequiredDialogActionOutputTypeDef",
+    {
+        "type": DialogActionTypeType,
+    },
+)
+_OptionalDialogActionOutputTypeDef = TypedDict(
+    "_OptionalDialogActionOutputTypeDef",
+    {
+        "intentName": str,
+        "slots": Dict[str, str],
+        "slotToElicit": str,
+        "fulfillmentState": FulfillmentStateType,
+        "message": str,
+        "messageFormat": MessageFormatTypeType,
     },
+    total=False,
 )
 
+
+class DialogActionOutputTypeDef(
+    _RequiredDialogActionOutputTypeDef, _OptionalDialogActionOutputTypeDef
+):
+    pass
+
+
 _RequiredDialogActionTypeDef = TypedDict(
     "_RequiredDialogActionTypeDef",
     {
         "type": DialogActionTypeType,
     },
 )
 _OptionalDialogActionTypeDef = TypedDict(
     "_OptionalDialogActionTypeDef",
     {
         "intentName": str,
-        "slots": Dict[str, str],
+        "slots": Mapping[str, str],
         "slotToElicit": str,
         "fulfillmentState": FulfillmentStateType,
         "message": str,
         "messageFormat": MessageFormatTypeType,
     },
     total=False,
 )
 
+
 class DialogActionTypeDef(_RequiredDialogActionTypeDef, _OptionalDialogActionTypeDef):
     pass
 
+
 _RequiredGetSessionRequestRequestTypeDef = TypedDict(
     "_RequiredGetSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
@@ -128,75 +165,157 @@
     "_OptionalGetSessionRequestRequestTypeDef",
     {
         "checkpointLabelFilter": str,
     },
     total=False,
 )
 
+
 class GetSessionRequestRequestTypeDef(
     _RequiredGetSessionRequestRequestTypeDef, _OptionalGetSessionRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredIntentSummaryOutputTypeDef = TypedDict(
+    "_RequiredIntentSummaryOutputTypeDef",
+    {
+        "dialogActionType": DialogActionTypeType,
+    },
+)
+_OptionalIntentSummaryOutputTypeDef = TypedDict(
+    "_OptionalIntentSummaryOutputTypeDef",
+    {
+        "intentName": str,
+        "checkpointLabel": str,
+        "slots": Dict[str, str],
+        "confirmationStatus": ConfirmationStatusType,
+        "fulfillmentState": FulfillmentStateType,
+        "slotToElicit": str,
+    },
+    total=False,
+)
+
+
+class IntentSummaryOutputTypeDef(
+    _RequiredIntentSummaryOutputTypeDef, _OptionalIntentSummaryOutputTypeDef
+):
+    pass
+
+
+IntentConfidenceTypeDef = TypedDict(
+    "IntentConfidenceTypeDef",
+    {
+        "score": float,
+    },
+    total=False,
+)
+
 _RequiredIntentSummaryTypeDef = TypedDict(
     "_RequiredIntentSummaryTypeDef",
     {
         "dialogActionType": DialogActionTypeType,
     },
 )
 _OptionalIntentSummaryTypeDef = TypedDict(
     "_OptionalIntentSummaryTypeDef",
     {
         "intentName": str,
         "checkpointLabel": str,
-        "slots": Dict[str, str],
+        "slots": Mapping[str, str],
         "confirmationStatus": ConfirmationStatusType,
         "fulfillmentState": FulfillmentStateType,
         "slotToElicit": str,
     },
     total=False,
 )
 
+
 class IntentSummaryTypeDef(_RequiredIntentSummaryTypeDef, _OptionalIntentSummaryTypeDef):
     pass
 
-IntentConfidenceTypeDef = TypedDict(
-    "IntentConfidenceTypeDef",
+
+SentimentResponseTypeDef = TypedDict(
+    "SentimentResponseTypeDef",
     {
-        "score": float,
+        "sentimentLabel": str,
+        "sentimentScore": str,
     },
     total=False,
 )
 
+ActiveContextOutputTypeDef = TypedDict(
+    "ActiveContextOutputTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Dict[str, str],
+    },
+)
+
+ActiveContextTypeDef = TypedDict(
+    "ActiveContextTypeDef",
+    {
+        "name": str,
+        "timeToLive": ActiveContextTimeToLiveTypeDef,
+        "parameters": Mapping[str, str],
+    },
+)
+
 _RequiredPostContentRequestRequestTypeDef = TypedDict(
     "_RequiredPostContentRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
         "contentType": str,
-        "inputStream": Union[str, bytes, IO[Any], StreamingBody],
+        "inputStream": BlobTypeDef,
     },
 )
 _OptionalPostContentRequestRequestTypeDef = TypedDict(
     "_OptionalPostContentRequestRequestTypeDef",
     {
         "sessionAttributes": str,
         "requestAttributes": str,
         "accept": str,
         "activeContexts": str,
     },
     total=False,
 )
 
+
 class PostContentRequestRequestTypeDef(
     _RequiredPostContentRequestRequestTypeDef, _OptionalPostContentRequestRequestTypeDef
 ):
     pass
 
+
+GenericAttachmentTypeDef = TypedDict(
+    "GenericAttachmentTypeDef",
+    {
+        "title": str,
+        "subTitle": str,
+        "attachmentLinkUrl": str,
+        "imageUrl": str,
+        "buttons": List[ButtonTypeDef],
+    },
+    total=False,
+)
+
+DeleteSessionResponseTypeDef = TypedDict(
+    "DeleteSessionResponseTypeDef",
+    {
+        "botName": str,
+        "botAlias": str,
+        "userId": str,
+        "sessionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 PostContentResponseTypeDef = TypedDict(
     "PostContentResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
         "nluIntentConfidence": str,
         "alternativeIntents": str,
@@ -210,25 +329,16 @@
         "slotToElicit": str,
         "inputTranscript": str,
         "encodedInputTranscript": str,
         "audioStream": StreamingBody,
         "botVersion": str,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-SentimentResponseTypeDef = TypedDict(
-    "SentimentResponseTypeDef",
-    {
-        "sentimentLabel": str,
-        "sentimentScore": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
 PutSessionResponseTypeDef = TypedDict(
     "PutSessionResponseTypeDef",
     {
         "contentType": str,
         "intentName": str,
@@ -238,70 +348,51 @@
         "encodedMessage": str,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "audioStream": StreamingBody,
         "sessionId": str,
         "activeContexts": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
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
-ActiveContextTypeDef = TypedDict(
-    "ActiveContextTypeDef",
-    {
-        "name": str,
-        "timeToLive": ActiveContextTimeToLiveTypeDef,
-        "parameters": Dict[str, str],
-    },
-)
-
-GenericAttachmentTypeDef = TypedDict(
-    "GenericAttachmentTypeDef",
-    {
-        "title": str,
-        "subTitle": str,
-        "attachmentLinkUrl": str,
-        "imageUrl": str,
-        "buttons": List[ButtonTypeDef],
-    },
-    total=False,
-)
-
+DialogActionUnionTypeDef = Union[DialogActionTypeDef, DialogActionOutputTypeDef]
 PredictedIntentTypeDef = TypedDict(
     "PredictedIntentTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "slots": Dict[str, str],
     },
     total=False,
 )
 
+IntentSummaryUnionTypeDef = Union[IntentSummaryTypeDef, IntentSummaryOutputTypeDef]
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
-        "recentIntentSummaryView": List[IntentSummaryTypeDef],
+        "recentIntentSummaryView": List[IntentSummaryOutputTypeDef],
         "sessionAttributes": Dict[str, str],
         "sessionId": str,
-        "dialogAction": DialogActionTypeDef,
-        "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "dialogAction": DialogActionOutputTypeDef,
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ActiveContextUnionTypeDef = Union[ActiveContextTypeDef, ActiveContextOutputTypeDef]
+ResponseCardTypeDef = TypedDict(
+    "ResponseCardTypeDef",
+    {
+        "version": str,
+        "contentType": Literal["application/vnd.amazonaws.card.generic"],
+        "genericAttachments": List[GenericAttachmentTypeDef],
     },
+    total=False,
 )
 
 _RequiredPostTextRequestRequestTypeDef = TypedDict(
     "_RequiredPostTextRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
@@ -310,58 +401,52 @@
     },
 )
 _OptionalPostTextRequestRequestTypeDef = TypedDict(
     "_OptionalPostTextRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "requestAttributes": Mapping[str, str],
-        "activeContexts": Sequence[ActiveContextTypeDef],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
+
 class PostTextRequestRequestTypeDef(
     _RequiredPostTextRequestRequestTypeDef, _OptionalPostTextRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredPutSessionRequestRequestTypeDef = TypedDict(
     "_RequiredPutSessionRequestRequestTypeDef",
     {
         "botName": str,
         "botAlias": str,
         "userId": str,
     },
 )
 _OptionalPutSessionRequestRequestTypeDef = TypedDict(
     "_OptionalPutSessionRequestRequestTypeDef",
     {
         "sessionAttributes": Mapping[str, str],
         "dialogAction": DialogActionTypeDef,
-        "recentIntentSummaryView": Sequence[IntentSummaryTypeDef],
+        "recentIntentSummaryView": Sequence[IntentSummaryUnionTypeDef],
         "accept": str,
-        "activeContexts": Sequence[ActiveContextTypeDef],
+        "activeContexts": Sequence[ActiveContextUnionTypeDef],
     },
     total=False,
 )
 
+
 class PutSessionRequestRequestTypeDef(
     _RequiredPutSessionRequestRequestTypeDef, _OptionalPutSessionRequestRequestTypeDef
 ):
     pass
 
-ResponseCardTypeDef = TypedDict(
-    "ResponseCardTypeDef",
-    {
-        "version": str,
-        "contentType": Literal["application/vnd.amazonaws.card.generic"],
-        "genericAttachments": List[GenericAttachmentTypeDef],
-    },
-    total=False,
-)
 
 PostTextResponseTypeDef = TypedDict(
     "PostTextResponseTypeDef",
     {
         "intentName": str,
         "nluIntentConfidence": IntentConfidenceTypeDef,
         "alternativeIntents": List[PredictedIntentTypeDef],
@@ -371,11 +456,11 @@
         "sentimentResponse": SentimentResponseTypeDef,
         "messageFormat": MessageFormatTypeType,
         "dialogState": DialogStateType,
         "slotToElicit": str,
         "responseCard": ResponseCardTypeDef,
         "sessionId": str,
         "botVersion": str,
-        "activeContexts": List[ActiveContextTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "activeContexts": List[ActiveContextOutputTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/PKG-INFO` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-lex-runtime
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.LexRuntimeService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore lex-runtime type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore lex-runtime type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-lex-runtime"></a>
 
 # types-aiobotocore-lex-runtime
 
 [![PyPI - types-aiobotocore-lex-runtime](https://img.shields.io/pypi/v/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-lex-runtime.svg?color=blue)](https://pypi.org/project/types-aiobotocore-lex-runtime)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-lex-runtime?color=blue)](https://pypistats.org/packages/types-aiobotocore-lex-runtime)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-lex-runtime)](https://pepy.tech/project/types-aiobotocore-lex-runtime)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.LexRuntimeService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-runtime.html#LexRuntimeService)
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
 [types-aiobotocore-lex-runtime docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_lex_runtime/).
 
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
@@ -286,48 +285,55 @@
 )
 
 
 def check_value(value: ConfirmationStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_lex_runtime.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_lex_runtime.type_defs import (
     ActiveContextTimeToLiveTypeDef,
+    BlobTypeDef,
     ButtonTypeDef,
     DeleteSessionRequestRequestTypeDef,
-    DeleteSessionResponseTypeDef,
+    ResponseMetadataTypeDef,
+    DialogActionOutputTypeDef,
     DialogActionTypeDef,
     GetSessionRequestRequestTypeDef,
-    IntentSummaryTypeDef,
+    IntentSummaryOutputTypeDef,
     IntentConfidenceTypeDef,
-    PostContentRequestRequestTypeDef,
-    PostContentResponseTypeDef,
+    IntentSummaryTypeDef,
     SentimentResponseTypeDef,
-    PutSessionResponseTypeDef,
-    ResponseMetadataTypeDef,
+    ActiveContextOutputTypeDef,
     ActiveContextTypeDef,
+    PostContentRequestRequestTypeDef,
     GenericAttachmentTypeDef,
+    DeleteSessionResponseTypeDef,
+    PostContentResponseTypeDef,
+    PutSessionResponseTypeDef,
+    DialogActionUnionTypeDef,
     PredictedIntentTypeDef,
+    IntentSummaryUnionTypeDef,
     GetSessionResponseTypeDef,
+    ActiveContextUnionTypeDef,
+    ResponseCardTypeDef,
     PostTextRequestRequestTypeDef,
     PutSessionRequestRequestTypeDef,
-    ResponseCardTypeDef,
     PostTextResponseTypeDef,
 )
 
 
-def get_structure() -> ActiveContextTimeToLiveTypeDef:
+def get_value() -> ActiveContextTimeToLiveTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-lex-runtime-2.5.2/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt` & `types-aiobotocore-lex-runtime-2.5.2.post1/types_aiobotocore_lex_runtime.egg-info/SOURCES.txt`

 * *Files identical despite different names*


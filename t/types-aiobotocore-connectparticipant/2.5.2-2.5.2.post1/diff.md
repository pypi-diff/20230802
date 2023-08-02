# Comparing `tmp/types-aiobotocore-connectparticipant-2.5.2.tar.gz` & `tmp/types-aiobotocore-connectparticipant-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-connectparticipant-2.5.2.tar", last modified: Sat Jul  8 01:43:28 2023, max compression
+gzip compressed data, was "types-aiobotocore-connectparticipant-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:07 2023, max compression
```

## Comparing `types-aiobotocore-connectparticipant-2.5.2.tar` & `types-aiobotocore-connectparticipant-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.353955 types-aiobotocore-connectparticipant-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-08 01:43:28.353955 types-aiobotocore-connectparticipant-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:28.353955 types-aiobotocore-connectparticipant-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.353955 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8337 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:28:18.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:28.353955 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-07-08 01:43:28.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-08 01:43:28.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:28.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:28.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 01:43:28.000000 types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.333613 types-aiobotocore-connectparticipant-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-08-02 14:52:07.333613 types-aiobotocore-connectparticipant-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:07.333613 types-aiobotocore-connectparticipant-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.333613 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9841 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9825 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8334 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8323 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:35:55.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:07.333613 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13440 2023-08-02 14:52:07.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:52:07.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:07.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:07.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:07.000000 types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/LICENSE` & `types-aiobotocore-connectparticipant-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/PKG-INFO` & `types-aiobotocore-connectparticipant-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectparticipant
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectparticipant type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore connectparticipant type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectparticipant"></a>
 
 # types-aiobotocore-connectparticipant
 
 [![PyPI - types-aiobotocore-connectparticipant](https://img.shields.io/pypi/v/types-aiobotocore-connectparticipant.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectparticipant)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectparticipant.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectparticipant)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectparticipant?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectparticipant)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectparticipant)](https://pepy.tech/project/types-aiobotocore-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectParticipant 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [types-aiobotocore-connectparticipant docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/).
 
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
@@ -286,50 +285,50 @@
 )
 
 
 def check_value(value: ArtifactStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectparticipant.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
-    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
-    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    GetAttachmentResponseTypeDef,
+    SendEventResponseTypeDef,
+    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentItemTypeDef:
+def get_value() -> AttachmentItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/README.md` & `types-aiobotocore-connectparticipant-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-connectparticipant"></a>
 
 # types-aiobotocore-connectparticipant
 
 [![PyPI - types-aiobotocore-connectparticipant](https://img.shields.io/pypi/v/types-aiobotocore-connectparticipant.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectparticipant)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectparticipant.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectparticipant)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectparticipant?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectparticipant)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectparticipant)](https://pepy.tech/project/types-aiobotocore-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectParticipant 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [types-aiobotocore-connectparticipant docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/).
 
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
@@ -253,50 +253,50 @@
 )
 
 
 def check_value(value: ArtifactStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectparticipant.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
-    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
-    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    GetAttachmentResponseTypeDef,
+    SendEventResponseTypeDef,
+    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentItemTypeDef:
+def get_value() -> AttachmentItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/setup.py` & `types-aiobotocore-connectparticipant-2.5.2.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-connectparticipant",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_connectparticipant"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with"
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
-        "aiobotocore connectparticipant type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore connectparticipant type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_connectparticipant": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/"
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/__init__.py` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/__init__.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/__main__.py` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.ConnectParticipant 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.ConnectParticipant 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant\nOther"
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

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/client.py` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/client.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/literals.py` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/literals.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/type_defs.py` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/type_defs.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_connectparticipant.type_defs import AttachmentItemTypeDef
 
-    data: AttachmentItemTypeDef = {...}
+    data: AttachmentItemTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     ArtifactStatusType,
@@ -30,27 +30,27 @@
 
 
 __all__ = (
     "AttachmentItemTypeDef",
     "CompleteAttachmentUploadRequestRequestTypeDef",
     "ConnectionCredentialsTypeDef",
     "CreateParticipantConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "WebsocketTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "GetAttachmentRequestRequestTypeDef",
-    "GetAttachmentResponseTypeDef",
     "StartPositionTypeDef",
     "ReceiptTypeDef",
-    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
-    "SendEventResponseTypeDef",
     "SendMessageRequestRequestTypeDef",
-    "SendMessageResponseTypeDef",
     "StartAttachmentUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
+    "GetAttachmentResponseTypeDef",
+    "SendEventResponseTypeDef",
+    "SendMessageResponseTypeDef",
     "CreateParticipantConnectionResponseTypeDef",
     "GetTranscriptRequestRequestTypeDef",
     "MessageMetadataTypeDef",
     "StartAttachmentUploadResponseTypeDef",
     "ItemTypeDef",
     "GetTranscriptResponseTypeDef",
 )
@@ -103,14 +103,25 @@
 class CreateParticipantConnectionRequestRequestTypeDef(
     _RequiredCreateParticipantConnectionRequestRequestTypeDef,
     _OptionalCreateParticipantConnectionRequestRequestTypeDef,
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
 WebsocketTypeDef = TypedDict(
     "WebsocketTypeDef",
     {
         "Url": str,
         "ConnectionExpiry": str,
     },
     total=False,
@@ -142,23 +153,14 @@
     "GetAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
         "ConnectionToken": str,
     },
 )
 
-GetAttachmentResponseTypeDef = TypedDict(
-    "GetAttachmentResponseTypeDef",
-    {
-        "Url": str,
-        "UrlExpiry": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartPositionTypeDef = TypedDict(
     "StartPositionTypeDef",
     {
         "Id": str,
         "AbsoluteTime": str,
         "MostRecent": int,
     },
@@ -171,25 +173,14 @@
         "DeliveredTimestamp": str,
         "ReadTimestamp": str,
         "RecipientParticipantId": str,
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "ContentType": str,
         "ConnectionToken": str,
     },
 )
@@ -205,23 +196,14 @@
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
 
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "ContentType": str,
         "Content": str,
         "ConnectionToken": str,
     },
@@ -237,23 +219,14 @@
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
 
-SendMessageResponseTypeDef = TypedDict(
-    "SendMessageResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAttachmentUploadRequestRequestTypeDef = TypedDict(
     "StartAttachmentUploadRequestRequestTypeDef",
     {
         "ContentType": str,
         "AttachmentSizeInBytes": int,
         "AttachmentName": str,
         "ClientToken": str,
@@ -267,20 +240,47 @@
         "Url": str,
         "UrlExpiry": str,
         "HeadersToInclude": Dict[str, str],
     },
     total=False,
 )
 
+GetAttachmentResponseTypeDef = TypedDict(
+    "GetAttachmentResponseTypeDef",
+    {
+        "Url": str,
+        "UrlExpiry": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResponseTypeDef = TypedDict(
+    "SendMessageResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateParticipantConnectionResponseTypeDef = TypedDict(
     "CreateParticipantConnectionResponseTypeDef",
     {
         "Websocket": WebsocketTypeDef,
         "ConnectionCredentials": ConnectionCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTranscriptRequestRequestTypeDef = TypedDict(
     "_RequiredGetTranscriptRequestRequestTypeDef",
     {
         "ConnectionToken": str,
@@ -316,15 +316,15 @@
 )
 
 StartAttachmentUploadResponseTypeDef = TypedDict(
     "StartAttachmentUploadResponseTypeDef",
     {
         "AttachmentId": str,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "AbsoluteTime": str,
@@ -345,10 +345,10 @@
 
 GetTranscriptResponseTypeDef = TypedDict(
     "GetTranscriptResponseTypeDef",
     {
         "InitialContactId": str,
         "Transcript": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant/type_defs.pyi` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant/type_defs.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_connectparticipant.type_defs import AttachmentItemTypeDef
 
-    data: AttachmentItemTypeDef = {...}
+    data: AttachmentItemTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import (
     ArtifactStatusType,
@@ -29,27 +29,27 @@
     from typing_extensions import TypedDict
 
 __all__ = (
     "AttachmentItemTypeDef",
     "CompleteAttachmentUploadRequestRequestTypeDef",
     "ConnectionCredentialsTypeDef",
     "CreateParticipantConnectionRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "WebsocketTypeDef",
     "DisconnectParticipantRequestRequestTypeDef",
     "GetAttachmentRequestRequestTypeDef",
-    "GetAttachmentResponseTypeDef",
     "StartPositionTypeDef",
     "ReceiptTypeDef",
-    "ResponseMetadataTypeDef",
     "SendEventRequestRequestTypeDef",
-    "SendEventResponseTypeDef",
     "SendMessageRequestRequestTypeDef",
-    "SendMessageResponseTypeDef",
     "StartAttachmentUploadRequestRequestTypeDef",
     "UploadMetadataTypeDef",
+    "GetAttachmentResponseTypeDef",
+    "SendEventResponseTypeDef",
+    "SendMessageResponseTypeDef",
     "CreateParticipantConnectionResponseTypeDef",
     "GetTranscriptRequestRequestTypeDef",
     "MessageMetadataTypeDef",
     "StartAttachmentUploadResponseTypeDef",
     "ItemTypeDef",
     "GetTranscriptResponseTypeDef",
 )
@@ -100,14 +100,25 @@
 
 class CreateParticipantConnectionRequestRequestTypeDef(
     _RequiredCreateParticipantConnectionRequestRequestTypeDef,
     _OptionalCreateParticipantConnectionRequestRequestTypeDef,
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
 WebsocketTypeDef = TypedDict(
     "WebsocketTypeDef",
     {
         "Url": str,
         "ConnectionExpiry": str,
     },
     total=False,
@@ -137,23 +148,14 @@
     "GetAttachmentRequestRequestTypeDef",
     {
         "AttachmentId": str,
         "ConnectionToken": str,
     },
 )
 
-GetAttachmentResponseTypeDef = TypedDict(
-    "GetAttachmentResponseTypeDef",
-    {
-        "Url": str,
-        "UrlExpiry": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartPositionTypeDef = TypedDict(
     "StartPositionTypeDef",
     {
         "Id": str,
         "AbsoluteTime": str,
         "MostRecent": int,
     },
@@ -166,25 +168,14 @@
         "DeliveredTimestamp": str,
         "ReadTimestamp": str,
         "RecipientParticipantId": str,
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
 _RequiredSendEventRequestRequestTypeDef = TypedDict(
     "_RequiredSendEventRequestRequestTypeDef",
     {
         "ContentType": str,
         "ConnectionToken": str,
     },
 )
@@ -198,23 +189,14 @@
 )
 
 class SendEventRequestRequestTypeDef(
     _RequiredSendEventRequestRequestTypeDef, _OptionalSendEventRequestRequestTypeDef
 ):
     pass
 
-SendEventResponseTypeDef = TypedDict(
-    "SendEventResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredSendMessageRequestRequestTypeDef = TypedDict(
     "_RequiredSendMessageRequestRequestTypeDef",
     {
         "ContentType": str,
         "Content": str,
         "ConnectionToken": str,
     },
@@ -228,23 +210,14 @@
 )
 
 class SendMessageRequestRequestTypeDef(
     _RequiredSendMessageRequestRequestTypeDef, _OptionalSendMessageRequestRequestTypeDef
 ):
     pass
 
-SendMessageResponseTypeDef = TypedDict(
-    "SendMessageResponseTypeDef",
-    {
-        "Id": str,
-        "AbsoluteTime": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StartAttachmentUploadRequestRequestTypeDef = TypedDict(
     "StartAttachmentUploadRequestRequestTypeDef",
     {
         "ContentType": str,
         "AttachmentSizeInBytes": int,
         "AttachmentName": str,
         "ClientToken": str,
@@ -258,20 +231,47 @@
         "Url": str,
         "UrlExpiry": str,
         "HeadersToInclude": Dict[str, str],
     },
     total=False,
 )
 
+GetAttachmentResponseTypeDef = TypedDict(
+    "GetAttachmentResponseTypeDef",
+    {
+        "Url": str,
+        "UrlExpiry": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendEventResponseTypeDef = TypedDict(
+    "SendEventResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+SendMessageResponseTypeDef = TypedDict(
+    "SendMessageResponseTypeDef",
+    {
+        "Id": str,
+        "AbsoluteTime": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 CreateParticipantConnectionResponseTypeDef = TypedDict(
     "CreateParticipantConnectionResponseTypeDef",
     {
         "Websocket": WebsocketTypeDef,
         "ConnectionCredentials": ConnectionCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredGetTranscriptRequestRequestTypeDef = TypedDict(
     "_RequiredGetTranscriptRequestRequestTypeDef",
     {
         "ConnectionToken": str,
@@ -305,15 +305,15 @@
 )
 
 StartAttachmentUploadResponseTypeDef = TypedDict(
     "StartAttachmentUploadResponseTypeDef",
     {
         "AttachmentId": str,
         "UploadMetadata": UploadMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ItemTypeDef = TypedDict(
     "ItemTypeDef",
     {
         "AbsoluteTime": str,
@@ -334,10 +334,10 @@
 
 GetTranscriptResponseTypeDef = TypedDict(
     "GetTranscriptResponseTypeDef",
     {
         "InitialContactId": str,
         "Transcript": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/PKG-INFO` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-connectparticipant
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ConnectParticipant 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore connectparticipant type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore connectparticipant type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-connectparticipant"></a>
 
 # types-aiobotocore-connectparticipant
 
 [![PyPI - types-aiobotocore-connectparticipant](https://img.shields.io/pypi/v/types-aiobotocore-connectparticipant.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectparticipant)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-connectparticipant.svg?color=blue)](https://pypi.org/project/types-aiobotocore-connectparticipant)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-connectparticipant?color=blue)](https://pypistats.org/packages/types-aiobotocore-connectparticipant)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-connectparticipant)](https://pepy.tech/project/types-aiobotocore-connectparticipant)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ConnectParticipant 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connectparticipant.html#ConnectParticipant)
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
 [types-aiobotocore-connectparticipant docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_connectparticipant/).
 
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
@@ -286,50 +285,50 @@
 )
 
 
 def check_value(value: ArtifactStatusType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_connectparticipant.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_connectparticipant.type_defs import (
     AttachmentItemTypeDef,
     CompleteAttachmentUploadRequestRequestTypeDef,
     ConnectionCredentialsTypeDef,
     CreateParticipantConnectionRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     WebsocketTypeDef,
     DisconnectParticipantRequestRequestTypeDef,
     GetAttachmentRequestRequestTypeDef,
-    GetAttachmentResponseTypeDef,
     StartPositionTypeDef,
     ReceiptTypeDef,
-    ResponseMetadataTypeDef,
     SendEventRequestRequestTypeDef,
-    SendEventResponseTypeDef,
     SendMessageRequestRequestTypeDef,
-    SendMessageResponseTypeDef,
     StartAttachmentUploadRequestRequestTypeDef,
     UploadMetadataTypeDef,
+    GetAttachmentResponseTypeDef,
+    SendEventResponseTypeDef,
+    SendMessageResponseTypeDef,
     CreateParticipantConnectionResponseTypeDef,
     GetTranscriptRequestRequestTypeDef,
     MessageMetadataTypeDef,
     StartAttachmentUploadResponseTypeDef,
     ItemTypeDef,
     GetTranscriptResponseTypeDef,
 )
 
 
-def get_structure() -> AttachmentItemTypeDef:
+def get_value() -> AttachmentItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-connectparticipant-2.5.2/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt` & `types-aiobotocore-connectparticipant-2.5.2.post1/types_aiobotocore_connectparticipant.egg-info/SOURCES.txt`

 * *Files identical despite different names*


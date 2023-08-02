# Comparing `tmp/types-aiobotocore-iotsecuretunneling-2.5.2.tar.gz` & `tmp/types-aiobotocore-iotsecuretunneling-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.5.2.tar", last modified: Sat Jul  8 01:43:46 2023, max compression
+gzip compressed data, was "types-aiobotocore-iotsecuretunneling-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:27 2023, max compression
```

## Comparing `types-aiobotocore-iotsecuretunneling-2.5.2.tar` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.898306 types-aiobotocore-iotsecuretunneling-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-08 01:43:46.886306 types-aiobotocore-iotsecuretunneling-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11714 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:46.898306 types-aiobotocore-iotsecuretunneling-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.882306 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-07-08 01:32:50.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9197 2023-07-08 01:32:50.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-07-08 01:32:50.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-07-08 01:32:50.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     6520 2023-07-08 01:32:50.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6513 2023-07-08 01:32:50.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:32:49.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:46.886306 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-07-08 01:43:46.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-08 01:43:46.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:46.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:46.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-08 01:43:46.000000 types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7139 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7130 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:40:52.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:27.513560 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 14:52:27.000000 types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/LICENSE` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotsecuretunneling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotsecuretunneling?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotsecuretunneling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTSecureTunneling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
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
@@ -283,47 +282,49 @@
 )
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotsecuretunneling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
+    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
-    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
-    UntagResourceRequestRequestTypeDef,
+    DestinationConfigUnionTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
-def get_structure() -> CloseTunnelRequestRequestTypeDef:
+def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/README.md` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotsecuretunneling?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotsecuretunneling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTSecureTunneling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
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
@@ -250,47 +250,49 @@
 )
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotsecuretunneling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
+    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
-    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
-    UntagResourceRequestRequestTypeDef,
+    DestinationConfigUnionTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
-def get_structure() -> CloseTunnelRequestRequestTypeDef:
+def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/setup.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,46 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-iotsecuretunneling",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_iotsecuretunneling"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with"
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
-        "aiobotocore iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete"
-    ),
+    keywords="aiobotocore iotsecuretunneling type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_iotsecuretunneling": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/"
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/__init__.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/__init__.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/__main__.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.IoTSecureTunneling 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling\nOther"
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

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/client.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ClientModeType
 from .type_defs import (
     DescribeTunnelResponseTypeDef,
-    DestinationConfigTypeDef,
+    DestinationConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
     TagTypeDef,
     TimeoutConfigTypeDef,
 )
@@ -132,15 +132,15 @@
         """
 
     async def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        destinationConfig: DestinationConfigTypeDef = ...,
+        destinationConfig: DestinationConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use to
         connect to the IoT Secure Tunneling proxy server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
@@ -148,15 +148,15 @@
         """
 
     async def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: DestinationConfigTypeDef = ...
+        destinationConfig: DestinationConfigUnionTypeDef = ...
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients to
         use when reconnecting to secure tunneling to access the same tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#rotate_tunnel_access_token)
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/client.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ClientModeType
 from .type_defs import (
     DescribeTunnelResponseTypeDef,
-    DestinationConfigTypeDef,
+    DestinationConfigUnionTypeDef,
     ListTagsForResourceResponseTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelResponseTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
     TagTypeDef,
     TimeoutConfigTypeDef,
 )
@@ -121,30 +121,30 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#list_tunnels)
         """
     async def open_tunnel(
         self,
         *,
         description: str = ...,
         tags: Sequence[TagTypeDef] = ...,
-        destinationConfig: DestinationConfigTypeDef = ...,
+        destinationConfig: DestinationConfigUnionTypeDef = ...,
         timeoutConfig: TimeoutConfigTypeDef = ...
     ) -> OpenTunnelResponseTypeDef:
         """
         Creates a new tunnel, and returns two client access tokens for clients to use to
         connect to the IoT Secure Tunneling proxy server.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.open_tunnel)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#open_tunnel)
         """
     async def rotate_tunnel_access_token(
         self,
         *,
         tunnelId: str,
         clientMode: ClientModeType,
-        destinationConfig: DestinationConfigTypeDef = ...
+        destinationConfig: DestinationConfigUnionTypeDef = ...
     ) -> RotateTunnelAccessTokenResponseTypeDef:
         """
         Revokes the current client access token (CAT) and returns new CAT for clients to
         use when reconnecting to secure tunneling to access the same tunnel.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling.Client.rotate_tunnel_access_token)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/client/#rotate_tunnel_access_token)
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/literals.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/literals.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/type_defs.py` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,43 +4,45 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
-    data: CloseTunnelRequestRequestTypeDef = {...}
+    data: CloseTunnelRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
-    "UntagResourceRequestRequestTypeDef",
+    "DestinationConfigUnionTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -79,18 +81,50 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
     },
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
+_RequiredDestinationConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationConfigOutputTypeDef",
+    {
+        "services": List[str],
+    },
+)
+_OptionalDestinationConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationConfigOutputTypeDef",
+    {
+        "thingName": str,
+    },
+    total=False,
+)
+
+
+class DestinationConfigOutputTypeDef(
+    _RequiredDestinationConfigOutputTypeDef, _OptionalDestinationConfigOutputTypeDef
+):
+    pass
+
+
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
-        "services": List[str],
+        "services": Sequence[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
     "_OptionalDestinationConfigTypeDef",
     {
         "thingName": str,
     },
@@ -146,54 +180,44 @@
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 OpenTunnelResponseTypeDef = TypedDict(
     "OpenTunnelResponseTypeDef",
     {
         "tunnelId": str,
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateTunnelAccessTokenResponseTypeDef = TypedDict(
     "RotateTunnelAccessTokenResponseTypeDef",
     {
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigUnionTypeDef = Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef]
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
         "clientMode": ClientModeType,
     },
 )
@@ -213,15 +237,15 @@
     pass
 
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -230,15 +254,15 @@
 )
 
 ListTunnelsResponseTypeDef = TypedDict(
     "ListTunnelsResponseTypeDef",
     {
         "tunnelSummaries": List[TunnelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
@@ -254,23 +278,23 @@
     {
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
-        "destinationConfig": DestinationConfigTypeDef,
+        "destinationConfig": DestinationConfigOutputTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": List[TagTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
     "DescribeTunnelResponseTypeDef",
     {
         "tunnel": TunnelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling/type_defs.pyi` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_iotsecuretunneling.type_defs import CloseTunnelRequestRequestTypeDef
 
-    data: CloseTunnelRequestRequestTypeDef = {...}
+    data: CloseTunnelRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import ClientModeType, ConnectionStatusType, TunnelStatusType
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CloseTunnelRequestRequestTypeDef",
     "ConnectionStateTypeDef",
     "DescribeTunnelRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
+    "DestinationConfigOutputTypeDef",
     "DestinationConfigTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "TagTypeDef",
     "ListTunnelsRequestRequestTypeDef",
     "TunnelSummaryTypeDef",
     "TimeoutConfigTypeDef",
+    "UntagResourceRequestRequestTypeDef",
     "OpenTunnelResponseTypeDef",
-    "ResponseMetadataTypeDef",
     "RotateTunnelAccessTokenResponseTypeDef",
-    "UntagResourceRequestRequestTypeDef",
+    "DestinationConfigUnionTypeDef",
     "RotateTunnelAccessTokenRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "ListTunnelsResponseTypeDef",
     "OpenTunnelRequestRequestTypeDef",
     "TunnelTypeDef",
     "DescribeTunnelResponseTypeDef",
@@ -76,18 +78,48 @@
 DescribeTunnelRequestRequestTypeDef = TypedDict(
     "DescribeTunnelRequestRequestTypeDef",
     {
         "tunnelId": str,
     },
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
+_RequiredDestinationConfigOutputTypeDef = TypedDict(
+    "_RequiredDestinationConfigOutputTypeDef",
+    {
+        "services": List[str],
+    },
+)
+_OptionalDestinationConfigOutputTypeDef = TypedDict(
+    "_OptionalDestinationConfigOutputTypeDef",
+    {
+        "thingName": str,
+    },
+    total=False,
+)
+
+class DestinationConfigOutputTypeDef(
+    _RequiredDestinationConfigOutputTypeDef, _OptionalDestinationConfigOutputTypeDef
+):
+    pass
+
 _RequiredDestinationConfigTypeDef = TypedDict(
     "_RequiredDestinationConfigTypeDef",
     {
-        "services": List[str],
+        "services": Sequence[str],
     },
 )
 _OptionalDestinationConfigTypeDef = TypedDict(
     "_OptionalDestinationConfigTypeDef",
     {
         "thingName": str,
     },
@@ -141,54 +173,44 @@
     "TimeoutConfigTypeDef",
     {
         "maxLifetimeTimeoutMinutes": int,
     },
     total=False,
 )
 
+UntagResourceRequestRequestTypeDef = TypedDict(
+    "UntagResourceRequestRequestTypeDef",
+    {
+        "resourceArn": str,
+        "tagKeys": Sequence[str],
+    },
+)
+
 OpenTunnelResponseTypeDef = TypedDict(
     "OpenTunnelResponseTypeDef",
     {
         "tunnelId": str,
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
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
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RotateTunnelAccessTokenResponseTypeDef = TypedDict(
     "RotateTunnelAccessTokenResponseTypeDef",
     {
         "tunnelArn": str,
         "sourceAccessToken": str,
         "destinationAccessToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-UntagResourceRequestRequestTypeDef = TypedDict(
-    "UntagResourceRequestRequestTypeDef",
-    {
-        "resourceArn": str,
-        "tagKeys": Sequence[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DestinationConfigUnionTypeDef = Union[DestinationConfigTypeDef, DestinationConfigOutputTypeDef]
 _RequiredRotateTunnelAccessTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRotateTunnelAccessTokenRequestRequestTypeDef",
     {
         "tunnelId": str,
         "clientMode": ClientModeType,
     },
 )
@@ -206,15 +228,15 @@
 ):
     pass
 
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
@@ -223,15 +245,15 @@
 )
 
 ListTunnelsResponseTypeDef = TypedDict(
     "ListTunnelsResponseTypeDef",
     {
         "tunnelSummaries": List[TunnelSummaryTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 OpenTunnelRequestRequestTypeDef = TypedDict(
     "OpenTunnelRequestRequestTypeDef",
     {
         "description": str,
@@ -247,23 +269,23 @@
     {
         "tunnelId": str,
         "tunnelArn": str,
         "status": TunnelStatusType,
         "sourceConnectionState": ConnectionStateTypeDef,
         "destinationConnectionState": ConnectionStateTypeDef,
         "description": str,
-        "destinationConfig": DestinationConfigTypeDef,
+        "destinationConfig": DestinationConfigOutputTypeDef,
         "timeoutConfig": TimeoutConfigTypeDef,
         "tags": List[TagTypeDef],
         "createdAt": datetime,
         "lastUpdatedAt": datetime,
     },
     total=False,
 )
 
 DescribeTunnelResponseTypeDef = TypedDict(
     "DescribeTunnelResponseTypeDef",
     {
         "tunnel": TunnelTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-iotsecuretunneling
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.IoTSecureTunneling 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore iotsecuretunneling type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore iotsecuretunneling type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-iotsecuretunneling"></a>
 
 # types-aiobotocore-iotsecuretunneling
 
 [![PyPI - types-aiobotocore-iotsecuretunneling](https://img.shields.io/pypi/v/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-iotsecuretunneling.svg?color=blue)](https://pypi.org/project/types-aiobotocore-iotsecuretunneling)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-iotsecuretunneling?color=blue)](https://pypistats.org/packages/types-aiobotocore-iotsecuretunneling)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-iotsecuretunneling)](https://pepy.tech/project/types-aiobotocore-iotsecuretunneling)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.IoTSecureTunneling 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/iotsecuretunneling.html#IoTSecureTunneling)
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
 [types-aiobotocore-iotsecuretunneling docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_iotsecuretunneling/).
 
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
@@ -283,47 +282,49 @@
 )
 
 
 def check_value(value: ClientModeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_iotsecuretunneling.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_iotsecuretunneling.type_defs import (
     CloseTunnelRequestRequestTypeDef,
     ConnectionStateTypeDef,
     DescribeTunnelRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
+    DestinationConfigOutputTypeDef,
     DestinationConfigTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     TagTypeDef,
     ListTunnelsRequestRequestTypeDef,
     TunnelSummaryTypeDef,
     TimeoutConfigTypeDef,
+    UntagResourceRequestRequestTypeDef,
     OpenTunnelResponseTypeDef,
-    ResponseMetadataTypeDef,
     RotateTunnelAccessTokenResponseTypeDef,
-    UntagResourceRequestRequestTypeDef,
+    DestinationConfigUnionTypeDef,
     RotateTunnelAccessTokenRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     ListTunnelsResponseTypeDef,
     OpenTunnelRequestRequestTypeDef,
     TunnelTypeDef,
     DescribeTunnelResponseTypeDef,
 )
 
 
-def get_structure() -> CloseTunnelRequestRequestTypeDef:
+def get_value() -> CloseTunnelRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-iotsecuretunneling-2.5.2/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt` & `types-aiobotocore-iotsecuretunneling-2.5.2.post1/types_aiobotocore_iotsecuretunneling.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-apigatewaymanagementapi-2.5.2.tar.gz` & `tmp/types-aiobotocore-apigatewaymanagementapi-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-apigatewaymanagementapi-2.5.2.tar", last modified: Sat Jul  8 01:43:12 2023, max compression
+gzip compressed data, was "types-aiobotocore-apigatewaymanagementapi-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:50 2023, max compression
```

## Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2.tar` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.405653 types-aiobotocore-apigatewaymanagementapi-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-08 01:43:12.405653 types-aiobotocore-apigatewaymanagementapi-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11445 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:12.405653 types-aiobotocore-apigatewaymanagementapi-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.389653 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:35.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:12.405653 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13074 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 01:43:12.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11419 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.437660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6177 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7647 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-02 14:33:02.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:01.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:50.445660 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:51:50.000000 types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/LICENSE` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/PKG-INFO` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewaymanagementapi
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore apigatewaymanagementapi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore apigatewaymanagementapi type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-apigatewaymanagementapi"></a>
 
 # types-aiobotocore-apigatewaymanagementapi
 
 [![PyPI - types-aiobotocore-apigatewaymanagementapi](https://img.shields.io/pypi/v/types-aiobotocore-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigatewaymanagementapi?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigatewaymanagementapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewaymanagementapi)](https://pepy.tech/project/types-aiobotocore-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApiGatewayManagementApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [types-aiobotocore-apigatewaymanagementapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/).
 
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
@@ -279,35 +278,36 @@
 )
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_apigatewaymanagementapi.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_apigatewaymanagementapi.type_defs import (
+    BlobTypeDef,
     DeleteConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteConnectionRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/README.md` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-apigatewaymanagementapi"></a>
 
 # types-aiobotocore-apigatewaymanagementapi
 
 [![PyPI - types-aiobotocore-apigatewaymanagementapi](https://img.shields.io/pypi/v/types-aiobotocore-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigatewaymanagementapi?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigatewaymanagementapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewaymanagementapi)](https://pepy.tech/project/types-aiobotocore-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApiGatewayManagementApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [types-aiobotocore-apigatewaymanagementapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/).
 
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
@@ -246,35 +246,36 @@
 )
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_apigatewaymanagementapi.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_apigatewaymanagementapi.type_defs import (
+    BlobTypeDef,
     DeleteConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteConnectionRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/setup.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,46 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-apigatewaymanagementapi",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_apigatewaymanagementapi"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with"
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
-        "aiobotocore apigatewaymanagementapi type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "aiobotocore apigatewaymanagementapi type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_apigatewaymanagementapi": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/",
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/__init__.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/__init__.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/__main__.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi\nOther"
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

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/client.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
 
     session = get_session()
     async with session.create_client("apigatewaymanagementapi") as client:
         client: ApiGatewayManagementApiClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
-from .type_defs import EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
+from .type_defs import BlobTypeDef, EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
 
 __all__ = ("ApiGatewayManagementApiClient",)
 
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
@@ -101,15 +100,15 @@
         Get information about the connection with the provided id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.get_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/client/#get_connection)
         """
 
     async def post_to_connection(
-        self, *, Data: Union[str, bytes, IO[Any], StreamingBody], ConnectionId: str
+        self, *, Data: BlobTypeDef, ConnectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends the provided data to the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.post_to_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/client/#post_to_connection)
         """
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/client.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,20 @@
     from types_aiobotocore_apigatewaymanagementapi.client import ApiGatewayManagementApiClient
 
     session = get_session()
     async with session.create_client("apigatewaymanagementapi") as client:
         client: ApiGatewayManagementApiClient
     ```
 """
-from typing import IO, Any, Dict, Mapping, Type, Union
+from typing import Any, Dict, Mapping, Type
 
 from aiobotocore.client import AioBaseClient
-from aiobotocore.response import StreamingBody
 from botocore.client import ClientMeta
 
-from .type_defs import EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
+from .type_defs import BlobTypeDef, EmptyResponseMetadataTypeDef, GetConnectionResponseTypeDef
 
 __all__ = ("ApiGatewayManagementApiClient",)
 
 class BotocoreClientError(BaseException):
     MSG_TEMPLATE: str
 
     def __init__(self, error_response: Mapping[str, Any], operation_name: str) -> None:
@@ -92,15 +91,15 @@
         """
         Get information about the connection with the provided id.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.get_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/client/#get_connection)
         """
     async def post_to_connection(
-        self, *, Data: Union[str, bytes, IO[Any], StreamingBody], ConnectionId: str
+        self, *, Data: BlobTypeDef, ConnectionId: str
     ) -> EmptyResponseMetadataTypeDef:
         """
         Sends the provided data to the specified connection.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi.Client.post_to_connection)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/client/#post_to_connection)
         """
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/literals.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/literals.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/type_defs.py` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 Type annotations for apigatewaymanagementapi service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef
+    from types_aiobotocore_apigatewaymanagementapi.type_defs import BlobTypeDef
 
-    data: DeleteConnectionRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, Union
 
 from aiobotocore.response import StreamingBody
@@ -20,34 +20,40 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
+    "BlobTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "IdentityTypeDef",
     "PostToConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetConnectionResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
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
 
 GetConnectionRequestRequestTypeDef = TypedDict(
     "GetConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
@@ -61,32 +67,28 @@
         "UserAgent": str,
     },
 )
 
 PostToConnectionRequestRequestTypeDef = TypedDict(
     "PostToConnectionRequestRequestTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "ConnectionId": str,
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
 
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "ConnectedAt": datetime,
         "Identity": IdentityTypeDef,
         "LastActiveAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,51 +2,57 @@
 Type annotations for apigatewaymanagementapi service type definitions.
 
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/type_defs/)
 
 Usage::
 
     ```python
-    from types_aiobotocore_apigatewaymanagementapi.type_defs import DeleteConnectionRequestRequestTypeDef
+    from types_aiobotocore_apigatewaymanagementapi.type_defs import BlobTypeDef
 
-    data: DeleteConnectionRequestRequestTypeDef = {...}
+    data: BlobTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import IO, Any, Dict, Union
 
 from aiobotocore.response import StreamingBody
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
+    "BlobTypeDef",
     "DeleteConnectionRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetConnectionRequestRequestTypeDef",
     "IdentityTypeDef",
     "PostToConnectionRequestRequestTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "GetConnectionResponseTypeDef",
 )
 
+BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
 DeleteConnectionRequestRequestTypeDef = TypedDict(
     "DeleteConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
     },
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
 
 GetConnectionRequestRequestTypeDef = TypedDict(
     "GetConnectionRequestRequestTypeDef",
     {
         "ConnectionId": str,
@@ -60,32 +66,28 @@
         "UserAgent": str,
     },
 )
 
 PostToConnectionRequestRequestTypeDef = TypedDict(
     "PostToConnectionRequestRequestTypeDef",
     {
-        "Data": Union[str, bytes, IO[Any], StreamingBody],
+        "Data": BlobTypeDef,
         "ConnectionId": str,
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
 
 GetConnectionResponseTypeDef = TypedDict(
     "GetConnectionResponseTypeDef",
     {
         "ConnectedAt": datetime,
         "Identity": IdentityTypeDef,
         "LastActiveAt": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-apigatewaymanagementapi
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApiGatewayManagementApi 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore apigatewaymanagementapi type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore apigatewaymanagementapi type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-apigatewaymanagementapi"></a>
 
 # types-aiobotocore-apigatewaymanagementapi
 
 [![PyPI - types-aiobotocore-apigatewaymanagementapi](https://img.shields.io/pypi/v/types-aiobotocore-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-apigatewaymanagementapi.svg?color=blue)](https://pypi.org/project/types-aiobotocore-apigatewaymanagementapi)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-apigatewaymanagementapi?color=blue)](https://pypistats.org/packages/types-aiobotocore-apigatewaymanagementapi)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-apigatewaymanagementapi)](https://pepy.tech/project/types-aiobotocore-apigatewaymanagementapi)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApiGatewayManagementApi 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/apigatewaymanagementapi.html#ApiGatewayManagementApi)
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
 [types-aiobotocore-apigatewaymanagementapi docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_apigatewaymanagementapi/).
 
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
@@ -279,35 +278,36 @@
 )
 
 
 def check_value(value: ApiGatewayManagementApiServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_apigatewaymanagementapi.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_apigatewaymanagementapi.type_defs import (
+    BlobTypeDef,
     DeleteConnectionRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetConnectionRequestRequestTypeDef,
     IdentityTypeDef,
     PostToConnectionRequestRequestTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     GetConnectionResponseTypeDef,
 )
 
 
-def get_structure() -> DeleteConnectionRequestRequestTypeDef:
+def get_value() -> BlobTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-apigatewaymanagementapi-2.5.2/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt` & `types-aiobotocore-apigatewaymanagementapi-2.5.2.post1/types_aiobotocore_apigatewaymanagementapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*


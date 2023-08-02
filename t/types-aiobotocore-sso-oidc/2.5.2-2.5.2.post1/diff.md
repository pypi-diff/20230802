# Comparing `tmp/types-aiobotocore-sso-oidc-2.5.2.tar.gz` & `tmp/types-aiobotocore-sso-oidc-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-oidc-2.5.2.tar", last modified: Sat Jul  8 01:44:22 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-oidc-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
```

## Comparing `types-aiobotocore-sso-oidc-2.5.2.tar` & `types-aiobotocore-sso-oidc-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.930951 types-aiobotocore-sso-oidc-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-08 01:44:22.930951 types-aiobotocore-sso-oidc-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10770 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:22.930951 types-aiobotocore-sso-oidc-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-07-08 01:41:40.000000 types-aiobotocore-sso-oidc-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.930951 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:41.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:22.930951 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12338 2023-07-08 01:44:22.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 01:44:22.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:22.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:22.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 01:44:22.000000 types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10753 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6480 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6469 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3325 2023-08-02 14:50:19.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:18.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.601447 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12274 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-02 14:53:04.000000 types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/LICENSE` & `types-aiobotocore-sso-oidc-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2/PKG-INFO` & `types-aiobotocore-sso-oidc-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso-oidc
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sso-oidc type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sso-oidc type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sso-oidc"></a>
 
 # types-aiobotocore-sso-oidc
 
 [![PyPI - types-aiobotocore-sso-oidc](https://img.shields.io/pypi/v/types-aiobotocore-sso-oidc.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso-oidc.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sso-oidc?color=blue)](https://pypistats.org/packages/types-aiobotocore-sso-oidc)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso-oidc)](https://pepy.tech/project/types-aiobotocore-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSOOIDC 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [types-aiobotocore-sso-oidc docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/).
 
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
@@ -279,34 +278,34 @@
 )
 
 
 def check_value(value: SSOOIDCServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sso_oidc.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    RegisterClientResponseTypeDef,
     ResponseMetadataTypeDef,
+    RegisterClientRequestRequestTypeDef,
     StartDeviceAuthorizationRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
+    RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
-def get_structure() -> CreateTokenRequestRequestTypeDef:
+def get_value() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/README.md` & `types-aiobotocore-sso-oidc-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sso-oidc"></a>
 
 # types-aiobotocore-sso-oidc
 
 [![PyPI - types-aiobotocore-sso-oidc](https://img.shields.io/pypi/v/types-aiobotocore-sso-oidc.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso-oidc.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sso-oidc?color=blue)](https://pypistats.org/packages/types-aiobotocore-sso-oidc)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso-oidc)](https://pepy.tech/project/types-aiobotocore-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSOOIDC 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [types-aiobotocore-sso-oidc docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/).
 
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
@@ -246,34 +246,34 @@
 )
 
 
 def check_value(value: SSOOIDCServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sso_oidc.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    RegisterClientResponseTypeDef,
     ResponseMetadataTypeDef,
+    RegisterClientRequestRequestTypeDef,
     StartDeviceAuthorizationRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
+    RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
-def get_structure() -> CreateTokenRequestRequestTypeDef:
+def get_value() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/setup.py` & `types-aiobotocore-sso-oidc-2.5.2.post1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso-oidc",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sso_oidc"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore sso-oidc type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sso-oidc type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sso_oidc": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/"
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/__main__.py` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSOOIDC 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SSOOIDC 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC\nOther"
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

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/client.py` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/client.pyi` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/literals.py` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/literals.pyi` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/type_defs.py` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,33 +4,32 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef
 
-    data: CreateTokenRequestRequestTypeDef = {...}
+    data: CreateTokenRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
-    "RegisterClientRequestRequestTypeDef",
-    "RegisterClientResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "RegisterClientRequestRequestTypeDef",
     "StartDeviceAuthorizationRequestRequestTypeDef",
+    "CreateTokenResponseTypeDef",
+    "RegisterClientResponseTypeDef",
     "StartDeviceAuthorizationResponseTypeDef",
 )
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "clientId": str,
@@ -46,30 +45,27 @@
         "refreshToken": str,
         "scope": Sequence[str],
         "redirectUri": str,
     },
     total=False,
 )
 
-
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accessToken": str,
-        "tokenType": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "idToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredRegisterClientRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
@@ -80,59 +76,58 @@
     "_OptionalRegisterClientRequestRequestTypeDef",
     {
         "scopes": Sequence[str],
     },
     total=False,
 )
 
-
 class RegisterClientRequestRequestTypeDef(
     _RequiredRegisterClientRequestRequestTypeDef, _OptionalRegisterClientRequestRequestTypeDef
 ):
     pass
 
-
-RegisterClientResponseTypeDef = TypedDict(
-    "RegisterClientResponseTypeDef",
+StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "clientIdIssuedAt": int,
-        "clientSecretExpiresAt": int,
-        "authorizationEndpoint": str,
-        "tokenEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "startUrl": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accessToken": str,
+        "tokenType": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "idToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
-    "StartDeviceAuthorizationRequestRequestTypeDef",
+RegisterClientResponseTypeDef = TypedDict(
+    "RegisterClientResponseTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "startUrl": str,
+        "clientIdIssuedAt": int,
+        "clientSecretExpiresAt": int,
+        "authorizationEndpoint": str,
+        "tokenEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDeviceAuthorizationResponseTypeDef = TypedDict(
     "StartDeviceAuthorizationResponseTypeDef",
     {
         "deviceCode": str,
         "userCode": str,
         "verificationUri": str,
         "verificationUriComplete": str,
         "expiresIn": int,
         "interval": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc/type_defs.pyi` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc/type_defs.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sso_oidc.type_defs import CreateTokenRequestRequestTypeDef
 
-    data: CreateTokenRequestRequestTypeDef = {...}
+    data: CreateTokenRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "CreateTokenRequestRequestTypeDef",
-    "CreateTokenResponseTypeDef",
-    "RegisterClientRequestRequestTypeDef",
-    "RegisterClientResponseTypeDef",
     "ResponseMetadataTypeDef",
+    "RegisterClientRequestRequestTypeDef",
     "StartDeviceAuthorizationRequestRequestTypeDef",
+    "CreateTokenResponseTypeDef",
+    "RegisterClientResponseTypeDef",
     "StartDeviceAuthorizationResponseTypeDef",
 )
 
 _RequiredCreateTokenRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTokenRequestRequestTypeDef",
     {
         "clientId": str,
@@ -45,28 +46,29 @@
         "refreshToken": str,
         "scope": Sequence[str],
         "redirectUri": str,
     },
     total=False,
 )
 
+
 class CreateTokenRequestRequestTypeDef(
     _RequiredCreateTokenRequestRequestTypeDef, _OptionalCreateTokenRequestRequestTypeDef
 ):
     pass
 
-CreateTokenResponseTypeDef = TypedDict(
-    "CreateTokenResponseTypeDef",
+
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "accessToken": str,
-        "tokenType": str,
-        "expiresIn": int,
-        "refreshToken": str,
-        "idToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredRegisterClientRequestRequestTypeDef = TypedDict(
     "_RequiredRegisterClientRequestRequestTypeDef",
     {
         "clientName": str,
@@ -77,57 +79,60 @@
     "_OptionalRegisterClientRequestRequestTypeDef",
     {
         "scopes": Sequence[str],
     },
     total=False,
 )
 
+
 class RegisterClientRequestRequestTypeDef(
     _RequiredRegisterClientRequestRequestTypeDef, _OptionalRegisterClientRequestRequestTypeDef
 ):
     pass
 
-RegisterClientResponseTypeDef = TypedDict(
-    "RegisterClientResponseTypeDef",
+
+StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
+    "StartDeviceAuthorizationRequestRequestTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "clientIdIssuedAt": int,
-        "clientSecretExpiresAt": int,
-        "authorizationEndpoint": str,
-        "tokenEndpoint": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "startUrl": str,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CreateTokenResponseTypeDef = TypedDict(
+    "CreateTokenResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "accessToken": str,
+        "tokenType": str,
+        "expiresIn": int,
+        "refreshToken": str,
+        "idToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-StartDeviceAuthorizationRequestRequestTypeDef = TypedDict(
-    "StartDeviceAuthorizationRequestRequestTypeDef",
+RegisterClientResponseTypeDef = TypedDict(
+    "RegisterClientResponseTypeDef",
     {
         "clientId": str,
         "clientSecret": str,
-        "startUrl": str,
+        "clientIdIssuedAt": int,
+        "clientSecretExpiresAt": int,
+        "authorizationEndpoint": str,
+        "tokenEndpoint": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartDeviceAuthorizationResponseTypeDef = TypedDict(
     "StartDeviceAuthorizationResponseTypeDef",
     {
         "deviceCode": str,
         "userCode": str,
         "verificationUri": str,
         "verificationUriComplete": str,
         "expiresIn": int,
         "interval": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/PKG-INFO` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso-oidc
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSOOIDC 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sso-oidc type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sso-oidc type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sso-oidc"></a>
 
 # types-aiobotocore-sso-oidc
 
 [![PyPI - types-aiobotocore-sso-oidc](https://img.shields.io/pypi/v/types-aiobotocore-sso-oidc.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-oidc)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso-oidc.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso-oidc)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sso-oidc?color=blue)](https://pypistats.org/packages/types-aiobotocore-sso-oidc)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso-oidc)](https://pepy.tech/project/types-aiobotocore-sso-oidc)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSOOIDC 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso-oidc.html#SSOOIDC)
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
 [types-aiobotocore-sso-oidc docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso_oidc/).
 
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
@@ -279,34 +278,34 @@
 )
 
 
 def check_value(value: SSOOIDCServiceName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sso_oidc.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sso_oidc.type_defs import (
     CreateTokenRequestRequestTypeDef,
-    CreateTokenResponseTypeDef,
-    RegisterClientRequestRequestTypeDef,
-    RegisterClientResponseTypeDef,
     ResponseMetadataTypeDef,
+    RegisterClientRequestRequestTypeDef,
     StartDeviceAuthorizationRequestRequestTypeDef,
+    CreateTokenResponseTypeDef,
+    RegisterClientResponseTypeDef,
     StartDeviceAuthorizationResponseTypeDef,
 )
 
 
-def get_structure() -> CreateTokenRequestRequestTypeDef:
+def get_value() -> CreateTokenRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sso-oidc-2.5.2/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt` & `types-aiobotocore-sso-oidc-2.5.2.post1/types_aiobotocore_sso_oidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*


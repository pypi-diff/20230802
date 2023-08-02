# Comparing `tmp/types-aiobotocore-sso-2.5.2.tar.gz` & `tmp/types-aiobotocore-sso-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sso-2.5.2.tar", last modified: Sat Jul  8 01:44:23 2023, max compression
+gzip compressed data, was "types-aiobotocore-sso-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:04 2023, max compression
```

## Comparing `types-aiobotocore-sso-2.5.2.tar` & `types-aiobotocore-sso-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.270957 types-aiobotocore-sso-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-07-08 01:44:23.270957 types-aiobotocore-sso-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11726 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:23.270957 types-aiobotocore-sso-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.270957 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3027 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-07-08 01:41:39.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:38.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:23.270957 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13275 2023-07-08 01:44:23.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:23.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:23.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:23.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:23.000000 types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11709 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8255 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5364 2023-08-02 14:50:17.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:16.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:04.741447 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13211 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:53:04.000000 types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sso-2.5.2/LICENSE` & `types-aiobotocore-sso-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/PKG-INFO` & `types-aiobotocore-sso-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sso type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sso type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sso"></a>
 
 # types-aiobotocore-sso
 
 [![PyPI - types-aiobotocore-sso](https://img.shields.io/pypi/v/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sso?color=blue)](https://pypistats.org/packages/types-aiobotocore-sso)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSO 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
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
@@ -307,42 +306,42 @@
 )
 
 
 def check_value(value: ListAccountRolesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sso.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sso.type_defs import (
     AccountInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInfoTypeDef:
+def get_value() -> AccountInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sso-2.5.2/README.md` & `types-aiobotocore-sso-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sso"></a>
 
 # types-aiobotocore-sso
 
 [![PyPI - types-aiobotocore-sso](https://img.shields.io/pypi/v/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sso?color=blue)](https://pypistats.org/packages/types-aiobotocore-sso)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSO 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
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
@@ -274,42 +274,42 @@
 )
 
 
 def check_value(value: ListAccountRolesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sso.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sso.type_defs import (
     AccountInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInfoTypeDef:
+def get_value() -> AccountInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sso-2.5.2/setup.py` & `types-aiobotocore-sso-2.5.2.post1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sso",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sso"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore sso type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sso type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sso": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/__init__.py` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/__init__.pyi` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/__main__.py` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SSO 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SSO 2.5.2\nVersion:         2.5.2.post1\nBuilder version:"
+        " 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO\nOther"
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

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/client.py` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/client.pyi` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/literals.py` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/literals.pyi` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/paginator.py` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 class ListAccountRolesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountrolespaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountrolespaginator)
         """
 
 
 class ListAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountspaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountspaginator)
         """
```

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/paginator.pyi` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 class ListAccountRolesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountrolespaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, accountId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, accountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountRolesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccountRoles.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountrolespaginator)
         """
 
 class ListAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountspaginator)
     """
 
     def paginate(
-        self, *, accessToken: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, accessToken: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListAccountsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO.Paginator.ListAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/paginators/#listaccountspaginator)
         """
```

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/type_defs.py` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,58 +4,62 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sso.type_defs import AccountInfoTypeDef
 
-    data: AccountInfoTypeDef = {...}
+    data: AccountInfoTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AccountInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
-    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
     "RoleInfoTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "LogoutRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListAccountsResponseTypeDef",
     "GetRoleCredentialsResponseTypeDef",
+    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountRolesResponseTypeDef",
 )
 
 AccountInfoTypeDef = TypedDict(
     "AccountInfoTypeDef",
     {
         "accountId": str,
         "accountName": str,
         "emailAddress": str,
     },
     total=False,
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
 
 GetRoleCredentialsRequestRequestTypeDef = TypedDict(
     "GetRoleCredentialsRequestRequestTypeDef",
     {
         "roleName": str,
@@ -71,37 +75,24 @@
         "secretAccessKey": str,
         "sessionToken": str,
         "expiration": int,
     },
     total=False,
 )
 
-_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "accessToken": str,
-        "accountId": str,
-    },
-)
-_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
-    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccountRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountRolesRequestRequestTypeDef",
     {
         "accessToken": str,
         "accountId": str,
     },
 )
@@ -126,36 +117,14 @@
     {
         "roleName": str,
         "accountId": str,
     },
     total=False,
 )
 
-_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "accessToken": str,
-    },
-)
-_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListAccountsRequestListAccountsPaginateTypeDef(
-    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
-    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListAccountsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 _OptionalListAccountsRequestRequestTypeDef = TypedDict(
@@ -177,53 +146,84 @@
 LogoutRequestRequestTypeDef = TypedDict(
     "LogoutRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "nextToken": str,
         "accountList": List[AccountInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoleCredentialsResponseTypeDef = TypedDict(
     "GetRoleCredentialsResponseTypeDef",
     {
         "roleCredentials": RoleCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "accessToken": str,
+        "accountId": str,
+    },
+)
+_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+
+class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
+    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "accessToken": str,
+    },
+)
+_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListAccountsRequestListAccountsPaginateTypeDef(
+    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
+    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
+):
+    pass
+
+
 ListAccountRolesResponseTypeDef = TypedDict(
     "ListAccountRolesResponseTypeDef",
     {
         "nextToken": str,
         "roleList": List[RoleInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso/type_defs.pyi` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,57 +4,61 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sso.type_defs import AccountInfoTypeDef
 
-    data: AccountInfoTypeDef = {...}
+    data: AccountInfoTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AccountInfoTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetRoleCredentialsRequestRequestTypeDef",
     "RoleCredentialsTypeDef",
-    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListAccountRolesRequestRequestTypeDef",
     "RoleInfoTypeDef",
-    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountsRequestRequestTypeDef",
     "LogoutRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListAccountsResponseTypeDef",
     "GetRoleCredentialsResponseTypeDef",
+    "ListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    "ListAccountsRequestListAccountsPaginateTypeDef",
     "ListAccountRolesResponseTypeDef",
 )
 
 AccountInfoTypeDef = TypedDict(
     "AccountInfoTypeDef",
     {
         "accountId": str,
         "accountName": str,
         "emailAddress": str,
     },
     total=False,
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
 
 GetRoleCredentialsRequestRequestTypeDef = TypedDict(
     "GetRoleCredentialsRequestRequestTypeDef",
     {
         "roleName": str,
@@ -70,35 +74,24 @@
         "secretAccessKey": str,
         "sessionToken": str,
         "expiration": int,
     },
     total=False,
 )
 
-_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
-    {
-        "accessToken": str,
-        "accountId": str,
-    },
-)
-_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
-    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
-    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
-    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccountRolesRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountRolesRequestRequestTypeDef",
     {
         "accessToken": str,
         "accountId": str,
     },
 )
@@ -121,34 +114,14 @@
     {
         "roleName": str,
         "accountId": str,
     },
     total=False,
 )
 
-_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "accessToken": str,
-    },
-)
-_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
-    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListAccountsRequestListAccountsPaginateTypeDef(
-    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
-    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
-):
-    pass
-
 _RequiredListAccountsRequestRequestTypeDef = TypedDict(
     "_RequiredListAccountsRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 _OptionalListAccountsRequestRequestTypeDef = TypedDict(
@@ -168,53 +141,80 @@
 LogoutRequestRequestTypeDef = TypedDict(
     "LogoutRequestRequestTypeDef",
     {
         "accessToken": str,
     },
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
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
 
 ListAccountsResponseTypeDef = TypedDict(
     "ListAccountsResponseTypeDef",
     {
         "nextToken": str,
         "accountList": List[AccountInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetRoleCredentialsResponseTypeDef = TypedDict(
     "GetRoleCredentialsResponseTypeDef",
     {
         "roleCredentials": RoleCredentialsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "accessToken": str,
+        "accountId": str,
+    },
+)
+_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef = TypedDict(
+    "_OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
     },
+    total=False,
 )
 
+class ListAccountRolesRequestListAccountRolesPaginateTypeDef(
+    _RequiredListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    _OptionalListAccountRolesRequestListAccountRolesPaginateTypeDef,
+):
+    pass
+
+_RequiredListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_RequiredListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "accessToken": str,
+    },
+)
+_OptionalListAccountsRequestListAccountsPaginateTypeDef = TypedDict(
+    "_OptionalListAccountsRequestListAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListAccountsRequestListAccountsPaginateTypeDef(
+    _RequiredListAccountsRequestListAccountsPaginateTypeDef,
+    _OptionalListAccountsRequestListAccountsPaginateTypeDef,
+):
+    pass
+
 ListAccountRolesResponseTypeDef = TypedDict(
     "ListAccountRolesResponseTypeDef",
     {
         "nextToken": str,
         "roleList": List[RoleInfoTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/PKG-INFO` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sso
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SSO 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sso type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sso type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sso"></a>
 
 # types-aiobotocore-sso
 
 [![PyPI - types-aiobotocore-sso](https://img.shields.io/pypi/v/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sso.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sso)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sso?color=blue)](https://pypistats.org/packages/types-aiobotocore-sso)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sso)](https://pepy.tech/project/types-aiobotocore-sso)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SSO 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sso.html#SSO)
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
 [types-aiobotocore-sso docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sso/).
 
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
@@ -307,42 +306,42 @@
 )
 
 
 def check_value(value: ListAccountRolesPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sso.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sso.type_defs import (
     AccountInfoTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetRoleCredentialsRequestRequestTypeDef,
     RoleCredentialsTypeDef,
-    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListAccountRolesRequestRequestTypeDef,
     RoleInfoTypeDef,
-    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountsRequestRequestTypeDef,
     LogoutRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListAccountsResponseTypeDef,
     GetRoleCredentialsResponseTypeDef,
+    ListAccountRolesRequestListAccountRolesPaginateTypeDef,
+    ListAccountsRequestListAccountsPaginateTypeDef,
     ListAccountRolesResponseTypeDef,
 )
 
 
-def get_structure() -> AccountInfoTypeDef:
+def get_value() -> AccountInfoTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sso-2.5.2/types_aiobotocore_sso.egg-info/SOURCES.txt` & `types-aiobotocore-sso-2.5.2.post1/types_aiobotocore_sso.egg-info/SOURCES.txt`

 * *Files identical despite different names*


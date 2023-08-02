# Comparing `tmp/types-aiobotocore-account-2.5.2.tar.gz` & `tmp/types-aiobotocore-account-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-account-2.5.2.tar", last modified: Sat Jul  8 01:43:09 2023, max compression
+gzip compressed data, was "types-aiobotocore-account-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:47 2023, max compression
```

## Comparing `types-aiobotocore-account-2.5.2.tar` & `types-aiobotocore-account-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.821605 types-aiobotocore-account-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-08 01:43:09.821605 types-aiobotocore-account-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12016 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:09.821605 types-aiobotocore-account-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.821605 types-aiobotocore-account-2.5.2/types_aiobotocore_account/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-07-08 01:25:15.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:14.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:09.821605 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-08 01:43:09.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-08 01:43:09.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:09.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:09.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 01:43:09.000000 types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.845667 types-aiobotocore-account-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-08-02 14:51:47.825667 types-aiobotocore-account-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:47.845667 types-aiobotocore-account-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.825667 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8380 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:32:41.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:47.825667 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13517 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 14:51:47.000000 types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-account-2.5.2/LICENSE` & `types-aiobotocore-account-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/PKG-INFO` & `types-aiobotocore-account-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-account
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore account type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore account type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-account"></a>
 
 # types-aiobotocore-account
 
 [![PyPI - types-aiobotocore-account](https://img.shields.io/pypi/v/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-account?color=blue)](https://pypistats.org/packages/types-aiobotocore-account)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-account)](https://pepy.tech/project/types-aiobotocore-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Account 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
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
@@ -305,20 +304,20 @@
 )
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_account.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_account.type_defs import (
     AlternateContactTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
@@ -337,15 +336,15 @@
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
     ListRegionsRequestListRegionsPaginateTypeDef,
     ListRegionsResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateContactTypeDef:
+def get_value() -> AlternateContactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-account-2.5.2/README.md` & `types-aiobotocore-account-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-account"></a>
 
 # types-aiobotocore-account
 
 [![PyPI - types-aiobotocore-account](https://img.shields.io/pypi/v/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-account?color=blue)](https://pypistats.org/packages/types-aiobotocore-account)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-account)](https://pepy.tech/project/types-aiobotocore-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Account 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
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
@@ -272,20 +272,20 @@
 )
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_account.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_account.type_defs import (
     AlternateContactTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
@@ -304,15 +304,15 @@
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
     ListRegionsRequestListRegionsPaginateTypeDef,
     ListRegionsResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateContactTypeDef:
+def get_value() -> AlternateContactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-account-2.5.2/setup.py` & `types-aiobotocore-account-2.5.2.post1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-account",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_account"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore account type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore account type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_account": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/"
```

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/__init__.py` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/__init__.pyi` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/__main__.py` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Account 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Account 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account//\nBoto3 docs:"
         "     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account\nOther"
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

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/client.py` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/client.pyi` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/literals.py` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/literals.pyi` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/paginator.py` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/paginator.pyi` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/paginator.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/type_defs.py` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_account.type_defs import AlternateContactTypeDef
 
-    data: AlternateContactTypeDef = {...}
+    data: AlternateContactTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import AlternateContactTypeType, RegionOptStatusType
```

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account/type_defs.pyi` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_account.type_defs import AlternateContactTypeDef
 
-    data: AlternateContactTypeDef = {...}
+    data: AlternateContactTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import AlternateContactTypeType, RegionOptStatusType
```

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/PKG-INFO` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-account
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Account 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore account type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore account type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-account"></a>
 
 # types-aiobotocore-account
 
 [![PyPI - types-aiobotocore-account](https://img.shields.io/pypi/v/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-account.svg?color=blue)](https://pypi.org/project/types-aiobotocore-account)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-account?color=blue)](https://pypistats.org/packages/types-aiobotocore-account)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-account)](https://pepy.tech/project/types-aiobotocore-account)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Account 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/account.html#Account)
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
 [types-aiobotocore-account docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_account/).
 
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
@@ -305,20 +304,20 @@
 )
 
 
 def check_value(value: AlternateContactTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_account.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_account.type_defs import (
     AlternateContactTypeDef,
     ContactInformationTypeDef,
     DeleteAlternateContactRequestRequestTypeDef,
     DisableRegionRequestRequestTypeDef,
@@ -337,15 +336,15 @@
     GetContactInformationResponseTypeDef,
     GetRegionOptStatusResponseTypeDef,
     ListRegionsRequestListRegionsPaginateTypeDef,
     ListRegionsResponseTypeDef,
 )
 
 
-def get_structure() -> AlternateContactTypeDef:
+def get_value() -> AlternateContactTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-account-2.5.2/types_aiobotocore_account.egg-info/SOURCES.txt` & `types-aiobotocore-account-2.5.2.post1/types_aiobotocore_account.egg-info/SOURCES.txt`

 * *Files identical despite different names*


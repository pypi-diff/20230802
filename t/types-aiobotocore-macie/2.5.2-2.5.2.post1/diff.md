# Comparing `tmp/types-aiobotocore-macie-2.5.2.tar.gz` & `tmp/types-aiobotocore-macie-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-macie-2.5.2.tar", last modified: Sat Jul  8 01:43:56 2023, max compression
+gzip compressed data, was "types-aiobotocore-macie-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:36 2023, max compression
```

## Comparing `types-aiobotocore-macie-2.5.2.tar` & `types-aiobotocore-macie-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.998477 types-aiobotocore-macie-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-07-08 01:43:55.994477 types-aiobotocore-macie-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:55.998477 types-aiobotocore-macie-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.994477 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-07-08 01:34:31.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-07-08 01:34:31.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-08 01:34:31.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-07-08 01:34:31.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:34:30.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:55.994477 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13943 2023-07-08 01:43:55.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-08 01:43:55.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:55.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:55.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 01:43:55.000000 types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.781530 types-aiobotocore-macie-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-08-02 14:52:36.773531 types-aiobotocore-macie-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:36.781530 types-aiobotocore-macie-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.773531 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9616 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-08-02 14:42:42.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8093 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8365 2023-08-02 14:42:42.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8352 2023-08-02 14:42:42.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:42:41.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:36.773531 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13879 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 14:52:36.000000 types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-macie-2.5.2/LICENSE` & `types-aiobotocore-macie-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/PKG-INFO` & `types-aiobotocore-macie-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore macie type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore macie type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-macie"></a>
 
 # types-aiobotocore-macie
 
 [![PyPI - types-aiobotocore-macie](https://img.shields.io/pypi/v/types-aiobotocore-macie.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-macie?color=blue)](https://pypistats.org/packages/types-aiobotocore-macie)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie)](https://pepy.tech/project/types-aiobotocore-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Macie 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [types-aiobotocore-macie docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/).
 
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
@@ -311,51 +310,51 @@
 )
 
 
 def check_value(value: ListMemberAccountsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_macie.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
 
 
-def get_structure() -> AssociateMemberAccountRequestRequestTypeDef:
+def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-macie-2.5.2/README.md` & `types-aiobotocore-macie-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-macie"></a>
 
 # types-aiobotocore-macie
 
 [![PyPI - types-aiobotocore-macie](https://img.shields.io/pypi/v/types-aiobotocore-macie.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-macie?color=blue)](https://pypistats.org/packages/types-aiobotocore-macie)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie)](https://pepy.tech/project/types-aiobotocore-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Macie 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [types-aiobotocore-macie docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/).
 
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
@@ -278,51 +278,51 @@
 )
 
 
 def check_value(value: ListMemberAccountsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_macie.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
 
 
-def get_structure() -> AssociateMemberAccountRequestRequestTypeDef:
+def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-macie-2.5.2/setup.py` & `types-aiobotocore-macie-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-macie",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_macie"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore macie type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore macie type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_macie": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/"
```

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/__init__.py` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/__init__.pyi` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/__main__.py` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Macie 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Macie 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie//\nBoto3 docs:  "
         "    https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie\nOther"
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

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/client.py` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/client.pyi` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/literals.py` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/literals.pyi` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/paginator.py` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,28 +49,28 @@
 class ListMemberAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMemberAccountsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#listmemberaccountspaginator)
         """
 
 
 class ListS3ResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#lists3resourcespaginator)
     """
 
     def paginate(
-        self, *, memberAccountId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, memberAccountId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListS3ResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#lists3resourcespaginator)
         """
```

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/paginator.pyi` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/paginator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -46,27 +46,27 @@
 class ListMemberAccountsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#listmemberaccountspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListMemberAccountsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListMemberAccounts.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#listmemberaccountspaginator)
         """
 
 class ListS3ResourcesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#lists3resourcespaginator)
     """
 
     def paginate(
-        self, *, memberAccountId: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, memberAccountId: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListS3ResourcesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie.Paginator.ListS3Resources.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/paginators/#lists3resourcespaginator)
         """
```

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/type_defs.py` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef
 
-    data: AssociateMemberAccountRequestRequestTypeDef = {...}
+    data: AssociateMemberAccountRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import S3OneTimeClassificationTypeType
 
@@ -24,30 +24,30 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListMemberAccountsResultTypeDef",
     "AssociateS3ResourcesRequestRequestTypeDef",
     "ListS3ResourcesResultTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
@@ -56,14 +56,25 @@
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
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
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
         "continuous": Literal["FULL"],
     },
 )
@@ -99,25 +110,20 @@
 )
 
 
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
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
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
@@ -131,51 +137,28 @@
     "MemberAccountTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
-    {
-        "memberAccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListS3ResourcesRequestRequestTypeDef = TypedDict(
     "ListS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
         "nextToken": str,
         "maxResults": int,
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
 
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
@@ -247,20 +230,37 @@
         "failedItem": S3ResourceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
+    {
+        "memberAccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListMemberAccountsResultTypeDef = TypedDict(
     "ListMemberAccountsResultTypeDef",
     {
         "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
@@ -283,15 +283,15 @@
 
 
 ListS3ResourcesResultTypeDef = TypedDict(
     "ListS3ResourcesResultTypeDef",
     {
         "s3Resources": List[S3ResourceClassificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
@@ -312,26 +312,26 @@
     pass
 
 
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateS3ResourcesResultTypeDef = TypedDict(
     "DisassociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateS3ResourcesResultTypeDef = TypedDict(
     "UpdateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie/type_defs.pyi` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_macie.type_defs import AssociateMemberAccountRequestRequestTypeDef
 
-    data: AssociateMemberAccountRequestRequestTypeDef = {...}
+    data: AssociateMemberAccountRequestRequestTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 from .literals import S3OneTimeClassificationTypeType
 
@@ -23,30 +23,30 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "AssociateMemberAccountRequestRequestTypeDef",
+    "ResponseMetadataTypeDef",
     "ClassificationTypeTypeDef",
     "ClassificationTypeUpdateTypeDef",
     "DisassociateMemberAccountRequestRequestTypeDef",
     "S3ResourceTypeDef",
-    "EmptyResponseMetadataTypeDef",
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListMemberAccountsRequestRequestTypeDef",
     "MemberAccountTypeDef",
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListS3ResourcesRequestRequestTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "S3ResourceClassificationTypeDef",
     "S3ResourceClassificationUpdateTypeDef",
     "DisassociateS3ResourcesRequestRequestTypeDef",
     "FailedS3ResourceTypeDef",
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
     "ListMemberAccountsResultTypeDef",
     "AssociateS3ResourcesRequestRequestTypeDef",
     "ListS3ResourcesResultTypeDef",
     "UpdateS3ResourcesRequestRequestTypeDef",
     "AssociateS3ResourcesResultTypeDef",
     "DisassociateS3ResourcesResultTypeDef",
     "UpdateS3ResourcesResultTypeDef",
@@ -55,14 +55,25 @@
 AssociateMemberAccountRequestRequestTypeDef = TypedDict(
     "AssociateMemberAccountRequestRequestTypeDef",
     {
         "memberAccountId": str,
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
 ClassificationTypeTypeDef = TypedDict(
     "ClassificationTypeTypeDef",
     {
         "oneTime": S3OneTimeClassificationTypeType,
         "continuous": Literal["FULL"],
     },
 )
@@ -96,25 +107,20 @@
     },
     total=False,
 )
 
 class S3ResourceTypeDef(_RequiredS3ResourceTypeDef, _OptionalS3ResourceTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
-    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
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
 
 ListMemberAccountsRequestRequestTypeDef = TypedDict(
     "ListMemberAccountsRequestRequestTypeDef",
     {
@@ -128,51 +134,28 @@
     "MemberAccountTypeDef",
     {
         "accountId": str,
     },
     total=False,
 )
 
-ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
-    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
-    {
-        "memberAccountId": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListS3ResourcesRequestRequestTypeDef = TypedDict(
     "ListS3ResourcesRequestRequestTypeDef",
     {
         "memberAccountId": str,
         "nextToken": str,
         "maxResults": int,
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
 
 _RequiredS3ResourceClassificationTypeDef = TypedDict(
     "_RequiredS3ResourceClassificationTypeDef",
     {
         "bucketName": str,
@@ -238,20 +221,37 @@
         "failedItem": S3ResourceTypeDef,
         "errorCode": str,
         "errorMessage": str,
     },
     total=False,
 )
 
+ListMemberAccountsRequestListMemberAccountsPaginateTypeDef = TypedDict(
+    "ListMemberAccountsRequestListMemberAccountsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListS3ResourcesRequestListS3ResourcesPaginateTypeDef = TypedDict(
+    "ListS3ResourcesRequestListS3ResourcesPaginateTypeDef",
+    {
+        "memberAccountId": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListMemberAccountsResultTypeDef = TypedDict(
     "ListMemberAccountsResultTypeDef",
     {
         "memberAccounts": List[MemberAccountTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAssociateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredAssociateS3ResourcesRequestRequestTypeDef",
     {
         "s3Resources": Sequence[S3ResourceClassificationTypeDef],
@@ -272,15 +272,15 @@
     pass
 
 ListS3ResourcesResultTypeDef = TypedDict(
     "ListS3ResourcesResultTypeDef",
     {
         "s3Resources": List[S3ResourceClassificationTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredUpdateS3ResourcesRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateS3ResourcesRequestRequestTypeDef",
     {
         "s3ResourcesUpdate": Sequence[S3ResourceClassificationUpdateTypeDef],
@@ -299,26 +299,26 @@
 ):
     pass
 
 AssociateS3ResourcesResultTypeDef = TypedDict(
     "AssociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DisassociateS3ResourcesResultTypeDef = TypedDict(
     "DisassociateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateS3ResourcesResultTypeDef = TypedDict(
     "UpdateS3ResourcesResultTypeDef",
     {
         "failedS3Resources": List[FailedS3ResourceTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/PKG-INFO` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-macie
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Macie 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore macie type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore macie type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-macie"></a>
 
 # types-aiobotocore-macie
 
 [![PyPI - types-aiobotocore-macie](https://img.shields.io/pypi/v/types-aiobotocore-macie.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-macie.svg?color=blue)](https://pypi.org/project/types-aiobotocore-macie)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-macie?color=blue)](https://pypistats.org/packages/types-aiobotocore-macie)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-macie)](https://pepy.tech/project/types-aiobotocore-macie)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Macie 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/macie.html#Macie)
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
 [types-aiobotocore-macie docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_macie/).
 
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
@@ -311,51 +310,51 @@
 )
 
 
 def check_value(value: ListMemberAccountsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_macie.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_macie.type_defs import (
     AssociateMemberAccountRequestRequestTypeDef,
+    ResponseMetadataTypeDef,
     ClassificationTypeTypeDef,
     ClassificationTypeUpdateTypeDef,
     DisassociateMemberAccountRequestRequestTypeDef,
     S3ResourceTypeDef,
-    EmptyResponseMetadataTypeDef,
-    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListMemberAccountsRequestRequestTypeDef,
     MemberAccountTypeDef,
-    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListS3ResourcesRequestRequestTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    EmptyResponseMetadataTypeDef,
     S3ResourceClassificationTypeDef,
     S3ResourceClassificationUpdateTypeDef,
     DisassociateS3ResourcesRequestRequestTypeDef,
     FailedS3ResourceTypeDef,
+    ListMemberAccountsRequestListMemberAccountsPaginateTypeDef,
+    ListS3ResourcesRequestListS3ResourcesPaginateTypeDef,
     ListMemberAccountsResultTypeDef,
     AssociateS3ResourcesRequestRequestTypeDef,
     ListS3ResourcesResultTypeDef,
     UpdateS3ResourcesRequestRequestTypeDef,
     AssociateS3ResourcesResultTypeDef,
     DisassociateS3ResourcesResultTypeDef,
     UpdateS3ResourcesResultTypeDef,
 )
 
 
-def get_structure() -> AssociateMemberAccountRequestRequestTypeDef:
+def get_value() -> AssociateMemberAccountRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-macie-2.5.2/types_aiobotocore_macie.egg-info/SOURCES.txt` & `types-aiobotocore-macie-2.5.2.post1/types_aiobotocore_macie.egg-info/SOURCES.txt`

 * *Files identical despite different names*


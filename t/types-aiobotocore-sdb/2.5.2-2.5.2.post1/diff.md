# Comparing `tmp/types-aiobotocore-sdb-2.5.2.tar.gz` & `tmp/types-aiobotocore-sdb-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-sdb-2.5.2.tar", last modified: Sat Jul  8 01:44:17 2023, max compression
+gzip compressed data, was "types-aiobotocore-sdb-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:59 2023, max compression
```

## Comparing `types-aiobotocore-sdb-2.5.2.tar` & `types-aiobotocore-sdb-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.586872 types-aiobotocore-sdb-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-08 01:44:17.586872 types-aiobotocore-sdb-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12007 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:17.586872 types-aiobotocore-sdb-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.586872 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-07-08 01:40:30.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8647 2023-07-08 01:40:30.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:40:29.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:17.586872 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-08 01:44:17.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-08 01:44:17.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:17.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:17.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-08 01:44:17.000000 types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.289462 types-aiobotocore-sdb-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-08-02 14:52:59.281462 types-aiobotocore-sdb-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:59.289462 types-aiobotocore-sdb-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-08-02 14:49:04.000000 types-aiobotocore-sdb-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.277462 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11682 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7937 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-08-02 14:49:08.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:49:05.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:59.281462 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13497 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 14:52:59.000000 types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-sdb-2.5.2/LICENSE` & `types-aiobotocore-sdb-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/PKG-INFO` & `types-aiobotocore-sdb-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sdb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sdb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sdb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sdb"></a>
 
 # types-aiobotocore-sdb
 
 [![PyPI - types-aiobotocore-sdb](https://img.shields.io/pypi/v/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sdb?color=blue)](https://pypistats.org/packages/types-aiobotocore-sdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sdb)](https://pepy.tech/project/types-aiobotocore-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SimpleDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [types-aiobotocore-sdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/).
 
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
@@ -305,52 +304,52 @@
 )
 
 
 def check_value(value: ListDomainsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sdb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sdb.type_defs import (
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListDomainsResultTypeDef,
     PaginatorConfigTypeDef,
+    ListDomainsRequestRequestTypeDef,
     ReplaceableAttributeTypeDef,
-    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
-    SelectRequestSelectPaginateTypeDef,
     DeletableItemTypeDef,
-    GetAttributesResultTypeDef,
     ItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributesResultTypeDef,
+    ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
     BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sdb-2.5.2/README.md` & `types-aiobotocore-sdb-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-sdb"></a>
 
 # types-aiobotocore-sdb
 
 [![PyPI - types-aiobotocore-sdb](https://img.shields.io/pypi/v/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sdb?color=blue)](https://pypistats.org/packages/types-aiobotocore-sdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sdb)](https://pepy.tech/project/types-aiobotocore-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SimpleDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [types-aiobotocore-sdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/).
 
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
@@ -272,52 +272,52 @@
 )
 
 
 def check_value(value: ListDomainsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sdb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sdb.type_defs import (
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListDomainsResultTypeDef,
     PaginatorConfigTypeDef,
+    ListDomainsRequestRequestTypeDef,
     ReplaceableAttributeTypeDef,
-    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
-    SelectRequestSelectPaginateTypeDef,
     DeletableItemTypeDef,
-    GetAttributesResultTypeDef,
     ItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributesResultTypeDef,
+    ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
     BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sdb-2.5.2/setup.py` & `types-aiobotocore-sdb-2.5.2.post1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-sdb",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_sdb"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore sdb type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore sdb type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_sdb": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
```

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/__init__.py` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/__init__.pyi` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/__main__.py` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.SimpleDB 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.SimpleDB 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB\nOther"
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

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/client.py` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/client.pyi` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/literals.py` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/literals.pyi` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/paginator.py` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -27,50 +27,46 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListDomainsResultTypeDef, PaginatorConfigTypeDef, SelectResultTypeDef
 
 __all__ = ("ListDomainsPaginator", "SelectPaginator")
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#listdomainspaginator)
         """
 
-
 class SelectPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#selectpaginator)
     """
 
     def paginate(
         self,
         *,
         SelectExpression: str,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SelectResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#selectpaginator)
         """
```

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/paginator.pyi` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/paginator.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,46 +27,50 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListDomainsResultTypeDef, PaginatorConfigTypeDef, SelectResultTypeDef
 
 __all__ = ("ListDomainsPaginator", "SelectPaginator")
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListDomainsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#listdomainspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDomainsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.ListDomains.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#listdomainspaginator)
         """
 
+
 class SelectPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#selectpaginator)
     """
 
     def paginate(
         self,
         *,
         SelectExpression: str,
         ConsistentRead: bool = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[SelectResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB.Paginator.Select.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/paginators/#selectpaginator)
         """
```

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/type_defs.py` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sdb.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -22,29 +22,29 @@
 
 __all__ = (
     "AttributeTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateConditionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainMetadataRequestRequestTypeDef",
-    "DomainMetadataResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetAttributesRequestRequestTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListDomainsRequestRequestTypeDef",
-    "ListDomainsResultTypeDef",
     "PaginatorConfigTypeDef",
+    "ListDomainsRequestRequestTypeDef",
     "ReplaceableAttributeTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectRequestRequestTypeDef",
-    "SelectRequestSelectPaginateTypeDef",
     "DeletableItemTypeDef",
-    "GetAttributesResultTypeDef",
     "ItemTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
+    "DomainMetadataResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributesResultTypeDef",
+    "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "SelectRequestSelectPaginateTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "ReplaceableItemTypeDef",
     "BatchDeleteAttributesRequestRequestTypeDef",
     "SelectResultTypeDef",
     "BatchPutAttributesRequestRequestTypeDef",
 )
 
@@ -96,32 +96,22 @@
 DomainMetadataRequestRequestTypeDef = TypedDict(
     "DomainMetadataRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DomainMetadataResultTypeDef = TypedDict(
-    "DomainMetadataResultTypeDef",
-    {
-        "ItemCount": int,
-        "ItemNamesSizeBytes": int,
-        "AttributeNameCount": int,
-        "AttributeNamesSizeBytes": int,
-        "AttributeValueCount": int,
-        "AttributeValuesSizeBytes": int,
-        "Timestamp": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 _RequiredGetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -140,50 +130,33 @@
 
 class GetAttributesRequestRequestTypeDef(
     _RequiredGetAttributesRequestRequestTypeDef, _OptionalGetAttributesRequestRequestTypeDef
 ):
     pass
 
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxNumberOfDomains": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDomainsResultTypeDef = TypedDict(
-    "ListDomainsResultTypeDef",
-    {
-        "DomainNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredReplaceableAttributeTypeDef = TypedDict(
     "_RequiredReplaceableAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -198,25 +171,14 @@
 
 class ReplaceableAttributeTypeDef(
     _RequiredReplaceableAttributeTypeDef, _OptionalReplaceableAttributeTypeDef
 ):
     pass
 
 
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
 _RequiredSelectRequestRequestTypeDef = TypedDict(
     "_RequiredSelectRequestRequestTypeDef",
     {
         "SelectExpression": str,
     },
 )
 _OptionalSelectRequestRequestTypeDef = TypedDict(
@@ -231,36 +193,14 @@
 
 class SelectRequestRequestTypeDef(
     _RequiredSelectRequestRequestTypeDef, _OptionalSelectRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_RequiredSelectRequestSelectPaginateTypeDef",
-    {
-        "SelectExpression": str,
-    },
-)
-_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_OptionalSelectRequestSelectPaginateTypeDef",
-    {
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class SelectRequestSelectPaginateTypeDef(
-    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
-):
-    pass
-
-
 _RequiredDeletableItemTypeDef = TypedDict(
     "_RequiredDeletableItemTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeletableItemTypeDef = TypedDict(
@@ -272,22 +212,14 @@
 )
 
 
 class DeletableItemTypeDef(_RequiredDeletableItemTypeDef, _OptionalDeletableItemTypeDef):
     pass
 
 
-GetAttributesResultTypeDef = TypedDict(
-    "GetAttributesResultTypeDef",
-    {
-        "Attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredItemTypeDef = TypedDict(
     "_RequiredItemTypeDef",
     {
         "Name": str,
         "Attributes": List[AttributeTypeDef],
     },
 )
@@ -323,14 +255,82 @@
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
 
+DomainMetadataResultTypeDef = TypedDict(
+    "DomainMetadataResultTypeDef",
+    {
+        "ItemCount": int,
+        "ItemNamesSizeBytes": int,
+        "AttributeNameCount": int,
+        "AttributeNamesSizeBytes": int,
+        "AttributeValueCount": int,
+        "AttributeValuesSizeBytes": int,
+        "Timestamp": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAttributesResultTypeDef = TypedDict(
+    "GetAttributesResultTypeDef",
+    {
+        "Attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsResultTypeDef = TypedDict(
+    "ListDomainsResultTypeDef",
+    {
+        "DomainNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_RequiredSelectRequestSelectPaginateTypeDef",
+    {
+        "SelectExpression": str,
+    },
+)
+_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_OptionalSelectRequestSelectPaginateTypeDef",
+    {
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class SelectRequestSelectPaginateTypeDef(
+    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
+):
+    pass
+
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
         "ItemName": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
@@ -367,15 +367,15 @@
 )
 
 SelectResultTypeDef = TypedDict(
     "SelectResultTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutAttributesRequestRequestTypeDef = TypedDict(
     "BatchPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
```

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb/type_defs.pyi` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_sdb.type_defs import AttributeTypeDef
 
-    data: AttributeTypeDef = {...}
+    data: AttributeTypeDef = ...
     ```
 """
 import sys
 from typing import Dict, List, Sequence
 
 if sys.version_info >= (3, 9):
     from typing import TypedDict
@@ -21,29 +21,29 @@
 
 __all__ = (
     "AttributeTypeDef",
     "CreateDomainRequestRequestTypeDef",
     "UpdateConditionTypeDef",
     "DeleteDomainRequestRequestTypeDef",
     "DomainMetadataRequestRequestTypeDef",
-    "DomainMetadataResultTypeDef",
-    "EmptyResponseMetadataTypeDef",
+    "ResponseMetadataTypeDef",
     "GetAttributesRequestRequestTypeDef",
-    "ListDomainsRequestListDomainsPaginateTypeDef",
-    "ListDomainsRequestRequestTypeDef",
-    "ListDomainsResultTypeDef",
     "PaginatorConfigTypeDef",
+    "ListDomainsRequestRequestTypeDef",
     "ReplaceableAttributeTypeDef",
-    "ResponseMetadataTypeDef",
     "SelectRequestRequestTypeDef",
-    "SelectRequestSelectPaginateTypeDef",
     "DeletableItemTypeDef",
-    "GetAttributesResultTypeDef",
     "ItemTypeDef",
     "DeleteAttributesRequestRequestTypeDef",
+    "DomainMetadataResultTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetAttributesResultTypeDef",
+    "ListDomainsResultTypeDef",
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    "SelectRequestSelectPaginateTypeDef",
     "PutAttributesRequestRequestTypeDef",
     "ReplaceableItemTypeDef",
     "BatchDeleteAttributesRequestRequestTypeDef",
     "SelectResultTypeDef",
     "BatchPutAttributesRequestRequestTypeDef",
 )
 
@@ -93,32 +93,22 @@
 DomainMetadataRequestRequestTypeDef = TypedDict(
     "DomainMetadataRequestRequestTypeDef",
     {
         "DomainName": str,
     },
 )
 
-DomainMetadataResultTypeDef = TypedDict(
-    "DomainMetadataResultTypeDef",
-    {
-        "ItemCount": int,
-        "ItemNamesSizeBytes": int,
-        "AttributeNameCount": int,
-        "AttributeNamesSizeBytes": int,
-        "AttributeValueCount": int,
-        "AttributeValuesSizeBytes": int,
-        "Timestamp": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 
 _RequiredGetAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredGetAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
@@ -135,50 +125,33 @@
 )
 
 class GetAttributesRequestRequestTypeDef(
     _RequiredGetAttributesRequestRequestTypeDef, _OptionalGetAttributesRequestRequestTypeDef
 ):
     pass
 
-ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
-    "ListDomainsRequestListDomainsPaginateTypeDef",
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
 
 ListDomainsRequestRequestTypeDef = TypedDict(
     "ListDomainsRequestRequestTypeDef",
     {
         "MaxNumberOfDomains": int,
         "NextToken": str,
     },
     total=False,
 )
 
-ListDomainsResultTypeDef = TypedDict(
-    "ListDomainsResultTypeDef",
-    {
-        "DomainNames": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
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
 _RequiredReplaceableAttributeTypeDef = TypedDict(
     "_RequiredReplaceableAttributeTypeDef",
     {
         "Name": str,
         "Value": str,
     },
 )
@@ -191,25 +164,14 @@
 )
 
 class ReplaceableAttributeTypeDef(
     _RequiredReplaceableAttributeTypeDef, _OptionalReplaceableAttributeTypeDef
 ):
     pass
 
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
 _RequiredSelectRequestRequestTypeDef = TypedDict(
     "_RequiredSelectRequestRequestTypeDef",
     {
         "SelectExpression": str,
     },
 )
 _OptionalSelectRequestRequestTypeDef = TypedDict(
@@ -222,34 +184,14 @@
 )
 
 class SelectRequestRequestTypeDef(
     _RequiredSelectRequestRequestTypeDef, _OptionalSelectRequestRequestTypeDef
 ):
     pass
 
-_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_RequiredSelectRequestSelectPaginateTypeDef",
-    {
-        "SelectExpression": str,
-    },
-)
-_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
-    "_OptionalSelectRequestSelectPaginateTypeDef",
-    {
-        "ConsistentRead": bool,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class SelectRequestSelectPaginateTypeDef(
-    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
-):
-    pass
-
 _RequiredDeletableItemTypeDef = TypedDict(
     "_RequiredDeletableItemTypeDef",
     {
         "Name": str,
     },
 )
 _OptionalDeletableItemTypeDef = TypedDict(
@@ -259,22 +201,14 @@
     },
     total=False,
 )
 
 class DeletableItemTypeDef(_RequiredDeletableItemTypeDef, _OptionalDeletableItemTypeDef):
     pass
 
-GetAttributesResultTypeDef = TypedDict(
-    "GetAttributesResultTypeDef",
-    {
-        "Attributes": List[AttributeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredItemTypeDef = TypedDict(
     "_RequiredItemTypeDef",
     {
         "Name": str,
         "Attributes": List[AttributeTypeDef],
     },
 )
@@ -306,14 +240,80 @@
 )
 
 class DeleteAttributesRequestRequestTypeDef(
     _RequiredDeleteAttributesRequestRequestTypeDef, _OptionalDeleteAttributesRequestRequestTypeDef
 ):
     pass
 
+DomainMetadataResultTypeDef = TypedDict(
+    "DomainMetadataResultTypeDef",
+    {
+        "ItemCount": int,
+        "ItemNamesSizeBytes": int,
+        "AttributeNameCount": int,
+        "AttributeNamesSizeBytes": int,
+        "AttributeValueCount": int,
+        "AttributeValuesSizeBytes": int,
+        "Timestamp": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetAttributesResultTypeDef = TypedDict(
+    "GetAttributesResultTypeDef",
+    {
+        "Attributes": List[AttributeTypeDef],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsResultTypeDef = TypedDict(
+    "ListDomainsResultTypeDef",
+    {
+        "DomainNames": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDomainsRequestListDomainsPaginateTypeDef = TypedDict(
+    "ListDomainsRequestListDomainsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_RequiredSelectRequestSelectPaginateTypeDef",
+    {
+        "SelectExpression": str,
+    },
+)
+_OptionalSelectRequestSelectPaginateTypeDef = TypedDict(
+    "_OptionalSelectRequestSelectPaginateTypeDef",
+    {
+        "ConsistentRead": bool,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class SelectRequestSelectPaginateTypeDef(
+    _RequiredSelectRequestSelectPaginateTypeDef, _OptionalSelectRequestSelectPaginateTypeDef
+):
+    pass
+
 _RequiredPutAttributesRequestRequestTypeDef = TypedDict(
     "_RequiredPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
         "ItemName": str,
         "Attributes": Sequence[ReplaceableAttributeTypeDef],
     },
@@ -348,15 +348,15 @@
 )
 
 SelectResultTypeDef = TypedDict(
     "SelectResultTypeDef",
     {
         "Items": List[ItemTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchPutAttributesRequestRequestTypeDef = TypedDict(
     "BatchPutAttributesRequestRequestTypeDef",
     {
         "DomainName": str,
```

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/PKG-INFO` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-sdb
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.SimpleDB 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore sdb type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore sdb type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-sdb"></a>
 
 # types-aiobotocore-sdb
 
 [![PyPI - types-aiobotocore-sdb](https://img.shields.io/pypi/v/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-sdb.svg?color=blue)](https://pypi.org/project/types-aiobotocore-sdb)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-sdb?color=blue)](https://pypistats.org/packages/types-aiobotocore-sdb)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-sdb)](https://pepy.tech/project/types-aiobotocore-sdb)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.SimpleDB 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/sdb.html#SimpleDB)
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
 [types-aiobotocore-sdb docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_sdb/).
 
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
@@ -305,52 +304,52 @@
 )
 
 
 def check_value(value: ListDomainsPaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_sdb.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_sdb.type_defs import (
     AttributeTypeDef,
     CreateDomainRequestRequestTypeDef,
     UpdateConditionTypeDef,
     DeleteDomainRequestRequestTypeDef,
     DomainMetadataRequestRequestTypeDef,
-    DomainMetadataResultTypeDef,
-    EmptyResponseMetadataTypeDef,
+    ResponseMetadataTypeDef,
     GetAttributesRequestRequestTypeDef,
-    ListDomainsRequestListDomainsPaginateTypeDef,
-    ListDomainsRequestRequestTypeDef,
-    ListDomainsResultTypeDef,
     PaginatorConfigTypeDef,
+    ListDomainsRequestRequestTypeDef,
     ReplaceableAttributeTypeDef,
-    ResponseMetadataTypeDef,
     SelectRequestRequestTypeDef,
-    SelectRequestSelectPaginateTypeDef,
     DeletableItemTypeDef,
-    GetAttributesResultTypeDef,
     ItemTypeDef,
     DeleteAttributesRequestRequestTypeDef,
+    DomainMetadataResultTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetAttributesResultTypeDef,
+    ListDomainsResultTypeDef,
+    ListDomainsRequestListDomainsPaginateTypeDef,
+    SelectRequestSelectPaginateTypeDef,
     PutAttributesRequestRequestTypeDef,
     ReplaceableItemTypeDef,
     BatchDeleteAttributesRequestRequestTypeDef,
     SelectResultTypeDef,
     BatchPutAttributesRequestRequestTypeDef,
 )
 
 
-def get_structure() -> AttributeTypeDef:
+def get_value() -> AttributeTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-sdb-2.5.2/types_aiobotocore_sdb.egg-info/SOURCES.txt` & `types-aiobotocore-sdb-2.5.2.post1/types_aiobotocore_sdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/types-aiobotocore-redshift-data-2.5.2.tar.gz` & `tmp/types-aiobotocore-redshift-data-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-redshift-data-2.5.2.tar", last modified: Sat Jul  8 01:44:10 2023, max compression
+gzip compressed data, was "types-aiobotocore-redshift-data-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:51 2023, max compression
```

## Comparing `types-aiobotocore-redshift-data-2.5.2.tar` & `types-aiobotocore-redshift-data-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:10.726751 types-aiobotocore-redshift-data-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-data-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-07-08 01:44:10.726751 types-aiobotocore-redshift-data-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13764 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-data-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:10.726751 types-aiobotocore-redshift-data-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-data-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:10.726751 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8735 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16736 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16707 2023-07-08 01:39:05.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:39:04.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:10.726751 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-07-08 01:44:10.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 01:44:10.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:10.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:10.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:10.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-08 01:44:10.000000 types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.893485 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15175 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8582 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16673 2023-08-02 14:47:43.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:47:40.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:51.897485 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 14:52:51.000000 types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/LICENSE` & `types-aiobotocore-redshift-data-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/PKG-INFO` & `types-aiobotocore-redshift-data-2.5.2.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-data
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore redshift-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-data)](https://pepy.tech/project/types-aiobotocore-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RedshiftDataAPIService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
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
@@ -325,61 +324,61 @@
 )
 
 
 def check_value(value: DescribeTablePaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    BatchExecuteStatementOutputTypeDef,
+    ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
-    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
     SqlParameterTypeDef,
     SubStatementDataTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    ExecuteStatementOutputTypeDef,
     FieldTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
-    ListSchemasResponseTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    CancelStatementResponseTypeDef,
+    ExecuteStatementOutputTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
     ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
-def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
+def get_value() -> BatchExecuteStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/README.md` & `types-aiobotocore-redshift-data-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-data)](https://pepy.tech/project/types-aiobotocore-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RedshiftDataAPIService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
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
@@ -292,61 +292,61 @@
 )
 
 
 def check_value(value: DescribeTablePaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    BatchExecuteStatementOutputTypeDef,
+    ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
-    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
     SqlParameterTypeDef,
     SubStatementDataTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    ExecuteStatementOutputTypeDef,
     FieldTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
-    ListSchemasResponseTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    CancelStatementResponseTypeDef,
+    ExecuteStatementOutputTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
     ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
-def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
+def get_value() -> BatchExecuteStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/setup.py` & `types-aiobotocore-redshift-data-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-redshift-data",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_redshift_data"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with"
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
-    keywords="aiobotocore redshift-data type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore redshift-data type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_redshift_data": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/"
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/__init__.py` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/__init__.pyi` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/__main__.py` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService\nOther"
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

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/client.py` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/client.pyi` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/literals.py` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/literals.pyi` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/paginator.py` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,30 +79,30 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#describetablepaginator)
         """
 
 
 class GetStatementResultPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#getstatementresultpaginator)
     """
 
     def paginate(
-        self, *, Id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetStatementResultResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#getstatementresultpaginator)
         """
 
 
@@ -116,15 +116,15 @@
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listdatabasespaginator)
         """
 
 
@@ -140,15 +140,15 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listschemaspaginator)
         """
 
 
@@ -160,15 +160,15 @@
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#liststatementspaginator)
         """
 
 
@@ -185,13 +185,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/paginator.pyi` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -76,29 +76,29 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         Schema: str = ...,
         SecretArn: str = ...,
         Table: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[DescribeTableResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.DescribeTable.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#describetablepaginator)
         """
 
 class GetStatementResultPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#getstatementresultpaginator)
     """
 
     def paginate(
-        self, *, Id: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Id: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetStatementResultResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.GetStatementResult.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#getstatementresultpaginator)
         """
 
 class ListDatabasesPaginator(AioPaginator):
@@ -111,15 +111,15 @@
         self,
         *,
         Database: str,
         ClusterIdentifier: str = ...,
         DbUser: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatabasesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listdatabasespaginator)
         """
 
 class ListSchemasPaginator(AioPaginator):
@@ -134,15 +134,15 @@
         Database: str,
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListSchemasResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListSchemas.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listschemaspaginator)
         """
 
 class ListStatementsPaginator(AioPaginator):
@@ -153,15 +153,15 @@
 
     def paginate(
         self,
         *,
         RoleLevel: bool = ...,
         StatementName: str = ...,
         Status: StatusStringType = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListStatementsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListStatements.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#liststatementspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
@@ -177,13 +177,13 @@
         ClusterIdentifier: str = ...,
         ConnectedDatabase: str = ...,
         DbUser: str = ...,
         SchemaPattern: str = ...,
         SecretArn: str = ...,
         TablePattern: str = ...,
         WorkgroupName: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTablesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/paginators/#listtablespaginator)
         """
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/type_defs.py` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputRequestTypeDef
 
-    data: BatchExecuteStatementInputRequestTypeDef = {...}
+    data: BatchExecuteStatementInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import StatementStatusStringType, StatusStringType
@@ -21,44 +21,44 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
-    "CancelStatementResponseTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
     "SqlParameterTypeDef",
     "SubStatementDataTypeDef",
-    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTableRequestRequestTypeDef",
-    "ExecuteStatementOutputTypeDef",
     "FieldTypeDef",
-    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "GetStatementResultRequestRequestTypeDef",
-    "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListDatabasesRequestRequestTypeDef",
-    "ListDatabasesResponseTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
-    "ListSchemasResponseTypeDef",
-    "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListStatementsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
+    "CancelStatementResponseTypeDef",
+    "ExecuteStatementOutputTypeDef",
+    "ListDatabasesResponseTypeDef",
+    "ListSchemasResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
+    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
+    "ListDatabasesRequestListDatabasesPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -85,43 +85,32 @@
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelStatementRequestRequestTypeDef = TypedDict(
     "CancelStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-CancelStatementResponseTypeDef = TypedDict(
-    "CancelStatementResponseTypeDef",
-    {
-        "Status": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "columnDefault": str,
         "isCaseSensitive": bool,
         "isCurrency": bool,
         "isSigned": bool,
@@ -177,43 +166,24 @@
 )
 
 
 class SubStatementDataTypeDef(_RequiredSubStatementDataTypeDef, _OptionalSubStatementDataTypeDef):
     pass
 
 
-_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "Schema": str,
-        "SecretArn": str,
-        "Table": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class DescribeTableRequestDescribeTablePaginateTypeDef(
-    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
-    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
-):
-    pass
-
-
 _RequiredDescribeTableRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTableRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalDescribeTableRequestRequestTypeDef = TypedDict(
@@ -235,63 +205,27 @@
 
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
 
-ExecuteStatementOutputTypeDef = TypedDict(
-    "ExecuteStatementOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
         "booleanValue": bool,
         "doubleValue": float,
         "isNull": bool,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
 )
 
-_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class GetStatementResultRequestGetStatementResultPaginateTypeDef(
-    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
-    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetStatementResultRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementResultRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStatementResultRequestRequestTypeDef = TypedDict(
@@ -306,40 +240,14 @@
 class GetStatementResultRequestRequestTypeDef(
     _RequiredGetStatementResultRequestRequestTypeDef,
     _OptionalGetStatementResultRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatabasesRequestListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatabasesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListDatabasesRequestRequestTypeDef = TypedDict(
@@ -358,51 +266,14 @@
 
 class ListDatabasesRequestRequestTypeDef(
     _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
 ):
     pass
 
 
-ListDatabasesResponseTypeDef = TypedDict(
-    "ListDatabasesResponseTypeDef",
-    {
-        "Databases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -423,75 +294,26 @@
 
 class ListSchemasRequestRequestTypeDef(
     _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
 ):
     pass
 
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
-    {
-        "NextToken": str,
-        "Schemas": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    {
-        "RoleLevel": bool,
-        "StatementName": str,
-        "Status": StatusStringType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStatementsRequestRequestTypeDef = TypedDict(
     "ListStatementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RoleLevel": bool,
         "StatementName": str,
         "Status": StatusStringType,
     },
     total=False,
 )
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "TablePattern": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -523,42 +345,75 @@
         "name": str,
         "schema": str,
         "type": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelStatementResponseTypeDef = TypedDict(
+    "CancelStatementResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExecuteStatementOutputTypeDef = TypedDict(
+    "ExecuteStatementOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatabasesResponseTypeDef = TypedDict(
+    "ListDatabasesResponseTypeDef",
+    {
+        "Databases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
+    {
+        "NextToken": str,
+        "Schemas": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "ColumnList": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "TableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Database": str,
@@ -632,39 +487,184 @@
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
         "SubStatements": List[SubStatementDataTypeDef],
         "UpdatedAt": datetime,
         "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "Schema": str,
+        "SecretArn": str,
+        "Table": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class DescribeTableRequestDescribeTablePaginateTypeDef(
+    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
+    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
+):
+    pass
+
+
+_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetStatementResultRequestGetStatementResultPaginateTypeDef(
+    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
+    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatabasesRequestListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+
+ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    {
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "TablePattern": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
+):
+    pass
+
+
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "NextToken": str,
         "Tables": List[TableMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "NextToken": str,
         "Statements": List[StatementDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data/type_defs.pyi` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_redshift_data.type_defs import BatchExecuteStatementInputRequestTypeDef
 
-    data: BatchExecuteStatementInputRequestTypeDef = {...}
+    data: BatchExecuteStatementInputRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import StatementStatusStringType, StatusStringType
@@ -20,44 +20,44 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "BatchExecuteStatementInputRequestTypeDef",
-    "BatchExecuteStatementOutputTypeDef",
+    "ResponseMetadataTypeDef",
     "CancelStatementRequestRequestTypeDef",
-    "CancelStatementResponseTypeDef",
     "ColumnMetadataTypeDef",
     "DescribeStatementRequestRequestTypeDef",
     "SqlParameterTypeDef",
     "SubStatementDataTypeDef",
-    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "DescribeTableRequestRequestTypeDef",
-    "ExecuteStatementOutputTypeDef",
     "FieldTypeDef",
-    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
     "GetStatementResultRequestRequestTypeDef",
-    "ListDatabasesRequestListDatabasesPaginateTypeDef",
     "ListDatabasesRequestRequestTypeDef",
-    "ListDatabasesResponseTypeDef",
-    "ListSchemasRequestListSchemasPaginateTypeDef",
     "ListSchemasRequestRequestTypeDef",
-    "ListSchemasResponseTypeDef",
-    "ListStatementsRequestListStatementsPaginateTypeDef",
     "ListStatementsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableMemberTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
+    "BatchExecuteStatementOutputTypeDef",
+    "CancelStatementResponseTypeDef",
+    "ExecuteStatementOutputTypeDef",
+    "ListDatabasesResponseTypeDef",
+    "ListSchemasResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ExecuteStatementInputRequestTypeDef",
     "StatementDataTypeDef",
     "DescribeStatementResponseTypeDef",
+    "DescribeTableRequestDescribeTablePaginateTypeDef",
+    "GetStatementResultRequestGetStatementResultPaginateTypeDef",
+    "ListDatabasesRequestListDatabasesPaginateTypeDef",
+    "ListSchemasRequestListSchemasPaginateTypeDef",
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
     "GetStatementResultResponseTypeDef",
     "ListTablesResponseTypeDef",
     "ListStatementsResponseTypeDef",
 )
 
 _RequiredBatchExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredBatchExecuteStatementInputRequestTypeDef",
@@ -82,43 +82,32 @@
 
 class BatchExecuteStatementInputRequestTypeDef(
     _RequiredBatchExecuteStatementInputRequestTypeDef,
     _OptionalBatchExecuteStatementInputRequestTypeDef,
 ):
     pass
 
-BatchExecuteStatementOutputTypeDef = TypedDict(
-    "BatchExecuteStatementOutputTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 CancelStatementRequestRequestTypeDef = TypedDict(
     "CancelStatementRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 
-CancelStatementResponseTypeDef = TypedDict(
-    "CancelStatementResponseTypeDef",
-    {
-        "Status": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ColumnMetadataTypeDef = TypedDict(
     "ColumnMetadataTypeDef",
     {
         "columnDefault": str,
         "isCaseSensitive": bool,
         "isCurrency": bool,
         "isSigned": bool,
@@ -172,41 +161,24 @@
     },
     total=False,
 )
 
 class SubStatementDataTypeDef(_RequiredSubStatementDataTypeDef, _OptionalSubStatementDataTypeDef):
     pass
 
-_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
-    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "Schema": str,
-        "SecretArn": str,
-        "Table": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class DescribeTableRequestDescribeTablePaginateTypeDef(
-    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
-    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
-):
-    pass
-
 _RequiredDescribeTableRequestRequestTypeDef = TypedDict(
     "_RequiredDescribeTableRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalDescribeTableRequestRequestTypeDef = TypedDict(
@@ -226,61 +198,27 @@
 )
 
 class DescribeTableRequestRequestTypeDef(
     _RequiredDescribeTableRequestRequestTypeDef, _OptionalDescribeTableRequestRequestTypeDef
 ):
     pass
 
-ExecuteStatementOutputTypeDef = TypedDict(
-    "ExecuteStatementOutputTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "CreatedAt": datetime,
-        "Database": str,
-        "DbUser": str,
-        "Id": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 FieldTypeDef = TypedDict(
     "FieldTypeDef",
     {
         "blobValue": bytes,
         "booleanValue": bool,
         "doubleValue": float,
         "isNull": bool,
         "longValue": int,
         "stringValue": str,
     },
     total=False,
 )
 
-_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "Id": str,
-    },
-)
-_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
-    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class GetStatementResultRequestGetStatementResultPaginateTypeDef(
-    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
-    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
-):
-    pass
-
 _RequiredGetStatementResultRequestRequestTypeDef = TypedDict(
     "_RequiredGetStatementResultRequestRequestTypeDef",
     {
         "Id": str,
     },
 )
 _OptionalGetStatementResultRequestRequestTypeDef = TypedDict(
@@ -293,38 +231,14 @@
 
 class GetStatementResultRequestRequestTypeDef(
     _RequiredGetStatementResultRequestRequestTypeDef,
     _OptionalGetStatementResultRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "DbUser": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatabasesRequestListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatabasesRequestRequestTypeDef = TypedDict(
     "_RequiredListDatabasesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListDatabasesRequestRequestTypeDef = TypedDict(
@@ -341,49 +255,14 @@
 )
 
 class ListDatabasesRequestRequestTypeDef(
     _RequiredListDatabasesRequestRequestTypeDef, _OptionalListDatabasesRequestRequestTypeDef
 ):
     pass
 
-ListDatabasesResponseTypeDef = TypedDict(
-    "ListDatabasesResponseTypeDef",
-    {
-        "Databases": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
-    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListSchemasRequestListSchemasPaginateTypeDef(
-    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
-    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
-):
-    pass
-
 _RequiredListSchemasRequestRequestTypeDef = TypedDict(
     "_RequiredListSchemasRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListSchemasRequestRequestTypeDef = TypedDict(
@@ -402,73 +281,26 @@
 )
 
 class ListSchemasRequestRequestTypeDef(
     _RequiredListSchemasRequestRequestTypeDef, _OptionalListSchemasRequestRequestTypeDef
 ):
     pass
 
-ListSchemasResponseTypeDef = TypedDict(
-    "ListSchemasResponseTypeDef",
-    {
-        "NextToken": str,
-        "Schemas": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
-    "ListStatementsRequestListStatementsPaginateTypeDef",
-    {
-        "RoleLevel": bool,
-        "StatementName": str,
-        "Status": StatusStringType,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListStatementsRequestRequestTypeDef = TypedDict(
     "ListStatementsRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
         "RoleLevel": bool,
         "StatementName": str,
         "Status": StatusStringType,
     },
     total=False,
 )
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "Database": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
-        "ClusterIdentifier": str,
-        "ConnectedDatabase": str,
-        "DbUser": str,
-        "SchemaPattern": str,
-        "SecretArn": str,
-        "TablePattern": str,
-        "WorkgroupName": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTablesRequestListTablesPaginateTypeDef(
-    _RequiredListTablesRequestListTablesPaginateTypeDef,
-    _OptionalListTablesRequestListTablesPaginateTypeDef,
-):
-    pass
-
 _RequiredListTablesRequestRequestTypeDef = TypedDict(
     "_RequiredListTablesRequestRequestTypeDef",
     {
         "Database": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -498,42 +330,75 @@
         "name": str,
         "schema": str,
         "type": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+BatchExecuteStatementOutputTypeDef = TypedDict(
+    "BatchExecuteStatementOutputTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+CancelStatementResponseTypeDef = TypedDict(
+    "CancelStatementResponseTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "Status": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ExecuteStatementOutputTypeDef = TypedDict(
+    "ExecuteStatementOutputTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "CreatedAt": datetime,
+        "Database": str,
+        "DbUser": str,
+        "Id": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListDatabasesResponseTypeDef = TypedDict(
+    "ListDatabasesResponseTypeDef",
+    {
+        "Databases": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListSchemasResponseTypeDef = TypedDict(
+    "ListSchemasResponseTypeDef",
+    {
+        "NextToken": str,
+        "Schemas": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "ColumnList": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "TableName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredExecuteStatementInputRequestTypeDef = TypedDict(
     "_RequiredExecuteStatementInputRequestTypeDef",
     {
         "Database": str,
@@ -603,39 +468,174 @@
         "ResultRows": int,
         "ResultSize": int,
         "SecretArn": str,
         "Status": StatusStringType,
         "SubStatements": List[SubStatementDataTypeDef],
         "UpdatedAt": datetime,
         "WorkgroupName": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+_RequiredDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_RequiredDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "Database": str,
     },
 )
+_OptionalDescribeTableRequestDescribeTablePaginateTypeDef = TypedDict(
+    "_OptionalDescribeTableRequestDescribeTablePaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "Schema": str,
+        "SecretArn": str,
+        "Table": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class DescribeTableRequestDescribeTablePaginateTypeDef(
+    _RequiredDescribeTableRequestDescribeTablePaginateTypeDef,
+    _OptionalDescribeTableRequestDescribeTablePaginateTypeDef,
+):
+    pass
+
+_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "Id": str,
+    },
+)
+_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef = TypedDict(
+    "_OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetStatementResultRequestGetStatementResultPaginateTypeDef(
+    _RequiredGetStatementResultRequestGetStatementResultPaginateTypeDef,
+    _OptionalGetStatementResultRequestGetStatementResultPaginateTypeDef,
+):
+    pass
+
+_RequiredListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListDatabasesRequestListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesRequestListDatabasesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "DbUser": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatabasesRequestListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesRequestListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesRequestListDatabasesPaginateTypeDef,
+):
+    pass
+
+_RequiredListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_RequiredListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListSchemasRequestListSchemasPaginateTypeDef = TypedDict(
+    "_OptionalListSchemasRequestListSchemasPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListSchemasRequestListSchemasPaginateTypeDef(
+    _RequiredListSchemasRequestListSchemasPaginateTypeDef,
+    _OptionalListSchemasRequestListSchemasPaginateTypeDef,
+):
+    pass
+
+ListStatementsRequestListStatementsPaginateTypeDef = TypedDict(
+    "ListStatementsRequestListStatementsPaginateTypeDef",
+    {
+        "RoleLevel": bool,
+        "StatementName": str,
+        "Status": StatusStringType,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "Database": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
+        "ClusterIdentifier": str,
+        "ConnectedDatabase": str,
+        "DbUser": str,
+        "SchemaPattern": str,
+        "SecretArn": str,
+        "TablePattern": str,
+        "WorkgroupName": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTablesRequestListTablesPaginateTypeDef(
+    _RequiredListTablesRequestListTablesPaginateTypeDef,
+    _OptionalListTablesRequestListTablesPaginateTypeDef,
+):
+    pass
 
 GetStatementResultResponseTypeDef = TypedDict(
     "GetStatementResultResponseTypeDef",
     {
         "ColumnMetadata": List[ColumnMetadataTypeDef],
         "NextToken": str,
         "Records": List[List[FieldTypeDef]],
         "TotalNumRows": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "NextToken": str,
         "Tables": List[TableMemberTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListStatementsResponseTypeDef = TypedDict(
     "ListStatementsResponseTypeDef",
     {
         "NextToken": str,
         "Statements": List[StatementDataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/PKG-INFO` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-redshift-data
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.RedshiftDataAPIService 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore redshift-data type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore redshift-data type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-redshift-data"></a>
 
 # types-aiobotocore-redshift-data
 
 [![PyPI - types-aiobotocore-redshift-data](https://img.shields.io/pypi/v/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-redshift-data.svg?color=blue)](https://pypi.org/project/types-aiobotocore-redshift-data)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-redshift-data?color=blue)](https://pypistats.org/packages/types-aiobotocore-redshift-data)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-redshift-data)](https://pepy.tech/project/types-aiobotocore-redshift-data)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.RedshiftDataAPIService 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/redshift-data.html#RedshiftDataAPIService)
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
 [types-aiobotocore-redshift-data docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_redshift_data/).
 
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
@@ -325,61 +324,61 @@
 )
 
 
 def check_value(value: DescribeTablePaginatorName) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_redshift_data.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_redshift_data.type_defs import (
     BatchExecuteStatementInputRequestTypeDef,
-    BatchExecuteStatementOutputTypeDef,
+    ResponseMetadataTypeDef,
     CancelStatementRequestRequestTypeDef,
-    CancelStatementResponseTypeDef,
     ColumnMetadataTypeDef,
     DescribeStatementRequestRequestTypeDef,
     SqlParameterTypeDef,
     SubStatementDataTypeDef,
-    DescribeTableRequestDescribeTablePaginateTypeDef,
+    PaginatorConfigTypeDef,
     DescribeTableRequestRequestTypeDef,
-    ExecuteStatementOutputTypeDef,
     FieldTypeDef,
-    GetStatementResultRequestGetStatementResultPaginateTypeDef,
     GetStatementResultRequestRequestTypeDef,
-    ListDatabasesRequestListDatabasesPaginateTypeDef,
     ListDatabasesRequestRequestTypeDef,
-    ListDatabasesResponseTypeDef,
-    ListSchemasRequestListSchemasPaginateTypeDef,
     ListSchemasRequestRequestTypeDef,
-    ListSchemasResponseTypeDef,
-    ListStatementsRequestListStatementsPaginateTypeDef,
     ListStatementsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableMemberTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
+    BatchExecuteStatementOutputTypeDef,
+    CancelStatementResponseTypeDef,
+    ExecuteStatementOutputTypeDef,
+    ListDatabasesResponseTypeDef,
+    ListSchemasResponseTypeDef,
     DescribeTableResponseTypeDef,
     ExecuteStatementInputRequestTypeDef,
     StatementDataTypeDef,
     DescribeStatementResponseTypeDef,
+    DescribeTableRequestDescribeTablePaginateTypeDef,
+    GetStatementResultRequestGetStatementResultPaginateTypeDef,
+    ListDatabasesRequestListDatabasesPaginateTypeDef,
+    ListSchemasRequestListSchemasPaginateTypeDef,
+    ListStatementsRequestListStatementsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
     GetStatementResultResponseTypeDef,
     ListTablesResponseTypeDef,
     ListStatementsResponseTypeDef,
 )
 
 
-def get_structure() -> BatchExecuteStatementInputRequestTypeDef:
+def get_value() -> BatchExecuteStatementInputRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-redshift-data-2.5.2/types_aiobotocore_redshift_data.egg-info/SOURCES.txt` & `types-aiobotocore-redshift-data-2.5.2.post1/types_aiobotocore_redshift_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*


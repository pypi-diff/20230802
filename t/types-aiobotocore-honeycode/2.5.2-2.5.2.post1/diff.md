# Comparing `tmp/types-aiobotocore-honeycode-2.5.2.tar.gz` & `tmp/types-aiobotocore-honeycode-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-honeycode-2.5.2.tar", last modified: Sat Jul  8 01:43:42 2023, max compression
+gzip compressed data, was "types-aiobotocore-honeycode-2.5.2.post1.tar", last modified: Wed Aug  2 14:52:23 2023, max compression
```

## Comparing `types-aiobotocore-honeycode-2.5.2.tar` & `types-aiobotocore-honeycode-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.434222 types-aiobotocore-honeycode-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-08 01:43:42.434222 types-aiobotocore-honeycode-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14029 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:42.434222 types-aiobotocore-honeycode-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.430222 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16914 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    20854 2023-07-08 01:31:59.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    20819 2023-07-08 01:31:58.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:31:57.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:42.434222 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15602 2023-07-08 01:43:42.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-08 01:43:42.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:42.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:42.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-08 01:43:42.000000 types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.013573 types-aiobotocore-honeycode-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-02 14:52:23.005573 types-aiobotocore-honeycode-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14112 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:52:23.013573 types-aiobotocore-honeycode-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.005573 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16924 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16896 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9166 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5466 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21445 2023-08-02 14:39:57.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21410 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:39:56.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:52:23.005573 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15638 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-08-02 14:52:22.000000 types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-honeycode-2.5.2/LICENSE` & `types-aiobotocore-honeycode-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2/PKG-INFO` & `types-aiobotocore-honeycode-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore honeycode type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore honeycode type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-honeycode"></a>
 
 # types-aiobotocore-honeycode
 
 [![PyPI - types-aiobotocore-honeycode](https://img.shields.io/pypi/v/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-honeycode?color=blue)](https://pypistats.org/packages/types-aiobotocore-honeycode)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Honeycode 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
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
@@ -324,85 +323,88 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_honeycode.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_honeycode.type_defs import (
     FailedBatchItemTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
+    DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
     ImportDataSourceTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
     TableDataImportJobMetadataTypeDef,
+    ImportOptionsUnionTypeDef,
+    StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
-def get_structure() -> FailedBatchItemTypeDef:
+def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-honeycode-2.5.2/README.md` & `types-aiobotocore-honeycode-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-honeycode"></a>
 
 # types-aiobotocore-honeycode
 
 [![PyPI - types-aiobotocore-honeycode](https://img.shields.io/pypi/v/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-honeycode?color=blue)](https://pypistats.org/packages/types-aiobotocore-honeycode)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Honeycode 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
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
@@ -291,85 +291,88 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_honeycode.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_honeycode.type_defs import (
     FailedBatchItemTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
+    DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
     ImportDataSourceTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
     TableDataImportJobMetadataTypeDef,
+    ImportOptionsUnionTypeDef,
+    StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
-def get_structure() -> FailedBatchItemTypeDef:
+def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-honeycode-2.5.2/setup.py` & `types-aiobotocore-honeycode-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-honeycode",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_honeycode"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore honeycode type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore honeycode type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_honeycode": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/"
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/__init__.py` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/__init__.pyi` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/__main__.py` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/__main__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Honeycode 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Honeycode 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode\nOther"
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

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/client.py` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
-    ImportOptionsTypeDef,
+    ImportOptionsUnionTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
     StartTableDataImportJobResultTypeDef,
@@ -299,15 +299,15 @@
     async def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: ImportOptionsTypeDef,
+        importOptions: ImportOptionsUnionTypeDef,
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#start_table_data_import_job)
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/client.pyi` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     BatchUpdateTableRowsResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     DescribeTableDataImportJobResultTypeDef,
     FilterTypeDef,
     GetScreenDataResultTypeDef,
     ImportDataSourceTypeDef,
-    ImportOptionsTypeDef,
+    ImportOptionsUnionTypeDef,
     InvokeScreenAutomationResultTypeDef,
     ListTableColumnsResultTypeDef,
     ListTableRowsResultTypeDef,
     ListTablesResultTypeDef,
     ListTagsForResourceResultTypeDef,
     QueryTableRowsResultTypeDef,
     StartTableDataImportJobResultTypeDef,
@@ -279,15 +279,15 @@
     async def start_table_data_import_job(
         self,
         *,
         workbookId: str,
         dataSource: ImportDataSourceTypeDef,
         dataFormat: Literal["DELIMITED_TEXT"],
         destinationTableId: str,
-        importOptions: ImportOptionsTypeDef,
+        importOptions: ImportOptionsUnionTypeDef,
         clientRequestToken: str
     ) -> StartTableDataImportJobResultTypeDef:
         """
         The StartTableDataImportJob API allows you to start an import job on a table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Client.start_table_data_import_job)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/client/#start_table_data_import_job)
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/literals.py` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/literals.pyi` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/paginator.py` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 class ListTableColumnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablecolumnspaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, tableId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, tableId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableColumnsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablecolumnspaginator)
         """
 
 
@@ -81,30 +81,30 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablerowspaginator)
         """
 
 
 class ListTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTablesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablespaginator)
         """
 
 
@@ -116,13 +116,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/paginator.pyi` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 class ListTableColumnsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablecolumnspaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, tableId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, tableId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableColumnsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableColumns.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablecolumnspaginator)
         """
 
 class ListTableRowsPaginator(AioPaginator):
@@ -77,29 +77,29 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         rowIds: Sequence[str] = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablerowspaginator)
         """
 
 class ListTablesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablespaginator)
     """
 
     def paginate(
-        self, *, workbookId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, workbookId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTablesResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.ListTables.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#listtablespaginator)
         """
 
 class QueryTableRowsPaginator(AioPaginator):
@@ -110,13 +110,13 @@
 
     def paginate(
         self,
         *,
         workbookId: str,
         tableId: str,
         filterFormula: FilterTypeDef,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryTableRowsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode.Paginator.QueryTableRows.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/paginators/#querytablerowspaginator)
         """
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/type_defs.py` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef
 
-    data: FailedBatchItemTypeDef = {...}
+    data: FailedBatchItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ErrorCodeType,
     FormatType,
     ImportDataCharacterEncodingType,
     TableDataImportJobStatusType,
     UpsertActionType,
@@ -31,81 +31,95 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "FailedBatchItemTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
-    "InvokeScreenAutomationResultTypeDef",
-    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
-    "ListTableRowsRequestListTableRowsPaginateTypeDef",
     "ListTableRowsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartTableDataImportJobResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchCreateTableRowsResultTypeDef",
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
+    "InvokeScreenAutomationResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
+    "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
-    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
     "ImportDataSourceTypeDef",
+    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "ListTableRowsRequestListTableRowsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
+    "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
-    "StartTableDataImportJobRequestRequestTypeDef",
     "TableDataImportJobMetadataTypeDef",
+    "ImportOptionsUnionTypeDef",
+    "StartTableDataImportJobRequestRequestTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
         "id": str,
         "errorMessage": str,
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
 _RequiredBatchDeleteTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowIds": Sequence[str],
     },
@@ -252,45 +266,24 @@
     {
         "email": str,
         "userArn": str,
     },
     total=False,
 )
 
-InvokeScreenAutomationResultTypeDef = TypedDict(
-    "InvokeScreenAutomationResultTypeDef",
-    {
-        "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
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
-class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
-    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTableColumnsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableColumnsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -315,38 +308,14 @@
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
     total=False,
 )
 
-_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "rowIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTableRowsRequestListTableRowsPaginateTypeDef(
-    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
-    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -363,36 +332,14 @@
 
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "workbookId": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
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
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -423,52 +370,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
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
-StartTableDataImportJobResultTypeDef = TypedDict(
-    "StartTableDataImportJobResultTypeDef",
-    {
-        "jobId": str,
-        "jobStatus": TableDataImportJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -483,43 +392,68 @@
 
 BatchCreateTableRowsResultTypeDef = TypedDict(
     "BatchCreateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "createdRows": Dict[str, str],
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteTableRowsResultTypeDef = TypedDict(
     "BatchDeleteTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateTableRowsResultTypeDef = TypedDict(
     "BatchUpdateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeScreenAutomationResultTypeDef = TypedDict(
+    "InvokeScreenAutomationResultTypeDef",
+    {
+        "workbookCursor": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTableDataImportJobResultTypeDef = TypedDict(
+    "StartTableDataImportJobResultTypeDef",
+    {
+        "jobId": str,
+        "jobStatus": TableDataImportJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpsertTableRowsResultTypeDef = TypedDict(
     "BatchUpsertTableRowsResultTypeDef",
     {
         "rows": Dict[str, UpsertRowsResultTypeDef],
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRowDataTypeDef = TypedDict(
     "CreateRowDataTypeDef",
     {
         "batchItemId": str,
@@ -558,46 +492,30 @@
 )
 
 
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
 
-DestinationOptionsTypeDef = TypedDict(
-    "DestinationOptionsTypeDef",
+DestinationOptionsOutputTypeDef = TypedDict(
+    "DestinationOptionsOutputTypeDef",
     {
         "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
-_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-        "filterFormula": FilterTypeDef,
-    },
-)
-_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+DestinationOptionsTypeDef = TypedDict(
+    "DestinationOptionsTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
-
-class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
-    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -682,31 +600,124 @@
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
+_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
+    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "rowIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTableRowsRequestListTableRowsPaginateTypeDef(
+    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
+    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "workbookId": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
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
+_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+        "filterFormula": FilterTypeDef,
+    },
+)
+_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
+    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+):
+    pass
+
+
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResultTypeDef = TypedDict(
     "ListTablesResultTypeDef",
     {
         "tables": List[TableTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -758,37 +769,46 @@
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryTableRowsResultTypeDef = TypedDict(
     "QueryTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
         "rows": List[ResultRowTypeDef],
     },
 )
 
+ImportOptionsOutputTypeDef = TypedDict(
+    "ImportOptionsOutputTypeDef",
+    {
+        "destinationOptions": DestinationOptionsOutputTypeDef,
+        "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
+    },
+    total=False,
+)
+
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
         "destinationOptions": DestinationOptionsTypeDef,
         "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
@@ -820,43 +840,44 @@
 
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TableDataImportJobMetadataTypeDef = TypedDict(
+    "TableDataImportJobMetadataTypeDef",
+    {
+        "submitter": ImportJobSubmitterTypeDef,
+        "submitTime": datetime,
+        "importOptions": ImportOptionsOutputTypeDef,
+        "dataSource": ImportDataSourceTypeDef,
+    },
+)
+
+ImportOptionsUnionTypeDef = Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef]
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
         "importOptions": ImportOptionsTypeDef,
         "clientRequestToken": str,
     },
 )
 
-TableDataImportJobMetadataTypeDef = TypedDict(
-    "TableDataImportJobMetadataTypeDef",
-    {
-        "submitter": ImportJobSubmitterTypeDef,
-        "submitTime": datetime,
-        "importOptions": ImportOptionsTypeDef,
-        "dataSource": ImportDataSourceTypeDef,
-    },
-)
-
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode/type_defs.pyi` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode/type_defs.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_honeycode.type_defs import FailedBatchItemTypeDef
 
-    data: FailedBatchItemTypeDef = {...}
+    data: FailedBatchItemTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Mapping, Sequence
+from typing import Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     ErrorCodeType,
     FormatType,
     ImportDataCharacterEncodingType,
     TableDataImportJobStatusType,
     UpsertActionType,
@@ -30,81 +30,95 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "FailedBatchItemTypeDef",
+    "ResponseMetadataTypeDef",
     "BatchDeleteTableRowsRequestRequestTypeDef",
     "UpsertRowsResultTypeDef",
     "CellInputTypeDef",
     "CellTypeDef",
     "ColumnMetadataTypeDef",
     "DataItemTypeDef",
     "DelimitedTextImportOptionsTypeDef",
     "DescribeTableDataImportJobRequestRequestTypeDef",
     "SourceDataColumnPropertiesTypeDef",
     "FilterTypeDef",
     "VariableValueTypeDef",
     "ImportDataSourceConfigTypeDef",
     "ImportJobSubmitterTypeDef",
-    "InvokeScreenAutomationResultTypeDef",
-    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListTableColumnsRequestRequestTypeDef",
     "TableColumnTypeDef",
-    "ListTableRowsRequestListTableRowsPaginateTypeDef",
     "ListTableRowsRequestRequestTypeDef",
-    "ListTablesRequestListTablesPaginateTypeDef",
     "ListTablesRequestRequestTypeDef",
     "TableTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResultTypeDef",
-    "PaginatorConfigTypeDef",
-    "ResponseMetadataTypeDef",
-    "StartTableDataImportJobResultTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "BatchCreateTableRowsResultTypeDef",
     "BatchDeleteTableRowsResultTypeDef",
     "BatchUpdateTableRowsResultTypeDef",
+    "InvokeScreenAutomationResultTypeDef",
+    "ListTagsForResourceResultTypeDef",
+    "StartTableDataImportJobResultTypeDef",
     "BatchUpsertTableRowsResultTypeDef",
     "CreateRowDataTypeDef",
     "UpdateRowDataTypeDef",
     "TableRowTypeDef",
     "ResultRowTypeDef",
+    "DestinationOptionsOutputTypeDef",
     "DestinationOptionsTypeDef",
-    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "QueryTableRowsRequestRequestTypeDef",
     "UpsertRowDataTypeDef",
     "GetScreenDataRequestRequestTypeDef",
     "InvokeScreenAutomationRequestRequestTypeDef",
     "ImportDataSourceTypeDef",
+    "ListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    "ListTableRowsRequestListTableRowsPaginateTypeDef",
+    "ListTablesRequestListTablesPaginateTypeDef",
+    "QueryTableRowsRequestQueryTableRowsPaginateTypeDef",
     "ListTableColumnsResultTypeDef",
     "ListTablesResultTypeDef",
     "BatchCreateTableRowsRequestRequestTypeDef",
     "BatchUpdateTableRowsRequestRequestTypeDef",
     "ListTableRowsResultTypeDef",
     "QueryTableRowsResultTypeDef",
     "ResultSetTypeDef",
+    "ImportOptionsOutputTypeDef",
     "ImportOptionsTypeDef",
     "BatchUpsertTableRowsRequestRequestTypeDef",
     "GetScreenDataResultTypeDef",
-    "StartTableDataImportJobRequestRequestTypeDef",
     "TableDataImportJobMetadataTypeDef",
+    "ImportOptionsUnionTypeDef",
+    "StartTableDataImportJobRequestRequestTypeDef",
     "DescribeTableDataImportJobResultTypeDef",
 )
 
 FailedBatchItemTypeDef = TypedDict(
     "FailedBatchItemTypeDef",
     {
         "id": str,
         "errorMessage": str,
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
 _RequiredBatchDeleteTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchDeleteTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "rowIds": Sequence[str],
     },
@@ -245,43 +259,24 @@
     {
         "email": str,
         "userArn": str,
     },
     total=False,
 )
 
-InvokeScreenAutomationResultTypeDef = TypedDict(
-    "InvokeScreenAutomationResultTypeDef",
-    {
-        "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
-    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
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
 
-class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
-    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
-    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTableColumnsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableColumnsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -304,36 +299,14 @@
         "tableColumnId": str,
         "tableColumnName": str,
         "format": FormatType,
     },
     total=False,
 )
 
-_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-    },
-)
-_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
-    {
-        "rowIds": Sequence[str],
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTableRowsRequestListTableRowsPaginateTypeDef(
-    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
-    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
-):
-    pass
-
 _RequiredListTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredListTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
     },
 )
@@ -348,34 +321,14 @@
 )
 
 class ListTableRowsRequestRequestTypeDef(
     _RequiredListTableRowsRequestRequestTypeDef, _OptionalListTableRowsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_RequiredListTablesRequestListTablesPaginateTypeDef",
-    {
-        "workbookId": str,
-    },
-)
-_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
-    "_OptionalListTablesRequestListTablesPaginateTypeDef",
-    {
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
         "workbookId": str,
     },
 )
 _OptionalListTablesRequestRequestTypeDef = TypedDict(
@@ -404,52 +357,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
     },
 )
 
-ListTagsForResourceResultTypeDef = TypedDict(
-    "ListTagsForResourceResultTypeDef",
-    {
-        "tags": Dict[str, str],
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
-StartTableDataImportJobResultTypeDef = TypedDict(
-    "StartTableDataImportJobResultTypeDef",
-    {
-        "jobId": str,
-        "jobStatus": TableDataImportJobStatusType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "resourceArn": str,
         "tags": Mapping[str, str],
     },
 )
@@ -464,43 +379,68 @@
 
 BatchCreateTableRowsResultTypeDef = TypedDict(
     "BatchCreateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "createdRows": Dict[str, str],
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchDeleteTableRowsResultTypeDef = TypedDict(
     "BatchDeleteTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpdateTableRowsResultTypeDef = TypedDict(
     "BatchUpdateTableRowsResultTypeDef",
     {
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+InvokeScreenAutomationResultTypeDef = TypedDict(
+    "InvokeScreenAutomationResultTypeDef",
+    {
+        "workbookCursor": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResultTypeDef = TypedDict(
+    "ListTagsForResourceResultTypeDef",
+    {
+        "tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartTableDataImportJobResultTypeDef = TypedDict(
+    "StartTableDataImportJobResultTypeDef",
+    {
+        "jobId": str,
+        "jobStatus": TableDataImportJobStatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchUpsertTableRowsResultTypeDef = TypedDict(
     "BatchUpsertTableRowsResultTypeDef",
     {
         "rows": Dict[str, UpsertRowsResultTypeDef],
         "workbookCursor": int,
         "failedBatchItems": List[FailedBatchItemTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateRowDataTypeDef = TypedDict(
     "CreateRowDataTypeDef",
     {
         "batchItemId": str,
@@ -537,44 +477,30 @@
     },
     total=False,
 )
 
 class ResultRowTypeDef(_RequiredResultRowTypeDef, _OptionalResultRowTypeDef):
     pass
 
-DestinationOptionsTypeDef = TypedDict(
-    "DestinationOptionsTypeDef",
+DestinationOptionsOutputTypeDef = TypedDict(
+    "DestinationOptionsOutputTypeDef",
     {
         "columnMap": Dict[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
-_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
-    {
-        "workbookId": str,
-        "tableId": str,
-        "filterFormula": FilterTypeDef,
-    },
-)
-_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
-    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+DestinationOptionsTypeDef = TypedDict(
+    "DestinationOptionsTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "columnMap": Mapping[str, SourceDataColumnPropertiesTypeDef],
     },
     total=False,
 )
 
-class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
-    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
-):
-    pass
-
 _RequiredQueryTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredQueryTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
         "tableId": str,
         "filterFormula": FilterTypeDef,
     },
@@ -653,31 +579,116 @@
 ImportDataSourceTypeDef = TypedDict(
     "ImportDataSourceTypeDef",
     {
         "dataSourceConfig": ImportDataSourceConfigTypeDef,
     },
 )
 
+_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef = TypedDict(
+    "_OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTableColumnsRequestListTableColumnsPaginateTypeDef(
+    _RequiredListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    _OptionalListTableColumnsRequestListTableColumnsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+    },
+)
+_OptionalListTableRowsRequestListTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalListTableRowsRequestListTableRowsPaginateTypeDef",
+    {
+        "rowIds": Sequence[str],
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTableRowsRequestListTableRowsPaginateTypeDef(
+    _RequiredListTableRowsRequestListTableRowsPaginateTypeDef,
+    _OptionalListTableRowsRequestListTableRowsPaginateTypeDef,
+):
+    pass
+
+_RequiredListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_RequiredListTablesRequestListTablesPaginateTypeDef",
+    {
+        "workbookId": str,
+    },
+)
+_OptionalListTablesRequestListTablesPaginateTypeDef = TypedDict(
+    "_OptionalListTablesRequestListTablesPaginateTypeDef",
+    {
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
+
+_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "workbookId": str,
+        "tableId": str,
+        "filterFormula": FilterTypeDef,
+    },
+)
+_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef = TypedDict(
+    "_OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryTableRowsRequestQueryTableRowsPaginateTypeDef(
+    _RequiredQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+    _OptionalQueryTableRowsRequestQueryTableRowsPaginateTypeDef,
+):
+    pass
+
 ListTableColumnsResultTypeDef = TypedDict(
     "ListTableColumnsResultTypeDef",
     {
         "tableColumns": List[TableColumnTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResultTypeDef = TypedDict(
     "ListTablesResultTypeDef",
     {
         "tables": List[TableTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredBatchCreateTableRowsRequestRequestTypeDef = TypedDict(
     "_RequiredBatchCreateTableRowsRequestRequestTypeDef",
     {
         "workbookId": str,
@@ -725,37 +736,46 @@
     "ListTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "rowIdsNotFound": List[str],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryTableRowsResultTypeDef = TypedDict(
     "QueryTableRowsResultTypeDef",
     {
         "columnIds": List[str],
         "rows": List[TableRowTypeDef],
         "nextToken": str,
         "workbookCursor": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "headers": List[ColumnMetadataTypeDef],
         "rows": List[ResultRowTypeDef],
     },
 )
 
+ImportOptionsOutputTypeDef = TypedDict(
+    "ImportOptionsOutputTypeDef",
+    {
+        "destinationOptions": DestinationOptionsOutputTypeDef,
+        "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
+    },
+    total=False,
+)
+
 ImportOptionsTypeDef = TypedDict(
     "ImportOptionsTypeDef",
     {
         "destinationOptions": DestinationOptionsTypeDef,
         "delimitedTextOptions": DelimitedTextImportOptionsTypeDef,
     },
     total=False,
@@ -785,43 +805,44 @@
 
 GetScreenDataResultTypeDef = TypedDict(
     "GetScreenDataResultTypeDef",
     {
         "results": Dict[str, ResultSetTypeDef],
         "workbookCursor": int,
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+TableDataImportJobMetadataTypeDef = TypedDict(
+    "TableDataImportJobMetadataTypeDef",
+    {
+        "submitter": ImportJobSubmitterTypeDef,
+        "submitTime": datetime,
+        "importOptions": ImportOptionsOutputTypeDef,
+        "dataSource": ImportDataSourceTypeDef,
+    },
+)
+
+ImportOptionsUnionTypeDef = Union[ImportOptionsTypeDef, ImportOptionsOutputTypeDef]
 StartTableDataImportJobRequestRequestTypeDef = TypedDict(
     "StartTableDataImportJobRequestRequestTypeDef",
     {
         "workbookId": str,
         "dataSource": ImportDataSourceTypeDef,
         "dataFormat": Literal["DELIMITED_TEXT"],
         "destinationTableId": str,
         "importOptions": ImportOptionsTypeDef,
         "clientRequestToken": str,
     },
 )
 
-TableDataImportJobMetadataTypeDef = TypedDict(
-    "TableDataImportJobMetadataTypeDef",
-    {
-        "submitter": ImportJobSubmitterTypeDef,
-        "submitTime": datetime,
-        "importOptions": ImportOptionsTypeDef,
-        "dataSource": ImportDataSourceTypeDef,
-    },
-)
-
 DescribeTableDataImportJobResultTypeDef = TypedDict(
     "DescribeTableDataImportJobResultTypeDef",
     {
         "jobStatus": TableDataImportJobStatusType,
         "message": str,
         "jobMetadata": TableDataImportJobMetadataTypeDef,
         "errorCode": ErrorCodeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/PKG-INFO` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-honeycode
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Honeycode 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore honeycode type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore honeycode type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-honeycode"></a>
 
 # types-aiobotocore-honeycode
 
 [![PyPI - types-aiobotocore-honeycode](https://img.shields.io/pypi/v/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-honeycode.svg?color=blue)](https://pypi.org/project/types-aiobotocore-honeycode)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-honeycode?color=blue)](https://pypistats.org/packages/types-aiobotocore-honeycode)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-honeycode)](https://pepy.tech/project/types-aiobotocore-honeycode)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Honeycode 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/honeycode.html#Honeycode)
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
 [types-aiobotocore-honeycode docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_honeycode/).
 
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
@@ -324,85 +323,88 @@
 )
 
 
 def check_value(value: ErrorCodeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_honeycode.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_honeycode.type_defs import (
     FailedBatchItemTypeDef,
+    ResponseMetadataTypeDef,
     BatchDeleteTableRowsRequestRequestTypeDef,
     UpsertRowsResultTypeDef,
     CellInputTypeDef,
     CellTypeDef,
     ColumnMetadataTypeDef,
     DataItemTypeDef,
     DelimitedTextImportOptionsTypeDef,
     DescribeTableDataImportJobRequestRequestTypeDef,
     SourceDataColumnPropertiesTypeDef,
     FilterTypeDef,
     VariableValueTypeDef,
     ImportDataSourceConfigTypeDef,
     ImportJobSubmitterTypeDef,
-    InvokeScreenAutomationResultTypeDef,
-    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListTableColumnsRequestRequestTypeDef,
     TableColumnTypeDef,
-    ListTableRowsRequestListTableRowsPaginateTypeDef,
     ListTableRowsRequestRequestTypeDef,
-    ListTablesRequestListTablesPaginateTypeDef,
     ListTablesRequestRequestTypeDef,
     TableTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResultTypeDef,
-    PaginatorConfigTypeDef,
-    ResponseMetadataTypeDef,
-    StartTableDataImportJobResultTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     BatchCreateTableRowsResultTypeDef,
     BatchDeleteTableRowsResultTypeDef,
     BatchUpdateTableRowsResultTypeDef,
+    InvokeScreenAutomationResultTypeDef,
+    ListTagsForResourceResultTypeDef,
+    StartTableDataImportJobResultTypeDef,
     BatchUpsertTableRowsResultTypeDef,
     CreateRowDataTypeDef,
     UpdateRowDataTypeDef,
     TableRowTypeDef,
     ResultRowTypeDef,
+    DestinationOptionsOutputTypeDef,
     DestinationOptionsTypeDef,
-    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     QueryTableRowsRequestRequestTypeDef,
     UpsertRowDataTypeDef,
     GetScreenDataRequestRequestTypeDef,
     InvokeScreenAutomationRequestRequestTypeDef,
     ImportDataSourceTypeDef,
+    ListTableColumnsRequestListTableColumnsPaginateTypeDef,
+    ListTableRowsRequestListTableRowsPaginateTypeDef,
+    ListTablesRequestListTablesPaginateTypeDef,
+    QueryTableRowsRequestQueryTableRowsPaginateTypeDef,
     ListTableColumnsResultTypeDef,
     ListTablesResultTypeDef,
     BatchCreateTableRowsRequestRequestTypeDef,
     BatchUpdateTableRowsRequestRequestTypeDef,
     ListTableRowsResultTypeDef,
     QueryTableRowsResultTypeDef,
     ResultSetTypeDef,
+    ImportOptionsOutputTypeDef,
     ImportOptionsTypeDef,
     BatchUpsertTableRowsRequestRequestTypeDef,
     GetScreenDataResultTypeDef,
-    StartTableDataImportJobRequestRequestTypeDef,
     TableDataImportJobMetadataTypeDef,
+    ImportOptionsUnionTypeDef,
+    StartTableDataImportJobRequestRequestTypeDef,
     DescribeTableDataImportJobResultTypeDef,
 )
 
 
-def get_structure() -> FailedBatchItemTypeDef:
+def get_value() -> FailedBatchItemTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-honeycode-2.5.2/types_aiobotocore_honeycode.egg-info/SOURCES.txt` & `types-aiobotocore-honeycode-2.5.2.post1/types_aiobotocore_honeycode.egg-info/SOURCES.txt`

 * *Files identical despite different names*


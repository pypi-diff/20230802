# Comparing `tmp/types-aiobotocore-applicationcostprofiler-2.5.2.tar.gz` & `tmp/types-aiobotocore-applicationcostprofiler-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.5.2.tar", last modified: Sat Jul  8 01:43:14 2023, max compression
+gzip compressed data, was "types-aiobotocore-applicationcostprofiler-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:52 2023, max compression
```

## Comparing `types-aiobotocore-applicationcostprofiler-2.5.2.tar` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.557694 types-aiobotocore-applicationcostprofiler-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-08 01:43:14.557694 types-aiobotocore-applicationcostprofiler-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:14.557694 types-aiobotocore-applicationcostprofiler-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.557694 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-07-08 01:25:50.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-07-08 01:25:50.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-07-08 01:25:50.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:25:49.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:14.557694 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14521 2023-07-08 01:43:14.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-08 01:43:14.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:14.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:14.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-08 01:43:14.000000 types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.817654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9501 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8031 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-08-02 14:33:16.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5658 2023-08-02 14:33:16.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:15.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:52.825654 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14457 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-08-02 14:51:52.000000 types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/LICENSE` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore applicationcostprofiler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore applicationcostprofiler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-applicationcostprofiler"></a>
 
 # types-aiobotocore-applicationcostprofiler
 
 [![PyPI - types-aiobotocore-applicationcostprofiler](https://img.shields.io/pypi/v/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-applicationcostprofiler?color=blue)](https://pypistats.org/packages/types-aiobotocore-applicationcostprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationCostProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
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
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
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
@@ -309,46 +308,46 @@
 )
 
 
 def check_value(value: FormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_applicationcostprofiler.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
+    ResponseMetadataTypeDef,
     GetReportDefinitionRequestRequestTypeDef,
     S3LocationTypeDef,
     SourceS3LocationTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListReportDefinitionsRequestRequestTypeDef,
+    DeleteReportDefinitionResultTypeDef,
+    ImportApplicationUsageResultTypeDef,
     PutReportDefinitionResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateReportDefinitionResultTypeDef,
     GetReportDefinitionResultTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
     ReportDefinitionTypeDef,
     UpdateReportDefinitionRequestRequestTypeDef,
     ImportApplicationUsageRequestRequestTypeDef,
+    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
     ListReportDefinitionsResultTypeDef,
 )
 
 
-def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
+def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/README.md` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-applicationcostprofiler"></a>
 
 # types-aiobotocore-applicationcostprofiler
 
 [![PyPI - types-aiobotocore-applicationcostprofiler](https://img.shields.io/pypi/v/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-applicationcostprofiler?color=blue)](https://pypistats.org/packages/types-aiobotocore-applicationcostprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationCostProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
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
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
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
@@ -276,46 +276,46 @@
 )
 
 
 def check_value(value: FormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_applicationcostprofiler.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
+    ResponseMetadataTypeDef,
     GetReportDefinitionRequestRequestTypeDef,
     S3LocationTypeDef,
     SourceS3LocationTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListReportDefinitionsRequestRequestTypeDef,
+    DeleteReportDefinitionResultTypeDef,
+    ImportApplicationUsageResultTypeDef,
     PutReportDefinitionResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateReportDefinitionResultTypeDef,
     GetReportDefinitionResultTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
     ReportDefinitionTypeDef,
     UpdateReportDefinitionRequestRequestTypeDef,
     ImportApplicationUsageRequestRequestTypeDef,
+    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
     ListReportDefinitionsResultTypeDef,
 )
 
 
-def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
+def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/setup.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,46 +6,44 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-applicationcostprofiler",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_applicationcostprofiler"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with"
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
-        "aiobotocore applicationcostprofiler type-annotations boto3-stubs mypy typeshed"
-        " autocomplete"
+        "aiobotocore applicationcostprofiler type-annotations botocore mypy typeshed autocomplete"
     ),
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_applicationcostprofiler": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/",
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/__init__.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/__init__.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/__main__.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,28 +6,28 @@
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
         "Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2\nVersion:        "
-        " 2.5.2\nBuilder version: 7.14.5\nDocs:           "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler\nOther"
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

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/client.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/client.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/client.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/literals.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/literals.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/paginator.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -25,31 +25,28 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListReportDefinitionsResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListReportDefinitionsPaginator",)
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListReportDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
         """
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/paginator.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/paginator.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,28 +25,31 @@
 from aiobotocore.paginate import AioPaginator
 from botocore.paginate import PageIterator
 
 from .type_defs import ListReportDefinitionsResultTypeDef, PaginatorConfigTypeDef
 
 __all__ = ("ListReportDefinitionsPaginator",)
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListReportDefinitionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListReportDefinitionsResultTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler.Paginator.ListReportDefinitions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/paginators/#listreportdefinitionspaginator)
         """
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/type_defs.py` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_applicationcostprofiler.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
-    data: DeleteReportDefinitionRequestRequestTypeDef = {...}
+    data: DeleteReportDefinitionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import FormatType, ReportFrequencyType, S3BucketRegionType
@@ -21,45 +21,48 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "DeleteReportDefinitionResultTypeDef",
+    "ResponseMetadataTypeDef",
     "GetReportDefinitionRequestRequestTypeDef",
     "S3LocationTypeDef",
     "SourceS3LocationTypeDef",
-    "ImportApplicationUsageResultTypeDef",
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
-    "ListReportDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ListReportDefinitionsRequestRequestTypeDef",
+    "DeleteReportDefinitionResultTypeDef",
+    "ImportApplicationUsageResultTypeDef",
     "PutReportDefinitionResultTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateReportDefinitionResultTypeDef",
     "GetReportDefinitionResultTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
     "ReportDefinitionTypeDef",
     "UpdateReportDefinitionRequestRequestTypeDef",
     "ImportApplicationUsageRequestRequestTypeDef",
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
     "ListReportDefinitionsResultTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-DeleteReportDefinitionResultTypeDef = TypedDict(
-    "DeleteReportDefinitionResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetReportDefinitionRequestRequestTypeDef = TypedDict(
     "GetReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
@@ -90,87 +93,76 @@
 )
 
 
 class SourceS3LocationTypeDef(_RequiredSourceS3LocationTypeDef, _OptionalSourceS3LocationTypeDef):
     pass
 
 
-ImportApplicationUsageResultTypeDef = TypedDict(
-    "ImportApplicationUsageResultTypeDef",
-    {
-        "importId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
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
 
 ListReportDefinitionsRequestRequestTypeDef = TypedDict(
     "ListReportDefinitionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteReportDefinitionResultTypeDef = TypedDict(
+    "DeleteReportDefinitionResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-PutReportDefinitionResultTypeDef = TypedDict(
-    "PutReportDefinitionResultTypeDef",
+ImportApplicationUsageResultTypeDef = TypedDict(
+    "ImportApplicationUsageResultTypeDef",
     {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "importId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+PutReportDefinitionResultTypeDef = TypedDict(
+    "PutReportDefinitionResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportDefinitionResultTypeDef = TypedDict(
     "UpdateReportDefinitionResultTypeDef",
     {
         "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReportDefinitionResultTypeDef = TypedDict(
     "GetReportDefinitionResultTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
         "destinationS3Location": S3LocationTypeDef,
         "createdAt": datetime,
         "lastUpdated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReportDefinitionRequestRequestTypeDef = TypedDict(
     "PutReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
@@ -209,15 +201,23 @@
 ImportApplicationUsageRequestRequestTypeDef = TypedDict(
     "ImportApplicationUsageRequestRequestTypeDef",
     {
         "sourceS3Location": SourceS3LocationTypeDef,
     },
 )
 
+ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListReportDefinitionsResultTypeDef = TypedDict(
     "ListReportDefinitionsResultTypeDef",
     {
         "reportDefinitions": List[ReportDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler/type_defs.pyi` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler/type_defs.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_applicationcostprofiler.type_defs import DeleteReportDefinitionRequestRequestTypeDef
 
-    data: DeleteReportDefinitionRequestRequestTypeDef = {...}
+    data: DeleteReportDefinitionRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Dict, List
 
 from .literals import FormatType, ReportFrequencyType, S3BucketRegionType
@@ -20,45 +20,48 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "DeleteReportDefinitionRequestRequestTypeDef",
-    "DeleteReportDefinitionResultTypeDef",
+    "ResponseMetadataTypeDef",
     "GetReportDefinitionRequestRequestTypeDef",
     "S3LocationTypeDef",
     "SourceS3LocationTypeDef",
-    "ImportApplicationUsageResultTypeDef",
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
-    "ListReportDefinitionsRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
+    "ListReportDefinitionsRequestRequestTypeDef",
+    "DeleteReportDefinitionResultTypeDef",
+    "ImportApplicationUsageResultTypeDef",
     "PutReportDefinitionResultTypeDef",
-    "ResponseMetadataTypeDef",
     "UpdateReportDefinitionResultTypeDef",
     "GetReportDefinitionResultTypeDef",
     "PutReportDefinitionRequestRequestTypeDef",
     "ReportDefinitionTypeDef",
     "UpdateReportDefinitionRequestRequestTypeDef",
     "ImportApplicationUsageRequestRequestTypeDef",
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
     "ListReportDefinitionsResultTypeDef",
 )
 
 DeleteReportDefinitionRequestRequestTypeDef = TypedDict(
     "DeleteReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
     },
 )
 
-DeleteReportDefinitionResultTypeDef = TypedDict(
-    "DeleteReportDefinitionResultTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 GetReportDefinitionRequestRequestTypeDef = TypedDict(
     "GetReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
@@ -87,87 +90,76 @@
     },
     total=False,
 )
 
 class SourceS3LocationTypeDef(_RequiredSourceS3LocationTypeDef, _OptionalSourceS3LocationTypeDef):
     pass
 
-ImportApplicationUsageResultTypeDef = TypedDict(
-    "ImportApplicationUsageResultTypeDef",
-    {
-        "importId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
-    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
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
 
 ListReportDefinitionsRequestRequestTypeDef = TypedDict(
     "ListReportDefinitionsRequestRequestTypeDef",
     {
         "nextToken": str,
         "maxResults": int,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
+DeleteReportDefinitionResultTypeDef = TypedDict(
+    "DeleteReportDefinitionResultTypeDef",
     {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
-    total=False,
 )
 
-PutReportDefinitionResultTypeDef = TypedDict(
-    "PutReportDefinitionResultTypeDef",
+ImportApplicationUsageResultTypeDef = TypedDict(
+    "ImportApplicationUsageResultTypeDef",
     {
-        "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "importId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
+PutReportDefinitionResultTypeDef = TypedDict(
+    "PutReportDefinitionResultTypeDef",
     {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
+        "reportId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateReportDefinitionResultTypeDef = TypedDict(
     "UpdateReportDefinitionResultTypeDef",
     {
         "reportId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetReportDefinitionResultTypeDef = TypedDict(
     "GetReportDefinitionResultTypeDef",
     {
         "reportId": str,
         "reportDescription": str,
         "reportFrequency": ReportFrequencyType,
         "format": FormatType,
         "destinationS3Location": S3LocationTypeDef,
         "createdAt": datetime,
         "lastUpdated": datetime,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 PutReportDefinitionRequestRequestTypeDef = TypedDict(
     "PutReportDefinitionRequestRequestTypeDef",
     {
         "reportId": str,
@@ -206,15 +198,23 @@
 ImportApplicationUsageRequestRequestTypeDef = TypedDict(
     "ImportApplicationUsageRequestRequestTypeDef",
     {
         "sourceS3Location": SourceS3LocationTypeDef,
     },
 )
 
+ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef = TypedDict(
+    "ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
 ListReportDefinitionsResultTypeDef = TypedDict(
     "ListReportDefinitionsResultTypeDef",
     {
         "reportDefinitions": List[ReportDefinitionTypeDef],
         "nextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-applicationcostprofiler
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.ApplicationCostProfiler 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore applicationcostprofiler type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore applicationcostprofiler type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-applicationcostprofiler"></a>
 
 # types-aiobotocore-applicationcostprofiler
 
 [![PyPI - types-aiobotocore-applicationcostprofiler](https://img.shields.io/pypi/v/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-applicationcostprofiler.svg?color=blue)](https://pypi.org/project/types-aiobotocore-applicationcostprofiler)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-applicationcostprofiler?color=blue)](https://pypistats.org/packages/types-aiobotocore-applicationcostprofiler)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-applicationcostprofiler)](https://pepy.tech/project/types-aiobotocore-applicationcostprofiler)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.ApplicationCostProfiler 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/applicationcostprofiler.html#ApplicationCostProfiler)
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
 [types-aiobotocore-applicationcostprofiler docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_applicationcostprofiler/).
 
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
@@ -309,46 +308,46 @@
 )
 
 
 def check_value(value: FormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_applicationcostprofiler.type_defs` module contains
-structures and shapes assembled to typed dictionaries for additional type
-checking.
+structures and shapes assembled to typed dictionaries and unions for additional
+type checking.
 
 ```python
 from types_aiobotocore_applicationcostprofiler.type_defs import (
     DeleteReportDefinitionRequestRequestTypeDef,
-    DeleteReportDefinitionResultTypeDef,
+    ResponseMetadataTypeDef,
     GetReportDefinitionRequestRequestTypeDef,
     S3LocationTypeDef,
     SourceS3LocationTypeDef,
-    ImportApplicationUsageResultTypeDef,
-    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
-    ListReportDefinitionsRequestRequestTypeDef,
     PaginatorConfigTypeDef,
+    ListReportDefinitionsRequestRequestTypeDef,
+    DeleteReportDefinitionResultTypeDef,
+    ImportApplicationUsageResultTypeDef,
     PutReportDefinitionResultTypeDef,
-    ResponseMetadataTypeDef,
     UpdateReportDefinitionResultTypeDef,
     GetReportDefinitionResultTypeDef,
     PutReportDefinitionRequestRequestTypeDef,
     ReportDefinitionTypeDef,
     UpdateReportDefinitionRequestRequestTypeDef,
     ImportApplicationUsageRequestRequestTypeDef,
+    ListReportDefinitionsRequestListReportDefinitionsPaginateTypeDef,
     ListReportDefinitionsResultTypeDef,
 )
 
 
-def get_structure() -> DeleteReportDefinitionRequestRequestTypeDef:
+def get_value() -> DeleteReportDefinitionRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-applicationcostprofiler-2.5.2/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt` & `types-aiobotocore-applicationcostprofiler-2.5.2.post1/types_aiobotocore_applicationcostprofiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*


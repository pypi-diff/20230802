# Comparing `tmp/types-aiobotocore-timestream-query-2.5.2.tar.gz` & `tmp/types-aiobotocore-timestream-query-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-query-2.5.2.tar", last modified: Sat Jul  8 01:44:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-query-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:06 2023, max compression
```

## Comparing `types-aiobotocore-timestream-query-2.5.2.tar` & `types-aiobotocore-timestream-query-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.198993 types-aiobotocore-timestream-query-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-07-08 01:44:25.198993 types-aiobotocore-timestream-query-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14154 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:25.198993 types-aiobotocore-timestream-query-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.194993 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14555 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14530 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    19477 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19446 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:41:59.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.198993 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14514 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14489 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8881 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21902 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21865 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:34.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:06.965439 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15906 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/LICENSE` & `types-aiobotocore-timestream-query-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2/PKG-INFO` & `types-aiobotocore-timestream-query-2.5.2.post1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-query
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore timestream-query type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore timestream-query type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-timestream-query"></a>
 
 # types-aiobotocore-timestream-query
 
 [![PyPI - types-aiobotocore-timestream-query](https://img.shields.io/pypi/v/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-timestream-query?color=blue)](https://pypistats.org/packages/types-aiobotocore-timestream-query)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TimestreamQuery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [types-aiobotocore-timestream-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/).
 
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
@@ -323,82 +322,88 @@
 )
 
 
 def check_value(value: DimensionValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_timestream_query.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
-    EmptyResponseMetadataTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
-    ExecuteScheduledQueryRequestRequestTypeDef,
+    TimestampTypeDef,
     ExecutionStatsTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ResponseMetadataTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateScheduledQueryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ExecuteScheduledQueryRequestRequestTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    QueryRequestQueryPaginateTypeDef,
+    MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
+    TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
-    CreateScheduledQueryRequestRequestTypeDef,
     ScheduledQueryDescriptionTypeDef,
+    CreateScheduledQueryRequestRequestTypeDef,
+    TargetConfigurationUnionTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
-def get_structure() -> CancelQueryRequestRequestTypeDef:
+def get_value() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/README.md` & `types-aiobotocore-timestream-query-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-timestream-query"></a>
 
 # types-aiobotocore-timestream-query
 
 [![PyPI - types-aiobotocore-timestream-query](https://img.shields.io/pypi/v/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-timestream-query?color=blue)](https://pypistats.org/packages/types-aiobotocore-timestream-query)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TimestreamQuery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [types-aiobotocore-timestream-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/).
 
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
@@ -290,82 +290,88 @@
 )
 
 
 def check_value(value: DimensionValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_timestream_query.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
-    EmptyResponseMetadataTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
-    ExecuteScheduledQueryRequestRequestTypeDef,
+    TimestampTypeDef,
     ExecutionStatsTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ResponseMetadataTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateScheduledQueryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ExecuteScheduledQueryRequestRequestTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    QueryRequestQueryPaginateTypeDef,
+    MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
+    TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
-    CreateScheduledQueryRequestRequestTypeDef,
     ScheduledQueryDescriptionTypeDef,
+    CreateScheduledQueryRequestRequestTypeDef,
+    TargetConfigurationUnionTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
-def get_structure() -> CancelQueryRequestRequestTypeDef:
+def get_value() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/setup.py` & `types-aiobotocore-timestream-query-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-query",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_timestream_query"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with"
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
-    keywords="aiobotocore timestream-query type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore timestream-query type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_timestream_query": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/"
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/__init__.py` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/__init__.pyi` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/__main__.py` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/__main__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TimestreamQuery 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.TimestreamQuery 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery\nOther"
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

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/client.py` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("timestream-query") as client:
         client: TimestreamQueryClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ScheduledQueryStateType
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 from .type_defs import (
@@ -33,15 +32,16 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationTypeDef,
+    TargetConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -116,15 +116,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationTypeDef = ...,
+        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
@@ -159,19 +159,15 @@
         Provides detailed information about a scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_scheduled_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/client/#describe_scheduled_query)
         """
 
     async def execute_scheduled_query(
-        self,
-        *,
-        ScheduledQueryArn: str,
-        InvocationTime: Union[datetime, str],
-        ClientToken: str = ...
+        self, *, ScheduledQueryArn: str, InvocationTime: TimestampTypeDef, ClientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         You can use this API to run a scheduled query manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.execute_scheduled_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/client/#execute_scheduled_query)
         """
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/client.pyi` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 
     session = get_session()
     async with session.create_client("timestream-query") as client:
         client: TimestreamQueryClient
     ```
 """
 import sys
-from datetime import datetime
-from typing import Any, Dict, Mapping, Sequence, Type, Union, overload
+from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from aiobotocore.client import AioBaseClient
 from botocore.client import ClientMeta
 
 from .literals import ScheduledQueryStateType
 from .paginator import ListScheduledQueriesPaginator, ListTagsForResourcePaginator, QueryPaginator
 from .type_defs import (
@@ -33,15 +32,16 @@
     ListScheduledQueriesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    TargetConfigurationTypeDef,
+    TargetConfigurationUnionTypeDef,
+    TimestampTypeDef,
 )
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
@@ -108,15 +108,15 @@
         *,
         Name: str,
         QueryString: str,
         ScheduleConfiguration: ScheduleConfigurationTypeDef,
         NotificationConfiguration: NotificationConfigurationTypeDef,
         ScheduledQueryExecutionRoleArn: str,
         ErrorReportConfiguration: ErrorReportConfigurationTypeDef,
-        TargetConfiguration: TargetConfigurationTypeDef = ...,
+        TargetConfiguration: TargetConfigurationUnionTypeDef = ...,
         ClientToken: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
         KmsKeyId: str = ...
     ) -> CreateScheduledQueryResponseTypeDef:
         """
         Create a scheduled query that will be run on your behalf at the configured
         schedule.
@@ -147,19 +147,15 @@
         """
         Provides detailed information about a scheduled query.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.describe_scheduled_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/client/#describe_scheduled_query)
         """
     async def execute_scheduled_query(
-        self,
-        *,
-        ScheduledQueryArn: str,
-        InvocationTime: Union[datetime, str],
-        ClientToken: str = ...
+        self, *, ScheduledQueryArn: str, InvocationTime: TimestampTypeDef, ClientToken: str = ...
     ) -> EmptyResponseMetadataTypeDef:
         """
         You can use this API to run a scheduled query manually.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Client.execute_scheduled_query)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/client/#execute_scheduled_query)
         """
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/literals.py` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/literals.pyi` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/paginator.py` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,30 +52,30 @@
 class ListScheduledQueriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listscheduledqueriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListScheduledQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listscheduledqueriespaginator)
         """
 
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listtagsforresourcepaginator)
         """
 
 
@@ -86,13 +86,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/paginator.pyi` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -49,29 +49,29 @@
 class ListScheduledQueriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listscheduledqueriespaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListScheduledQueriesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListScheduledQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listscheduledqueriespaginator)
         """
 
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#listtagsforresourcepaginator)
         """
 
 class QueryPaginator(AioPaginator):
@@ -81,13 +81,13 @@
     """
 
     def paginate(
         self,
         *,
         QueryString: str,
         ClientToken: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[QueryResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery.Paginator.Query.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/paginators/#querypaginator)
         """
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/type_defs.py` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_timestream_query.type_defs import CancelQueryRequestRequestTypeDef
 
-    data: CancelQueryRequestRequestTypeDef = {...}
+    data: CancelQueryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
@@ -32,82 +32,91 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
-    "CreateScheduledQueryResponseTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
     "DimensionMappingTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
-    "ExecuteScheduledQueryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ExecutionStatsTypeDef",
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "SnsConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
-    "QueryRequestQueryPaginateTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
-    "ResponseMetadataTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateScheduledQueryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
+    "ExecuteScheduledQueryRequestRequestTypeDef",
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "QueryRequestQueryPaginateTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
+    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "CreateScheduledQueryRequestRequestTypeDef",
     "ScheduledQueryDescriptionTypeDef",
+    "CreateScheduledQueryRequestRequestTypeDef",
+    "TargetConfigurationUnionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CancellationMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Type": Dict[str, Any],
@@ -137,22 +146,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateScheduledQueryResponseTypeDef = TypedDict(
-    "CreateScheduledQueryResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List["DatumTypeDef"],
     },
 )
 
@@ -190,21 +191,14 @@
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ConfigurationTypeDef = TypedDict(
@@ -226,88 +220,46 @@
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
-_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ScheduledQueryArn": str,
-        "InvocationTime": Union[datetime, str],
-    },
-)
-_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-
-class ExecuteScheduledQueryRequestRequestTypeDef(
-    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
-    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
-):
-    pass
-
-
+TimestampTypeDef = Union[datetime, str]
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
         "QueryResultRows": int,
     },
     total=False,
 )
 
-ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
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
 
 ListScheduledQueriesRequestRequestTypeDef = TypedDict(
     "ListScheduledQueriesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -352,24 +304,14 @@
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
     },
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
 ParameterMappingTypeDef = TypedDict(
     "ParameterMappingTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
     },
 )
@@ -403,36 +345,14 @@
         "DatabaseName": str,
         "TableName": str,
         "Aliased": bool,
     },
     total=False,
 )
 
-_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryRequestQueryPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryRequestQueryPaginateTypeDef",
-    {
-        "ClientToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class QueryRequestQueryPaginateTypeDef(
-    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
-):
-    pass
-
-
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -458,25 +378,14 @@
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
     total=False,
 )
 
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
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
     total=False,
@@ -505,20 +414,43 @@
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
 
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
+    {
+        "CancellationMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledQueryResponseTypeDef = TypedDict(
+    "CreateScheduledQueryResponseTypeDef",
+    {
+        "Arn": str,
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -538,15 +470,15 @@
     total=False,
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -557,14 +489,113 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ScheduledQueryArn": str,
+        "InvocationTime": TimestampTypeDef,
+    },
+)
+_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+
+class ExecuteScheduledQueryRequestRequestTypeDef(
+    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
+    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
+):
+    pass
+
+
+ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
+_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryRequestQueryPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryRequestQueryPaginateTypeDef",
+    {
+        "ClientToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class QueryRequestQueryPaginateTypeDef(
+    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
+):
+    pass
+
+
+_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_RequiredMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+    },
+)
+_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_OptionalMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureName": str,
+        "SourceColumn": str,
+        "TargetMeasureName": str,
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+    total=False,
+)
+
+
+class MixedMeasureMappingOutputTypeDef(
+    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
+):
+    pass
+
+
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -581,14 +612,35 @@
 
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
 
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
@@ -615,27 +667,27 @@
 
 PrepareQueryResponseTypeDef = TypedDict(
     "PrepareQueryResponseTypeDef",
     {
         "QueryString": str,
         "Columns": List[SelectColumnTypeDef],
         "Parameters": List[ParameterMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": TimestreamDestinationTypeDef,
@@ -652,14 +704,40 @@
         "ExecutionStats": ExecutionStatsTypeDef,
         "ErrorReportLocation": ErrorReportLocationTypeDef,
         "FailureReason": str,
     },
     total=False,
 )
 
+_RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTimestreamConfigurationOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "TimeColumn": str,
+        "DimensionMappings": List[DimensionMappingTypeDef],
+    },
+)
+_OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTimestreamConfigurationOutputTypeDef",
+    {
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+
+class TimestreamConfigurationOutputTypeDef(
+    _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -704,94 +782,104 @@
 )
 
 
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
 
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
+    },
+)
+
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
+_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
+    "_RequiredScheduledQueryDescriptionTypeDef",
     {
+        "Arn": str,
         "Name": str,
         "QueryString": str,
+        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
+_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
+    "_OptionalScheduledQueryDescriptionTypeDef",
     {
-        "TargetConfiguration": TargetConfigurationTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
+        "PreviousInvocationTime": datetime,
+        "NextInvocationTime": datetime,
+        "TargetConfiguration": TargetConfigurationOutputTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
+        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
 
-class CreateScheduledQueryRequestRequestTypeDef(
-    _RequiredCreateScheduledQueryRequestRequestTypeDef,
-    _OptionalCreateScheduledQueryRequestRequestTypeDef,
+class ScheduledQueryDescriptionTypeDef(
+    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
 
-_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
-    "_RequiredScheduledQueryDescriptionTypeDef",
+_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
-        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
-    "_OptionalScheduledQueryDescriptionTypeDef",
+_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
     {
-        "CreationTime": datetime,
-        "PreviousInvocationTime": datetime,
-        "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
-        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
 
-class ScheduledQueryDescriptionTypeDef(
-    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
+class CreateScheduledQueryRequestRequestTypeDef(
+    _RequiredCreateScheduledQueryRequestRequestTypeDef,
+    _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
 
+TargetConfigurationUnionTypeDef = Union[
+    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query/type_defs.pyi` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_timestream_query.type_defs import CancelQueryRequestRequestTypeDef
 
-    data: CancelQueryRequestRequestTypeDef = {...}
+    data: CancelQueryRequestRequestTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
 from typing import Any, Dict, List, Sequence, Union
 
 from .literals import (
@@ -31,82 +31,91 @@
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 __all__ = (
     "CancelQueryRequestRequestTypeDef",
-    "CancelQueryResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "ColumnInfoTypeDef",
     "ScheduleConfigurationTypeDef",
     "TagTypeDef",
-    "CreateScheduledQueryResponseTypeDef",
     "RowTypeDef",
     "TimeSeriesDataPointTypeDef",
     "DeleteScheduledQueryRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeScheduledQueryRequestRequestTypeDef",
     "DimensionMappingTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "S3ConfigurationTypeDef",
     "S3ReportLocationTypeDef",
-    "ExecuteScheduledQueryRequestRequestTypeDef",
+    "TimestampTypeDef",
     "ExecutionStatsTypeDef",
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "ListScheduledQueriesRequestRequestTypeDef",
-    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "SnsConfigurationTypeDef",
-    "PaginatorConfigTypeDef",
     "ParameterMappingTypeDef",
     "PrepareQueryRequestRequestTypeDef",
     "SelectColumnTypeDef",
-    "QueryRequestQueryPaginateTypeDef",
     "QueryRequestRequestTypeDef",
     "QueryStatusTypeDef",
-    "ResponseMetadataTypeDef",
     "TimestreamDestinationTypeDef",
     "TypeTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateScheduledQueryRequestRequestTypeDef",
+    "CancelQueryResponseTypeDef",
+    "CreateScheduledQueryResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "DatumTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "ErrorReportConfigurationTypeDef",
     "ErrorReportLocationTypeDef",
+    "ExecuteScheduledQueryRequestRequestTypeDef",
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    "ListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    "QueryRequestQueryPaginateTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
     "NotificationConfigurationTypeDef",
     "PrepareQueryResponseTypeDef",
     "QueryResponseTypeDef",
     "TargetDestinationTypeDef",
     "ScheduledQueryRunSummaryTypeDef",
+    "TimestreamConfigurationOutputTypeDef",
     "TimestreamConfigurationTypeDef",
     "ScheduledQueryTypeDef",
+    "TargetConfigurationOutputTypeDef",
     "TargetConfigurationTypeDef",
     "ListScheduledQueriesResponseTypeDef",
-    "CreateScheduledQueryRequestRequestTypeDef",
     "ScheduledQueryDescriptionTypeDef",
+    "CreateScheduledQueryRequestRequestTypeDef",
+    "TargetConfigurationUnionTypeDef",
     "DescribeScheduledQueryResponseTypeDef",
 )
 
 CancelQueryRequestRequestTypeDef = TypedDict(
     "CancelQueryRequestRequestTypeDef",
     {
         "QueryId": str,
     },
 )
 
-CancelQueryResponseTypeDef = TypedDict(
-    "CancelQueryResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "CancellationMessage": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
         "Type": Dict[str, Any],
@@ -134,22 +143,14 @@
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
 
-CreateScheduledQueryResponseTypeDef = TypedDict(
-    "CreateScheduledQueryResponseTypeDef",
-    {
-        "Arn": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List["DatumTypeDef"],
     },
 )
 
@@ -187,21 +188,14 @@
     "DimensionMappingTypeDef",
     {
         "Name": str,
         "DimensionValueType": Literal["VARCHAR"],
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredS3ConfigurationTypeDef = TypedDict(
     "_RequiredS3ConfigurationTypeDef",
     {
         "BucketName": str,
     },
 )
 _OptionalS3ConfigurationTypeDef = TypedDict(
@@ -221,84 +215,46 @@
     {
         "BucketName": str,
         "ObjectKey": str,
     },
     total=False,
 )
 
-_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ScheduledQueryArn": str,
-        "InvocationTime": Union[datetime, str],
-    },
-)
-_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
-    {
-        "ClientToken": str,
-    },
-    total=False,
-)
-
-class ExecuteScheduledQueryRequestRequestTypeDef(
-    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
-    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
-):
-    pass
-
+TimestampTypeDef = Union[datetime, str]
 ExecutionStatsTypeDef = TypedDict(
     "ExecutionStatsTypeDef",
     {
         "ExecutionTimeInMillis": int,
         "DataWrites": int,
         "BytesMetered": int,
         "RecordsIngested": int,
         "QueryResultRows": int,
     },
     total=False,
 )
 
-ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
-    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
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
 
 ListScheduledQueriesRequestRequestTypeDef = TypedDict(
     "ListScheduledQueriesRequestRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
 )
 
-_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceRequestRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceRequestRequestTypeDef = TypedDict(
@@ -339,24 +295,14 @@
 SnsConfigurationTypeDef = TypedDict(
     "SnsConfigurationTypeDef",
     {
         "TopicArn": str,
     },
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
 ParameterMappingTypeDef = TypedDict(
     "ParameterMappingTypeDef",
     {
         "Name": str,
         "Type": "TypeTypeDef",
     },
 )
@@ -388,34 +334,14 @@
         "DatabaseName": str,
         "TableName": str,
         "Aliased": bool,
     },
     total=False,
 )
 
-_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_RequiredQueryRequestQueryPaginateTypeDef",
-    {
-        "QueryString": str,
-    },
-)
-_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
-    "_OptionalQueryRequestQueryPaginateTypeDef",
-    {
-        "ClientToken": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class QueryRequestQueryPaginateTypeDef(
-    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
-):
-    pass
-
 _RequiredQueryRequestRequestTypeDef = TypedDict(
     "_RequiredQueryRequestRequestTypeDef",
     {
         "QueryString": str,
     },
 )
 _OptionalQueryRequestRequestTypeDef = TypedDict(
@@ -439,25 +365,14 @@
         "ProgressPercentage": float,
         "CumulativeBytesScanned": int,
         "CumulativeBytesMetered": int,
     },
     total=False,
 )
 
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
 TimestreamDestinationTypeDef = TypedDict(
     "TimestreamDestinationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
     total=False,
@@ -486,20 +401,43 @@
     "UpdateScheduledQueryRequestRequestTypeDef",
     {
         "ScheduledQueryArn": str,
         "State": ScheduledQueryStateType,
     },
 )
 
+CancelQueryResponseTypeDef = TypedDict(
+    "CancelQueryResponseTypeDef",
+    {
+        "CancellationMessage": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateScheduledQueryResponseTypeDef = TypedDict(
+    "CreateScheduledQueryResponseTypeDef",
+    {
+        "Arn": str,
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
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -519,15 +457,15 @@
     total=False,
 )
 
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ErrorReportConfigurationTypeDef = TypedDict(
     "ErrorReportConfigurationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -538,14 +476,105 @@
     "ErrorReportLocationTypeDef",
     {
         "S3ReportLocation": S3ReportLocationTypeDef,
     },
     total=False,
 )
 
+_RequiredExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ScheduledQueryArn": str,
+        "InvocationTime": TimestampTypeDef,
+    },
+)
+_OptionalExecuteScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalExecuteScheduledQueryRequestRequestTypeDef",
+    {
+        "ClientToken": str,
+    },
+    total=False,
+)
+
+class ExecuteScheduledQueryRequestRequestTypeDef(
+    _RequiredExecuteScheduledQueryRequestRequestTypeDef,
+    _OptionalExecuteScheduledQueryRequestRequestTypeDef,
+):
+    pass
+
+ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef = TypedDict(
+    "ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceRequestListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+_RequiredQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_RequiredQueryRequestQueryPaginateTypeDef",
+    {
+        "QueryString": str,
+    },
+)
+_OptionalQueryRequestQueryPaginateTypeDef = TypedDict(
+    "_OptionalQueryRequestQueryPaginateTypeDef",
+    {
+        "ClientToken": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class QueryRequestQueryPaginateTypeDef(
+    _RequiredQueryRequestQueryPaginateTypeDef, _OptionalQueryRequestQueryPaginateTypeDef
+):
+    pass
+
+_RequiredMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_RequiredMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureValueType": MeasureValueTypeType,
+    },
+)
+_OptionalMixedMeasureMappingOutputTypeDef = TypedDict(
+    "_OptionalMixedMeasureMappingOutputTypeDef",
+    {
+        "MeasureName": str,
+        "SourceColumn": str,
+        "TargetMeasureName": str,
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+    total=False,
+)
+
+class MixedMeasureMappingOutputTypeDef(
+    _RequiredMixedMeasureMappingOutputTypeDef, _OptionalMixedMeasureMappingOutputTypeDef
+):
+    pass
+
 _RequiredMixedMeasureMappingTypeDef = TypedDict(
     "_RequiredMixedMeasureMappingTypeDef",
     {
         "MeasureValueType": MeasureValueTypeType,
     },
 )
 _OptionalMixedMeasureMappingTypeDef = TypedDict(
@@ -560,14 +589,33 @@
 )
 
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+_RequiredMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_RequiredMultiMeasureMappingsOutputTypeDef",
+    {
+        "MultiMeasureAttributeMappings": List[MultiMeasureAttributeMappingTypeDef],
+    },
+)
+_OptionalMultiMeasureMappingsOutputTypeDef = TypedDict(
+    "_OptionalMultiMeasureMappingsOutputTypeDef",
+    {
+        "TargetMultiMeasureName": str,
+    },
+    total=False,
+)
+
+class MultiMeasureMappingsOutputTypeDef(
+    _RequiredMultiMeasureMappingsOutputTypeDef, _OptionalMultiMeasureMappingsOutputTypeDef
+):
+    pass
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
@@ -592,27 +640,27 @@
 
 PrepareQueryResponseTypeDef = TypedDict(
     "PrepareQueryResponseTypeDef",
     {
         "QueryString": str,
         "Columns": List[SelectColumnTypeDef],
         "Parameters": List[ParameterMappingTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryResponseTypeDef = TypedDict(
     "QueryResponseTypeDef",
     {
         "QueryId": str,
         "NextToken": str,
         "Rows": List[RowTypeDef],
         "ColumnInfo": List["ColumnInfoTypeDef"],
         "QueryStatus": QueryStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TargetDestinationTypeDef = TypedDict(
     "TargetDestinationTypeDef",
     {
         "TimestreamDestination": TimestreamDestinationTypeDef,
@@ -629,14 +677,38 @@
         "ExecutionStats": ExecutionStatsTypeDef,
         "ErrorReportLocation": ErrorReportLocationTypeDef,
         "FailureReason": str,
     },
     total=False,
 )
 
+_RequiredTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_RequiredTimestreamConfigurationOutputTypeDef",
+    {
+        "DatabaseName": str,
+        "TableName": str,
+        "TimeColumn": str,
+        "DimensionMappings": List[DimensionMappingTypeDef],
+    },
+)
+_OptionalTimestreamConfigurationOutputTypeDef = TypedDict(
+    "_OptionalTimestreamConfigurationOutputTypeDef",
+    {
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+class TimestreamConfigurationOutputTypeDef(
+    _RequiredTimestreamConfigurationOutputTypeDef, _OptionalTimestreamConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredTimestreamConfigurationTypeDef = TypedDict(
     "_RequiredTimestreamConfigurationTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "TimeColumn": str,
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
@@ -677,90 +749,100 @@
     },
     total=False,
 )
 
 class ScheduledQueryTypeDef(_RequiredScheduledQueryTypeDef, _OptionalScheduledQueryTypeDef):
     pass
 
+TargetConfigurationOutputTypeDef = TypedDict(
+    "TargetConfigurationOutputTypeDef",
+    {
+        "TimestreamConfiguration": TimestreamConfigurationOutputTypeDef,
+    },
+)
+
 TargetConfigurationTypeDef = TypedDict(
     "TargetConfigurationTypeDef",
     {
         "TimestreamConfiguration": TimestreamConfigurationTypeDef,
     },
 )
 
 ListScheduledQueriesResponseTypeDef = TypedDict(
     "ListScheduledQueriesResponseTypeDef",
     {
         "ScheduledQueries": List[ScheduledQueryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
+_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
+    "_RequiredScheduledQueryDescriptionTypeDef",
     {
+        "Arn": str,
         "Name": str,
         "QueryString": str,
+        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
-    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
+_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
+    "_OptionalScheduledQueryDescriptionTypeDef",
     {
-        "TargetConfiguration": TargetConfigurationTypeDef,
-        "ClientToken": str,
-        "Tags": Sequence[TagTypeDef],
+        "CreationTime": datetime,
+        "PreviousInvocationTime": datetime,
+        "NextInvocationTime": datetime,
+        "TargetConfiguration": TargetConfigurationOutputTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
         "KmsKeyId": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
+        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
+        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-class CreateScheduledQueryRequestRequestTypeDef(
-    _RequiredCreateScheduledQueryRequestRequestTypeDef,
-    _OptionalCreateScheduledQueryRequestRequestTypeDef,
+class ScheduledQueryDescriptionTypeDef(
+    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
 ):
     pass
 
-_RequiredScheduledQueryDescriptionTypeDef = TypedDict(
-    "_RequiredScheduledQueryDescriptionTypeDef",
+_RequiredCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_RequiredCreateScheduledQueryRequestRequestTypeDef",
     {
-        "Arn": str,
         "Name": str,
         "QueryString": str,
-        "State": ScheduledQueryStateType,
         "ScheduleConfiguration": ScheduleConfigurationTypeDef,
         "NotificationConfiguration": NotificationConfigurationTypeDef,
+        "ScheduledQueryExecutionRoleArn": str,
+        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
     },
 )
-_OptionalScheduledQueryDescriptionTypeDef = TypedDict(
-    "_OptionalScheduledQueryDescriptionTypeDef",
+_OptionalCreateScheduledQueryRequestRequestTypeDef = TypedDict(
+    "_OptionalCreateScheduledQueryRequestRequestTypeDef",
     {
-        "CreationTime": datetime,
-        "PreviousInvocationTime": datetime,
-        "NextInvocationTime": datetime,
         "TargetConfiguration": TargetConfigurationTypeDef,
-        "ScheduledQueryExecutionRoleArn": str,
+        "ClientToken": str,
+        "Tags": Sequence[TagTypeDef],
         "KmsKeyId": str,
-        "ErrorReportConfiguration": ErrorReportConfigurationTypeDef,
-        "LastRunSummary": ScheduledQueryRunSummaryTypeDef,
-        "RecentlyFailedRuns": List[ScheduledQueryRunSummaryTypeDef],
     },
     total=False,
 )
 
-class ScheduledQueryDescriptionTypeDef(
-    _RequiredScheduledQueryDescriptionTypeDef, _OptionalScheduledQueryDescriptionTypeDef
+class CreateScheduledQueryRequestRequestTypeDef(
+    _RequiredCreateScheduledQueryRequestRequestTypeDef,
+    _OptionalCreateScheduledQueryRequestRequestTypeDef,
 ):
     pass
 
+TargetConfigurationUnionTypeDef = Union[
+    TargetConfigurationTypeDef, TargetConfigurationOutputTypeDef
+]
 DescribeScheduledQueryResponseTypeDef = TypedDict(
     "DescribeScheduledQueryResponseTypeDef",
     {
         "ScheduledQuery": ScheduledQueryDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/PKG-INFO` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-query
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TimestreamQuery 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore timestream-query type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore timestream-query type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-timestream-query"></a>
 
 # types-aiobotocore-timestream-query
 
 [![PyPI - types-aiobotocore-timestream-query](https://img.shields.io/pypi/v/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-query.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-query)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-timestream-query?color=blue)](https://pypistats.org/packages/types-aiobotocore-timestream-query)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-query)](https://pepy.tech/project/types-aiobotocore-timestream-query)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TimestreamQuery 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-query.html#TimestreamQuery)
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
 [types-aiobotocore-timestream-query docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_query/).
 
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
@@ -323,82 +322,88 @@
 )
 
 
 def check_value(value: DimensionValueTypeType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_timestream_query.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_timestream_query.type_defs import (
     CancelQueryRequestRequestTypeDef,
-    CancelQueryResponseTypeDef,
+    ResponseMetadataTypeDef,
     ColumnInfoTypeDef,
     ScheduleConfigurationTypeDef,
     TagTypeDef,
-    CreateScheduledQueryResponseTypeDef,
     RowTypeDef,
     TimeSeriesDataPointTypeDef,
     DeleteScheduledQueryRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeScheduledQueryRequestRequestTypeDef,
     DimensionMappingTypeDef,
-    EmptyResponseMetadataTypeDef,
     S3ConfigurationTypeDef,
     S3ReportLocationTypeDef,
-    ExecuteScheduledQueryRequestRequestTypeDef,
+    TimestampTypeDef,
     ExecutionStatsTypeDef,
-    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    PaginatorConfigTypeDef,
     ListScheduledQueriesRequestRequestTypeDef,
-    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     SnsConfigurationTypeDef,
-    PaginatorConfigTypeDef,
     ParameterMappingTypeDef,
     PrepareQueryRequestRequestTypeDef,
     SelectColumnTypeDef,
-    QueryRequestQueryPaginateTypeDef,
     QueryRequestRequestTypeDef,
     QueryStatusTypeDef,
-    ResponseMetadataTypeDef,
     TimestreamDestinationTypeDef,
     TypeTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateScheduledQueryRequestRequestTypeDef,
+    CancelQueryResponseTypeDef,
+    CreateScheduledQueryResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     DatumTypeDef,
     DescribeEndpointsResponseTypeDef,
     ErrorReportConfigurationTypeDef,
     ErrorReportLocationTypeDef,
+    ExecuteScheduledQueryRequestRequestTypeDef,
+    ListScheduledQueriesRequestListScheduledQueriesPaginateTypeDef,
+    ListTagsForResourceRequestListTagsForResourcePaginateTypeDef,
+    QueryRequestQueryPaginateTypeDef,
+    MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
     NotificationConfigurationTypeDef,
     PrepareQueryResponseTypeDef,
     QueryResponseTypeDef,
     TargetDestinationTypeDef,
     ScheduledQueryRunSummaryTypeDef,
+    TimestreamConfigurationOutputTypeDef,
     TimestreamConfigurationTypeDef,
     ScheduledQueryTypeDef,
+    TargetConfigurationOutputTypeDef,
     TargetConfigurationTypeDef,
     ListScheduledQueriesResponseTypeDef,
-    CreateScheduledQueryRequestRequestTypeDef,
     ScheduledQueryDescriptionTypeDef,
+    CreateScheduledQueryRequestRequestTypeDef,
+    TargetConfigurationUnionTypeDef,
     DescribeScheduledQueryResponseTypeDef,
 )
 
 
-def get_structure() -> CancelQueryRequestRequestTypeDef:
+def get_value() -> CancelQueryRequestRequestTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-timestream-query-2.5.2/types_aiobotocore_timestream_query.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-query-2.5.2.post1/types_aiobotocore_timestream_query.egg-info/SOURCES.txt`

 * *Files identical despite different names*


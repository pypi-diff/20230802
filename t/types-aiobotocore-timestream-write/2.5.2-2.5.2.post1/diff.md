# Comparing `tmp/types-aiobotocore-timestream-write-2.5.2.tar.gz` & `tmp/types-aiobotocore-timestream-write-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-timestream-write-2.5.2.tar", last modified: Sat Jul  8 01:44:25 2023, max compression
+gzip compressed data, was "types-aiobotocore-timestream-write-2.5.2.post1.tar", last modified: Wed Aug  2 14:53:07 2023, max compression
```

## Comparing `types-aiobotocore-timestream-write-2.5.2.tar` & `types-aiobotocore-timestream-write-2.5.2.post1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.450997 types-aiobotocore-timestream-write-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-08 01:44:25.450997 types-aiobotocore-timestream-write-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13309 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:44:25.450997 types-aiobotocore-timestream-write-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.450997 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    16867 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21359 2023-07-08 01:42:01.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21328 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:42:00.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:44:25.450997 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14909 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-08 01:44:25.000000 types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.069438 types-aiobotocore-timestream-write-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-02 14:53:07.065438 types-aiobotocore-timestream-write-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:53:07.069438 types-aiobotocore-timestream-write-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.065438 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16919 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16892 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8756 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8754 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    23940 2023-08-02 14:50:36.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23903 2023-08-02 14:50:36.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:50:35.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:53:07.065438 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 14:53:06.000000 types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/LICENSE` & `types-aiobotocore-timestream-write-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-write-2.5.2/PKG-INFO` & `types-aiobotocore-timestream-write-2.5.2.post1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-write
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore timestream-write type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore timestream-write type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-timestream-write"></a>
 
 # types-aiobotocore-timestream-write
 
 [![PyPI - types-aiobotocore-timestream-write](https://img.shields.io/pypi/v/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-timestream-write?color=blue)](https://pypistats.org/packages/types-aiobotocore-timestream-write)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-write)](https://pepy.tech/project/types-aiobotocore-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TimestreamWrite 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
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
@@ -290,90 +289,97 @@
 )
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_timestream_write.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
     CsvConfigurationTypeDef,
     DataModelS3ConfigurationTypeDef,
     DimensionMappingTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
+    MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
+    DataModelOutputTypeDef,
     DataModelTypeDef,
+    SchemaUnionTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
     UpdateTableRequestRequestTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
 )
 
 
-def get_structure() -> BatchLoadProgressReportTypeDef:
+def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/README.md` & `types-aiobotocore-timestream-write-2.5.2.post1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-timestream-write"></a>
 
 # types-aiobotocore-timestream-write
 
 [![PyPI - types-aiobotocore-timestream-write](https://img.shields.io/pypi/v/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-timestream-write?color=blue)](https://pypistats.org/packages/types-aiobotocore-timestream-write)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-write)](https://pepy.tech/project/types-aiobotocore-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TimestreamWrite 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
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
@@ -257,90 +257,97 @@
 )
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_timestream_write.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
     CsvConfigurationTypeDef,
     DataModelS3ConfigurationTypeDef,
     DimensionMappingTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
+    MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
+    DataModelOutputTypeDef,
     DataModelTypeDef,
+    SchemaUnionTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
     UpdateTableRequestRequestTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
 )
 
 
-def get_structure() -> BatchLoadProgressReportTypeDef:
+def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/setup.py` & `types-aiobotocore-timestream-write-2.5.2.post1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-timestream-write",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with"
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
-    keywords="aiobotocore timestream-write type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore timestream-write type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_timestream_write": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/"
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/__main__.py` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.TimestreamWrite 2.5.2\nVersion:         2.5.2\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.TimestreamWrite 2.5.2\nVersion:        "
+        " 2.5.2.post1\nBuilder version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write//\nBoto3"
         " docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
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

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/client.py` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from botocore.client import ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
-    DataModelConfigurationTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -107,15 +107,15 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: DataModelConfigurationTypeDef = ...,
+        DataModelConfiguration: DataModelConfigurationUnionTypeDef = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_batch_load_task)
@@ -135,15 +135,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_table)
         """
@@ -301,15 +301,15 @@
     async def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#update_table)
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/client.pyi` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 from botocore.client import ClientMeta
 
 from .literals import BatchLoadStatusType
 from .type_defs import (
     CreateBatchLoadTaskResponseTypeDef,
     CreateDatabaseResponseTypeDef,
     CreateTableResponseTypeDef,
-    DataModelConfigurationTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     DescribeEndpointsResponseTypeDef,
     DescribeTableResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaTypeDef,
+    SchemaUnionTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -101,15 +101,15 @@
         self,
         *,
         DataSourceConfiguration: DataSourceConfigurationTypeDef,
         ReportConfiguration: ReportConfigurationTypeDef,
         TargetDatabaseName: str,
         TargetTableName: str,
         ClientToken: str = ...,
-        DataModelConfiguration: DataModelConfigurationTypeDef = ...,
+        DataModelConfiguration: DataModelConfigurationUnionTypeDef = ...,
         RecordVersion: int = ...
     ) -> CreateBatchLoadTaskResponseTypeDef:
         """
         Creates a new Timestream batch load task.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_batch_load_task)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_batch_load_task)
@@ -127,15 +127,15 @@
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#create_table)
         """
@@ -277,15 +277,15 @@
     async def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        Schema: SchemaUnionTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/client/#update_table)
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/literals.py` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/literals.pyi` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/type_defs.py` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
-    data: BatchLoadProgressReportTypeDef = {...}
+    data: BatchLoadProgressReportTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
     PartitionKeyEnforcementLevelType,
     PartitionKeyTypeType,
     S3EncryptionOptionType,
@@ -31,78 +31,84 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
-    "CreateBatchLoadTaskResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
     "CsvConfigurationTypeDef",
     "DataModelS3ConfigurationTypeDef",
     "DimensionMappingTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
     "ReportS3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
+    "CreateBatchLoadTaskResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
+    "DataModelOutputTypeDef",
     "DataModelTypeDef",
+    "SchemaUnionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
+    "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
+    "DataModelConfigurationUnionTypeDef",
     "DescribeBatchLoadTaskResponseTypeDef",
 )
 
 BatchLoadProgressReportTypeDef = TypedDict(
     "BatchLoadProgressReportTypeDef",
     {
         "RecordsProcessed": int,
@@ -125,19 +131,22 @@
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
     },
     total=False,
 )
 
-CreateBatchLoadTaskResponseTypeDef = TypedDict(
-    "CreateBatchLoadTaskResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "TaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -206,21 +215,19 @@
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
-
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
-
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -273,26 +280,17 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
-
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
-
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -356,21 +354,19 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-
 _RequiredPartitionKeyTypeDef = TypedDict(
     "_RequiredPartitionKeyTypeDef",
     {
         "Type": PartitionKeyTypeType,
     },
 )
 _OptionalPartitionKeyTypeDef = TypedDict(
@@ -378,19 +374,17 @@
     {
         "Name": str,
         "EnforcementInRecord": PartitionKeyEnforcementLevelType,
     },
     total=False,
 )
 
-
 class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
     pass
 
-
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
@@ -409,32 +403,19 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
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
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
@@ -450,20 +431,35 @@
     "UpdateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "KmsKeyId": str,
     },
 )
 
+CreateBatchLoadTaskResponseTypeDef = TypedDict(
+    "CreateBatchLoadTaskResponseTypeDef",
+    {
+        "TaskId": str,
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
 ListBatchLoadTasksResponseTypeDef = TypedDict(
     "ListBatchLoadTasksResponseTypeDef",
     {
         "NextToken": str,
         "BatchLoadTasks": List[BatchLoadTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -474,26 +470,24 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -501,40 +495,40 @@
     },
 )
 
 CreateDatabaseResponseTypeDef = TypedDict(
     "CreateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatabaseResponseTypeDef = TypedDict(
     "DescribeDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesResponseTypeDef = TypedDict(
     "ListDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDatabaseResponseTypeDef = TypedDict(
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
@@ -545,26 +539,24 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
-
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -583,14 +575,36 @@
         "TimeUnit": TimeUnitType,
         "Version": int,
         "MeasureValues": Sequence[MeasureValueTypeDef],
     },
     total=False,
 )
 
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
@@ -600,20 +614,37 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
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
 
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
@@ -621,34 +652,40 @@
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
+    {
+        "CompositePartitionKey": List[PartitionKeyTypeDef],
+    },
+    total=False,
+)
 
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
     },
     total=False,
 )
 
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
@@ -666,21 +703,19 @@
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
-
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
-
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -689,20 +724,39 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
-
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
+_RequiredDataModelOutputTypeDef = TypedDict(
+    "_RequiredDataModelOutputTypeDef",
+    {
+        "DimensionMappings": List[DimensionMappingTypeDef],
+    },
+)
+_OptionalDataModelOutputTypeDef = TypedDict(
+    "_OptionalDataModelOutputTypeDef",
+    {
+        "TimeColumn": str,
+        "TimeUnit": TimeUnitType,
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
+    pass
 
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
@@ -714,19 +768,18 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
-
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -737,33 +790,31 @@
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-
 TableTypeDef = TypedDict(
     "TableTypeDef",
     {
         "Arn": str,
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
+        "Schema": SchemaOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -777,72 +828,79 @@
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+DataModelConfigurationOutputTypeDef = TypedDict(
+    "DataModelConfigurationOutputTypeDef",
+    {
+        "DataModel": DataModelOutputTypeDef,
+        "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
+    },
+    total=False,
+)
 
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
 )
 
 CreateTableResponseTypeDef = TypedDict(
     "CreateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "Tables": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableResponseTypeDef = TypedDict(
     "UpdateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
         "ReportConfiguration": ReportConfigurationTypeDef,
-        "DataModelConfiguration": DataModelConfigurationTypeDef,
+        "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
@@ -865,22 +923,23 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
-
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
-
+DataModelConfigurationUnionTypeDef = Union[
+    DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
+]
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write/type_defs.pyi` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_timestream_write.type_defs import BatchLoadProgressReportTypeDef
 
-    data: BatchLoadProgressReportTypeDef = {...}
+    data: BatchLoadProgressReportTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Dict, List, Sequence
+from typing import Dict, List, Sequence, Union
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
     PartitionKeyEnforcementLevelType,
     PartitionKeyTypeType,
     S3EncryptionOptionType,
@@ -31,77 +31,85 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
-    "CreateBatchLoadTaskResponseTypeDef",
+    "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
     "CsvConfigurationTypeDef",
     "DataModelS3ConfigurationTypeDef",
     "DimensionMappingTypeDef",
     "DataSourceS3ConfigurationTypeDef",
     "DeleteDatabaseRequestRequestTypeDef",
     "DeleteTableRequestRequestTypeDef",
     "DescribeBatchLoadTaskRequestRequestTypeDef",
     "DescribeDatabaseRequestRequestTypeDef",
     "EndpointTypeDef",
     "DescribeTableRequestRequestTypeDef",
     "DimensionTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
     "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
     "ReportS3ConfigurationTypeDef",
-    "ResponseMetadataTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
+    "CreateBatchLoadTaskResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
     "ListBatchLoadTasksResponseTypeDef",
     "CreateDatabaseRequestRequestTypeDef",
     "ListTagsForResourceResponseTypeDef",
     "TagResourceRequestRequestTypeDef",
     "CreateDatabaseResponseTypeDef",
     "DescribeDatabaseResponseTypeDef",
     "ListDatabasesResponseTypeDef",
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
+    "MixedMeasureMappingOutputTypeDef",
     "MixedMeasureMappingTypeDef",
+    "MultiMeasureMappingsOutputTypeDef",
     "MultiMeasureMappingsTypeDef",
+    "SchemaOutputTypeDef",
     "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
+    "DataModelOutputTypeDef",
     "DataModelTypeDef",
+    "SchemaUnionTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
     "UpdateTableRequestRequestTypeDef",
+    "DataModelConfigurationOutputTypeDef",
     "DataModelConfigurationTypeDef",
     "CreateTableResponseTypeDef",
     "DescribeTableResponseTypeDef",
     "ListTablesResponseTypeDef",
     "UpdateTableResponseTypeDef",
     "BatchLoadTaskDescriptionTypeDef",
     "CreateBatchLoadTaskRequestRequestTypeDef",
+    "DataModelConfigurationUnionTypeDef",
     "DescribeBatchLoadTaskResponseTypeDef",
 )
 
 BatchLoadProgressReportTypeDef = TypedDict(
     "BatchLoadProgressReportTypeDef",
     {
         "RecordsProcessed": int,
@@ -124,19 +132,22 @@
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
     },
     total=False,
 )
 
-CreateBatchLoadTaskResponseTypeDef = TypedDict(
-    "CreateBatchLoadTaskResponseTypeDef",
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
     {
-        "TaskId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
     },
 )
 
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
@@ -205,19 +216,21 @@
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
+
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
+
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -270,23 +283,18 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
+
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
 
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
@@ -351,19 +359,21 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
+
 _RequiredPartitionKeyTypeDef = TypedDict(
     "_RequiredPartitionKeyTypeDef",
     {
         "Type": PartitionKeyTypeType,
     },
 )
 _OptionalPartitionKeyTypeDef = TypedDict(
@@ -371,17 +381,19 @@
     {
         "Name": str,
         "EnforcementInRecord": PartitionKeyEnforcementLevelType,
     },
     total=False,
 )
 
+
 class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
     pass
 
+
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
@@ -400,29 +412,20 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
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
 
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
@@ -439,20 +442,35 @@
     "UpdateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "KmsKeyId": str,
     },
 )
 
+CreateBatchLoadTaskResponseTypeDef = TypedDict(
+    "CreateBatchLoadTaskResponseTypeDef",
+    {
+        "TaskId": str,
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
 ListBatchLoadTasksResponseTypeDef = TypedDict(
     "ListBatchLoadTasksResponseTypeDef",
     {
         "NextToken": str,
         "BatchLoadTasks": List[BatchLoadTaskTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateDatabaseRequestRequestTypeDef = TypedDict(
     "_RequiredCreateDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
@@ -463,24 +481,26 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceARN": str,
@@ -488,40 +508,40 @@
     },
 )
 
 CreateDatabaseResponseTypeDef = TypedDict(
     "CreateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeDatabaseResponseTypeDef = TypedDict(
     "DescribeDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesResponseTypeDef = TypedDict(
     "ListDatabasesResponseTypeDef",
     {
         "Databases": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateDatabaseResponseTypeDef = TypedDict(
     "UpdateDatabaseResponseTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredDataSourceConfigurationTypeDef = TypedDict(
     "_RequiredDataSourceConfigurationTypeDef",
     {
         "DataSourceS3Configuration": DataSourceS3ConfigurationTypeDef,
@@ -532,24 +552,26 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 MagneticStoreRejectedDataLocationTypeDef = TypedDict(
     "MagneticStoreRejectedDataLocationTypeDef",
     {
         "S3Configuration": S3ConfigurationTypeDef,
@@ -568,14 +590,38 @@
         "TimeUnit": TimeUnitType,
         "Version": int,
         "MeasureValues": Sequence[MeasureValueTypeDef],
     },
     total=False,
 )
 
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
@@ -585,51 +631,84 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+
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
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
+
+SchemaOutputTypeDef = TypedDict(
+    "SchemaOutputTypeDef",
+    {
+        "CompositePartitionKey": List[PartitionKeyTypeDef],
+    },
+    total=False,
+)
+
 SchemaTypeDef = TypedDict(
     "SchemaTypeDef",
     {
         "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
     },
     total=False,
 )
 
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ReportConfigurationTypeDef = TypedDict(
     "ReportConfigurationTypeDef",
     {
         "ReportS3Configuration": ReportS3ConfigurationTypeDef,
@@ -647,19 +726,21 @@
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
+
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
+
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -668,19 +749,44 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
+
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
+
+_RequiredDataModelOutputTypeDef = TypedDict(
+    "_RequiredDataModelOutputTypeDef",
+    {
+        "DimensionMappings": List[DimensionMappingTypeDef],
+    },
+)
+_OptionalDataModelOutputTypeDef = TypedDict(
+    "_OptionalDataModelOutputTypeDef",
+    {
+        "TimeColumn": str,
+        "TimeUnit": TimeUnitType,
+        "MultiMeasureMappings": MultiMeasureMappingsOutputTypeDef,
+        "MixedMeasureMappings": List[MixedMeasureMappingOutputTypeDef],
+        "MeasureNameColumn": str,
+    },
+    total=False,
+)
+
+
+class DataModelOutputTypeDef(_RequiredDataModelOutputTypeDef, _OptionalDataModelOutputTypeDef):
+    pass
+
+
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -691,17 +797,20 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
+
+SchemaUnionTypeDef = Union[SchemaTypeDef, SchemaOutputTypeDef]
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
@@ -712,31 +821,33 @@
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+
 TableTypeDef = TypedDict(
     "TableTypeDef",
     {
         "Arn": str,
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
+        "Schema": SchemaOutputTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -750,70 +861,81 @@
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
         "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+
+DataModelConfigurationOutputTypeDef = TypedDict(
+    "DataModelConfigurationOutputTypeDef",
+    {
+        "DataModel": DataModelOutputTypeDef,
+        "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
+    },
+    total=False,
+)
+
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
 )
 
 CreateTableResponseTypeDef = TypedDict(
     "CreateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeTableResponseTypeDef = TypedDict(
     "DescribeTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTablesResponseTypeDef = TypedDict(
     "ListTablesResponseTypeDef",
     {
         "Tables": List[TableTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateTableResponseTypeDef = TypedDict(
     "UpdateTableResponseTypeDef",
     {
         "Table": TableTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchLoadTaskDescriptionTypeDef = TypedDict(
     "BatchLoadTaskDescriptionTypeDef",
     {
         "TaskId": str,
         "ErrorMessage": str,
         "DataSourceConfiguration": DataSourceConfigurationTypeDef,
         "ProgressReport": BatchLoadProgressReportTypeDef,
         "ReportConfiguration": ReportConfigurationTypeDef,
-        "DataModelConfiguration": DataModelConfigurationTypeDef,
+        "DataModelConfiguration": DataModelConfigurationOutputTypeDef,
         "TargetDatabaseName": str,
         "TargetTableName": str,
         "TaskStatus": BatchLoadStatusType,
         "RecordVersion": int,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "ResumableUntil": datetime,
@@ -836,20 +958,25 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
+
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
+
+DataModelConfigurationUnionTypeDef = Union[
+    DataModelConfigurationTypeDef, DataModelConfigurationOutputTypeDef
+]
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/PKG-INFO` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-timestream-write
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.TimestreamWrite 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore timestream-write type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore timestream-write type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-timestream-write"></a>
 
 # types-aiobotocore-timestream-write
 
 [![PyPI - types-aiobotocore-timestream-write](https://img.shields.io/pypi/v/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-timestream-write.svg?color=blue)](https://pypi.org/project/types-aiobotocore-timestream-write)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-timestream-write?color=blue)](https://pypistats.org/packages/types-aiobotocore-timestream-write)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-timestream-write)](https://pepy.tech/project/types-aiobotocore-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.TimestreamWrite 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
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
 [types-aiobotocore-timestream-write docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_timestream_write/).
 
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
@@ -290,90 +289,97 @@
 )
 
 
 def check_value(value: BatchLoadDataFormatType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_timestream_write.type_defs` module contains structures and
-shapes assembled to typed dictionaries for additional type checking.
+shapes assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_timestream_write.type_defs import (
     BatchLoadProgressReportTypeDef,
     BatchLoadTaskTypeDef,
-    CreateBatchLoadTaskResponseTypeDef,
+    ResponseMetadataTypeDef,
     TagTypeDef,
     DatabaseTypeDef,
     RetentionPropertiesTypeDef,
     CsvConfigurationTypeDef,
     DataModelS3ConfigurationTypeDef,
     DimensionMappingTypeDef,
     DataSourceS3ConfigurationTypeDef,
     DeleteDatabaseRequestRequestTypeDef,
     DeleteTableRequestRequestTypeDef,
     DescribeBatchLoadTaskRequestRequestTypeDef,
     DescribeDatabaseRequestRequestTypeDef,
     EndpointTypeDef,
     DescribeTableRequestRequestTypeDef,
     DimensionTypeDef,
-    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
     PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
-    ResponseMetadataTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
+    CreateBatchLoadTaskResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
     ListBatchLoadTasksResponseTypeDef,
     CreateDatabaseRequestRequestTypeDef,
     ListTagsForResourceResponseTypeDef,
     TagResourceRequestRequestTypeDef,
     CreateDatabaseResponseTypeDef,
     DescribeDatabaseResponseTypeDef,
     ListDatabasesResponseTypeDef,
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
+    MixedMeasureMappingOutputTypeDef,
     MixedMeasureMappingTypeDef,
+    MultiMeasureMappingsOutputTypeDef,
     MultiMeasureMappingsTypeDef,
+    SchemaOutputTypeDef,
     SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
+    DataModelOutputTypeDef,
     DataModelTypeDef,
+    SchemaUnionTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
     UpdateTableRequestRequestTypeDef,
+    DataModelConfigurationOutputTypeDef,
     DataModelConfigurationTypeDef,
     CreateTableResponseTypeDef,
     DescribeTableResponseTypeDef,
     ListTablesResponseTypeDef,
     UpdateTableResponseTypeDef,
     BatchLoadTaskDescriptionTypeDef,
     CreateBatchLoadTaskRequestRequestTypeDef,
+    DataModelConfigurationUnionTypeDef,
     DescribeBatchLoadTaskResponseTypeDef,
 )
 
 
-def get_structure() -> BatchLoadProgressReportTypeDef:
+def get_value() -> BatchLoadProgressReportTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-timestream-write-2.5.2/types_aiobotocore_timestream_write.egg-info/SOURCES.txt` & `types-aiobotocore-timestream-write-2.5.2.post1/types_aiobotocore_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*


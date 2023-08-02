# Comparing `tmp/types-aiobotocore-athena-2.5.2.tar.gz` & `tmp/types-aiobotocore-athena-2.5.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-aiobotocore-athena-2.5.2.tar", last modified: Sat Jul  8 01:43:16 2023, max compression
+gzip compressed data, was "types-aiobotocore-athena-2.5.2.post1.tar", last modified: Wed Aug  2 14:51:55 2023, max compression
```

## Comparing `types-aiobotocore-athena-2.5.2.tar` & `types-aiobotocore-athena-2.5.2.post1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.633733 types-aiobotocore-athena-2.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-07-08 01:43:16.633733 types-aiobotocore-athena-2.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    19764 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 01:43:16.633733 types-aiobotocore-athena-2.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.633733 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48904 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    48820 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8695 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    62824 2023-07-08 01:26:06.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    62735 2023-07-08 01:26:05.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-08 01:26:04.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 01:43:16.633733 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    21325 2023-07-08 01:43:16.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-08 01:43:16.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 01:43:16.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 01:43:16.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 01:43:16.000000 types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    19895 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2065 2023-08-02 14:33:30.000000 types-aiobotocore-athena-2.5.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.069648 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48924 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48840 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8690 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8681 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    63863 2023-08-02 14:33:33.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63772 2023-08-02 14:33:32.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 14:33:31.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:51:55.073649 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    21409 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-02 14:51:54.000000 types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/top_level.txt
```

### Comparing `types-aiobotocore-athena-2.5.2/LICENSE` & `types-aiobotocore-athena-2.5.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2/PKG-INFO` & `types-aiobotocore-athena-2.5.2.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-athena
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore athena type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore athena type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-athena"></a>
 
 # types-aiobotocore-athena
 
 [![PyPI - types-aiobotocore-athena](https://img.shields.io/pypi/v/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-athena?color=blue)](https://pypistats.org/packages/types-aiobotocore-athena)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Athena 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [types-aiobotocore-athena docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/).
 
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
@@ -350,187 +349,191 @@
 )
 
 
 def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_athena.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
     CancelCapacityReservationInputRequestTypeDef,
     CapacityAllocationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
-    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
-    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
     GetCapacityAssignmentConfigurationInputRequestTypeDef,
     GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
-    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
     ListCapacityReservationsInputRequestTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
-    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
-    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
-    ResponseMetadataTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
-    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
+    CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListNamedQueriesOutputTypeDef,
+    ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
-    PutCapacityAssignmentConfigurationInputRequestTypeDef,
+    CapacityAssignmentUnionTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
     SessionConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -544,15 +547,15 @@
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_value() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-athena-2.5.2/README.md` & `types-aiobotocore-athena-2.5.2.post1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="types-aiobotocore-athena"></a>
 
 # types-aiobotocore-athena
 
 [![PyPI - types-aiobotocore-athena](https://img.shields.io/pypi/v/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-athena?color=blue)](https://pypistats.org/packages/types-aiobotocore-athena)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Athena 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [types-aiobotocore-athena docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/).
 
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
@@ -317,187 +317,191 @@
 )
 
 
 def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_athena.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
     CancelCapacityReservationInputRequestTypeDef,
     CapacityAllocationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
-    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
-    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
     GetCapacityAssignmentConfigurationInputRequestTypeDef,
     GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
-    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
     ListCapacityReservationsInputRequestTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
-    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
-    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
-    ResponseMetadataTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
-    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
+    CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListNamedQueriesOutputTypeDef,
+    ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
-    PutCapacityAssignmentConfigurationInputRequestTypeDef,
+    CapacityAssignmentUnionTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
     SessionConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -511,15 +515,15 @@
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_value() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-athena-2.5.2/setup.py` & `types-aiobotocore-athena-2.5.2.post1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="types-aiobotocore-athena",
-    version="2.5.2",
+    version="2.5.2.post1",
     packages=["types_aiobotocore_athena"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
         "Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder"
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
-    keywords="aiobotocore athena type-annotations boto3-stubs mypy typeshed autocomplete",
+    keywords="aiobotocore athena type-annotations botocore mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     package_data={"types_aiobotocore_athena": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": (
             "https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/"
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/__init__.py` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/__init__.pyi` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/__main__.py` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for aiobotocore.Athena 2.5.2\nVersion:         2.5.2\nBuilder version:"
-        " 7.14.5\nDocs:           "
+        "Type annotations for aiobotocore.Athena 2.5.2\nVersion:         2.5.2.post1\nBuilder"
+        " version: 7.17.1\nDocs:           "
         " https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena//\nBoto3 docs: "
         "     https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena\nOther"
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

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/client.py` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentTypeDef,
+    CapacityAssignmentUnionTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -730,15 +730,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_work_groups)
         """
 
     async def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#put_capacity_assignment_configuration)
@@ -778,15 +778,15 @@
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_query_execution)
         """
 
     async def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationTypeDef,
+        EngineConfiguration: EngineConfigurationUnionTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/client.pyi` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     ListTagsForResourcePaginator,
 )
 from .type_defs import (
     BatchGetNamedQueryOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     CalculationConfigurationTypeDef,
-    CapacityAssignmentTypeDef,
+    CapacityAssignmentUnionTypeDef,
     CreateNamedQueryOutputTypeDef,
     CreateNotebookOutputTypeDef,
     CreatePresignedNotebookUrlResponseTypeDef,
-    EngineConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     ExportNotebookOutputTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
     GetCapacityReservationOutputTypeDef,
@@ -670,15 +670,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.list_work_groups)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#list_work_groups)
         """
     async def put_capacity_assignment_configuration(
         self,
         *,
         CapacityReservationName: str,
-        CapacityAssignments: Sequence[CapacityAssignmentTypeDef]
+        CapacityAssignments: Sequence[CapacityAssignmentUnionTypeDef]
     ) -> Dict[str, Any]:
         """
         Puts a new capacity assignment configuration for a specified capacity
         reservation.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.put_capacity_assignment_configuration)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#put_capacity_assignment_configuration)
@@ -715,15 +715,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Client.start_query_execution)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/client/#start_query_execution)
         """
     async def start_session(
         self,
         *,
         WorkGroup: str,
-        EngineConfiguration: EngineConfigurationTypeDef,
+        EngineConfiguration: EngineConfigurationUnionTypeDef,
         Description: str = ...,
         NotebookVersion: str = ...,
         SessionIdleTimeoutInMinutes: int = ...,
         ClientRequestToken: str = ...
     ) -> StartSessionResponseTypeDef:
         """
         Creates a session for running calculations within a workgroup.
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/literals.py` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.py`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/literals.pyi` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/literals.pyi`

 * *Files identical despite different names*

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/paginator.py` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -54,126 +54,117 @@
     "ListDatabasesPaginator",
     "ListNamedQueriesPaginator",
     "ListQueryExecutionsPaginator",
     "ListTableMetadataPaginator",
     "ListTagsForResourcePaginator",
 )
 
-
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class GetQueryResultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#getqueryresultspaginator)
     """
 
     def paginate(
-        self, *, QueryExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetQueryResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#getqueryresultspaginator)
         """
 
-
 class ListDataCatalogsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatacatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataCatalogsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatacatalogspaginator)
         """
 
-
 class ListDatabasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatabasespaginator)
     """
 
     def paginate(
-        self, *, CatalogName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CatalogName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatabasespaginator)
         """
 
-
 class ListNamedQueriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listnamedqueriespaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNamedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listnamedqueriespaginator)
         """
 
-
 class ListQueryExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listqueryexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQueryExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listqueryexecutionspaginator)
         """
 
-
 class ListTableMetadataPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtablemetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtablemetadatapaginator)
         """
 
-
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/paginator.pyi` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,117 +54,126 @@
     "ListDatabasesPaginator",
     "ListNamedQueriesPaginator",
     "ListQueryExecutionsPaginator",
     "ListTableMetadataPaginator",
     "ListTagsForResourcePaginator",
 )
 
+
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class GetQueryResultsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#getqueryresultspaginator)
     """
 
     def paginate(
-        self, *, QueryExecutionId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, QueryExecutionId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[GetQueryResultsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.GetQueryResults.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#getqueryresultspaginator)
         """
 
+
 class ListDataCatalogsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatacatalogspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDataCatalogsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDataCatalogs.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatacatalogspaginator)
         """
 
+
 class ListDatabasesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatabasespaginator)
     """
 
     def paginate(
-        self, *, CatalogName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, CatalogName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListDatabasesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListDatabases.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listdatabasespaginator)
         """
 
+
 class ListNamedQueriesPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listnamedqueriespaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListNamedQueriesOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListNamedQueries.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listnamedqueriespaginator)
         """
 
+
 class ListQueryExecutionsPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listqueryexecutionspaginator)
     """
 
     def paginate(
-        self, *, WorkGroup: str = ..., PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, WorkGroup: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListQueryExecutionsOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListQueryExecutions.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listqueryexecutionspaginator)
         """
 
+
 class ListTableMetadataPaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtablemetadatapaginator)
     """
 
     def paginate(
         self,
         *,
         CatalogName: str,
         DatabaseName: str,
         Expression: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTableMetadataOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTableMetadata.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtablemetadatapaginator)
         """
 
+
 class ListTagsForResourcePaginator(AioPaginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource)
     [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtagsforresourcepaginator)
     """
 
     def paginate(
-        self, *, ResourceARN: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, ResourceARN: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> AsyncIterator[ListTagsForResourceOutputTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena.Paginator.ListTagsForResource.paginate)
         [Show types-aiobotocore documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/paginators/#listtagsforresourcepaginator)
         """
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/type_defs.py` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_athena.type_defs import AclConfigurationTypeDef
 
-    data: AclConfigurationTypeDef = {...}
+    data: AclConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -42,173 +42,177 @@
 
 __all__ = (
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
+    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
-    "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
-    "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
-    "CreatePresignedNotebookUrlResponseTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
-    "GetCalculationExecutionCodeResponseTypeDef",
     "GetCalculationExecutionRequestRequestTypeDef",
     "GetCalculationExecutionStatusRequestRequestTypeDef",
     "GetCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetCapacityReservationInputRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
     "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
-    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "SessionStatisticsTypeDef",
     "SessionStatusTypeDef",
     "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
     "ImportNotebookInputRequestTypeDef",
-    "ImportNotebookOutputTypeDef",
     "ListApplicationDPUSizesInputRequestTypeDef",
     "ListCalculationExecutionsRequestRequestTypeDef",
     "ListCapacityReservationsInputRequestTypeDef",
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
     "ListExecutorsRequestRequestTypeDef",
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
-    "ListNamedQueriesOutputTypeDef",
     "ListNotebookSessionsRequestRequestTypeDef",
     "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
-    "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
-    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
-    "ResponseMetadataTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
-    "StartCalculationExecutionResponseTypeDef",
-    "StartQueryExecutionOutputTypeDef",
-    "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
-    "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCapacityReservationInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
     "UpdateNotebookInputRequestTypeDef",
     "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
-    "ListApplicationDPUSizesOutputTypeDef",
     "QueryExecutionStatusTypeDef",
+    "CreateNamedQueryOutputTypeDef",
+    "CreateNotebookOutputTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
+    "ImportNotebookOutputTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
+    "ListNamedQueriesOutputTypeDef",
+    "ListQueryExecutionsOutputTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
+    "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    "CapacityAssignmentUnionTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
+    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
+    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -278,14 +282,25 @@
 )
 
 
 class NamedQueryTypeDef(_RequiredNamedQueryTypeDef, _OptionalNamedQueryTypeDef):
     pass
 
 
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
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -404,18 +419,26 @@
 
 class CapacityAllocationTypeDef(
     _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
 ):
     pass
 
 
+CapacityAssignmentOutputTypeDef = TypedDict(
+    "CapacityAssignmentOutputTypeDef",
+    {
+        "WorkGroupNames": List[str],
+    },
+    total=False,
+)
+
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": List[str],
+        "WorkGroupNames": Sequence[str],
     },
     total=False,
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
@@ -493,22 +516,14 @@
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
 
-CreateNamedQueryOutputTypeDef = TypedDict(
-    "CreateNamedQueryOutputTypeDef",
-    {
-        "NamedQueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateNotebookInputRequestTypeDef = TypedDict(
     "_RequiredCreateNotebookInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Name": str,
     },
 )
@@ -523,22 +538,14 @@
 
 class CreateNotebookInputRequestTypeDef(
     _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
 ):
     pass
 
 
-CreateNotebookOutputTypeDef = TypedDict(
-    "CreateNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -562,24 +569,14 @@
 CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    {
-        "NotebookUrl": str,
-        "AuthToken": str,
-        "AuthTokenExpirationTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -715,27 +712,51 @@
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
 
+_RequiredEngineConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEngineConfigurationOutputTypeDef",
+    {
+        "MaxConcurrentDpus": int,
+    },
+)
+_OptionalEngineConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEngineConfigurationOutputTypeDef",
+    {
+        "CoordinatorDpuSize": int,
+        "DefaultExecutorDpuSize": int,
+        "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+
+class EngineConfigurationOutputTypeDef(
+    _RequiredEngineConfigurationOutputTypeDef, _OptionalEngineConfigurationOutputTypeDef
+):
+    pass
+
+
 _RequiredEngineConfigurationTypeDef = TypedDict(
     "_RequiredEngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
     },
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Dict[str, str],
-        "SparkProperties": Dict[str, str],
+        "AdditionalConfigs": Mapping[str, str],
+        "SparkProperties": Mapping[str, str],
     },
     total=False,
 )
 
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
@@ -806,22 +827,14 @@
 GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-GetCalculationExecutionCodeResponseTypeDef = TypedDict(
-    "GetCalculationExecutionCodeResponseTypeDef",
-    {
-        "CodeBlock": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCalculationExecutionRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
@@ -886,36 +899,24 @@
 GetQueryExecutionInputRequestTypeDef = TypedDict(
     "GetQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
-_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "QueryExecutionId": str,
-    },
-)
-_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
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
-class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
-    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredGetQueryResultsInputRequestTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputRequestTypeDef = TypedDict(
@@ -1012,22 +1013,14 @@
 
 class ImportNotebookInputRequestTypeDef(
     _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
 ):
     pass
 
 
-ImportNotebookOutputTypeDef = TypedDict(
-    "ImportNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
     "ListApplicationDPUSizesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1062,53 +1055,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "CatalogName": str,
-    },
-)
-_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListDatabasesInputListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListDatabasesInputRequestTypeDef = TypedDict(
     "_RequiredListDatabasesInputRequestTypeDef",
     {
         "CatalogName": str,
     },
 )
 _OptionalListDatabasesInputRequestTypeDef = TypedDict(
@@ -1155,42 +1118,24 @@
 
 class ListExecutorsRequestRequestTypeDef(
     _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
 ):
     pass
 
 
-ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListNamedQueriesOutputTypeDef = TypedDict(
-    "ListNamedQueriesOutputTypeDef",
-    {
-        "NamedQueryIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListNotebookSessionsRequestRequestTypeDef",
     {
         "NotebookId": str,
     },
 )
 _OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
@@ -1247,42 +1192,24 @@
     {
         "StatementName": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryExecutionsInputRequestTypeDef = TypedDict(
     "ListQueryExecutionsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListQueryExecutionsOutputTypeDef = TypedDict(
-    "ListQueryExecutionsOutputTypeDef",
-    {
-        "QueryExecutionIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionsRequestRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListSessionsRequestRequestTypeDef = TypedDict(
@@ -1298,38 +1225,14 @@
 
 class ListSessionsRequestRequestTypeDef(
     _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "CatalogName": str,
-        "DatabaseName": str,
-    },
-)
-_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "Expression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTableMetadataInputListTableMetadataPaginateTypeDef(
-    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
-    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -1346,36 +1249,14 @@
 
 class ListTableMetadataInputRequestTypeDef(
     _RequiredListTableMetadataInputRequestTypeDef, _OptionalListTableMetadataInputRequestTypeDef
 ):
     pass
 
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1399,24 +1280,14 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1475,25 +1346,14 @@
         "ExecutionTime": int,
         "QueryStagePlan": "QueryStagePlanNodeTypeDef",
         "SubStages": List[Dict[str, Any]],
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
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1507,77 +1367,35 @@
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
 
-StartCalculationExecutionResponseTypeDef = TypedDict(
-    "StartCalculationExecutionResponseTypeDef",
-    {
-        "CalculationExecutionId": str,
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartQueryExecutionOutputTypeDef = TypedDict(
-    "StartQueryExecutionOutputTypeDef",
-    {
-        "QueryExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopCalculationExecutionRequestRequestTypeDef = TypedDict(
     "StopCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-StopCalculationExecutionResponseTypeDef = TypedDict(
-    "StopCalculationExecutionResponseTypeDef",
-    {
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1703,66 +1521,168 @@
 class UpdatePreparedStatementInputRequestTypeDef(
     _RequiredUpdatePreparedStatementInputRequestTypeDef,
     _OptionalUpdatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
 
-ListApplicationDPUSizesOutputTypeDef = TypedDict(
-    "ListApplicationDPUSizesOutputTypeDef",
-    {
-        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 QueryExecutionStatusTypeDef = TypedDict(
     "QueryExecutionStatusTypeDef",
     {
         "State": QueryExecutionStateType,
         "StateChangeReason": str,
         "SubmissionDateTime": datetime,
         "CompletionDateTime": datetime,
         "AthenaError": AthenaErrorTypeDef,
     },
     total=False,
 )
 
+CreateNamedQueryOutputTypeDef = TypedDict(
+    "CreateNamedQueryOutputTypeDef",
+    {
+        "NamedQueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNamedQueriesOutputTypeDef = TypedDict(
+    "ListNamedQueriesOutputTypeDef",
+    {
+        "NamedQueryIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueryExecutionsOutputTypeDef = TypedDict(
+    "ListQueryExecutionsOutputTypeDef",
+    {
+        "QueryExecutionIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryExecutionOutputTypeDef = TypedDict(
+    "StartQueryExecutionOutputTypeDef",
+    {
+        "QueryExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPreparedStatementOutputTypeDef = TypedDict(
     "GetPreparedStatementOutputTypeDef",
     {
         "PreparedStatement": PreparedStatementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetPreparedStatementOutputTypeDef = TypedDict(
     "BatchGetPreparedStatementOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCalculationExecutionRequestRequestTypeDef",
     {
         "SessionId": str,
@@ -1803,24 +1723,24 @@
         "CalculationExecutionId": str,
         "SessionId": str,
         "Description": str,
         "WorkingDirectory": str,
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
         "Result": CalculationResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCalculationExecutionStatusResponseTypeDef = TypedDict(
     "GetCalculationExecutionStatusResponseTypeDef",
     {
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCapacityReservationTypeDef = TypedDict(
     "_RequiredCapacityReservationTypeDef",
     {
         "Name": str,
@@ -1846,27 +1766,20 @@
     pass
 
 
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": List[CapacityAssignmentTypeDef],
+        "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
     },
     total=False,
 )
 
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
-    },
-)
-
+CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1943,15 +1856,15 @@
 
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1960,40 +1873,40 @@
 )
 
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
@@ -2034,14 +1947,17 @@
         "WorkingDirectory": str,
         "IdleTimeoutSeconds": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+EngineConfigurationUnionTypeDef = Union[
+    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
+]
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -2064,15 +1980,15 @@
 
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
@@ -2086,41 +2002,41 @@
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
         "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotebookMetadataOutputTypeDef = TypedDict(
     "GetNotebookMetadataOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
         "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -2140,20 +2056,136 @@
 class ListNotebookMetadataInputRequestTypeDef(
     _RequiredListNotebookMetadataInputRequestTypeDef,
     _OptionalListNotebookMetadataInputRequestTypeDef,
 ):
     pass
 
 
+_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "QueryExecutionId": str,
+    },
+)
+_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
+    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+):
+    pass
+
+
+ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "CatalogName": str,
+    },
+)
+_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListDatabasesInputListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
+):
+    pass
+
+
+ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "CatalogName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "Expression": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTableMetadataInputListTableMetadataPaginateTypeDef(
+    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
+    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
+
 GetSessionStatusResponseTypeDef = TypedDict(
     "GetSessionStatusResponseTypeDef",
     {
         "SessionId": str,
         "Status": SessionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
@@ -2166,24 +2198,24 @@
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
@@ -2217,57 +2249,65 @@
 )
 
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityReservationOutputTypeDef = TypedDict(
     "GetCapacityReservationOutputTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCapacityReservationsOutputTypeDef = TypedDict(
     "ListCapacityReservationsOutputTypeDef",
     {
         "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
     },
 )
 
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": List[RowTypeDef],
@@ -2315,46 +2355,46 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "SessionId": str,
         "Description": str,
         "WorkGroup": str,
         "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationTypeDef,
+        "EngineConfiguration": EngineConfigurationOutputTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
@@ -2401,15 +2441,15 @@
 
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
@@ -2478,26 +2518,26 @@
 
 
 BatchGetQueryExecutionOutputTypeDef = TypedDict(
     "BatchGetQueryExecutionOutputTypeDef",
     {
         "QueryExecutions": List[QueryExecutionTypeDef],
         "UnprocessedQueryExecutionIds": List[UnprocessedQueryExecutionIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryExecutionOutputTypeDef = TypedDict(
     "GetQueryExecutionOutputTypeDef",
     {
         "QueryExecution": QueryExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkGroupOutputTypeDef = TypedDict(
     "GetWorkGroupOutputTypeDef",
     {
         "WorkGroup": WorkGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena/type_defs.pyi` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena/type_defs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 [Open documentation](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/type_defs/)
 
 Usage::
 
     ```python
     from types_aiobotocore_athena.type_defs import AclConfigurationTypeDef
 
-    data: AclConfigurationTypeDef = {...}
+    data: AclConfigurationTypeDef = ...
     ```
 """
 import sys
 from datetime import datetime
-from typing import Any, Dict, List, Mapping, Sequence
+from typing import Any, Dict, List, Mapping, Sequence, Union
 
 from .literals import (
     CalculationExecutionStateType,
     CapacityAllocationStatusType,
     CapacityReservationStatusType,
     ColumnNullableType,
     DataCatalogTypeType,
@@ -41,173 +41,177 @@
 
 __all__ = (
     "AclConfigurationTypeDef",
     "ApplicationDPUSizesTypeDef",
     "AthenaErrorTypeDef",
     "BatchGetNamedQueryInputRequestTypeDef",
     "NamedQueryTypeDef",
+    "ResponseMetadataTypeDef",
     "UnprocessedNamedQueryIdTypeDef",
     "BatchGetPreparedStatementInputRequestTypeDef",
     "PreparedStatementTypeDef",
     "UnprocessedPreparedStatementNameTypeDef",
     "BatchGetQueryExecutionInputRequestTypeDef",
     "UnprocessedQueryExecutionIdTypeDef",
     "CalculationConfigurationTypeDef",
     "CalculationResultTypeDef",
     "CalculationStatisticsTypeDef",
     "CalculationStatusTypeDef",
     "CancelCapacityReservationInputRequestTypeDef",
     "CapacityAllocationTypeDef",
+    "CapacityAssignmentOutputTypeDef",
     "CapacityAssignmentTypeDef",
     "ColumnInfoTypeDef",
     "ColumnTypeDef",
     "TagTypeDef",
     "CreateNamedQueryInputRequestTypeDef",
-    "CreateNamedQueryOutputTypeDef",
     "CreateNotebookInputRequestTypeDef",
-    "CreateNotebookOutputTypeDef",
     "CreatePreparedStatementInputRequestTypeDef",
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
-    "CreatePresignedNotebookUrlResponseTypeDef",
     "CustomerContentEncryptionConfigurationTypeDef",
     "DataCatalogSummaryTypeDef",
     "DataCatalogTypeDef",
     "DatabaseTypeDef",
     "DatumTypeDef",
     "DeleteCapacityReservationInputRequestTypeDef",
     "DeleteDataCatalogInputRequestTypeDef",
     "DeleteNamedQueryInputRequestTypeDef",
     "DeleteNotebookInputRequestTypeDef",
     "DeletePreparedStatementInputRequestTypeDef",
     "DeleteWorkGroupInputRequestTypeDef",
     "EncryptionConfigurationTypeDef",
+    "EngineConfigurationOutputTypeDef",
     "EngineConfigurationTypeDef",
     "EngineVersionTypeDef",
     "ExecutorsSummaryTypeDef",
     "ExportNotebookInputRequestTypeDef",
     "NotebookMetadataTypeDef",
     "FilterDefinitionTypeDef",
     "GetCalculationExecutionCodeRequestRequestTypeDef",
-    "GetCalculationExecutionCodeResponseTypeDef",
     "GetCalculationExecutionRequestRequestTypeDef",
     "GetCalculationExecutionStatusRequestRequestTypeDef",
     "GetCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetCapacityReservationInputRequestTypeDef",
     "GetDataCatalogInputRequestTypeDef",
     "GetDatabaseInputRequestTypeDef",
     "GetNamedQueryInputRequestTypeDef",
     "GetNotebookMetadataInputRequestTypeDef",
     "GetPreparedStatementInputRequestTypeDef",
     "GetQueryExecutionInputRequestTypeDef",
-    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "GetQueryResultsInputRequestTypeDef",
     "GetQueryRuntimeStatisticsInputRequestTypeDef",
     "GetSessionRequestRequestTypeDef",
     "SessionStatisticsTypeDef",
     "SessionStatusTypeDef",
     "GetSessionStatusRequestRequestTypeDef",
     "GetTableMetadataInputRequestTypeDef",
     "GetWorkGroupInputRequestTypeDef",
     "ImportNotebookInputRequestTypeDef",
-    "ImportNotebookOutputTypeDef",
     "ListApplicationDPUSizesInputRequestTypeDef",
     "ListCalculationExecutionsRequestRequestTypeDef",
     "ListCapacityReservationsInputRequestTypeDef",
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
     "ListDataCatalogsInputRequestTypeDef",
-    "ListDatabasesInputListDatabasesPaginateTypeDef",
     "ListDatabasesInputRequestTypeDef",
     "ListEngineVersionsInputRequestTypeDef",
     "ListExecutorsRequestRequestTypeDef",
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
     "ListNamedQueriesInputRequestTypeDef",
-    "ListNamedQueriesOutputTypeDef",
     "ListNotebookSessionsRequestRequestTypeDef",
     "NotebookSessionSummaryTypeDef",
     "ListPreparedStatementsInputRequestTypeDef",
     "PreparedStatementSummaryTypeDef",
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
     "ListQueryExecutionsInputRequestTypeDef",
-    "ListQueryExecutionsOutputTypeDef",
     "ListSessionsRequestRequestTypeDef",
-    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
     "ListTableMetadataInputRequestTypeDef",
-    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "ListTagsForResourceInputRequestTypeDef",
     "ListWorkGroupsInputRequestTypeDef",
-    "PaginatorConfigTypeDef",
     "QueryExecutionContextTypeDef",
     "ResultReuseInformationTypeDef",
     "QueryRuntimeStatisticsRowsTypeDef",
     "QueryRuntimeStatisticsTimelineTypeDef",
     "QueryStagePlanNodeTypeDef",
     "QueryStageTypeDef",
-    "ResponseMetadataTypeDef",
     "ResultReuseByAgeConfigurationTypeDef",
-    "StartCalculationExecutionResponseTypeDef",
-    "StartQueryExecutionOutputTypeDef",
-    "StartSessionResponseTypeDef",
     "StopCalculationExecutionRequestRequestTypeDef",
-    "StopCalculationExecutionResponseTypeDef",
     "StopQueryExecutionInputRequestTypeDef",
     "TerminateSessionRequestRequestTypeDef",
-    "TerminateSessionResponseTypeDef",
     "UntagResourceInputRequestTypeDef",
     "UpdateCapacityReservationInputRequestTypeDef",
     "UpdateDataCatalogInputRequestTypeDef",
     "UpdateNamedQueryInputRequestTypeDef",
     "UpdateNotebookInputRequestTypeDef",
     "UpdateNotebookMetadataInputRequestTypeDef",
     "UpdatePreparedStatementInputRequestTypeDef",
-    "ListApplicationDPUSizesOutputTypeDef",
     "QueryExecutionStatusTypeDef",
+    "CreateNamedQueryOutputTypeDef",
+    "CreateNotebookOutputTypeDef",
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    "GetCalculationExecutionCodeResponseTypeDef",
     "GetNamedQueryOutputTypeDef",
+    "ImportNotebookOutputTypeDef",
+    "ListApplicationDPUSizesOutputTypeDef",
+    "ListNamedQueriesOutputTypeDef",
+    "ListQueryExecutionsOutputTypeDef",
+    "StartCalculationExecutionResponseTypeDef",
+    "StartQueryExecutionOutputTypeDef",
+    "StartSessionResponseTypeDef",
+    "StopCalculationExecutionResponseTypeDef",
+    "TerminateSessionResponseTypeDef",
     "BatchGetNamedQueryOutputTypeDef",
     "GetPreparedStatementOutputTypeDef",
     "BatchGetPreparedStatementOutputTypeDef",
     "StartCalculationExecutionRequestRequestTypeDef",
     "CalculationSummaryTypeDef",
     "GetCalculationExecutionResponseTypeDef",
     "GetCalculationExecutionStatusResponseTypeDef",
     "CapacityReservationTypeDef",
     "CapacityAssignmentConfigurationTypeDef",
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    "CapacityAssignmentUnionTypeDef",
     "ResultSetMetadataTypeDef",
     "TableMetadataTypeDef",
     "CreateCapacityReservationInputRequestTypeDef",
     "CreateDataCatalogInputRequestTypeDef",
     "ListTagsForResourceOutputTypeDef",
     "TagResourceInputRequestTypeDef",
     "ListDataCatalogsOutputTypeDef",
     "GetDataCatalogOutputTypeDef",
     "GetDatabaseOutputTypeDef",
     "ListDatabasesOutputTypeDef",
     "RowTypeDef",
     "ResultConfigurationTypeDef",
     "ResultConfigurationUpdatesTypeDef",
     "SessionConfigurationTypeDef",
+    "EngineConfigurationUnionTypeDef",
     "StartSessionRequestRequestTypeDef",
     "ListEngineVersionsOutputTypeDef",
     "WorkGroupSummaryTypeDef",
     "ListExecutorsResponseTypeDef",
     "ExportNotebookOutputTypeDef",
     "GetNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataOutputTypeDef",
     "ListNotebookMetadataInputRequestTypeDef",
+    "GetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    "ListDatabasesInputListDatabasesPaginateTypeDef",
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    "ListTableMetadataInputListTableMetadataPaginateTypeDef",
+    "ListTagsForResourceInputListTagsForResourcePaginateTypeDef",
     "GetSessionStatusResponseTypeDef",
     "SessionSummaryTypeDef",
     "ListNotebookSessionsResponseTypeDef",
     "ListPreparedStatementsOutputTypeDef",
     "QueryExecutionStatisticsTypeDef",
     "QueryRuntimeStatisticsTypeDef",
     "ResultReuseConfigurationTypeDef",
     "ListCalculationExecutionsResponseTypeDef",
     "GetCapacityReservationOutputTypeDef",
     "ListCapacityReservationsOutputTypeDef",
     "GetCapacityAssignmentConfigurationOutputTypeDef",
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
     "GetTableMetadataOutputTypeDef",
     "ListTableMetadataOutputTypeDef",
     "ResultSetTypeDef",
     "WorkGroupConfigurationTypeDef",
     "WorkGroupConfigurationUpdatesTypeDef",
     "GetSessionResponseTypeDef",
     "ListWorkGroupsOutputTypeDef",
@@ -275,14 +279,25 @@
     },
     total=False,
 )
 
 class NamedQueryTypeDef(_RequiredNamedQueryTypeDef, _OptionalNamedQueryTypeDef):
     pass
 
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
 UnprocessedNamedQueryIdTypeDef = TypedDict(
     "UnprocessedNamedQueryIdTypeDef",
     {
         "NamedQueryId": str,
         "ErrorCode": str,
         "ErrorMessage": str,
     },
@@ -399,18 +414,26 @@
 )
 
 class CapacityAllocationTypeDef(
     _RequiredCapacityAllocationTypeDef, _OptionalCapacityAllocationTypeDef
 ):
     pass
 
+CapacityAssignmentOutputTypeDef = TypedDict(
+    "CapacityAssignmentOutputTypeDef",
+    {
+        "WorkGroupNames": List[str],
+    },
+    total=False,
+)
+
 CapacityAssignmentTypeDef = TypedDict(
     "CapacityAssignmentTypeDef",
     {
-        "WorkGroupNames": List[str],
+        "WorkGroupNames": Sequence[str],
     },
     total=False,
 )
 
 _RequiredColumnInfoTypeDef = TypedDict(
     "_RequiredColumnInfoTypeDef",
     {
@@ -482,22 +505,14 @@
 )
 
 class CreateNamedQueryInputRequestTypeDef(
     _RequiredCreateNamedQueryInputRequestTypeDef, _OptionalCreateNamedQueryInputRequestTypeDef
 ):
     pass
 
-CreateNamedQueryOutputTypeDef = TypedDict(
-    "CreateNamedQueryOutputTypeDef",
-    {
-        "NamedQueryId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreateNotebookInputRequestTypeDef = TypedDict(
     "_RequiredCreateNotebookInputRequestTypeDef",
     {
         "WorkGroup": str,
         "Name": str,
     },
 )
@@ -510,22 +525,14 @@
 )
 
 class CreateNotebookInputRequestTypeDef(
     _RequiredCreateNotebookInputRequestTypeDef, _OptionalCreateNotebookInputRequestTypeDef
 ):
     pass
 
-CreateNotebookOutputTypeDef = TypedDict(
-    "CreateNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredCreatePreparedStatementInputRequestTypeDef = TypedDict(
     "_RequiredCreatePreparedStatementInputRequestTypeDef",
     {
         "StatementName": str,
         "WorkGroup": str,
         "QueryStatement": str,
     },
@@ -547,24 +554,14 @@
 CreatePresignedNotebookUrlRequestRequestTypeDef = TypedDict(
     "CreatePresignedNotebookUrlRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
-    "CreatePresignedNotebookUrlResponseTypeDef",
-    {
-        "NotebookUrl": str,
-        "AuthToken": str,
-        "AuthTokenExpirationTime": int,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 CustomerContentEncryptionConfigurationTypeDef = TypedDict(
     "CustomerContentEncryptionConfigurationTypeDef",
     {
         "KmsKey": str,
     },
 )
 
@@ -692,27 +689,49 @@
 )
 
 class EncryptionConfigurationTypeDef(
     _RequiredEncryptionConfigurationTypeDef, _OptionalEncryptionConfigurationTypeDef
 ):
     pass
 
+_RequiredEngineConfigurationOutputTypeDef = TypedDict(
+    "_RequiredEngineConfigurationOutputTypeDef",
+    {
+        "MaxConcurrentDpus": int,
+    },
+)
+_OptionalEngineConfigurationOutputTypeDef = TypedDict(
+    "_OptionalEngineConfigurationOutputTypeDef",
+    {
+        "CoordinatorDpuSize": int,
+        "DefaultExecutorDpuSize": int,
+        "AdditionalConfigs": Dict[str, str],
+        "SparkProperties": Dict[str, str],
+    },
+    total=False,
+)
+
+class EngineConfigurationOutputTypeDef(
+    _RequiredEngineConfigurationOutputTypeDef, _OptionalEngineConfigurationOutputTypeDef
+):
+    pass
+
 _RequiredEngineConfigurationTypeDef = TypedDict(
     "_RequiredEngineConfigurationTypeDef",
     {
         "MaxConcurrentDpus": int,
     },
 )
 _OptionalEngineConfigurationTypeDef = TypedDict(
     "_OptionalEngineConfigurationTypeDef",
     {
         "CoordinatorDpuSize": int,
         "DefaultExecutorDpuSize": int,
-        "AdditionalConfigs": Dict[str, str],
-        "SparkProperties": Dict[str, str],
+        "AdditionalConfigs": Mapping[str, str],
+        "SparkProperties": Mapping[str, str],
     },
     total=False,
 )
 
 class EngineConfigurationTypeDef(
     _RequiredEngineConfigurationTypeDef, _OptionalEngineConfigurationTypeDef
 ):
@@ -779,22 +798,14 @@
 GetCalculationExecutionCodeRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionCodeRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-GetCalculationExecutionCodeResponseTypeDef = TypedDict(
-    "GetCalculationExecutionCodeResponseTypeDef",
-    {
-        "CodeBlock": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 GetCalculationExecutionRequestRequestTypeDef = TypedDict(
     "GetCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
@@ -859,34 +870,24 @@
 GetQueryExecutionInputRequestTypeDef = TypedDict(
     "GetQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
-_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
-    {
-        "QueryExecutionId": str,
-    },
-)
-_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
-    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
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
 
-class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
-    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
-):
-    pass
-
 _RequiredGetQueryResultsInputRequestTypeDef = TypedDict(
     "_RequiredGetQueryResultsInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 _OptionalGetQueryResultsInputRequestTypeDef = TypedDict(
@@ -979,22 +980,14 @@
 )
 
 class ImportNotebookInputRequestTypeDef(
     _RequiredImportNotebookInputRequestTypeDef, _OptionalImportNotebookInputRequestTypeDef
 ):
     pass
 
-ImportNotebookOutputTypeDef = TypedDict(
-    "ImportNotebookOutputTypeDef",
-    {
-        "NotebookId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ListApplicationDPUSizesInputRequestTypeDef = TypedDict(
     "ListApplicationDPUSizesInputRequestTypeDef",
     {
         "MaxResults": int,
         "NextToken": str,
     },
     total=False,
@@ -1027,51 +1020,23 @@
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
-    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListDataCatalogsInputRequestTypeDef = TypedDict(
     "ListDataCatalogsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
     },
     total=False,
 )
 
-_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "CatalogName": str,
-    },
-)
-_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
-    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListDatabasesInputListDatabasesPaginateTypeDef(
-    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
-    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
-):
-    pass
-
 _RequiredListDatabasesInputRequestTypeDef = TypedDict(
     "_RequiredListDatabasesInputRequestTypeDef",
     {
         "CatalogName": str,
     },
 )
 _OptionalListDatabasesInputRequestTypeDef = TypedDict(
@@ -1114,42 +1079,24 @@
 )
 
 class ListExecutorsRequestRequestTypeDef(
     _RequiredListExecutorsRequestRequestTypeDef, _OptionalListExecutorsRequestRequestTypeDef
 ):
     pass
 
-ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
-    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListNamedQueriesInputRequestTypeDef = TypedDict(
     "ListNamedQueriesInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListNamedQueriesOutputTypeDef = TypedDict(
-    "ListNamedQueriesOutputTypeDef",
-    {
-        "NamedQueryIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListNotebookSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListNotebookSessionsRequestRequestTypeDef",
     {
         "NotebookId": str,
     },
 )
 _OptionalListNotebookSessionsRequestRequestTypeDef = TypedDict(
@@ -1202,42 +1149,24 @@
     {
         "StatementName": str,
         "LastModifiedTime": datetime,
     },
     total=False,
 )
 
-ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
-    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
-    {
-        "WorkGroup": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 ListQueryExecutionsInputRequestTypeDef = TypedDict(
     "ListQueryExecutionsInputRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "WorkGroup": str,
     },
     total=False,
 )
 
-ListQueryExecutionsOutputTypeDef = TypedDict(
-    "ListQueryExecutionsOutputTypeDef",
-    {
-        "QueryExecutionIds": List[str],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListSessionsRequestRequestTypeDef = TypedDict(
     "_RequiredListSessionsRequestRequestTypeDef",
     {
         "WorkGroup": str,
     },
 )
 _OptionalListSessionsRequestRequestTypeDef = TypedDict(
@@ -1251,36 +1180,14 @@
 )
 
 class ListSessionsRequestRequestTypeDef(
     _RequiredListSessionsRequestRequestTypeDef, _OptionalListSessionsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "CatalogName": str,
-        "DatabaseName": str,
-    },
-)
-_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
-    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
-    {
-        "Expression": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTableMetadataInputListTableMetadataPaginateTypeDef(
-    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
-    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
-):
-    pass
-
 _RequiredListTableMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListTableMetadataInputRequestTypeDef",
     {
         "CatalogName": str,
         "DatabaseName": str,
     },
 )
@@ -1295,34 +1202,14 @@
 )
 
 class ListTableMetadataInputRequestTypeDef(
     _RequiredListTableMetadataInputRequestTypeDef, _OptionalListTableMetadataInputRequestTypeDef
 ):
     pass
 
-_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "ResourceARN": str,
-    },
-)
-_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
-    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
-    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
-):
-    pass
-
 _RequiredListTagsForResourceInputRequestTypeDef = TypedDict(
     "_RequiredListTagsForResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
     },
 )
 _OptionalListTagsForResourceInputRequestTypeDef = TypedDict(
@@ -1344,24 +1231,14 @@
     {
         "NextToken": str,
         "MaxResults": int,
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
 QueryExecutionContextTypeDef = TypedDict(
     "QueryExecutionContextTypeDef",
     {
         "Database": str,
         "Catalog": str,
     },
     total=False,
@@ -1420,25 +1297,14 @@
         "ExecutionTime": int,
         "QueryStagePlan": "QueryStagePlanNodeTypeDef",
         "SubStages": List[Dict[str, Any]],
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
 _RequiredResultReuseByAgeConfigurationTypeDef = TypedDict(
     "_RequiredResultReuseByAgeConfigurationTypeDef",
     {
         "Enabled": bool,
     },
 )
 _OptionalResultReuseByAgeConfigurationTypeDef = TypedDict(
@@ -1450,77 +1316,35 @@
 )
 
 class ResultReuseByAgeConfigurationTypeDef(
     _RequiredResultReuseByAgeConfigurationTypeDef, _OptionalResultReuseByAgeConfigurationTypeDef
 ):
     pass
 
-StartCalculationExecutionResponseTypeDef = TypedDict(
-    "StartCalculationExecutionResponseTypeDef",
-    {
-        "CalculationExecutionId": str,
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartQueryExecutionOutputTypeDef = TypedDict(
-    "StartQueryExecutionOutputTypeDef",
-    {
-        "QueryExecutionId": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
-StartSessionResponseTypeDef = TypedDict(
-    "StartSessionResponseTypeDef",
-    {
-        "SessionId": str,
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopCalculationExecutionRequestRequestTypeDef = TypedDict(
     "StopCalculationExecutionRequestRequestTypeDef",
     {
         "CalculationExecutionId": str,
     },
 )
 
-StopCalculationExecutionResponseTypeDef = TypedDict(
-    "StopCalculationExecutionResponseTypeDef",
-    {
-        "State": CalculationExecutionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 StopQueryExecutionInputRequestTypeDef = TypedDict(
     "StopQueryExecutionInputRequestTypeDef",
     {
         "QueryExecutionId": str,
     },
 )
 
 TerminateSessionRequestRequestTypeDef = TypedDict(
     "TerminateSessionRequestRequestTypeDef",
     {
         "SessionId": str,
     },
 )
 
-TerminateSessionResponseTypeDef = TypedDict(
-    "TerminateSessionResponseTypeDef",
-    {
-        "State": SessionStateType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UntagResourceInputRequestTypeDef = TypedDict(
     "UntagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
         "TagKeys": Sequence[str],
     },
 )
@@ -1636,66 +1460,168 @@
 
 class UpdatePreparedStatementInputRequestTypeDef(
     _RequiredUpdatePreparedStatementInputRequestTypeDef,
     _OptionalUpdatePreparedStatementInputRequestTypeDef,
 ):
     pass
 
-ListApplicationDPUSizesOutputTypeDef = TypedDict(
-    "ListApplicationDPUSizesOutputTypeDef",
-    {
-        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
-        "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 QueryExecutionStatusTypeDef = TypedDict(
     "QueryExecutionStatusTypeDef",
     {
         "State": QueryExecutionStateType,
         "StateChangeReason": str,
         "SubmissionDateTime": datetime,
         "CompletionDateTime": datetime,
         "AthenaError": AthenaErrorTypeDef,
     },
     total=False,
 )
 
+CreateNamedQueryOutputTypeDef = TypedDict(
+    "CreateNamedQueryOutputTypeDef",
+    {
+        "NamedQueryId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateNotebookOutputTypeDef = TypedDict(
+    "CreateNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreatePresignedNotebookUrlResponseTypeDef = TypedDict(
+    "CreatePresignedNotebookUrlResponseTypeDef",
+    {
+        "NotebookUrl": str,
+        "AuthToken": str,
+        "AuthTokenExpirationTime": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCalculationExecutionCodeResponseTypeDef = TypedDict(
+    "GetCalculationExecutionCodeResponseTypeDef",
+    {
+        "CodeBlock": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 GetNamedQueryOutputTypeDef = TypedDict(
     "GetNamedQueryOutputTypeDef",
     {
         "NamedQuery": NamedQueryTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ImportNotebookOutputTypeDef = TypedDict(
+    "ImportNotebookOutputTypeDef",
+    {
+        "NotebookId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListApplicationDPUSizesOutputTypeDef = TypedDict(
+    "ListApplicationDPUSizesOutputTypeDef",
+    {
+        "ApplicationDPUSizes": List[ApplicationDPUSizesTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListNamedQueriesOutputTypeDef = TypedDict(
+    "ListNamedQueriesOutputTypeDef",
+    {
+        "NamedQueryIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListQueryExecutionsOutputTypeDef = TypedDict(
+    "ListQueryExecutionsOutputTypeDef",
+    {
+        "QueryExecutionIds": List[str],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartCalculationExecutionResponseTypeDef = TypedDict(
+    "StartCalculationExecutionResponseTypeDef",
+    {
+        "CalculationExecutionId": str,
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartQueryExecutionOutputTypeDef = TypedDict(
+    "StartQueryExecutionOutputTypeDef",
+    {
+        "QueryExecutionId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StartSessionResponseTypeDef = TypedDict(
+    "StartSessionResponseTypeDef",
+    {
+        "SessionId": str,
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+StopCalculationExecutionResponseTypeDef = TypedDict(
+    "StopCalculationExecutionResponseTypeDef",
+    {
+        "State": CalculationExecutionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+TerminateSessionResponseTypeDef = TypedDict(
+    "TerminateSessionResponseTypeDef",
+    {
+        "State": SessionStateType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetNamedQueryOutputTypeDef = TypedDict(
     "BatchGetNamedQueryOutputTypeDef",
     {
         "NamedQueries": List[NamedQueryTypeDef],
         "UnprocessedNamedQueryIds": List[UnprocessedNamedQueryIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetPreparedStatementOutputTypeDef = TypedDict(
     "GetPreparedStatementOutputTypeDef",
     {
         "PreparedStatement": PreparedStatementTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 BatchGetPreparedStatementOutputTypeDef = TypedDict(
     "BatchGetPreparedStatementOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementTypeDef],
         "UnprocessedPreparedStatementNames": List[UnprocessedPreparedStatementNameTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredStartCalculationExecutionRequestRequestTypeDef = TypedDict(
     "_RequiredStartCalculationExecutionRequestRequestTypeDef",
     {
         "SessionId": str,
@@ -1734,24 +1660,24 @@
         "CalculationExecutionId": str,
         "SessionId": str,
         "Description": str,
         "WorkingDirectory": str,
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
         "Result": CalculationResultTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCalculationExecutionStatusResponseTypeDef = TypedDict(
     "GetCalculationExecutionStatusResponseTypeDef",
     {
         "Status": CalculationStatusTypeDef,
         "Statistics": CalculationStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCapacityReservationTypeDef = TypedDict(
     "_RequiredCapacityReservationTypeDef",
     {
         "Name": str,
@@ -1775,27 +1701,20 @@
 ):
     pass
 
 CapacityAssignmentConfigurationTypeDef = TypedDict(
     "CapacityAssignmentConfigurationTypeDef",
     {
         "CapacityReservationName": str,
-        "CapacityAssignments": List[CapacityAssignmentTypeDef],
+        "CapacityAssignments": List[CapacityAssignmentOutputTypeDef],
     },
     total=False,
 )
 
-PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
-    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
-    {
-        "CapacityReservationName": str,
-        "CapacityAssignments": Sequence[CapacityAssignmentTypeDef],
-    },
-)
-
+CapacityAssignmentUnionTypeDef = Union[CapacityAssignmentTypeDef, CapacityAssignmentOutputTypeDef]
 ResultSetMetadataTypeDef = TypedDict(
     "ResultSetMetadataTypeDef",
     {
         "ColumnInfo": List[ColumnInfoTypeDef],
     },
     total=False,
 )
@@ -1866,15 +1785,15 @@
     pass
 
 ListTagsForResourceOutputTypeDef = TypedDict(
     "ListTagsForResourceOutputTypeDef",
     {
         "Tags": List[TagTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 TagResourceInputRequestTypeDef = TypedDict(
     "TagResourceInputRequestTypeDef",
     {
         "ResourceARN": str,
@@ -1883,40 +1802,40 @@
 )
 
 ListDataCatalogsOutputTypeDef = TypedDict(
     "ListDataCatalogsOutputTypeDef",
     {
         "DataCatalogsSummary": List[DataCatalogSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDataCatalogOutputTypeDef = TypedDict(
     "GetDataCatalogOutputTypeDef",
     {
         "DataCatalog": DataCatalogTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDatabaseOutputTypeDef = TypedDict(
     "GetDatabaseOutputTypeDef",
     {
         "Database": DatabaseTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDatabasesOutputTypeDef = TypedDict(
     "ListDatabasesOutputTypeDef",
     {
         "DatabaseList": List[DatabaseTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RowTypeDef = TypedDict(
     "RowTypeDef",
     {
         "Data": List[DatumTypeDef],
@@ -1957,14 +1876,17 @@
         "WorkingDirectory": str,
         "IdleTimeoutSeconds": int,
         "EncryptionConfiguration": EncryptionConfigurationTypeDef,
     },
     total=False,
 )
 
+EngineConfigurationUnionTypeDef = Union[
+    EngineConfigurationTypeDef, EngineConfigurationOutputTypeDef
+]
 _RequiredStartSessionRequestRequestTypeDef = TypedDict(
     "_RequiredStartSessionRequestRequestTypeDef",
     {
         "WorkGroup": str,
         "EngineConfiguration": EngineConfigurationTypeDef,
     },
 )
@@ -1985,15 +1907,15 @@
     pass
 
 ListEngineVersionsOutputTypeDef = TypedDict(
     "ListEngineVersionsOutputTypeDef",
     {
         "EngineVersions": List[EngineVersionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 WorkGroupSummaryTypeDef = TypedDict(
     "WorkGroupSummaryTypeDef",
     {
         "Name": str,
@@ -2007,41 +1929,41 @@
 
 ListExecutorsResponseTypeDef = TypedDict(
     "ListExecutorsResponseTypeDef",
     {
         "SessionId": str,
         "NextToken": str,
         "ExecutorsSummary": List[ExecutorsSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ExportNotebookOutputTypeDef = TypedDict(
     "ExportNotebookOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
         "Payload": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetNotebookMetadataOutputTypeDef = TypedDict(
     "GetNotebookMetadataOutputTypeDef",
     {
         "NotebookMetadata": NotebookMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListNotebookMetadataOutputTypeDef = TypedDict(
     "ListNotebookMetadataOutputTypeDef",
     {
         "NextToken": str,
         "NotebookMetadataList": List[NotebookMetadataTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredListNotebookMetadataInputRequestTypeDef = TypedDict(
     "_RequiredListNotebookMetadataInputRequestTypeDef",
     {
         "WorkGroup": str,
@@ -2059,20 +1981,128 @@
 
 class ListNotebookMetadataInputRequestTypeDef(
     _RequiredListNotebookMetadataInputRequestTypeDef,
     _OptionalListNotebookMetadataInputRequestTypeDef,
 ):
     pass
 
+_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "QueryExecutionId": str,
+    },
+)
+_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef = TypedDict(
+    "_OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class GetQueryResultsInputGetQueryResultsPaginateTypeDef(
+    _RequiredGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    _OptionalGetQueryResultsInputGetQueryResultsPaginateTypeDef,
+):
+    pass
+
+ListDataCatalogsInputListDataCatalogsPaginateTypeDef = TypedDict(
+    "ListDataCatalogsInputListDataCatalogsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_RequiredListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "CatalogName": str,
+    },
+)
+_OptionalListDatabasesInputListDatabasesPaginateTypeDef = TypedDict(
+    "_OptionalListDatabasesInputListDatabasesPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListDatabasesInputListDatabasesPaginateTypeDef(
+    _RequiredListDatabasesInputListDatabasesPaginateTypeDef,
+    _OptionalListDatabasesInputListDatabasesPaginateTypeDef,
+):
+    pass
+
+ListNamedQueriesInputListNamedQueriesPaginateTypeDef = TypedDict(
+    "ListNamedQueriesInputListNamedQueriesPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef = TypedDict(
+    "ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef",
+    {
+        "WorkGroup": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_RequiredListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "CatalogName": str,
+        "DatabaseName": str,
+    },
+)
+_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef = TypedDict(
+    "_OptionalListTableMetadataInputListTableMetadataPaginateTypeDef",
+    {
+        "Expression": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTableMetadataInputListTableMetadataPaginateTypeDef(
+    _RequiredListTableMetadataInputListTableMetadataPaginateTypeDef,
+    _OptionalListTableMetadataInputListTableMetadataPaginateTypeDef,
+):
+    pass
+
+_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "ResourceARN": str,
+    },
+)
+_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef = TypedDict(
+    "_OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(
+    _RequiredListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+    _OptionalListTagsForResourceInputListTagsForResourcePaginateTypeDef,
+):
+    pass
+
 GetSessionStatusResponseTypeDef = TypedDict(
     "GetSessionStatusResponseTypeDef",
     {
         "SessionId": str,
         "Status": SessionStatusTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SessionSummaryTypeDef = TypedDict(
     "SessionSummaryTypeDef",
     {
         "SessionId": str,
@@ -2085,24 +2115,24 @@
 )
 
 ListNotebookSessionsResponseTypeDef = TypedDict(
     "ListNotebookSessionsResponseTypeDef",
     {
         "NotebookSessionsList": List[NotebookSessionSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListPreparedStatementsOutputTypeDef = TypedDict(
     "ListPreparedStatementsOutputTypeDef",
     {
         "PreparedStatements": List[PreparedStatementSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionStatisticsTypeDef = TypedDict(
     "QueryExecutionStatisticsTypeDef",
     {
         "EngineExecutionTimeInMillis": int,
@@ -2136,57 +2166,65 @@
 )
 
 ListCalculationExecutionsResponseTypeDef = TypedDict(
     "ListCalculationExecutionsResponseTypeDef",
     {
         "NextToken": str,
         "Calculations": List[CalculationSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityReservationOutputTypeDef = TypedDict(
     "GetCapacityReservationOutputTypeDef",
     {
         "CapacityReservation": CapacityReservationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListCapacityReservationsOutputTypeDef = TypedDict(
     "ListCapacityReservationsOutputTypeDef",
     {
         "NextToken": str,
         "CapacityReservations": List[CapacityReservationTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetCapacityAssignmentConfigurationOutputTypeDef = TypedDict(
     "GetCapacityAssignmentConfigurationOutputTypeDef",
     {
         "CapacityAssignmentConfiguration": CapacityAssignmentConfigurationTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+PutCapacityAssignmentConfigurationInputRequestTypeDef = TypedDict(
+    "PutCapacityAssignmentConfigurationInputRequestTypeDef",
+    {
+        "CapacityReservationName": str,
+        "CapacityAssignments": Sequence[CapacityAssignmentUnionTypeDef],
     },
 )
 
 GetTableMetadataOutputTypeDef = TypedDict(
     "GetTableMetadataOutputTypeDef",
     {
         "TableMetadata": TableMetadataTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListTableMetadataOutputTypeDef = TypedDict(
     "ListTableMetadataOutputTypeDef",
     {
         "TableMetadataList": List[TableMetadataTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResultSetTypeDef = TypedDict(
     "ResultSetTypeDef",
     {
         "Rows": List[RowTypeDef],
@@ -2234,46 +2272,46 @@
 GetSessionResponseTypeDef = TypedDict(
     "GetSessionResponseTypeDef",
     {
         "SessionId": str,
         "Description": str,
         "WorkGroup": str,
         "EngineVersion": str,
-        "EngineConfiguration": EngineConfigurationTypeDef,
+        "EngineConfiguration": EngineConfigurationOutputTypeDef,
         "NotebookVersion": str,
         "SessionConfiguration": SessionConfigurationTypeDef,
         "Status": SessionStatusTypeDef,
         "Statistics": SessionStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListWorkGroupsOutputTypeDef = TypedDict(
     "ListWorkGroupsOutputTypeDef",
     {
         "WorkGroups": List[WorkGroupSummaryTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListSessionsResponseTypeDef = TypedDict(
     "ListSessionsResponseTypeDef",
     {
         "NextToken": str,
         "Sessions": List[SessionSummaryTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryRuntimeStatisticsOutputTypeDef = TypedDict(
     "GetQueryRuntimeStatisticsOutputTypeDef",
     {
         "QueryRuntimeStatistics": QueryRuntimeStatisticsTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 QueryExecutionTypeDef = TypedDict(
     "QueryExecutionTypeDef",
     {
         "QueryExecutionId": str,
@@ -2318,15 +2356,15 @@
 
 GetQueryResultsOutputTypeDef = TypedDict(
     "GetQueryResultsOutputTypeDef",
     {
         "UpdateCount": int,
         "ResultSet": ResultSetTypeDef,
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateWorkGroupInputRequestTypeDef = TypedDict(
     "_RequiredCreateWorkGroupInputRequestTypeDef",
     {
         "Name": str,
@@ -2389,26 +2427,26 @@
     pass
 
 BatchGetQueryExecutionOutputTypeDef = TypedDict(
     "BatchGetQueryExecutionOutputTypeDef",
     {
         "QueryExecutions": List[QueryExecutionTypeDef],
         "UnprocessedQueryExecutionIds": List[UnprocessedQueryExecutionIdTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetQueryExecutionOutputTypeDef = TypedDict(
     "GetQueryExecutionOutputTypeDef",
     {
         "QueryExecution": QueryExecutionTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetWorkGroupOutputTypeDef = TypedDict(
     "GetWorkGroupOutputTypeDef",
     {
         "WorkGroup": WorkGroupTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/PKG-INFO` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 Metadata-Version: 2.1
 Name: types-aiobotocore-athena
-Version: 2.5.2
-Summary: Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder 7.14.5
+Version: 2.5.2.post1
+Summary: Type annotations for aiobotocore.Athena 2.5.2 service generated with mypy-boto3-builder 7.17.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
-Keywords: aiobotocore athena type-annotations boto3-stubs mypy typeshed autocomplete
+Keywords: aiobotocore athena type-annotations botocore mypy typeshed autocomplete
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
 <a id="types-aiobotocore-athena"></a>
 
 # types-aiobotocore-athena
 
 [![PyPI - types-aiobotocore-athena](https://img.shields.io/pypi/v/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/types-aiobotocore-athena.svg?color=blue)](https://pypi.org/project/types-aiobotocore-athena)
 [![Docs](https://img.shields.io/readthedocs/types-aiobotocore.svg?color=blue)](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/)
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/types-aiobotocore-athena?color=blue)](https://pypistats.org/packages/types-aiobotocore-athena)
+[![PyPI - Downloads](https://static.pepy.tech/badge/types-aiobotocore-athena)](https://pepy.tech/project/types-aiobotocore-athena)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
 [aiobotocore.Athena 2.5.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
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
 [types-aiobotocore-athena docs](https://youtype.github.io/types_aiobotocore_docs/types_aiobotocore_athena/).
 
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
@@ -350,187 +349,191 @@
 )
 
 
 def check_value(value: CalculationExecutionStateType) -> bool:
     ...
 ```
 
-<a id="typed-dictionaries"></a>
+<a id="type-definitions"></a>
 
-### Typed dictionaries
+### Type definitions
 
 `types_aiobotocore_athena.type_defs` module contains structures and shapes
-assembled to typed dictionaries for additional type checking.
+assembled to typed dictionaries and unions for additional type checking.
 
 ```python
 from types_aiobotocore_athena.type_defs import (
     AclConfigurationTypeDef,
     ApplicationDPUSizesTypeDef,
     AthenaErrorTypeDef,
     BatchGetNamedQueryInputRequestTypeDef,
     NamedQueryTypeDef,
+    ResponseMetadataTypeDef,
     UnprocessedNamedQueryIdTypeDef,
     BatchGetPreparedStatementInputRequestTypeDef,
     PreparedStatementTypeDef,
     UnprocessedPreparedStatementNameTypeDef,
     BatchGetQueryExecutionInputRequestTypeDef,
     UnprocessedQueryExecutionIdTypeDef,
     CalculationConfigurationTypeDef,
     CalculationResultTypeDef,
     CalculationStatisticsTypeDef,
     CalculationStatusTypeDef,
     CancelCapacityReservationInputRequestTypeDef,
     CapacityAllocationTypeDef,
+    CapacityAssignmentOutputTypeDef,
     CapacityAssignmentTypeDef,
     ColumnInfoTypeDef,
     ColumnTypeDef,
     TagTypeDef,
     CreateNamedQueryInputRequestTypeDef,
-    CreateNamedQueryOutputTypeDef,
     CreateNotebookInputRequestTypeDef,
-    CreateNotebookOutputTypeDef,
     CreatePreparedStatementInputRequestTypeDef,
     CreatePresignedNotebookUrlRequestRequestTypeDef,
-    CreatePresignedNotebookUrlResponseTypeDef,
     CustomerContentEncryptionConfigurationTypeDef,
     DataCatalogSummaryTypeDef,
     DataCatalogTypeDef,
     DatabaseTypeDef,
     DatumTypeDef,
     DeleteCapacityReservationInputRequestTypeDef,
     DeleteDataCatalogInputRequestTypeDef,
     DeleteNamedQueryInputRequestTypeDef,
     DeleteNotebookInputRequestTypeDef,
     DeletePreparedStatementInputRequestTypeDef,
     DeleteWorkGroupInputRequestTypeDef,
     EncryptionConfigurationTypeDef,
+    EngineConfigurationOutputTypeDef,
     EngineConfigurationTypeDef,
     EngineVersionTypeDef,
     ExecutorsSummaryTypeDef,
     ExportNotebookInputRequestTypeDef,
     NotebookMetadataTypeDef,
     FilterDefinitionTypeDef,
     GetCalculationExecutionCodeRequestRequestTypeDef,
-    GetCalculationExecutionCodeResponseTypeDef,
     GetCalculationExecutionRequestRequestTypeDef,
     GetCalculationExecutionStatusRequestRequestTypeDef,
     GetCapacityAssignmentConfigurationInputRequestTypeDef,
     GetCapacityReservationInputRequestTypeDef,
     GetDataCatalogInputRequestTypeDef,
     GetDatabaseInputRequestTypeDef,
     GetNamedQueryInputRequestTypeDef,
     GetNotebookMetadataInputRequestTypeDef,
     GetPreparedStatementInputRequestTypeDef,
     GetQueryExecutionInputRequestTypeDef,
-    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    PaginatorConfigTypeDef,
     GetQueryResultsInputRequestTypeDef,
     GetQueryRuntimeStatisticsInputRequestTypeDef,
     GetSessionRequestRequestTypeDef,
     SessionStatisticsTypeDef,
     SessionStatusTypeDef,
     GetSessionStatusRequestRequestTypeDef,
     GetTableMetadataInputRequestTypeDef,
     GetWorkGroupInputRequestTypeDef,
     ImportNotebookInputRequestTypeDef,
-    ImportNotebookOutputTypeDef,
     ListApplicationDPUSizesInputRequestTypeDef,
     ListCalculationExecutionsRequestRequestTypeDef,
     ListCapacityReservationsInputRequestTypeDef,
-    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
     ListDataCatalogsInputRequestTypeDef,
-    ListDatabasesInputListDatabasesPaginateTypeDef,
     ListDatabasesInputRequestTypeDef,
     ListEngineVersionsInputRequestTypeDef,
     ListExecutorsRequestRequestTypeDef,
-    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
     ListNamedQueriesInputRequestTypeDef,
-    ListNamedQueriesOutputTypeDef,
     ListNotebookSessionsRequestRequestTypeDef,
     NotebookSessionSummaryTypeDef,
     ListPreparedStatementsInputRequestTypeDef,
     PreparedStatementSummaryTypeDef,
-    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
     ListQueryExecutionsInputRequestTypeDef,
-    ListQueryExecutionsOutputTypeDef,
     ListSessionsRequestRequestTypeDef,
-    ListTableMetadataInputListTableMetadataPaginateTypeDef,
     ListTableMetadataInputRequestTypeDef,
-    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     ListTagsForResourceInputRequestTypeDef,
     ListWorkGroupsInputRequestTypeDef,
-    PaginatorConfigTypeDef,
     QueryExecutionContextTypeDef,
     ResultReuseInformationTypeDef,
     QueryRuntimeStatisticsRowsTypeDef,
     QueryRuntimeStatisticsTimelineTypeDef,
     QueryStagePlanNodeTypeDef,
     QueryStageTypeDef,
-    ResponseMetadataTypeDef,
     ResultReuseByAgeConfigurationTypeDef,
-    StartCalculationExecutionResponseTypeDef,
-    StartQueryExecutionOutputTypeDef,
-    StartSessionResponseTypeDef,
     StopCalculationExecutionRequestRequestTypeDef,
-    StopCalculationExecutionResponseTypeDef,
     StopQueryExecutionInputRequestTypeDef,
     TerminateSessionRequestRequestTypeDef,
-    TerminateSessionResponseTypeDef,
     UntagResourceInputRequestTypeDef,
     UpdateCapacityReservationInputRequestTypeDef,
     UpdateDataCatalogInputRequestTypeDef,
     UpdateNamedQueryInputRequestTypeDef,
     UpdateNotebookInputRequestTypeDef,
     UpdateNotebookMetadataInputRequestTypeDef,
     UpdatePreparedStatementInputRequestTypeDef,
-    ListApplicationDPUSizesOutputTypeDef,
     QueryExecutionStatusTypeDef,
+    CreateNamedQueryOutputTypeDef,
+    CreateNotebookOutputTypeDef,
+    CreatePresignedNotebookUrlResponseTypeDef,
+    GetCalculationExecutionCodeResponseTypeDef,
     GetNamedQueryOutputTypeDef,
+    ImportNotebookOutputTypeDef,
+    ListApplicationDPUSizesOutputTypeDef,
+    ListNamedQueriesOutputTypeDef,
+    ListQueryExecutionsOutputTypeDef,
+    StartCalculationExecutionResponseTypeDef,
+    StartQueryExecutionOutputTypeDef,
+    StartSessionResponseTypeDef,
+    StopCalculationExecutionResponseTypeDef,
+    TerminateSessionResponseTypeDef,
     BatchGetNamedQueryOutputTypeDef,
     GetPreparedStatementOutputTypeDef,
     BatchGetPreparedStatementOutputTypeDef,
     StartCalculationExecutionRequestRequestTypeDef,
     CalculationSummaryTypeDef,
     GetCalculationExecutionResponseTypeDef,
     GetCalculationExecutionStatusResponseTypeDef,
     CapacityReservationTypeDef,
     CapacityAssignmentConfigurationTypeDef,
-    PutCapacityAssignmentConfigurationInputRequestTypeDef,
+    CapacityAssignmentUnionTypeDef,
     ResultSetMetadataTypeDef,
     TableMetadataTypeDef,
     CreateCapacityReservationInputRequestTypeDef,
     CreateDataCatalogInputRequestTypeDef,
     ListTagsForResourceOutputTypeDef,
     TagResourceInputRequestTypeDef,
     ListDataCatalogsOutputTypeDef,
     GetDataCatalogOutputTypeDef,
     GetDatabaseOutputTypeDef,
     ListDatabasesOutputTypeDef,
     RowTypeDef,
     ResultConfigurationTypeDef,
     ResultConfigurationUpdatesTypeDef,
     SessionConfigurationTypeDef,
+    EngineConfigurationUnionTypeDef,
     StartSessionRequestRequestTypeDef,
     ListEngineVersionsOutputTypeDef,
     WorkGroupSummaryTypeDef,
     ListExecutorsResponseTypeDef,
     ExportNotebookOutputTypeDef,
     GetNotebookMetadataOutputTypeDef,
     ListNotebookMetadataOutputTypeDef,
     ListNotebookMetadataInputRequestTypeDef,
+    GetQueryResultsInputGetQueryResultsPaginateTypeDef,
+    ListDataCatalogsInputListDataCatalogsPaginateTypeDef,
+    ListDatabasesInputListDatabasesPaginateTypeDef,
+    ListNamedQueriesInputListNamedQueriesPaginateTypeDef,
+    ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef,
+    ListTableMetadataInputListTableMetadataPaginateTypeDef,
+    ListTagsForResourceInputListTagsForResourcePaginateTypeDef,
     GetSessionStatusResponseTypeDef,
     SessionSummaryTypeDef,
     ListNotebookSessionsResponseTypeDef,
     ListPreparedStatementsOutputTypeDef,
     QueryExecutionStatisticsTypeDef,
     QueryRuntimeStatisticsTypeDef,
     ResultReuseConfigurationTypeDef,
     ListCalculationExecutionsResponseTypeDef,
     GetCapacityReservationOutputTypeDef,
     ListCapacityReservationsOutputTypeDef,
     GetCapacityAssignmentConfigurationOutputTypeDef,
+    PutCapacityAssignmentConfigurationInputRequestTypeDef,
     GetTableMetadataOutputTypeDef,
     ListTableMetadataOutputTypeDef,
     ResultSetTypeDef,
     WorkGroupConfigurationTypeDef,
     WorkGroupConfigurationUpdatesTypeDef,
     GetSessionResponseTypeDef,
     ListWorkGroupsOutputTypeDef,
@@ -544,15 +547,15 @@
     UpdateWorkGroupInputRequestTypeDef,
     BatchGetQueryExecutionOutputTypeDef,
     GetQueryExecutionOutputTypeDef,
     GetWorkGroupOutputTypeDef,
 )
 
 
-def get_structure() -> AclConfigurationTypeDef:
+def get_value() -> AclConfigurationTypeDef:
     return {...}
 ```
 
 <a id="how-it-works"></a>
 
 ## How it works
```

### Comparing `types-aiobotocore-athena-2.5.2/types_aiobotocore_athena.egg-info/SOURCES.txt` & `types-aiobotocore-athena-2.5.2.post1/types_aiobotocore_athena.egg-info/SOURCES.txt`

 * *Files identical despite different names*

